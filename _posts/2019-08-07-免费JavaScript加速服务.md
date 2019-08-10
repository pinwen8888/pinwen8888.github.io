---
layout: post
title:  "免费JavaScript加速服务"
date:   2019-08-07 15:40:00 +0800
tags: free_things
color: 'rgb(255,210,32)'
cover: 'https://img.c7sky.com/photobucket/javascript-libraries-cdn_zps1db67ec0.png'
subtitle: '免费JavaScript加速服务'
---
作为开发者，经常会用到一些开源的JS库，这时候一个免费JavaScript加速服务就显得极为重要，因为它最先加载，如果它加载的速度快，整个网站的加载速度也快了。下面我就来盘点一下那些免费JavaScript加速服务。<br>

## [又拍云JS库加速服务](http://jscdn.upai.com/)<br>

> 又拍云为您托管常用的JavaScript库，您可以在自己的网页上直接通过script标记引用这些资源。这样做不仅可以为您节省流量，还能通过我们的CDN加速，获得更快的访问速度。<br>

## [Staticfile CDN](http://staticfile.org/)（七牛云存储提供）<br>

> 我们的目标是提供这样一个仓库，让它尽可能全面收录优秀的开源库，并免费为之提供 CDN 加速服务，使之有更好的访问速度和稳定的环境。<br>

## [75CDN 前端静态资源库](https://cdn.baomitu.com/)<br>

> 360 前端静态资源库是由奇舞团支持并维护的开源项目免费 CDN 服务，支持 HTTPS 和 HTTP/2，囊括上千个前端资源库和 Google 字体库。<br>

## [今日头条静态资源公共库](https://cdn.bytedance.com/)<br>

> 今日头条静态资源库支持多协议、资源动态拼接、快速检索及资源的动态更新,安全、稳定、实时。<br>

## [css.loli.net](https://css.loli.net/)<br>

> 常用前端公共库 & 和谐使用 Google 公共库、字体库的方法<br>

## [新浪 SAE 公共资源](http://lib.sinaapp.com/)<br>

> SAE的为很多流行的开源js/css库提供了CDN加速服务，开发者可以引用我们的js/css库来提升你的应用的访问速度。<br>

## [Google Hosted Libraries](https://developers.google.cn/speed/libraries/)<br>
**重要：由于Google在国内无法访问，请点击上面的链接获取对应的库的链接后，用 ajax.loli.net 替换 ajax.googleapis.com 。**

> 
## [Microsoft Ajax Content Delivery Network](https://docs.microsoft.com/en-us/aspnet/ajax/cdn/overview)<br>

> The Microsoft Ajax Content Delivery Network (CDN) hosts popular third party JavaScript libraries such as jQuery and enables you to easily add them to your Web applications.<br>

## [cdnjs](http://cdnjs.com/) (by CloudFlare)<br>

> The free and open source CDN for web related libraries to speed up your website!<br>

## [cdnjs.net](https://cdnjs.net)<br>

> 永久免费的静态资源公共库<br>

## [jsDelivr](http://www.jsdelivr.com/) (Multi-CDN, 有[国内节点](https://www.jsdelivr.com/network))<br>

> jsDelivr is a public open-source CDN (Content Delivery Network) where anyone can submit a project to be hosted and delivered by our network.<br>

## [unpkg](https://unpkg.com/) (by Heroku & CloudFlare)<br>

> unpkg is a fast, global content delivery network for everything on npm.<br>

注：unpkg使用cloudflare，速度可能会慢，可使用下面列出的知乎或饿了么cdn的网址来代替。<br>

## [饿了么cdn](https://npm.elemecdn.com/)<br>
使用方法如上注。<br>

## [知乎cdn](https://unpkg.zhimg.com)<br>
使用方法如上。<br>


## 综合对比：

| 服务商                                                       | 更新频率 | 国内访问速度 | HTTPS/SSL |
| :----------------------------------------------------------- | :------- | :----------- | :-------- |
| 国内                                                         |          |              |           |
| css.loli.net                                                 | ★★★★★    | ★★★★★        | 支持      |
| 又拍云JS库加速服务                                           | ★        | ★★★★★        | 支持      |
| Staticfile CDN                                               | ★★★★     | ★★           | 支持      |
| 75CDN 前端静态资源库                                         | ★★★★★    | ★★★★★        | 支持      |
| 今日头条静态资源公共库                                       | ★★★      | ★★★★★        | 支持      |
| 新浪 SAE                                                     | ★★       | ★★★★         | 支持      |
| 国外                                                         |          |              |           |
| Google                                                       | ★★★★★    | 无法访问     | 支持      |
| Microsoft                                                    | ★★★★★    | ★★★          | 强制      |
| cdnjs                                                        | ★★★★★    | ★★★★         | 支持      |
| jsDelivr                                                     | ★★★★★    | ★★★★★        | 支持      |
| unpkg                                                        | ★★★★★    | ★★★          | 强制      |
| * 测试文件为各服务商在 http 协议下的 jQuery 2.0.0 minified 版本 |          |              |           |
