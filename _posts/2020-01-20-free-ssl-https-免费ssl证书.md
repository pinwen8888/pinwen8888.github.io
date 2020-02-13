---
layout: post
tite: "最全的ssl获取指南"
date:   2020-01-26 17:30:30 +0800
tags: free_things build_websites
color: '#FF6666'
cover: 'https://files4.liangxu.wang/img/security.svg'
subtitle: '最全的ssl获取指南'
---
最近我又开始整ssl证书，而且了解我的人都知道，我是个非常非常穷的人，没有什么钱买每年上百、上千、甚至上万的证书，只能买**免费的**！于是，我这篇文章写出来的也都是**免费的证书了**。

Q:ssl证书是啥？

A:不多废话，去[百度百科](https://baike.baidu.com/item/SSL%E8%AF%81%E4%B9%A6/5201468)、[Myssl资料（特长警告）](https://static.myssl.com/resurces/myssl/bestpractices/HTTPS%D7%EE%BC%D1%CA%B5%BC%F9V1.0.pdf
)了解一下。

Q:为什么要用ssl证书？

A:百度一搜一大堆：Chrome、Safari都已经把http网站标记为不安全，Chrome自从80版本起要求将更加严格，微信强制使用https，http/2基于HTTPS（需要证书），百度、Google提升HTTPS网站排名（具体可见：[又拍云说明](https://www.upyun.com/https)）……

Q:有没有什么方便的证书管理工具？

A:Yep，[KeyManager](https://keymanager.org/)了解一下。

敲黑板了，下面是本人整理了一周多时间整理出来的免费证书颁发以及试用平台，看！好！了！

**重要：请注意证书的有效期：
TrustOcean的免费证书为1年<br>
Let's encrypt证书为3个月；<br>
TrustAsia证书为1年；<br>
Buypass证书6个月；<br>
Rapidssl证书为1个月；<br>
COMODO（Sectigo）证书为3个月；<br>
若平台没有自动续期或你是手动绑定的证书，请在证书过期前记得续期，同时建议到[Myssl](https://myssl.com)输入你的网站，点击右面的“证书到期提醒”订阅。**

## 0.[TrustOcean免费证书](https://console.trustocean.com/cart.php?a=confproduct&i=0)（2020.2.11更新）

![出现此文字请在评论区联系我TrustOcean](https://ae01.alicdn.com/kf/H19005efcc0e14cf4b846fd3560e2df9cW.png)

前几天看夜半观星的文章写着TrustOcean有免费多域名、通配符证书，找了好久还没找到，放弃了。今天突然发现了，我很激动，在这里分享给大家。

**注：可能是因为官方的限制，上面图片里的链接直接访问不行，需点击标题的链接然后再点击右面的“立即试用”来访问。（或者按照下面的图片来操作）**

![](https://img01.sogoucdn.com/app/a/100520146/c1832c0e4e7d946911a1f18e94d16809)

- 支持保护**多条域名（包括通配符，最多3000）**
- 全球信任 SSL证书
- 仅提供社区技术支持
- 非商业保障级别证书

## 1.[sslforfree](https://www.sslforfree.com/)

[sslforfree](https://www.sslforfree.com/)是一个国外的免费在线颁发ssl证书的平台，颁发的证书为[Let's encrypt](https://letsencrypt.org/)的免费DV证书。这个网站我没用过，不过Let's encrypt的证书我还是用过的，我来介绍一下：<br>
它是由一个Mozilla、思科、Akamai、IdenTrust、EFF 和密歇根大学研究人员联合打造的非盈利 CA 项目，由非赢利组织 Internet Security Research Group (ISRG) 运营。<br>

- 官网有教程，但是无法访问（所以请自行百度）
- **保证100%可用性**

## 2.[Certbot](https://certbot.eff.org/)

[Certbot](https://certbot.eff.org/)是一个用Python写的自动化证书颁发程序，由著名的非盈利组织EEF成员编写，是目前为止我看到的唯一一个自动化颁发证书的程序。不过，你需要Shell access来使用它。

- Let's encrypt 官方推荐
- 全自动，证书不会过期
- 需要有Shell access
- **保证100%可用性**

## 3.[Freessl.cn](https://freessl.cn)（推荐）

freessl.cn是一个国内的免费ssl证书颁发网站，我另一个网站的证书就是在这个网站生成的。它GUI做得蛮好的，根据步骤一步一步来应该就可以，只有一点需要注意：在使用“浏览器生成”模式在验证完之后，浏览器会显示三个框，若只复制“证书”框的话，在有的云平台部署会证书链不完整，需点击“下载证书”下载后部署。

- 提供多种证书，有效期最久为1年
- Let's encrypt证书可用性为100%，TrustAsia证书可用性也很高
- TrustAsia证书同一主域*限制申请20张证书*
- 登录后可看到证书控制面板，可自行上传证书、管理证书

## 4.[来此加密](https://letsencrypt.osfipin.com/)

来此加密是一个国内网站开发的和上面提到的差不多的在线颁发ssl证书的网站，截止至几个月前（2019年8月10日），已经累计成功 80264次。它和上面的sslforfree功能一样，自己随便选着用吧。

- 官网有中文教程
- **保证100%可用性**

## 5.[Freessl.org](https://freessl.org)

freessl.org是个GUI神似freessl.cn的免费ssl证书颁发网站，默认语言为英文，不过你也可以设置，注意事项和freessl.cn一样，要注意避免证书链不完整。

- 提供多种证书，有效期最久为6个月
- 登录后可看到证书控制面板，可自行上传证书、管理证书

## 6.[Mianfeissl.com](https://www.mianfeissl.com/)

免费SSL证书是个提供在线生成多种ssl证书的网站，需要注册账号，申请教程[在这儿](https://www.mianfeissl.com/docs/sort_6/pages_44)。若申请过freessl.cn的同学应该就会了，具体过程差不多 ~~差可拟~~。

- 需要注册账号
- 有教程

## 7.[Cloudflare ssl](https://www.cloudflare.com/zh-cn/ssl/)

这个其实*对国内用户不太友好*，因为这只是一个cdn服务，证书不能导出，而且免费版在中国没有节点。但是，我前几天用Myssl检测了一下，发现它们颁发的居然是OV ssl！这还是我**目前看到的唯一一家免费OV ssl**。顺便说一句，对于面向国外的网站，使用它的cdn服务还是挺好的，因为国外访问速度奇快。

- **目前看到的唯一一家免费OV ssl**
- 支持自动续期

## 8.[数安时代Let‘s encrypt](https://certmall.trustauth.cn/Free/)

关于这个，其实我从来没有听过这个公司，翻搜索引擎翻到第3面才看到他，仔细端详一下，它居然还上市了。点击标题上的链接，你就能看到它目前提供的免费证书，是Let's encrypt的。

- **保证100%可用性**
- 有中文教程

## 9.[Zerossl在线工具](https://zerossl.com/free-ssl/#crt)

这是一个提供在线生成ssl证书的网站，看了一眼，是Let‘s encrypt颁发的。我就不多说什么了，和上面的差不多。

- **保证100%可用性**
- 没有中文教程

## 10.[加密啦](https://www.ssl.la/)

这是一个官网上写着“一键免费创建SSL安全证书”的网站，注册账户可能有些问题，可使用文件认证或DNS认证，自己看吧。

- 需要登录

## 11.[金网科技](https://www.kingnettech.com/ssl/freessl/#apply-free-form)

- 一天内免费重新颁发
- 验证支持申请人邮箱验证;域名所有权验证

## 12.[Gethttpsforfree](https://gethttpsforfree.com/)

注意，这个网站需要提供Public key和CSR，csr可以[点击这里](https://www.chinassl.net/ssltools/generator-csr.html)生成，Public key可能需要shell access生成。

- 提供100%可用性
- 可离线使用
- [开源](https://github.com/diafygi/gethttpsforfree)在Github

## 13.[Geotrust试用](https://www.geotrust.com/ssl/free-ssl-certificate/)

这个我感觉实在是没有什么必要，虽然GeoTrust的品牌很响，[GeoTrust官网申请](https://www.geotrust.com/ssl/free-ssl-certificate/)。

**最后，祝大家在鼠年万事如意！希望疫情早早过去！atatc同学 ~~保重~~ 玩得开心！**