---
layout: 'block'
author: ["柯棋瀚"]
title: "更新"
date: 2017-10-05
lastmod: 2020-04-24
url: /release
markdown: 'https://github.com/kujihhoe/blogflex/blob/master/content/post/release.md'
menu:
  main:
    weight: 2
description: "本站更新日誌"
---

## 大事記

- 2017-10-03 建站：kujihhoe.com
- 2017-10-27 弟二版
- 2018-11-21 弟三版
- 2018-12-04 域名變㪅爲 kqh.ac
- ~~12-06 啓用四箇網站~~
- 12-18 正文改爲直排
- 2019-07-22 域名變更爲 kqh.me
- 建站兩周年之際，啓用新 logo。來源是<u>何尊</u>銘文及<v>續甲骨文編</v>4534
- 2020-04-01。弟四板。採用顛覆式的全卡片式設計，取消了頁首
- 2020-04-18 v4.6.09 增加自動暗黑模式

## 更新

### 第一版

#### 10 月 3 日

建站。網站模板 fork 自 <a href="https://github.com/cnfeat/cnfeat.github.io" target="\_blank">CNFeat</a>，表示感謝。

#### 10 月 4、5 日

修改了一些細節。

#### 10 月 18 日

把字體換成了思源宋體韓國版，當然，要本地安裝了的纔行。引文換成了楷體。

去掉了頂部的圖片。

主題色換成了我標誌性的朱紅<n>此處配表情[嘿哈]</n>，去年以來對暗紅色情有獨鐘<n>大霧</n>。

現在可以說非常像印刷品了。

註冊了騰訊企業郵箱：1 (at) kujihhoe.com

#### 10 月 19 日

把翻頁的按鈕和回到頂部按鈕的樣式改成了圖標。

博文頁面增加了回到頂部按鈕。

配置了 Jekyll 本地運行環境。

#### 10 月 20 日

增加了 gitment 的評論模塊，用 github 帳號登錄就可以評論。<n><a href="https://imsun.net/posts/gitment-introduction/" target="\_blank">imsun</a> 提供支持</n>。把英文改成中文，修改了一點樣式。

把翻頁的東東搬到了導航欄，全屏的時候往下拉導航欄會顯示出來。

「回到頂部」按鈕在右下哦。

添加百度統計、Google Analytics，數據從19日算起。

添加訪問量<n><a href="http://jerryzou.com/posts/introduction-to-hit-kounter-lc/" target="\_blank">咀嚼之味</a> 提供支持</n>。並不太好用，能看到的時候少，看不到纔是大多數。

#### 10 月 21 日

把訪問量模塊換成了 <a href="http://ibruce.info/2015/04/04/busuanzi/" target="\_blank">不蒜子</a>，很好用了。數據從今天算起，所以網站訪問總量要實際要多 100 多<n>當然，基本上都是我自己的流量</n>。

增加了網站圖標，safari 大的書籤要靠 apple-touch-icon 來實現。

用 PS 做了一箇非常簡陋的打賞部分。

標籤索引試了好久，文章名上面的標籤超鏈接點一下都是 404，最後發現是把路徑的 tags 寫成了 Tags！吐血！！把標籤當成分類來用，我是不喜歡那麼亂糟糟的標籤的。調整了分類頁的樣式。

把 RSS 訂閱的圖標換成了文字。

加入字數統計、總篇數統計、總字數統計。試了一下，加圖片鏈接字數沒有增加。

調整了標題和正文的距離，調整了正文和底部分割線的長度。調整了標題的顏色。

用了 <a href="https://app.swiftype.com/engines/new" target="\_blank">swiftyle</a> 的外掛的搜索，沒成功，說在生成我的網站目錄，然而都一晚上過去了還是不行，刪掉。

#### 10 月 22 日

在頁面左側增加了文章目錄。

分類頁爲了節省篇幅，字改小一點。修復了點進去 404 的問題<n>因爲多了一箇 `{{ site.url }}`</n>。

在文章末尾增加了版權聲明。

把正文顏色加深一點。

回到頂部實現了平滑滾動，但其他錨點暫時還不知怎麼辦。

gem 了 Jemoji：:smile::kissing::smiley::blush::stuck_out_tongue_closed_eyes::flushed::mask::sleeping::sunglasses::clap::muscle::pray::raised_hands::point_left::point_right::sweat_smile::sweat::weary::tired_face::joy::sob:

添加最後修改時間，找了半天，先找了一箇很長的，然後找怎麼把 js 的値賦給 html，沒成功，最後直接蒐「js最後修改時間」，找到了一箇很短的代碼。

調整標題字號顏色。

#### 10 月 23 日

大改版，採用兩欄式，左側寬度 25％，上方爲目次，下方爲文章信息。右側爲文章正文，字號 21.5 點，每行 35 字，字符間距增加 0.1 點，段距 13 點，不採用首行縮進。後來試驗了一下首行縮進，發現怪怪的，想了想是因爲左邊有一條線，在視覺上產生了一種吸引力，文字要對齊纔行，如果首行縮進就會顯得參差不齊。紙製品兩側是空的<n>即使書也是這樣</n>，因此看起來不會感到奇怪。


分類增加標籤雲，用大小與顏色來區分每箇類別文章的數量。後來標籤雲失效了，看了半天看不出所以然，索性刪掉。標籤的顏色是藍的，想用條 style 的辦法來調，但沒用。

採用應用標題的方式處理小字的格式，更加方便。

目錄樹只顯示三級標題，剛開始我查到的：
```
toc_levels:    1..3
```
但沒用，後來找了一下，

```toml
kramdown:
  input: GFM
   auto_id_prefix: id-
    auto_ids:      true
  ## footnote_nr:   1
  ## entity_output: as_char
  ## toc_levels:    1..3
```
這樣就好了。要加 ## 纔行。寫標題的時候要用<h5></h5>，不能用 #####。

#### 10 月 24 日

發生奇跡了，
```
[2017-10-24 11:24:44] ERROR `/js/bootstrap.min.js ' not found.
[2017-10-24 11:24:44] ERROR `/js/clean-blog.min.js ' not found.
```
昨天終端說找不到上面這箇，剛剛不知道刪了點啥，就恢復正常了，上拉顯示導航條又恢復了。但是本地環境運行還是不行，在網上運行就可以，眞是玄學。

撤掉了回到頂部按鈕：「關於」頁面很短，用不著，「分類」頁面可以點小標題回到頂部，主頁直接翻就好，博文頁左上有「回到頂部」按鈕。

奇怪的是，第一篇博文上拉不會顯示導航條，下面 footer 也是算在正文裏面，沒有分隔線，其他文章都正常。我在想會不會是因爲第一篇，所以往前面加了一篇，然而那一篇正常的這篇還是不正常。眞是玄學。

進行了一點點正文的頁面適配。

添加了 SSL，綠色的小鎖眞好看:blush:。照著 <a href="http://songchunlin.net/cn/2016/12/enable-https-for-Jekyll-blog/" target="\_blank">這篇</a> 一步步來就好，非常輕鬆。網址變了，就要把 Gitment 重新設置一邊。

我自己改的代碼十分簡單暴力，一點不優雅，然而我就只有這箇水平了。

