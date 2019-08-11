---
layout: post
title:  "利用wxpy快速创建微信机器人"
date:   2019-08-04 15:40:00 +0800
tags: python
color: '#FF9933'
cover: '/img/wxpy.png'
subtitle: '利用wxpy快速创建微信机器人'
---
> python是个好东西。为什么？第一，当然是因为TA简洁易懂，第二，是因为TA支持强大的三方库。<br>

今天，我就给大家介绍一个强大的python第三方库——[wxpy](https://wxpy.readthedocs.io/zh/latest/)。<br>
它到底有多强大？虽然这个第三方库基于itchat（也是一个强大的操控微信的第三方库），但是却比它简单地多。简单到什么程度？按照官方文档以及我自己的使用 创建一个微信机器人只需要2行代码。代码如下：
```python
# -*- coding: utf-8 -*-
#本程序对python2.7，3.3及以上有效
from wxpy import *
bot=Bot() 
'''
如果你在服务器上用ssh执行程序，看不见打开的图片，可以在括号里加上console_qr=True, 若二维码变形则加上console_qr=1或其他倍数
'''
#后面就是你的代码，我会示范一些，Happy coding
my_friend = bot.friends().search('你朋友的微信名,若有备注名则是备注名')[0]
#自动回复朋友的消息
@bot.register(my_friend)
def reply_my_friend(msg):
    return '你要发的消息{}'.format(msg.text)
'''
msg.text是朋友发送的消息，引号内的中括号也是ta发送的消息
'''
another_friend = bot.friends().search('只要和刚刚那个不一样就行')[0]
tuling = Tuling(api_key='请在图灵机器人平台自行注册并获取api_key')

# 使用图灵机器人自动与指定好友聊天
@bot.register(another_friend)
def reply_another_friend(msg):
    tuling.do_reply(msg)

# 自动接受新的好友请求
@bot.register(msg_types=FRIENDS)
def auto_accept_friends(msg):
    # 接受好友请求
    new_friend = msg.card.accept()
    # 向新的好友发送消息
    new_friend.send('哈哈，我自动接受了你的好友请求')

embed() #保持程序持续运行
```
本人只是列举了wxpy的一些用法，更多用法等着你去官网发掘！🙂
