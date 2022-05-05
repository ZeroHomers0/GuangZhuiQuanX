# GuangZhuiQuanX

自用QuanX规则，以及一些注释、使用说明

------

## **复制链接进入 quanX -> 点击右下角圆圈(进入后拉到最底端) -> 下载**
``` url
https://raw.githubusercontent.com/JQWS/GuangZhuiQuanX/main/GzQuanX.conf
```
或者
``` url
https://ghproxy.com/https://raw.githubusercontent.com/JQWS/GuangZhuiQuanX/main/GzQuanX.conf
```

## **！注意（必看，你遇到的问题这里都可以解决）！**
   - 节点订阅----自带了免费的代理，每15分钟更新一次，使用前一定要开启资源解析器，记得长按订阅及时更新，切换策略或者导入自己的节点订阅。
   - B站自动换区----方法请参见代码注释,内含BoxJS订阅地址[哔哩哔哩, 港澳台番剧自动切换地区 & 显示豆瓣评分](https://raw.githubusercontent.com/NobyDa/Script/master/Surge/JS/Bili_Auto_Regions.js)，如果使用我的配置则BoxJS配置如图[换区配置](https://github.com/JQWS/GuangZhuiQuanX/blob/main/img/bilibili.jpg)。
   - Hyseen大佬的Netflix 解锁检测和Neflix 策略切换----需BoxJS订阅->[Helge_0x00 脚本合集](https://raw.githubusercontent.com/Hyseen/Scripts/master/QuantumultX/task.json) 如果使用我的配置则BoxJS配置如图[Neflix配置](https://github.com/JQWS/GuangZhuiQuanX/blob/main/img/Neflix.jpg)，具体教程参见毒奶的[BoxJS（With Quantumult X） - Disney+ 和Netflix 策略组批量解锁检测+一键切换节点](https://limbopro.com/archives/19265.html)。
   - tiktok解锁----请勿同时启用多个，最新版tiktok未支持，保持版本在v21.1.0及以下。
   - 京东比价----比价信息显示在商品下方，淘宝比价历史价格在“保障”中显示，需要点击“保障”才能看到，“保障”显示在商品下方，如未生效请清除缓存或重新安装试试（不太准）。
   - 知乎去广告----需要BoxJS订阅，教程->[知乎助手](https://github.com/JQWS/ios_rule_script/tree/master/script/zhihu)，保证知乎广告在分流的位置靠上，至少在国内网站和国内IP池的上方， 或者将规则复制出来放在本地分流'geoip, cn, direct'的上方才能保证有效。
   - 重写，MitM----导入配置之后在quanX设置中开启重写和MitM，之后IOS设置中安装并信任证书，用于Https解析，这一步很重要，必须！ 。
   - 解锁VIP----这里只筛选出来了自己使用的且有效的，包含西窗烛、彩云天气、WPS、有道云、emby、spotify、酷我音乐，如有需要请去这里看看，大部分都失效了，自己尝试->[zwf234](https://raw.githubusercontent.com/zwf234/rules/master/QuantumultX/qxrules.conf)，[Quan Crack 脚本](https://raw.githubusercontent.com/ddgksf2013/Cuttlefish/master/Rewrite/UnlockApp.conf)，并且将此规则保持在重写规则顺序靠上的位置，这样才有用。
   - 代理模式----请启用规则分流代理模式，方法见->[代理模式](https://xtrojan.cc/client/quantumult-x.html#guan_yu_dai_li_mo_shi)，这一步也很重要， 规则分流就是国内请求直连不走代理，国外走代理，并且按照设置的策略组走各自的代理，这样quanX可以一直开着访问任何网站都互不影响。 请单击软件右下角的功能按钮，然后在新窗口拉到最下面点击其他设置，在模式中选择‘规则分流’，或者长按右下角功能按钮选择‘规则分流’。
   - 广告拦截----该策略组起作用需选择REJECT，如果例如游戏中需要看广告获取奖励则广告拦截策略组选择direct。
   - 隐私拦截与运营劫持在去广告中已经包含，知乎去广告的重写和B站去广告重写在去广告AllInOne的重写中包含，这些规则请勿重复添加。
   - 关于task脚本----我的脚本用青龙挂在了服务器，所以这里就不提quanX的脚本订阅了，需要的朋友这里放一个教程[青龙教程合集](https://www.notion.so/1c598629675145988b43a37998a1604a)。
   - 最后----只维护个人使用的配置，如有需求请自己动手。

## **说明**
1. 以下为QuanX配置教程
   - [Quantumult X 官方示例](https://github.com/crossutility/Quantumult-X)
   - [Quantumult X 不完全教程](https://www.notion.so/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917)
   - 推荐（因为比较简单，适合小白）->[小白教程](https://xtrojan.cc/client/quantumult-x.html)
   - 推荐（对软件介绍及玩法比较详细）->[QuantumultX 使用教程：策略组&分流规则&自定义图标&过滤节点的进阶玩法](https://limbopro.com/archives/3846.html)
   - [BoxJS官方文档](https://chavyleung.gitbook.io/boxjs)
   - [毒奶配置示例](https://raw.githubusercontent.com/limbopro/Profiles4limbo/main/full.conf)
   - [KOP-XIAO配置示例](https://raw.githubusercontent.com/KOP-XIAO/QuantumultX/master/QuantumultX_Profiles.conf)
   - [少年歌行pro](https://ghproxy.com/https://raw.githubusercontent.com/sngxmini/QuanX/main/sngx2021.conf)
   - ↑以上三个配置均为大佬的懒人配置，里面也有一些参数说明，觉得合适可以试试。

2. 免费节点及机场推荐

   - [分享来自互联网上免费的shadowsocks(SS)/ShadowsocksR(SSR)/V2ray(vmess)代理 每15分钟更新一次，每次各分享4个临时可用代理。](https://github.com/JQWS/free_proxy_ss)
   - [SS/SSR/V2Ray/Clash 简介和客户端软件下载](https://congcong0806.github.io/2018/04/20/SS/)

3. 以下为分流&复写&JS备份大佬的仓库，以防原仓库被封禁，但配置中除了某些删库的以外仍使用原作者仓库。

   - 整合分流&复写
      - [各平台的分流规则、复写规则及自动化脚本](https://github.com/JQWS/ios_rule_script)
   - NobyDa规则&JS
      - [NobyDa](https://github.com/JQWS/Script)
   - KOP-XIAO资源解析器
      - [QuantumultX资源解析器](https://github.com/JQWS/QuantumultX)
   - DivineEngine规则分流及复写
      - [DivineEngine规则](https://github.com/JQWS/Profiles/tree/master)
   - Orz-3
      - [Orz-3](https://github.com/JQWS/QuantumultX-1)
   - 少年
      - [Oreomeow](https://github.com/JQWS/QuanX-1)
      - [少年](https://github.com/JQWS/QuanX)

4. 京东全自动退会

   - [京东全自动退会](https://github.com/JQWS/JDMemberCloseAccount)

5. 图标

   - [Quantumult X Policy Icon Set](https://github.com/JQWS/Qure)
   - [mini icon](https://github.com/JQWS/mini)