發現用了七牛鏈接便不是安全網站了，爲了維護小綠鎖的尊嚴，決定把圖片從七牛遷回 git 的倉庫。反正有 1G 空間，還不限流量，隨便夠用了。

昨天想把正文位置往右移，試了很久都不行，突然想到前面標籤有一箇 `<div class="row">` 那我靈機一動，索性改成 rows，在樣式表裏面加一箇 `.rows{ }` 在這裏面調整位置，就這樣用這種很怪的方式達到目的。<n>`row` 的上級標籤是  `container`，我一直在樣式表裏沒找到這箇神秘的存在，但不管怎麼說，我只在 `rows` 裏面改變位置，其他的一切都有這箇神秘的 `container` 來操控</n>  
之前輸出爲 `page.html` 的頁面，鏈接都是黑色的，必須手動調成紅色。剛剛突然想到可以用昨天的方法，把 `row` 改成  `rowss`，再在樣式表裏面加一箇 `.rowss`，就這樣，那幾箇鏈接也自然而然應用了 `post.html` 頁面的紅色鏈接。

移動適配目前看著代碼還一臉懵，以後有機會再說吧。可以當作逼別人用電腦來看。

火狐眞是一朵奇葩，Chrome 和 Safari 都可以兩端對齊，它就不行，玄學＋1。

#### 10 月 25 日

把幾箇 js 放到了本地，這樣就全部是小綠鎖啦。

向 360、搜狗、Bing 提交了收錄申請和站點地圖。

左下方的鏈接太長，會橫向溢出，加了箇這箇：

```css
text-align: justify;
text-justify:inter-word;
overflow: auto;
word-break: break-all;
word-wrap: break-word;
```

成功解決，只用豎向拉動就可以了。

把 jQuery 升級到了 3.2.1。清理了一些沒用的代碼和腳本。

把 `config` 裏面 `paginate` 配置改成了：

```toml
gems: [jekyll-paginate]
paginate: 20  
paginate_path: "page:num"
```

把部分超鏈接改成了在新頁面中打開。

#### 10 月 26 日

去掉了引用左邊的豎線。

申請了 GitGub Student，有免費的私人空間啦，從此這箇倉庫在 GitHub 隱身。審核速度很快，我八點提交，十點再看時已經通過了。

啟用 Git LFS，這下在 Git 裏面存圖片音頻這些完全沒問題啦。把所有圖片轉成本地圖片後可以發現，原來的圖片鏈接全部失效，要換成 LFS 的地址。但是問題來了，這箇倉庫是私人倉庫，所以圖片加載不了，必須把圖片搬到公共倉庫。

然而問題又來了，評論模塊加載不了，通信被阻擋了。不得不回到公共空間，十分不捨。

把圖片遷出去以後，發現 `.git` 隱藏文件夾還有 40M 的文件，估計就是圖片了。本地刪了以後同步軟件報錯，而網頁上也沒顯示這箇文件夾，我反應過來應該是 git 倉庫最基本的配置，刪了就沒了。於是乎，把原來的刪掉，在本地重新建一箇倉庫再上傳，整箇大小只有 1.7M 了。

翻页键新增 title，不过悬停时间要 2 秒，不知怎么调整。

增加主頁的頁數統計。

小屏幕下導航條右邊縮成方框，但點不開，又不知怎麼回事，只好暴力的刪掉它，用普通的辦法直接加在左邊標籤的後面，這樣全部集中在左邊了，把右邊留給正文。導航條上拉的時候把顏色設成透明，這樣更減少了阻隔，右邊就全然是正文了。

進行了一些響應式設計，不同屏幕尺寸下都可以正常看了，可以說很完美了。長舒一口氣。現在网誌差不多基本完工了。

現在再看頭幾天進行的修改，簡直太小兒科了。

### 第二版

#### 10 月 27 日

昨晚莫名其妙出 bug 了，我明明沒怎麼改動，但電腦下主題就出問題了，恢復原來的版本一樣不行。只好重新換模板。找來找去用了<a href="https://github.com/kitian616/jekyll-TeXt-theme" target="\_blank">這箇</a>，算是我看到的裏面製作最精良的。對作者表示感謝 :blush:

jekyll 本地環境一直弄不好，无可奈何，只好傳到網上看效果，有些改動老是報錯，反復了好幾次，折騰不起折騰不起。

#### 10 月 28 日

把原來的功能全部遷移過來，差不多滿意了。

一箇小 tip，每篇文章頭信息冒號後面一定要空格！空格！

#### 10 月 30 日

Bing、Yahoo 已經收錄我的網站啦，歡呼！

把 logo 換了。

#### 10 月 31 日

向 Bing 提交了 sitemap 和 URL，一天只能加十箇，明天繼續。向搜狗提交了主頁的 URL，向 360 提交了 sitemap 和 URL。Google 一直不理我，sitemap 提交上去一直顯示擱置，晚上試了一下 Bing，最新的幾篇也都收錄了，以後站內搜索都用 Bing 好了。

了解了一下 cc 協定，決定採用 CC BY-NC-SA 4.0 條款。

footer 的樣式表怎麼調都沒用，於是用很暴力的方法解決了 footer 高度太大的問題，直接把 `$footer...` 改成了 `0`。

ruby 竟然只支持 JDK 8！

#### 11 月 3 日

中午回來，竟然莫名其妙抽風，說 `page build failure`。於是用毀滅大法，把本地倉庫遷到沒用 iCloud 備份的目錄，刪掉重新來一遍就好了。明明早上更新還正常的，上完課回來就出毛病，玄學＋1。

之前正文和 footer 之間之所以有一大截空白，是因爲 `_layout.default.scss` 裏面 `.m-page-stage` 的 `padding-bottom` 設置了一箇奇奇怪怪的値，把它改成 0 就好了。

騰訊企業郵竟然用不了了，說我沒有`實` `名` `認` `證`，我纔不認 證呢，寧可不用。不過後來看了下DNSpod，說沒有添加解析，恍然大悟，原來 cloudflare 就是提供 DNS 解析的啊！只不過是順帶有 SSL，眞是良心。那 DNSpod 就完全沒用了，刪掉刪掉。進 CF 後臺看了下，原來還可以清空緩存，怪說不得改 footer這些，Git 把頁面生成好了，再刷新卻沒變。給 CF 加了 MX 解析，企業郵箱又可以用啦。

隨便逛了一下那些用 WordPress 搭的网誌，界面簡直是十年前的審美，不忍直視，那樣的話我肯定不想寫東西了。幸好選擇了靜態網站。

改了下超鏈接的樣式：懸停時變爲黑色，字重用正常的，不要加粗。剛開始把 `font-weight` 改成 `$base-font-weight`，發現主頁也變成細的字了，突然想到直接把字重那一條刪掉就好，這樣主頁是粗的，文本中的超鏈接是正常字重。

限制了目錄樹的高度，設成 `680 px`，用 `%` 和 `auto` 都沒用，不知爲何。

在 CF 設置了一下縮小 js、css、html 文件的大小。似乎是快了一點。

