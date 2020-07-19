---
layout: 'block'
type: 'block'
author: ["柯棋瀚"]
title: "about"
date: 2017-10-04
lastmod: 2020-04-25
menu:
  main:
    weight: 1
url: /about
description: '此文爲本站緫序，包含介紹、說明書與聲明。除了這箇緫序，「古琴」「實地錄音」「書法」「讀切韻音」「旁白配音」均有各自的小序，介紹我爲什麼做這些事情。'
---

## 吿示

- 本站所有文章授權方式采用 <a rel="license" href="https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh" target="\_blank">CC BY-NC-SA 4.0</a> <n>署名-非商業性使用-相同方式共享</n>國際條款，若需使用，請務必閱讀竝遵循條款內容。說簡單點，非商業性使用無須告知作者，只要標明作者、出處就好<n>當然，沒人會轉載我的文章的，想多了</n>。爲便於排版，直接取用 md 源文件卽可。如果發現有錯別字，也可以在 Git 上幫我改正。
- 若發現文章中有不適冝的內容<n>如侵犯箇人隱私，牽涉箇人利益，損害箇人聲譽等</n>，請儘速郵件或評論告知我。
- 我用繁體字，還有一些奇怪的寫法，一來爲了滿足自己的一些癖好；二來爲了過濾一些不想看的來訪者；三來照顧牆外能用 Google 的華人們；還有一箇原因是系統自帶的簡體宋體无一能看。
- 如果看官歡喜，歡迎打賞救濟 \_(:з」∠)_ 收益將用於网站運營及公益，㪅多見 [公益、贊賞、收支](/blog/2018/11/06/zjuh.html)。可通過支付寶、[paypal](https://paypal.me/kujihhoe) 或 bitcoin `1GWQhWVpFGxKqwp7R6C7ayb2jyPrdPgCYr` 向我捐助。
- 通過這箇 [邀請鏈接](https://www.superbed.cn/signup?from_id=5be2af239dc6d6b928f1a085) 註冊聚合圖床，我將會得到 30% 反現，您也可以通過這種方式支持我。聚合圖床非常好用，速度快不怕丟失。

<img src="https://api.superbed.cn/pic/5bf82416c4ff9e058246008d" width="150" >

## 技術

- 【支持】託管於 ~~<a href="https://pages.github.com" target="\_blank">Github Pages</a>~~ [netlify](https://www.netlify.com) 平臺，由 ~~<a href="https://jekyllrb.com/" target="\_blank">Jekyll</a>~~ [hugo](https://gohugo.io/) 引擎驅動，~~<a href="https://github.com/kitian616/jekyll-TeXt-theme" target="\_blank">kitian616</a> 提供网誌主題模板 Text[jane](https://github.com/xianmin/hugo-theme-jane)，~~，主題基於 Flex 修改。~~<a href="https://tw.godaddy.com/" target="\_blank">GoDaddy</a>~~ [dynadot](https://www.dynadot.com) 提供域名，~~<a href="https://www.cloudflare.com/" target="\_blank">Cloudflare</a>~~ netlify 提供 DNS 解析、SSL，<a href="https://git-lfs.github.com/" target="\_blank">Git LFS</a> 提供文件存儲，<a href="https://portal.qiniu.com/dora" target="\_blank">~~七牛雲~~</a>圖牀采用 [聚合圖牀](https://www.superbed.cn)，~~<a href="http://busuanzi.ibruce.info/" target="\_blank">不蒜子</a> 提供全站 UV、PV 統計<n>自 20171021 開始，目前不顯示，因爲跟谷歌的比誤差有點大</n>~~評論模塊爲 [詔預Isso開放服務](https://open.saintic.com/openservice/isso) ~~[Valine](https://valine.js.org) [Gitalk](https://gitalk.github.io/)，leancloud 提供文章點擊量統計<n>20181026 之歬爲 UV，之後開始累加 PV</n>，採用 [Google AdSense ](https://www.google.com/adsense/) 廣告~~，流量分析採用 Google Analytics，全部博文存儲於 IPFS 分布式系統。古琴關注數統計用的 [Substats](https://sspai.com/post/59593) api。
- 【隱私】見 [本站的隱私、安全、速度 privacy policy]({{< ref "253-privacy" >}})
- 【檢索】1、本站已支持 Algolia！歡迎使用！2、直接用 <a href="https://www.google.com/search?q=site:kqh.me" target="\_blank">Google</a><n>Google 收錄得又全又快</n>，例子：`site:kqh.me 芋圓`，中閒記得加空格。搜索引擎對网葉內容的更新不會很頻繁，很可能我修改了一些內容，但沒有被收錄，衟致搜索結果不準確。
- 【大事記】見 [更新](/release)
- 【板式】見 [示例葉面](/149)
- 【文章推薦算法】見 [Hugo文章推薦算法舉例](/223)
- 【文章統計算法】見 [Hugo文章統計算法舉例](/224)

## 內容

本站結構：

```
赫赫文王 ──────────── 主葉
  ├─ 作品
  ├─ 网誌 ─────── 文章
  │  ├─ 發現 ───────┤
  │  │  ├─ 最近發布 ─┤
  │  │  ├─ 最近修改 ─┤
  │  │  ├─ 分類 ────┤
  │  │  ├─ 其他作者 ─┤
  │  │  ╰─ 年度 ────┤
  │  ╰─ 索引 ───────┤
  │      ├─ 分類 ───┤
  │      ├─ 系列 ───┤
  │      ├─ 標籤 ───┤
  │      ╰─ 作者 ───╯
  ├─ 知識
  │  ├─ 讀書
  │  ├─ 敎程
  │  ╰─ 考試
  ╰─ 數據庫
     ├─ 赫赫讚府
     ├─ 傳世琴譜數字文本化工程
     ├─ 春秋學刊
     ╰─ 文庫   
```

本站文章按「分類」「系列」「標籤」「作者」進行索引。分類近似於學科門類，標籤近似於更小的分類。每篇文章只有一箇分類、一箇系列，可以有多個標籤。

### 網誌

#### 分類

- 經：關於經學史的內容，我的主業
- 琴：關於古琴的隨想、考査、日記等
- 書：書法作品、隨想等
- 史：關於歷史學的，以廢話垃圾作業居多
- 人文：其他人文藝術學科的，以廢話垃圾作業居多
- 錄音：關於實地錄音、古琴錄音、錄音技術的紀錄
- 漢語：文字音韻語言學的皮毛
- 彫梓：有關字體、排版、編輯的
- 生活：日常瑣事
- 站務：網站本身的運營紀錄

#### 系列

- 㢧耕記：有關古琴的一些心得、論文。弦的甲骨文是指事字，弓上加一符號。「㢧」本來是「卷」的異體字，我用來當「弦」
- 㢧耕知聞：非自己原刱的，如筆記、見聞、交遊等
- 訪琴記：本來是絃耕知聞裏面的，篇數多了就單獨抽出來
- 紀日：各類日記，一般半秊一篇。古琴日記，日常感想、與琴友的交遊、通信、看到的訊息都記上去；書法日記；其他日記
- 玨壴記：有關<v>三禮</v>的。因爲禮的初文是豊，豊的初文从玨壴
- 尼凥記：有關<v>孝經</v>的，因爲開篇是「仲尼凥，曽子侍」
- 雩若記：有關<v>尙書</v>的，因爲開頭那幾篇都是「曰若稽古某某」，而「曰」一作「粵」，「粵」古又作「雩」
- 元麟記：有關<v>春秌</v>的，始元終麟嘛
- 无衺記：有關<v>詩經</v>的
- 學務：上學期間雜七雜八的東西
- 觀後：博物館展覽；電影；音樂
- 墨池記：有關書法的想法、記錄等
- 講閒譚：這是溫州話「聊天」的意思，譚通談。各種日常瑣碎啊，囘憶啊，用品啊，看法啊
- 斿記：斿通遊。出去逛逛
- 立言記：算「遊記」的一部分，但特殊一些，獨立出來。2017 下半秊在臺灣交換，會發一些沒見識的流水帳口水話遊記
- 中學：關於中學時代的記憶

#### 備註

- 課業：上課的作業。這一部分完全可以不用看，沒什麼價値，完全用來湊字數。放在這裏不過是爲了方便有需要的同學可以拿來用，以減少一些寫課程論文的不必要的時閒浪費，也算是對大學浪費的時閒一箇小小的交代。想想我爲了交作業，寫了多少垃圾，浪費了多少寶貴旹閒啊。至於版權的問題，如果用來當作業素材的話，隨便複製粘貼就是。至於在網上傳播用，則遵循本网誌一貫的 [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.zh)

### 知識

- 讀書：讀書筆記
- 赫赫指北：搭建知識框架
- 資源：一些信息聚合
- 考試：考試複習資料

### 數據庫

- ~~赫赫讚府：收集網路評論等，按主題進行編排，爲當下的厤㕜提供一些索引~~
- 春秋學刊：北師大歷史學院本科生學術刊物<v>春秋學刊</v>的目次<n>半秊刊，至少未來幾年我還在師大就會繼續㪅</n>
- 傳世琴譜數字文本化工程：希望有生之年能夠繼續
- 文庫：一些標點作業
