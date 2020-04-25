---
author: ["柯棋瀚"]
title: "Deploying Hugo Site Periodically to Netlify by GitHub Actions"
date: 2020-04-20
lastmod: 2020-04-20
categories: ["站務"]
tags: ["coding"]
url: /226
markdown: 'https://github.com/kujihhoe/HUGO-Theme-CJK/master/content/post/226actions.md'
description: '用 GitHub Actions 執行定時任務，生成 Hugo 網頁，發布到 Netlify 託管。沒什麼創新的，只是給自己留箇備忘'
vertical: false
---

## 一、

此前我網站的運行流程是：

1. 修改後推送到 GitHub
2. Netlify 獲取更新
3. Netlify 運行 Hugo，生成站點，發布

現在加上了隨機推薦後<n>整點更新；主葉分類；各文章下面的隨機推薦</n>，我們要運行定時生成任務，以定時生成隨機推薦。有兩種方法：

其一、

1. 修改後推送到 GitHub；GitHub Actions 发布定时任务
2. Netlify 獲取更新
3. Netlify 運行 Hugo，生成站點，發布

其二、

1. 修改後推送到 GitHub；GitHub Actions 发布定时任务
2. GitHub Actions 運行 Hugo，生成站點
3. Netlify 獲取更新
4. Netlify 發布

## 二、

首先看第一種方法。我用的這箇：[GitHub Actions for Hugo](https://github.com/peaceiris/actions-hugo)。在你的倉庫中，新建一個文件夾、文件 `.github/workflows/anyname.yml`，內容如下：

```yml
name: github pages

on:
  push:
    branches:
      - master
  schedule:
  - cron: '0 */1 * * *'

jobs:
  deploy:
    runs-on: ubuntu-18.04
    steps:
      - uses: actions/checkout@v2
        with:
          submodules: true  ## Fetch Hugo themes
          fetch-depth: 0    ## Fetch all history for .GitInfo and .Lastmod

      - name: Setup Hugo
        uses: peaceiris/actions-hugo@v2
        with:
          hugo-version: 'latest'
          extended: true

      - name: Build
        run: hugo --minify

      - name: Deploy
        uses: peaceiris/actions-gh-pages@v3
        with:
          github_token: ${{ secrets.GITHUB_TOKEN }}
          publish_dir: ./public
```

然後我們需要在 GitHub 中生成一個私人密鑰。點自己的頭像 — Settings — 最下面的 Developer settings — Personal access tokens — 權限勾選 repo, workflow。需要注意，`${{ secrets.GITHUB_TOKEN }}` 要和你的密鑰名字保持一致，並且原封不動，不用改成密鑰具體的値。比如這裏用的 `${{ secrets.GITHUB_TOKEN }}`，那麼你的密鑰名字就是 `GITHUB_TOKEN`。

生成的網頁文件會出現在 `gh-pages` 這箇分支中。

另外，關於定時任務的設置 `- cron`，可以用這個網址 https://crontab.guru/ 來測試。我設置的是每二小時生成一次，就是 `- cron: '0 */2 * * *'`。之前不知道，設成了 `- cron: '* */2 * * *'`，那就是每時每刻都在生成！幸虧發現得早。

接下來，就是 Netlify 的設置。

<img src="https://pic.imgdb.cn/item/5e9d0260c2a9a83be50d196e.jpg" width="400">

我們不用 Netlify 來運行 Hugo，中間三個都爲空。

<img src="https://pic.imgdb.cn/item/5e9d0260c2a9a83be50d1931.jpg" width="550">

Produnction branch 就是從倉庫的哪個分支獲取源碼，此處是 `gh-pages`。

大功告成！

## 三、

第二種方法，依然讓 Netlify 來運行 Hugo。我用的這箇 https://www.voorhoede.nl/en/blog/scheduling-netlify-deploys-with-github-actions/

```yml
name: Scheduled build
on:
  schedule:
  - cron: '0 */2 * * *'
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
    - name: Trigger our build webhook on Netlify
      run: curl -s -X POST "https://api.netlify.com/build_hooks/{yourhook}"
      env:
        TOKEN: ${{ secrets.NETLIFY_TOKEN }}
```

然後需要在 Netlify 中生成一個密鑰。

<img src="https://pic.imgdb.cn/item/5e9d08d0c2a9a83be5137ae9.jpg" width="400">

名字同理，和 ` ${{ secrets.NETLIFY_TOKEN }}` 保持一致，卽  `NETLIFY_TOKEN`。

然後把 `run: curl -s -X POST "https://api.netlify.com/build_hooks/{yourhook}"` 中的 `{yourhook}` 替換成密鑰的値。

大功告成！

## 四、

Netlify 有 300 分鐘每月的運行時長，這箇時間是怎麼定義的呢？

> When counting build minutes, we start the count when we begin loading your dependencies, and end it when we’ve finished uploading any new or changed files to our servers. In your deploy logs, you can check for `Fetching cached dependencies`
 as the first line when counting starts, and `Starting post processing` as the first line after counting stops. This pattern matches what we’ve found across other similar services.

<img src="https://pic.imgdb.cn/item/5e9d025fc2a9a83be50d18b3.jpg" width="500">

也就是圖中前面的 `Build Time`。我看了一下，如果給 Netlify 自己生成，Build Time 在 29-35s 之間，也就是每月可以生成 514-620 次，每日 17-20 次。如果給 GitHub Actions 生成，在 16-21s 之間，每月可以生成 857-1125 次，每日 28-37 次。多出來的次數還是很可觀的，足夠讓我們每小時定時生成一次。

現在，本站已經實現了半動態化，每小時重新生成一次隨機推薦。和動態網站相比還沒有的功能是：按閱讀量排序；排列最新評論。