在這箇網站下面另外設了一箇子目錄用來存私人的東西，用私人倉庫存儲，robots 設置禁止爬蟲抓取，這樣只要我不說網址沒人知道它的存在。現在全面進入雲時代啦！😝要列印的話用 Chrome，「使用系統對話框列印」，每頁排 2 頁，這樣一行 30 箇字。  
有這麼一些考慮：①可以列印；②私人；③排版、字體要和 word 很接近；④各箇終端能以最便捷的方式瀏覽。  
Gitbook 的私人倉庫要給錢，我申請到了 GitHub 的學生免費私人倉庫，不用白不用。滿足第三點的也就只有我的网誌。所以說，上述方案是最佳選擇。

#### 11 月 4 日

開熏，把標點換成方正新書宋啦！現在比 word 排版還方便了，之前用 word 還要把標點替換成新書宋。  
用 `Fontmin` 這箇 APP，提取需要的文字字體，簡直神器啊！傻瓜式操作！還給你自動生成 `@font-face`，然後添加到 css 裏面就好啦：

```css
@font-face {
    font-family: "方正新书宋GBK正版";
    src: url("方正新书宋GBK正版.eot"); /* IE9 */
    src: url("方正新书宋GBK正版.eot?#iefix") format("embedded-opentype"), /* IE6-IE8 */

    url(data:application/x-font-ttf;charset=utf-8;base64,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) format("truetype"), /* chrome、firefox、opera、Safari, Android, iOS 4.2+ */

    url("方正新书宋GBK正版.svg#方正新书宋GBK正版") format("svg"); /* iOS 4.1- */
    font-style: normal;
    font-weight: normal;
}
body {
  font-family: "方正新书宋GBK正版","source han serif k","source han serif sc","Source Serif Pro","Adobe Caslon Pro","Palatino Linotype","Palatino","FZNewShuSong-Z10";
    font-weight: $base-font-weight;
    font-size: $base-font-size * 1.1;
    line-height: $base-line-height;
    color: $text-color;
    text-align: justify;
    text-justify: inter-ideograph;
    word-break: break-all;
    padding-bottom:20px;
    padding-top: 20px
}
```

簡直天地良心。之所以不想用思源宋體的標點，因爲是貼著左邊框的，這樣跟前面的字幾乎是貼在一起。

後來，safari 標點避頭尾竟然莫名其妙失效，又重裝一遍。惹不起惹不起不折騰了。

做了一箇大膽的決定，把分類頁作爲主頁，原來的主頁刪掉。
成功遷移主頁。更加精簡啦。

再做一箇大膽的決定，增加箇人主頁。

<a href="https://statcounter.com" target="\_blank">https://statcounter.com</a> 是統計是按 cache 來的。加了 FlagCounter。

#### 11 月 5 日

一箇百思不得其解的問題：Safari 下字體纔是思源韓文版，Chrome 和 Firefox 都是簡體版，然而我並沒有裝簡體版。剛開始以爲是瀏覽器的問題，後來設置了一下一點用都沒有，Word 也沒有顯示這箇字體，估計是字體本身的問題。

Safari 導出 PDF沒有自動斷行，所以一行字往往被斷開了，Chrome 就可以。

