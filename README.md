# CU學生內地上網資料彙總

因为一些众所周知的原因，内地的网络环境让我们十分不想学习，面对着怎么都刷不出来的blackboard和时不时就会崩掉的onedrive，再加上永远无法连接的google，简直会让我们放弃学习。那么这篇文章就是来拯救你的，笔者将自己实现网络自由的方法以及所参考资源都列在这里，希望网络不会成为大家在苦难时期学习的掣肘。

*有钱没时间想快速解决问题参见 操作-选购服务- https://bywave.fun/aff.php?aff=56*

## 基础

1. 关于CU 未批恩

   有一说一，2019十一十二月份因为很少人在学校，CU 未批恩的性能还是非常棒的，在300M宽带下YouTube能跑到十几万分，4K视频秒开。可是等到一月份网络压力变大，CU 未批恩在YouTube下只能达到500分，大概是50KB/s. 在最近社会怨气加重的情况下，防火墙势必会越来越高，因此使用CU 未批恩不再是一个合适的选择。更别提在网络环境不好的时候根本无法连接。

2. 广泛使用的科学学习方式

   需要指出的是，现在更加安全快速和流行的科学学习方式不再是在App Store下载某某某加速器某某某未批恩（不排除其中有很好的产品，但是已经不推荐了）。更新的方式是基于一些设计好的加密协议，帮助你连接到境外的某台服务器（即电脑），然后使用这台电脑的网络来上网。在这种环境下，我们的科学学习方式是各个平台都通用的，即iOS，Android, Windows, macOS, Linux... 

   关于不同的平台你需要下载什么工具，这里给出通用的工具。

   iOS：Shadowrocket（付费），Potasto Lite(免费，不支持V2Ray)

   Android：Shadowrockrt

   Windows: 搜索 小飞机

   macOS: Shadowsock-X-NG-R8， V2rayU

   Linux: If you use this system, I believe you can find by yourself

一个相对全面的软件使用方法 https://ohssr.bid/user/tutorial

**需要指出的是，上面链接中的服务商已经不维护他们的服务了**

**千万别买**

## 操作

1. 关于自己搭建
   1. 我要自己搭！！

      如果你选择自己搭建，请找工科学生帮忙，尽管目前有很方便的一键脚本，但是一些关于UNIX系统的操作还是很麻烦，遇到问题就问，

   2. 哪里搞服务器

      鉴于大家可能只是在家待很短的事件，建议AWS或者谷歌云，谷歌云凭借中大信用卡可以得到300USD的试用额度，够用了

   3. 搭建什么服务

      * 唯一推荐搭建V2Ray，一个比SSR更先进的协议，详情参见官网 https://www.v2ray.com/， **但是**，单纯的V2Ray没法带来很快的网速，**需要开启BBR** 加速。

      * 233一键脚本里整合了BBR加速的模块，这是目前搭建V2ray最方便的脚本[https://github.com/233boy/v2ray/wiki/V2Ray%E4%B8%80%E9%94%AE%E5%AE%89%E8%A3%85%E8%84%9A%E6%9C%AC](https://github.com/233boy/v2ray/wiki/V2Ray一键安装脚本)

      * 关于tls和Torjan：此方法门槛较高，如果您有意研究或补充请PR。简单来说，**这是一种几乎没有办法封锁的科学联网方法**

2. 关于选购什么服务

   上面已经提到，最近的树洞及其回复也已经提过，ssr已死，大家尽量购买V2Ray服务商，这里推荐一个 https://bywave.fun/aff.php?aff=56

   20RMB50GB，可以看Netflix和Hulu，这是上面提到的自建方法很难办到的（需要DNS解锁）。

   这是本人用的最爽快的没有之一了，其他的几鸡和Baji等等在各方面都优缺点。而且这个服务商的客服可以做到秒回，出问题也很好解决。

## 后备资源  

不能一成不变！

推荐文章：

* https://program-think.blogspot.com/2009/05/how-to-break-through-gfw.html 新手扫盲 by 编程随想



推荐YouTube Channel：

* 洋葱
* JS神技能

## 关于Telegram

保护你的隐私，不用怕你说的话被mei sun看到，telegram用起来

tg中有很多实用的频道和群组，能帮你把握最新消息



## 程序员Tips

* How to solve "git clone is so slow"

  use this config in your .gitconfig file

  ```
  [http]
      proxy = socks5://127.0.0.1:1081
  [https]
      proxy = socks5://127.0.0.1:1081
  
  ```

  Here I use the port 1081, check your **Local Sock Listen Port** in the sfotware you use

* "pip install" is so slow

  Find mirrors for these resources. Search "tuna thu mirrors



暂时只能想到这么多，足以给大家带来媲美甚至超越香港的网络体验。

祝愿大家在特殊时刻能够静下心来安心学习，弯道超越。

仓促写成，总结了一些实用的适用于小白的经验，如有不完善之处，请提出issue或者在 t.me/CUSaveYourself 中滴滴（telegram频道）。