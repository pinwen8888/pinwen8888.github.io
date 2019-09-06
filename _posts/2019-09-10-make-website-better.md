---
layout: post
title:  "网站优化"
date:   2019-09-10 17:00:00 +0800
tags: free-things web
color: '#99CC99'
cover: '/img/seo.svg'
subtitle: '网站优化'

---

嗨，我前几天写了一篇老长老长的文章。在文章的结尾，我说要在下一篇文章介绍网站优化。这不，“下一篇文章”来了。<br>

网站优化不是一件简单的事情。小到个人博客，大到商业网站，只要是优秀的网站，都会耗费大量的时间来做网站优化。为什么它如此重要？这是因为，只有把网站优化做好了，比如，提升加载速度，才能更好地留住访问者，**保持（甚至提升）网站流量。**<br>
下面就是我捣腾N年的结果，希望对你有帮助。<br>

## 一、网站分析<br>

### 1.[百度统计](https://tongji.baidu.com)<br>

> 全球最大的中文网站流量分析平台。<br>

这是官网上的评价。我相信，因为大部分国内的站长无法访问Google Analytics。国内有些站长说百度统计会乱显示，这是不对的（距离产生美）。百度统计的应用范围不止在于网站，也支持移动应用。你可以在[这里](https://tongji.baidu.com/web/demo/overview/index?siteId=5503017)查看控制面板示例。<br>

- 在国内访问速度特快<br>
- 大公司，不怕倒闭<br>

### 2.[Google Analytics](https://analytics.google.com/)（中国大陆无法访问）<br>

注：鉴于中国大陆境内的网络状况，**在中国大陆境内无法访问Google Analytics（但是可以正常使用）**。请使用百度统计或者被的统计工具。<br>

Google Analytics是由Google推出的分析服务，虽然它没有说，但想也不用想，它肯定是全球最大的网络分析工具。和百度统计不同，它不支持移动分析。和[Google Adsense](https://www.google.cn/adsense)配合，它还能显示出网页价值（即每页广告赚的钱）。这点对企业来说很有用。~~不过，不幸的是，由于这也是Google的服务，在中国大陆境内访问慢。~~经17ce检测，GA居然有国内Ip，下载速度也挺快，我就不说什么了。<br>

- 在国内访问速度还行<br>
- 不需要怕倒闭<br>
- 数据类型多样<br>

### 3.[CNZZ](https://web.umeng.com/main.php?c=user&a=index)<br>

CNZZ也是一个在中文网站中有不少人用的一个网络分析，现在改名叫友盟，也做移动分析。<br>

### 4.[腾讯分析](https://ta.qq.com/analysis/index)<br>

腾讯分析从2011年开始运营，至今仍然在运营，虽然页面从2012年起从未改变，但是也从未下线。<br>

### 5.[51LA](https://www.51.la/)<br>

据官网介绍，它已经服务了19,450,579个网站（截止到2019.08.31）。看着Demo还行，我没用过，自己选吧。<br>

## 二、SEO（Search Engine Optimise，搜索引擎优化，很重要）<br>

SEO是另一个非常重要的事情，自从世界上第一个好用的搜索引擎Google于1998年成立后（之前的搜索引擎都很慢），几乎所有的人访问没访问过的网站都是从搜索引擎进入的。因此，SEO是头等大事。SEO有很多种途径，我将列举几种方法和建议。<br>

### 1.创建sitemap.xml<br>

守规矩、主流的搜索引擎都会抓取sitemap.xml，因为这提升了它们的抓取时间。个人博客建议每写完一篇博客都把它加到sitemap。创建完成后，请务必将Sitemap添加到robots.txt（参照[本博客](https://pinwen.cc/robots.txt)）。<br>

### 2.创建robots.txt<br>

搜索引擎也会抓取robots.txt。一般，你只需要把你的Sitemap写在robots.txt里就行了。如果在网站里有个人隐私或者其他你不想让搜索引擎抓取的信息，就写在Disallow里。冒号后面一定要有空格。具体写法参照[GIthub](https://github.com/robots.txt)和[本博客](https://pinwen.cc/robots.txt)。<br>

### 3.零碎的一些建议<br>

下面一些建议大多很有用，从原理上优化搜索结果。<br>

1.不要大量使用Flash<br>

现在，Adobe已经宣布于2020年停止支持Flash插件。各大主流浏览器也默认屏蔽Flash。Flash还会导致搜索引擎难以抓取。Flash还很耗电，极大地降低了用户体验。如果你有视频需要播放，你可以使用[西瓜视频播放器](https://h5player.bytedance.com/)，有很多功能。<br>

注：哔哩哔哩视频下载点[这里](https://pinwen.cc/2019/09/15/%E4%B8%8B%E8%BD%BD%E5%93%94%E5%93%A9%E5%93%94%E5%93%A9%E8%A7%86%E9%A2%91.html)<br>

2.不要把大量内容转化成图片<br>

由于搜索引擎要抓取所有的网站，很占CPU，肯定没有空识别图片里的文字。所以它只能抓取文字内容。不要抱怨，这已经很好了。我们要做的就是尽力方便搜索引擎抓取我们的网站。<br>

## 三、评论系统<br>

评论系统可以方便你和用户之间的沟通。别忘了，用户就是上帝，我们要尽全力为用户服务。评论系统也是我倒腾了很久的结果（生命在于折腾）。<br>

### 1.[来必力](https://www.livere.com/)<br>

来必力是一个韩国公司开发和运营的评论系统。我最看重它的地方是它集成了很多国内社交网站的登录系统（因为很难申请）。还有，它在国内备了案，不会突然出现访问不了的时候。我的博客现在就用的是来必力的评论系统，你可以滑到页面的底部或者点击右面的“FOOT”查看示例。<br>

### 2.[Utterances](https://utteranc.es/)<br>

Utterances是一个基于Github issue的评论系统。它其实并没有别的git-issue的评论系统火（比如[Gitalk](https://github.com/gitalk/gitalk)、[Gitment](https://github.com/imsun/gitment)），但是我看中的是它的方便。使用它并不需要注册自己的OAuth App（别的都需要），而且每次使用也不需要手动初始化。只要把你的Github Repo连接到它的Github apps，就可以开始使用了。具体详情可以[参考这篇文章](https://nusr.github.io/post/2019/2019-05-04-utterances-introduce/)和官网。<br>

### 3.[DISQUS](https://disqus.com)（中国大陆无法访问）<br>

**注：鉴于中国的网络状况，DISQUS在中国大陆境内可能无法访问。来必力在中国大陆境内备了案，不会出现无法访问的情况，你可以使用。**<br>

DISQUS是一家国外的评论系统。由于在中国大陆它无法访问，建议只有做面向国外的网站的人使用。虽然也有人做了一个什么api，但是它也没有中国的社交网站登录。它的安装倒是挺简单，直接复制代码就可以了。请自行选择。<br>

## 四、内容分享系统（不必须）<br>

### 1.[Share.js](https://github.com/overtrue/share.js)<br>

Share.js是一个用JavaScript编的很好的内容分享系统。它的加载速度还挺快，支持多家社交媒体。具体配置和使用见官方Github主页。<br>

### 2.[AddToAny](https://www.addtoany.com/)<br>

AddToAny是一个国外的分享平台，如果你的网站面向国外，你可以使用。<br>

### 3.[AddThis](https://www.addthis.com/)（加载速度奇慢）<br>

**注：可能是因为没有国内的服务器的原因，AddThis在国内加载速度奇慢无比（移动设备上有时候要加载一分多钟。建议只有面向国外的网站使用。**<br>

Addthis也是一个国外的分享平台，加载速度挺慢。和它类似的有AddToAny。国外的分享平台有一个共同的缺点：分享到国内的平台都有点烦.所以还是建议国外的站长使用。<br>

我来总结一下：在这几类中，SEO最重要，有些也可以使你的网站更好。建站愉快O(∩_∩)O~~<br>