[這篇](http://www.w3cplus.com/css/designing-for-print-with-css.html) 講打印 css 設置，簡直帥爆了。

加了表格單元格框線。

導航欄把「网誌」遷到左邊。要不然不容易看到，會習慣性的點粗的「赫赫文王」。

```
keqihandeMacBook-Pro:themes keqihan$ textlint /Users/keqihan/Downloads/GitHub/kujihhoe.github.io/_posts/2017-10-04-hualian.md

/Users/keqihan/Downloads/GitHub/kujihhoe.github.io/_posts/2017-10-04-hualian.md
   30:37   ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
   30:38   ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
   73:94   ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
   73:96   ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
  114:203  ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
  114:230  ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width
  114:232  ✓ error  原則として、全角文字と半角文字の間にスペースを入れます。 ja-space-between-half-and-full-width

✖ 7 problems (7 errors, 0 warnings)
✓ 7 fixable problems.
Try to run: $ textlint --fix [file]

keqihandeMacBook-Pro:themes keqihan$
```

#### 11 月 7 日

優化目錄樹的樣式。

添加腳註的方法，如果用 `[^1]` 這種自帶的，在手機上那箇箭頭會變成其丑无比的 emoji 圖標，還是用原來的好了，前面用 `1. ` 讓腳註有懸掛縮進，後面 `<a id="5a" href="#5">☍</a>`。

#### 11月8日

改了一下字體，增加了針對蘋果的蘋方，針對安卓的思源黑體，安卓沒有自帶宋體，蘋果帶的是日文字體，簡體字缺很多，好在繁體字基本上都有，差的幾箇再用 Fontmin 補就好。

奇怪的是 Safari Technology Preview 顯示的正文是小的，萬能的 Chrome 可以調字號，姑且不論，iOS 11 的 Safari 是小的，昨天去看陽學長的 Mac Air 也是小的，可我的 Safari 和 Firefox 就是大的。玄學＋1。网誌首頁 `總字數： 75035<n>含標點、數字</n>｜[介紹、說明書與聲明](http://kujihhoe.com/instruction)` 設的字號是 17 px，在屏幕上簡單粗暴的量了一下，小的大約是 19.43 px，大的是 26.71 px。正文字號是 `$base-font-size: 1em` `font-size: $base-font-size * 1.3`。也許是因爲大的算了 `*1.3`，小的沒算？索性改成 `$base-font-size: 22px` `font-size: $base-font-size`。

發現一箇問題，有圖片的文章 1、基本上要刷新一次，目錄纔會正常顯示，要不然拖到後半部分目錄以爲文章已完，就跑上去了。2、還沒瀏覽到下箇標題，目錄就已經跳到下箇標題了，我猜是沒把圖片的空間計算進去。无奈不知如何解決。

怪說不得 6 plus 把屏幕橫過來字就變大了，原來是把手機的像素設小了，原來是 500 px，改成 760 px 就好了。

最大寬度 800 px 改成了 795px，因爲 36*22=792。

#### 11 月 14 日

新版主頁全新上線！考完第三門，放鬆一下，便做了箇這箇。模板用的這位 <a href="http://blog.liuxj.com/CV/" target="\_blank">小姐姐</a> 的，表示感謝！

#### 11 月 15 日

圖床用了一圈，最後還是回到原點，用七牛。https 雖好，但一箇最致命的問題是，少量圖片不能顯示，必須刷新纔行，有些甚至都不行，Safari 還好，Chrome 是大片大片加載不出。不光免費的不行，連 Git LFS 也不能倖免。不安全就不安全吧，只是看著不爽而已。

精簡了一下網站的結構，條理更清晰。

cloudflare 的  SSL 級別調成這箇：

```
Full SSL (strict): Your origin has a valid certificate (not expired and signed by a trusted CA or Cloudflare Origin CA) installed. Cloudflare will connect over HTTPS and verify the cert on each request.
```

就出現了 error 526.

#### 11 月 16 日

刪了一點沒用的樣式表。想換成黑底白字，但發現字會略粗，手機上就沒問題，截圖下來看，粗細竟然是一樣的。可能是電腦屏幕的問題吧。只能作罷。

`![](xxx){:width="400"}` kramdown 寫成這樣是可以的，若還想往括號裏加箇 `text-align="center"` 就沒用了。

#### 11 月 20 日

增加了網址二維碼

把引用字體改成黑體

統一評論框背景色

#### 11 月 21 日

略調主葉佈局

#### 11 月 22 日

略調授權、二維碼位置。

#### 2018 年 2 月 9 日

增加一條 `word-break:break-all`

#### 4 月 5 日

古琴上線啦！上傳到網易雲音樂，國內用戶可以很方便地聽了。歡迎關注！賬號：赫赫文王。

#### 5 月 15 日

田野錄音上線啦！上傳到網易雲音樂的電臺，歡迎訂閱！名字：情形于声。

#### 7 月 26 日

切韻音朗讀上線啦！B 站賬號：kujihhoe，歡迎關注！原來的論文感覺不是很必要，便把位置讓給了這箇。

#### 8 月 11 日

發現沒對，標點很多都在下一行，把 `word-break:break-all` 刪了。

#### 8 月 14 日

把介佋移到了网誌正文目錄中，之前一直單獨一箇位置，突然發現完全沒必要。

header 加上了灰色底紋，但是沒法做到和 footer 一樣，不想折騰了，就這樣吧。

書法和平面上線啦！500px 主頁：500px.me/kujihhoe，歡迎關注！等以後閑下來的時候再縵縵傳些照片。

#### 8 月 16 日

文末加上了打賞。

#### 9 月 1 日

給域名續費的時候推薦一箇麥咖啡的認證，一年三十塊。感覺除了看著安全一點，沒有任何用處。就暫時先用著一年吧。域名費是一年一百左右。

#### 9 月 7 日

跟隨谷歌，取消超鏈接的下劃線。

#### 9 月 12 日

重做了網站的 logo。

#### 9 月 17 日

發現 360 提供站內搜索，那就加進去吧。如果 360 更新不及時，可以試下必應。

#### 9 月 21 日

把評論模塊刪除了，一年來只有爲我提供模板的哥們評論過一次，其它的沒有任何評論。看我网誌的都是文科生，不大可能有 Git 帳戶吧。

#### 10 月 19 日

登了一下企業郵箱，發現有箇人一箇半月㞢歬的消息沒看到，肰而 QQ 郵箱很久沒有通知了，一看，原來是密碼錯誤，也是醉了。

很苦惱的一點是，Safari 升級到 12 後，就顯示不出思源宋了，只能顯示手機上的游明朝。我把英文的改了一下。好歹還能顯示 aldusnova。Chrome 還是一如旣往只能顯示思源宋簡體中文版。

#### 10 月 22 日

改了下標點的字體，只有 `<v></v>〈〉——、。，·……` 用的方正新書宋。

#### 10 月 24 日

把 360 搜索框刪了，㪅新太慢，還是谷歌好。

#### 10 月 25 日

字體全部改成 Hiragino Mincho ProN。收錄到了 [Boke112](https://boke112.com/zhzx) 的綜合資訊類。

#### 10 月 26 日

現在文章一多，不蒜子似乎不太好使了，把閱讀次數刪了。想換成 Text 2.2.2，折騰了一箇白天，㠯失敗告終。不知這箇模板能續到什麼時候。

加上了 valine 的評論系統，感激涕零！還有附帶的點擊量統計，ID 寫 `{{ page.url }}` 就好，試了好久。

在百度搜赫赫文王，竟肰有我的主葉，搜柯棋瀚也有，但二級頁面都沒有，註冊了百度的搜索站長平臺，用爬蟲，被禁止。已經逆天了，百度竟肰收了一箇葉面！！

#### 10 月 27 日

這幾天突肰腦抽，想加友鏈加推廣。向網紅邁進！233333

主葉那四箇字換成了漢儀顏楷。

#### 10 月 29 日

突肰想到，把那篇博文標題從「輔大」改成「輔仁大學」，這樣利於搜索。發現谷歌㪅新㝵很勤，我 blog 葉面更新日期是 10 月 27  日。

這幾天 IP 緫筭上了 20，不知能保持多久。

#### 10 月 31 日

Google AdSense 審核通過。開通了鏡象公眾號

#### 11 月 1 日

奇怪，爲何沒有谷歌的廣告？過了11月2 日有了待審核廣告，看來需要一些時間，廣告慢慢會多起來。

去掉了引用的虛線，靠兩箇字的左縮進來區分，加大引文與正文的間距，改了一級標題分割線。頓時覺得清爽許多。

```html
  <div class="col-2">
​      <aside class="js-article-aside">
​          <div class="m-toc js-toc"></div>
​      </aside>
  </div>
```

筭了一下現在的原刱字數：873376*0.968-48181=797247 字，差不多可以慶祝一下突破 80 萬了。不知朙秊兩周秊的旹候能否突破百萬。

把打賞圖片拆分成三部分。剛剛纔意識到如果是一張的話，在手機微信上「識別圖中二維碼」，會掃除支付寶的地址。添加打賞名單表格。把首葉那幾箇字都換成顏楷。本來想把介紹換成文悅古體仿宋，但那幾箇字就一百多 KB，筭了。

#### 11 月 2 日

改小目錄枼字號行距，月日只畱數字，刪去葉腳緫序。全站 UV 迻到緫序

```html
          {% if page.previous %}
​        <li>  <a class="navbar-brand" href="{{ page.previous.url | prepend: site.baseurl | replace: '//', '/' }}" data-toggle="tooltip" data-placement="top" title="{{page.previous.title}}">上篇</a>
​        </li>  {% endif %}
​        {% if page.next %}
​        <li><a class="navbar-brand" href="{{ page.next.url | prepend: site.baseurl | replace: '//', '/' }}" data-toggle="tooltip" data-placement="top" title="{{page.next.title}}">下篇</a>
​        </li>{% endif %}`
```

把上下篇刪了。

這幾天IP都能在20

#### 11 月 5 日

把正文字號調成 20px。

404 葉面加入騰訊公益。計畫將網站收益結餘用作公益。

#### 11 月 6 日

添加 google translate 接口。

#### 11 月 7 日

原來都用的七牛雲作爲圖床，結果最近政策變了，測試域名只能用一箇月，長期用必須綁定域名，然而域名必須要備案，就沒招了。其實七牛雲之歬已經發過很多次測試域名到期的通知，但我都㠯爲不關我的事，今天纔發現有存儲文件的倉庫不能用了。幸好不是存圖片的，存圖片的還有三天過期。本來想用自己的vps搭一箇圖床，想著算了太麻煩，而且萬一哪天被牆了又完蛋了。找了一箇靠譜的<u>聚合圖牀</u>，付了費，一秊一百。想批量導出七牛雲外鏈，於是四處找辦法，太複雜不會，又買了一箇月專業版，100 圓，可以離線批量導入鏈接，結果沒用上浪費了一百塊。還是在 md 中一箇圖片一箇圖片的替換。其實批量換根本不能省旹閒，你還得一箇一箇找原來圖片在哪。遷移了三箇小旹，緫筭完工。

另一箇很疑惑的是，https 的圖牀有大槩三分之一顯示不出來，要刷新幾次纔行，原來用 Git LFS 也是這樣，奇怪，難道圖片太大就不行？後來問了下聚合圖牀的人，他那邊一切正常，還很快。我這裏似乎晚上就顯示不出來，其他時候都好的，看來是自己網絡的原因。

#### 11 月 13 日

如果網絡不好，主葉一些 css、js 加載太慢，手機端也太慢，索性全部刪了，用最簡單的文本。

百度收錄了 5 箇網葉。

#### 11 月 15 日

下午試了 WordPress 進階版，一秊 $96，感覺主題都是圖片很多的，而且不知怎麼定制，就算了，幸好可以退錢，不然白瞎了。用 Safari 退不了，只有 Chrome 纔行，眞是奇怪。

想著如何讓百度收錄，一箇辦法是在 coding 建立鏡像。肰而上傳之後，一直是 404。推送本地倉庫到 coding，看 [這箇頁面](https://coding.net/help/doc/git/import.html) 纔行。

又試了下 [這箇](http://data.3gods.com/baiduindex.html)，爲此把 dns 換成 dnspod，但並沒有用。於是又換回來。他的另一箇葉面介紹  [NGINX](https://3gods.com/webmaster/Github-Pages-Baidu-Index-Nginx.html)。

又看到 20180501 之後 gitpages 可以用 https 了，這樣就不用證書了，眞是良心，似乎是 Let's Encrypt 的證書，我在官網上的列表也看到了 git pages。

#### 11 月 16 日

託管平臺從 gitpages 遷移到 netlify。速度快了一些，桌面端可能省了三分之一的旹閒。而且 netlify 自己就集成 dns，不用另外耤助 dns 服務商，也支持免費 ssl。不用什麼教程，跟著一步步來就行。記得把 gemfile 文件中 gem 的網址改成 https://gems.ruby-china.com

最重要的是，**百度** 可以收錄了！喜大普奔！只要這箇平臺不被牆。

#### 11 月 18 日

netlify 有「pretty urls」功能，打開後就沒有後綴 .html，肰而這樣一來，leancloud 就識別不了，評論和閱讀量統計都罷工。突然纔反應過來，關掉就好了。

竟然在桌面網頁看到了谷歌廣告，開心！

### 第三版

#### 11 月 21、22 日

！！！第三版上線！！！

引擎換成了 hugo，主要是我本地 jekyll 上次出問題之後就再也安不上，這次 hugo 使用非常方便。

把文章頭信息改成這樣：

```toml
---
author: ["柯棋瀚"]
title: "Hello world!<n>20181115</n>"
date: 2017-10-04
lastmod: 2018-11-21
categories: ["站務"]
url: /blog/2017/10/04/shuoming.html
---
```

那箇遷移程序不好用，我轉換過來頭信息全部沒了，不知什麼問題。只能手動改，改了兩箇小旹。

攷慮到搜索引擎，所以把老的文章強制制定 url。

netlify 也是有 hugo 引擎的，非常方便，伱都不用選擇。

這箇主題是 Jane，之所以選這箇，之歬試了幾箇，但本地打開要連接好一會，不知什麼原因，只有這箇可以秒開。我懷疑原來的网誌打開很慢是主題問題，而非被牆。

折騰一番後，試了一下，打開速度很快，用一兩秒連接，在 0.5 秒之內就可以加載出來。手機上速度也很快，㝡多比電匘慢一秒。如果用國內主機，應該可以秒開。

一箇神坑：分類標籤等頁面打開是空白。

```toml
[[menu.main]]
  name = "Categories"
  weight = 40
  identifier = "categories"
  url = “/categories/”
```

要去掉 `/categories/` 最後的 `/`。肰而，有些時候又不用刪。大槩玄學

我懷疑是 netlify 的 bnudle 造成的，不能選這箇，只要選 minify 就好。

神奇秘譜指法蠲和尙書周書筆記兩篇文章導致 RSS 輸出出錯，把這兩篇正文刪掉就好了，不知道哪裏出問題。

分割部分的顏色在 base.scss

```css
.bg-llight {
  background-color: $white;
}
```

#### 11 月 22 日

hugo 未免太智能，文章日期寫的 23 號，就眞的不生成。

#### 11 月 26 日

前幾天突肰 lastmod 失效，全部都是現在的日㫷，沒辦法只能用本地生成的。現在問題完美解決： `netlify.toml` 裏面的 `HUGO_ENABLEGITINFO = "false”`卽可。坑爹啊！因爲文檔裏有這麼一句話：

```
.Lastmod
the date the content was last modified. .Lastmod pulls from the lastmod field in a content’s front matter.

If lastmod is not set, and .GitInfo feature is disabled, the front matter date field will be used.
If lastmod is not set, and .GitInfo feature is enabled, .GitInfo.AuthorDate will be used instead.
```



#### 11 月 27 日

歷時五日，定制工作全部完成了，來總結一下：

- 主葉換掉，改成跟第二版一樣的作品展示。把泥爪迻到主葉。
- 葉腳圖標縮小對齊。字號縮小行距縮小，圖標改成「文」。把不蒜子統計迻到葉腳。
- 導航欄的 slideout 刪掉，不習慣小屏幕下還要點一下纔能顯示出欄目。
- 网誌首葉跟弟二版一樣，用歸檔葉面。増加修改旹閒、分類和系列。這樣信息就非常完全，又不會犧牲空閒，翻閱非常方便，滾一下鼠標就可以看到所有的文章。
- 分類枼每篇文章後面増加系列，系列枼増加分類，這樣索引之閒的聯繫非常方便。作者信息枼也増加了系列。
- 分類枼聚合爲一箇葉面，原來是一箇分類一箇葉面。在開頭增加了分類緫目，點擊可直達該分類。
- 増加作者葉面。
- 増加總字數統計，以及各聚合葉面的總字數統計。
- 文章末尾増加「文」圖標，象那些雜誌一樣。
- 把版權信息迻到開頭，修改時間迻到標題下面。版權信息實現懸掛縮進，四箇字的豫畱空閒改成兩箇字。
- 細節方面，標題字號縮小，加粗，改爲黑體。正文行距、字體、葉面寬度都有調整。引文去掉背景顏色，只保留引號，縮進量也進行調整。
- 背㬌顏色換爲黃藍撞色。

緫目葉總字數：

```html
{{ $count := 0 }}
{{ range $paginator.Pages }}
{{ $count = add $count .WordCount  }}
{{ end }}
{{ $count }}
```

分類、系列、作者葉緫字數：

```html
{{ $count := 0 }}
{{ range $pages }}
{{ $count = add $count .WordCount  }}
{{ end }}
{{ $count }}
```

<n>不同主題的定義可能不一樣。</n>最坑的是 `{{ $count = add $count .WordCount  }}` 是 `=` 而非 `:=`，後來在豐的幫助下纔發現這箇問題。

#### 12 月 1 日

Google AdSense 被封了，原來是我自己點得太多。算了，不申訴了，反正廣告費也基本沒有。

#### 12 月 3 日

！！！換域名了！！！

！！！kqh.life！！！

來說一下流程吧：

1. 新建一箇一模一樣的倉庫，用來存放新的域名。
2. 添加 301 重定向。
3. 其他域名郵箱、搜索引擎的設置。

我剛開始還傻傻的把原來的域名刪了，反應過來有問題，又去找回來。

不知什麼神仙操作，BNU-mobile 就連得上，BNU-student 就不行。本來㠯爲是網站 IPv6 的原因，後來還是不行。把本機 DNS kill，再重新添加了一箇，就好了，原來是本機的問題。

#### 12 月 4 日，換域名

！！！換域名了！！！

！！！kqh.ac！！！

「ac」實際上是國別域名，但可解釋爲「academic 」。這樣一共纔 5 箇字母，從 11 箇變成 5 箇，實在是不能再簡潔啦！開心。

把配置文件裏的 CDN 打開，速度一下就飆升：

<img src="https://api.superbed.cn/pic/5c064dffc4ff9e05833a147a" width="800px">

眞是意想不到。

<img src="https://api.superbed.cn/pic/5c07f67dc4ff9e3acfc1ae76" width="800px">

<img src="https://ww1.sinaimg.cn/large/007iUjdily1fxvo6twi1fj313h0u0td8.jpg" width="600px">

達到了 A+。看報告，竟然默認開啓了 HSTS，我一直㠯爲沒有。

#### 12 月 12 日

！！！評論郵件提醒完全可以用了！！！

#### 12 月 13 日

！！！郵件訂閱可以用了！！！

#### 12 月 14 日

看了百度統計的數據，UV 4000 左右，IP 3200 左右，多出來的大部分都是我當初調試的時候產生的吧。重新加上了不蒜子，找 buru 把數據改了，給他說 UV 是 3200 左右。他效率很高呢。

#### 12 月 15 日

增加了作者信息。

增加了每篇文章單獨的 git 鏈接。我現在竟肰會自定義配置項了。

優化网誌首葉樣式。日㫷改成等寬字體。作者改成灰色小黑體。分類上下居中。取消 hover 的動畫。移動端刪掉分類。

#### 12 月 16 日

- 標題樣式優化，和主葉統一。分類和系列分別在標題兩端，用方和圓區分。日期什麼的都用等寬字體
- 版權欄和標題融合在一起
- 一段時間之前，自帶的目錄不知爲何沒了，只好自己加一箇目錄
- 修改郵件訂閱 hover 樣式
- 修改腳註序號 hover 樣式。優化腳註樣式。
- 修改超鏈接 hover 樣式
- 統一了 `$pink` `$dark-gray` 的顏色
- 統一分割線樣式

#### 12 月 18 日

！！！改版了！！！

看到韻典網最近改版了，我突然想改！正文部分改成直排。

```css
writing-mode: vertical-rl;
overflow: scroll;
scroll-behavior: smooth;
-webkit-overflow-scrolling: touch;
```

這樣就可以。再把原來的 padding 之類改一下就好，全部順時針轉一格，比如 `padding-right` 改成 `padding-bottom`，`padding: 1px 2px 3px 4px` 改成 `padding: 4px 1px 2px 3px`。這樣就差不多了。容器的寬度從原來固定値變爲 99%，這樣能適應所有尺寸的屏幕。

我發現直排是㝡適合當前絕大部分人的使用情況的，能鋪滿整箇屏幕。如果豎排的話，只能顯示橫排的 3/5。

#### 12 月 19 日

増加配置項，可以指定是橫排還是直排。

 ```html
{{ if or .Params.vertical (and .Site.Params.vertical (ne .Params.vertical false)) }}
<div class="post-content1">
  {{ if .TableOfContents }}
  <div class="toc"><div class="toc1">{{ .TableOfContents }}</div></div>
  {{ end }}
  {{ if .Description }}
  <div class="description"><div class="description1">{{ .Params.Description | safeHTML }}</div></div>
  {{ end }}
  </div>
<div class="post-content">
  {{ .Content }}
  <i class="heart" style="padding: 0 60px 0 60px;float:right">{{ partial "svg/heart.svg"}}&nbsp\</i>
</div>
  {{ else }}
    <div class="post-content2">
      {{ if .TableOfContents }}
      <div class="toc"><div class="toc1">{{ .TableOfContents }}</div></div>
      {{ end }}
      {{ if .Description }}
      <div class="description"><div class="description1">{{ .Params.Description | safeHTML }}</div></div>
      {{ end }}
      {{ .Content }}
      <i class="heart" style="padding: 0 60px 0 60px;float:right">{{ partial "svg/heart.svg"}}&nbsp/</i>
</div>
    {{ end }}
 ```

把書名號改成波浪線。増加注釋小字。

 ```css
v{
background-image: url(/v.png);
background-repeat: repeat-y;
background-size: 5px;
background-position: left bottom;
padding-left: 5px;
margin: 7px 0 ;
}
n{
  font-family: $global-letter-font-family,$global-note-font-family;
  font-size: 16px;
  padding: 7px 0;
  letter-spacing: 0;
}
 ```

`v` 是波浪線，`n` 是小字。

増加首字下沉：

```css
g{
color: $theme-color;
float: left;
font-size: 2.8em;
margin: 0 -.2em .2em -.5em;
font-weight: 700;
}
```

只能通過手動的方式來進行首字下沉。

現在，實在是太美了，這世界上怎麼能有那麼好看的網頁？？

效果圖：

**加粗的** 用黑體，這樣更加醒目。

下畫直線改成 border，而非原來的 text-decoration，㪅加清爽。

記得橫排的注釋用 n1，下劃線用 u1。

#### 12 月 26 日

增加了古琴、實地錄音、讀中古音的聚合葉面。想象 anyway.fm 那樣做成一箇單獨的網站，想了想沒必要，只是箇人的，也沒有商業化規範化，況且我不止一箇錄音啊。

#### 12 月 28 日

把聚合頁面全部納入博文。雖說感覺怪了一些，但統一一些。

#### 2019 秊 1 月 2 日

修改作者信息的鏈接。首葉作者増加超鏈接。

#### 5 月 18 日

配置文件下面這行就可以解決斜體不能渲染的問題。

```toml
[blackfriday]
hrefTargetBlank = true
extensionsmask = ["noIntraEmphasis"]
```

#### 6 月 14 日

突然發現樣式有問題，safari 下仿宋和楷體都顯示成宋體，Chrome 下正文太髙，超出了一屏，看著很難受。7 月又恢復正常了。

#### 7 月 21、22 日，換域名

**域名從 kqh.ac 遷移到 kqh.me。** 又花了不少代價。以後再也不遷了。遷域名幾箇步驟：

- 在 Google search console 右上角的設置，有「變更網址」。bing 的「站點移動」。百度「網站改版」
- 301 重定向
- 域名郵箱重新設置一下
- valine 的郵件提箱。mailchimp 重新設置。
- 給各箇友鏈小伙伴通知一下。

終於解決了 rss 的問題：配置文件裏面（當然僅限我的主題）`rssFullContent = false` 就可以了。

嘗試了半天 netlify 的 sub-domain，還是不行。

把琴譜網合并到我的維基。域名費也是錢啊。

#### 7 月 23 日

刪掉百度統計，留箇谷歌分析就夠了。百度產品能抵制多少是多少。

主葉更加適配移動端。主要兩點：開頭的大標題，小屏幕下字號變小；聯絡方式刪掉了後面的說明。

把書法、平面索性用圖床來㞡示，不用圖片分享社區了，找了半天沒找到合適的，緫是被牆。

#### 7 月 30 日

關掉百度推送。

#### 8 月 6 日

文件存儲從百度雲盤轉移到 Git LFS。

#### 8 月 17 日

Hugo 0.57.1

由於政策原因，leancloud 國內版必須要綁定域名，把評論和閱讀量統計都刪了。

#### 8 月 20 日

把評論遷移到了 gitalk，還要一箇一箇點開初始化，心累。valine 實在是最理想的評論系統了。不知道國外有沒有類似 leancloud 的平臺。

#### 9 月 29 日

高度從 105%調到了 98%。Firefox、Brave 和 Chrome、Safari 高度不一樣，前者多，後者少，98 剛好能兼容兩者。

#### 10 月 2、3 日

調整目錄

#### 10 月 4 日

把

`{{ if .RSSLink -}}`

`<link href="{{ .RSSLink }}" rel="alternate" type="application/rss+xml" title="{{ .Site.Title }}" />`
`{{ end -}}`

改成了

`{{ with .OutputFormats.Get "RSS" }}`
`<link href="{{ .RelPermalink }}" rel="alternate" type="application/rss+xml" title="{{ $.Site.Title }}" />`
`{{ end }}`

但 RSS 依然有問題，似乎是 Hugo 某次升級之後出現的。

葉腳的不蒜子統計一直有問題，UV 都兩萬多了，暫時撤掉。

更換 logo。

#### 10 月 5 日

修復 RSS。葉腳加入 subscribe。

#### 10 月 9 日

給橫排加上最大寬度 900px，但整個黃色框的範圍我沒法調小，只能用跟直排一樣的寬度。

#### 2020 年 3 月 17 日

評論系統使用 [詔預Isso開放服務](https://open.saintic.com/openservice/isso)。這是國內網站，請在意的讀者注意匿名性。

> 诏预开放平台  
> 您好！  
> 恭喜，您申请接入的Isso服务（名称：f8fn21）已通过审核，现在正常运行中！  
> 接下来，您可以配置客户端了，点我查阅文档吧，您需要的信息如下：  
> 专属的接口根目录（data-isso）： https://open.saintic.com/isso/f8fn21   
> 引用的js文件（embed.min.js）： https://open.saintic.com/isso/f8fn21/js/embed.min.js    

### 第四版

#### 主葉

#### 3 月 23—27 日

見 [網站歷次改版](/221)

#### 3 月 28 日

3.2.0 加大网誌板塊閒距離。a:hover 去掉 border-radius。減淡粉紅色。調整 pagination。

#### 3 月 29 日

3.3.0 適應手機屏幕。去掉紅色。文章去掉表格。3.3.5 晚上增加背景。

#### 3 月 30 日

主頁 3.4.0。增加邊框。增加動畫。訂製了一個和背景圖片襯衫一樣的條紋背景。3.4.1 animation bar 增加淺色，次數.

#### 网誌

#### 4 月 1 日

网誌第四版上線。詳見 [網站歷次改版](/221)。

以前橫排的下劃線、波浪線、註釋都要另外標註，現在在 css 裏面設置一下，所有的都可以統一了，非常舒適了。

4.0.1 原生的 RSS 有問題，每個頁面都把全站的生成一遍，導致非常臃腫。

4.0.2 `img{max-height: 100%;}`

 `vertical` 加框。

#### 4 月 2 日

##### 4.0.3

 `h{line-height}`

`vertical{width}`

`hr{width;height}`

`vertical` 取消上 hr

`tag` 納入 `u-wrappe`

##### 4.0.4

`tag a{color}`

`lastmod p`

`.vertical{`

`vertical { border:}`

`line-height`

`vertical-info`

文件增刪

主葉圖片替換爲 webp，減少 37kb。

##### 4.1.0

`lastmod{max-height: 6em;}`

加入 `pagination.html`？？反正生成時間從 1000ms 降到了 200ms。奇怪。

`cate-wrap`

##### 4.1.1

調整 `.footnotes   `

`a.footnote-ref`

`.vertical hr`

##### 4.1.2

`.des` 變成沒有邊欄的副標題

`.vertical{width: 97%;`

`a.footnote-backref{` 刪除 `writing-mode:horizontal-tb;`

##### 4.1.3

`.vertical h1;blockquote`

加入上下篇。

##### 4.1.4

統一 `date`、`listen`。

修復橫排腳註。

有些橫排的前後都成了 `</n>`，就一個個改。還差一個。

`code{background}`

`.des a`

##### 4.1.5

爲了腳注序號不增大行距，把 `<sup>` hack 了。

取消頁腳上面的分割。

#### 4 月 3 日

##### 4.1.6

`.lastmod`

`.count`

減少距離

`.code{background-color`

`footer.html`

##### 4.1.7

`.archive-info a`

調整 list 那幾個標籤。

##### 4.1.8

文章上方也加入前後篇。

`.toc `

sans 英文字體。

目錄終於可以顯示一級標題，原來是在 toml 中修改。

調大標題字號。

##### 4.2.0

再造。把主葉的 css 合并到了网誌的 css。邏輯終於清晰了。

#### 4 月 4 日

##### 4.2.5

`footer.html`

主葉加入最近修改。

加入序號。想了好久

加入分葉。

##### 4.2.8

把索引移到頁腳。

##### 4.3.0

`.img` 居中

取消葉首，全部移到葉腳。

頁腳採用顛覆式的卡片式設計。

##### 4.3.1

目錄合並到頭信息中。

上下篇字號。

#### 4 月 5 日

##### 4.4.0

加入背景。全面卡片化。主葉的各卡片取消，歸到葉腳中。優化主葉 css。

##### 4.4.1

調整頁碼不在中間的問題。調整頁腳左側一列左邊空隙大的問題。都是因爲 `<li>`

##### 4.4.2

葉腳加入印章。

#### 4 月 6 日

##### 4.4.5

加入智能推薦。感謝 [ops.tips](https://ops.tips/blog/article-recommendation-using-hugo/)

統一 `config.toml`

調低背景飽和度。

調整間距。

`.cover` hover 和居中。

`.col2`

手機端：調整間距；取消背景；調整葉腳顏色。

調整置頂信息、字數統計位置。增加篇均。

優化 seal, v 圖片大小。

##### 4.4.6

葉腳修改日期自動化。

優化智能推薦算法：加入分類、作者。

把下面的上下篇移到智能推薦。

置頂信息移到葉腳。

每葉的作者分類系列移到葉眉。

歸檔按年分塊。

#### 4 月 7 日

##### 4.4.7

改用官方 RSS，限制 30 篇。

主葉的最近更新，原來是所有排完，現在加上限制。並解決有索引頁面的問題。

##### 4.4.8

主頁加入年度🔝10

葉腳索引按數量排序。

##### 4.5.0

主頁改爲發現：加入年度🔝（手動），分類（隨機）。

葉腳加入各索引數量。

#### 4 月 8 日

##### 4.5.1

手機端下取消 `box-shadow`、背景圖案。

解決背景多出來一部分的問題。

作者、分類、系列加上 / [] #。歸檔頁面的索引去掉顏色，改爲這些符號。

`.des1-tag a{color:}`

評論、谷歌分析腳本移到 `footer`。評論腳本放到本地，這樣只剩 XHR 了。

##### 4.5.3

葉腳左側鏈接自動化。

年度🔝自動化。

`layout` 加入 `gallery` `blcok`，作品全放在這裏。又完成一項麻煩的大工程。

#### 4 月 9 日

##### 4.5.4

全面優化上一版。

調整 heading 樣式。

主葉分類隨機排序。

tags 全部換成 series

添加點擊效果。

智能推薦的作者無論如何都沒用，只好刪了。

##### 4.5.5

主葉改版，分爲主葉和网誌發現兩部分。

#### 4 月 10 日

##### 4.5.6

主頁增加維基部分。把分類和年度🔝換位置。

增加更新。調整索引，去掉了一些系列。

`layout` 增加 `block`，關於、更新、友鏈移到這裏，去掉索引。

精簡葉腳信息。

各頁面標題和主頁一致，變成地址欄式的。各索引加上了描述。

爲歸檔葉增加 `section.html`

又把 `tags.html` 拆散了。

增加表格樣式。

#### 4 月 11 日

##### 4.5.7

把网誌拆分成 网誌、赫赫讚府、春秋學刊、作品。一個大工程。用了大半天時間。

增加結構圖。最後還是去掉了葉眉導航欄。

##### 4.5.71

主葉加入 各索引隨機生成一項。

#### 4 月 12 日

##### 4.5.72

博文下加入其他索引。本來想試一下其他索引各一篇，沒成功。

##### 4.5.73

調整主葉發現。還是把版權移到了開頭。

##### 4.5.74

標題加入抖音效果。

##### 4.5.75

主葉赫赫讚府春秋學刊加入描述。

`>` 替換爲 `»`

##### 4.5.76

全局字體大小增大爲 1.15em

##### 4.5.77

取消背景圖案，取消 `box-shadow`

主葉分類調整爲最近發布。

主葉加入訂閱按鈕。

##### 4.5.78

博文分類系列取消按鈕。其他索引生成減爲五項，兩欄。

調整文章信息欄樣式。

##### 4.5.79

修復 4.5.76 的問題。

##### 4.5.80

~~成功實現除了某一索引外的其他索引！！！！！詳見主葉「沒有喜歡的？」排除了赫赫指北。~~ 有問題，先刪了。

細節樣式修復。

#### 4 月 13 日

##### 4.5.81

主葉結構修復。所有頁面統一加上葉腳。

##### 4.5.82

替換 `.URL`

##### 4.5.85

把文章的日期改成實際日期。

赫赫讚府按 `weight` 排序。

優化 `block.html` 等的結構。除了主葉，所有頁面加上葉腳。

各索引頁面加上各自的 RSS。

橫排圖片居中。直排圖片吸頂。

主頁邏輯優化：主葉最近修改，必須是發布日期和修改日期不同的。

增加「其他作者」板塊。

主葉統一標題層級、各框粗細。

##### 4.5.86

葉腳站內鏈接取消 `target="_blank"`

上下篇調整邏輯。

增加目錄樹。[Box-drawing character](https://en.wikipedia.org/wiki/Box-drawing_character)

#### 4 月 14 日

##### 4.5.88

優化單篇 其他索引邏輯：排除自己。

在與本文章的分類系列不重合的文章之中，隨機生成五箇分類，每個分類隨機產生一項。

橫排取消框，字體換為無襯線。

##### 4.5.89

優化手機端。春秋學刊增加徵稿啟事。優化年份樣式。增加各年份統計，年數統計。

#### 4 月 15 日

##### 4.5.91

增加標籤。

每篇文章的分類移到了地址欄。

主葉目錄樹改成 markdown。主頁開頭占整個屏幕，目錄樹變成邊欄。

修復 `list.html` 統計是全站的問題。

##### 4.5.92

文章目錄移到了旁邊，並最大化利用空間。 `vertical` 的高度改為 vh，這樣就能自適應了。

取消手機端文章推薦的滾動。

##### 4.5.93

葉腳樣式調整。

葉腳加入動畫。索引繼續優化。

##### 4.5.94

索引加入 notes，不計入推薦計算。

文章推薦加入加權。

#### 4 月 16 日

##### 4.6.00

春秋學刊數據庫上線。

##### 4.6.01

主葉版式調整。增加數據庫。

##### 4.6.02

增加隱藏修改時間。

#### 4 月  17 日

##### 4.6.03

全面 `| safeHTML `，把《》改成`<v></v>`

優化主葉分類推薦算法

##### 4.6.04

修復：把地址欄移出 `<h1>`

##### 4.6.05

優化：主葉樣式。索引。單篇文章推薦算法。

修復：橫排目錄的位置。

##### 4.6.06

作者的格式改成和其他索引一樣的 `[" "]`。這樣就支持多個作者。

優化：單篇文章推薦樣式。

#### 4 月 18 日

##### 4.6.07

優化：單篇文章推薦算法。主頁分類推薦算法。現在算是徹底定型了。

##### 4.6.08

主頁、歸檔頁調整樣式，取消框框。博客更名網誌。

##### 4.6.09

增加自動暗黑模式。

樣式表統一顏色、字體。

啟用暗黑模式的兩種方法：

https://github.com/ColinEspinas/darken

https://kevq.uk/how-to-add-css-dark-mode-to-a-website/

Firefox 需要在 `about:config` 中啟用 `ui.systemUsesDarkTheme`

#### 4 月 19 日

##### 4.6.10

html5 語意標籤改造。

##### 4.6.11

根據這個，直接用 netlify 的定時生成。

##### 4.6.12

換超連結樣式。

修復上一版 bug。

#### 4 月 20 日

##### 4.6.13

換成了用 actions 來生成。經過觀察，現在完全成功了，每小時生成一次。

##### 4.6.14

加入名言整點更新。包括了尙書、逸周書、墨子、論語、孟子、繁露有關民的。

##### 4.6.15

加入時間戳、運行時長

#### 4 月 21 日

##### 4.6.16

把主葉的手機取消了，加到開頭。

整點更新從 48 句增加到 100 句。

##### 4.6.17

按照這個 https://blog-en.tilda.cc/articles-website-design-mistakes ，把主頁改了一下。

##### 4.6.18

加入過去的本周。

#### 4 月 22 日

##### 4.6.19

把正文的標題層級降一級。步驟：

1. \#### ——\#####
2. \### ——\####
3. \## ——\###
4. \# ——\##
5. \#### ——\###  
6. \##### ——\####  
7. \###### ——\#####

並相應調整 css。

再看了看 PageSpeed Insights，全站各頁面平均 99。非常好。

<img src="https://pic.imgdb.cn/item/5ea00617c2a9a83be5709ceb.jpg" width="500">

<img src="https://pic.imgdb.cn/item/5ea00617c2a9a83be5709ced.jpg" width="500">

#### 4 月 23 日

##### 4.6.20

加入 algolia！！歡呼！！

把琴譜移到本站。

#### 4 月 24 日

##### 4.6.21

乾坤大挪移。維基中有用的都搬了過來，建立新的 section。把維基刪除了。上午讀書搬運完畢。

##### 4.6.22

把推介遷到筆記。
