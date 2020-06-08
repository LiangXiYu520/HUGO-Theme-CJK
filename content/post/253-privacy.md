---
author: ["柯棋瀚"]
title: "本站的隱私、安全、速度 privacy policy"
date: 2020-06-07
categories: ["站務"]
tags: ["coding"]
description: '我有必要將本站所有涉及隱私的情況完全透明展示給您。'
vertical: false
---

## 隱私

以下服務會直接記錄您的信息（高敏感）：

- 诏预 Isso 評論服务（國內網站，我無法直接管理）
- Google Analytics 流量分析（由我直接管理）

以下服務可能會記錄您的 IP 地址（中敏感）：

- 托管於 Netlify（我無法直接管理）
- 聚合圖牀（國內網站，我無法直接管理）

還使用了如下腳本（低敏感）：

- Algolia 搜索（我無法管理）
- InstantPage（我無法管理）

## 安全

只要用 Netlify 託管，一般的 SSL 測試很容易得到 A+：

- [Qualys](https://www.ssllabs.com/ssltest/analyze.html?d=kqh.me&s=104.248.50.87)：A+
- 國內的 [MySSL](https://myssl.com/kqh.me?status=q)：A+

<img src="https://pic.imgdb.cn/item/5edd84dac2a9a83be5a65cd8.jpg" width="600">

無意間發現 [webbkoll](https://webbkoll.dataskydd.net/en)，測試有很多問題，便按照指引補了一下安全漏洞。

我託管於 Netlify，在根目錄下新建響應頭純文本文件，名爲 `_headers` ：

```
/*
Referrer-Policy:no-referrer
Strict-Transport-Security:max-age=31536000;includeSubDomains;preload
X-Frame-Options:DENY
X-Content-Type-Options:nosniff
X-XSS-Protection:1;mode=block
Content-Security-Policy: block-all-mixed-content
```

本來還加了 CSP，這樣就顯示通過測試：

```
Content-Security-Policy:default-src https:;base-uri 'none';object-src 'none';form-action cdn.jsdelivr.net open.saintic.com/isso/f8fn21/js/embed.min.js;img-src *;script-src 'unsafe-inline' cdn.jsdelivr.net googletagmanager.com google-analytics.com open.saintic.com/isso/f8fn21/js/embed.min.js;style-src cdn.jsdelivr.net 'self';frame-ancestors 'none' 
```

但搜索功能沒法工作，不想去硏究了，索性去掉。

<img src="https://pic.imgdb.cn/item/5edd0bbbc2a9a83be5ee01f3.jpg" width="500">

合格的有：

<img src="https://pic.imgdb.cn/item/5edd0b4bc2a9a83be5ed1f5c.jpg" width="700">

<img src="https://pic.imgdb.cn/item/5edd0b4bc2a9a83be5ed1f57.jpg" width="600">

<img src="https://pic.imgdb.cn/item/5edd0b4bc2a9a83be5ed1f53.jpg" width="600">

<img src="https://pic.imgdb.cn/item/5edd0b4bc2a9a83be5ed1f51.jpg" width="700">

不合格的：

CSP 和 SRI

<img src="https://pic.imgdb.cn/item/5edd0b4bc2a9a83be5ed1f47.jpg" width="700">

CSP, Content Security Policy 是一個白名單，告訴瀏覽器能加載哪些資源。

SRI, Subresource Integrity 是一個核對清單，將遠程加載資源的 sha 値與你設置的進行對比，相同的就可以加載。

## 速度

- 使用 [InstantPage](https://instant.page/) 腳本，實現站內預加載
- 生成時使用 `hugo --minify`，把 css、js 壓縮到最小
- js 放在最後，竝使用延遲加載、異步加載
- 無框架；無多餘 js

PageSpeed Insights：電腦上全站各頁面平均 98。非常好。

<img src="https://pic.imgdb.cn/item/5ea00617c2a9a83be5709ceb.jpg" width="700">

<img src="https://pic.imgdb.cn/item/5ea00617c2a9a83be5709ced.jpg" width="700">