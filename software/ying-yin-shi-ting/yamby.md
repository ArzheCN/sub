---
cover: ../../.gitbook/assets/未命名的设计 (1).png
coverY: 0
---

# Yamby

### 介绍

长久以来，第三方emby客户端一直活跃在IOS平台上，出现了一大批优秀的软件，比如infuse、fileball、vidhub、影音宝等app，究其原因是因为iOS端安装破解软件较为困难，且官方emby客户端体验较差。

回到安卓端，大部分人都在用小秘开发的修改版Emby客户端，这版客户端优化了很多功能，比官方客户端更加完善

前不久，一款名为Yamby的软件开始在各大tg群内传播，那时候还是内测阶段，只有部分人能下载到这个软件，而最近他已经进入了公测阶段，安装包也放了出来，大家可以自行去下载体验。

目前软件的UI对大部分设备都支持的比较好，如果大家遇到问题可以去反馈一下看看。软件的UI整体来说比较美观，图片加载不会像emby那样一行一行出来，版本选择字幕选择音频选择等功能也很完善，还可以调取 弹弹Play 的弹幕接口，一般动漫资源会有比较多弹幕。由于是国人开发者（据说就是小秘），相信日后也会针对国人常用的观看emby公益服需求进行完善。

功能方面，基础的必备功能都免费提供，且主界面上没有Pro版广告或购买入口，非常干净，如果不是别人告诉我第一次用我还真不知道还可以买Pro版。目前软件还没有上架Google play平台，上架后会开启购买渠道，Pro版主要是提供了MPV播放器支持，可以添加更多的服务器，可以更改主题色等功能，据说价格也不是很贵，有能力的可以支持一下

目前该软件仍处于测试阶段，如有问题欢迎大家去反馈

### 最近更新日志

✍️新版变化\
适配多语言\
优化搜索结果显示\
增加自定义多版本选择\
增加封面评分\
🎉版本\
1.0.2\
✨更新时间\
北京时间 2024年 04 月 18 日\
🤖所需操作系统\
Android 7.1及更高版本

✍️新版变化\
增加竖屏播放\
增加删除最近观看\
优化播放器UI\
修复拼写错误\
修复部分显示效果\
修复倍速调整逻辑\
修复手势操作过于灵敏\
加商店账号登录\
增加元数据编辑功能\
重制MD3主题色\
适配横屏封面库\
优化演职人员详情页\
进度条增加动态模糊\
增加视图选择\
增加排序记忆\
🎉版本\
0.9.64\
✨更新时间\
北京时间 2024年 04 月 12 日\
🤖所需操作系统\
Android 7.1及更高版本

### 内测用户留言

> 卑微『南瓜』 /闭嘴版🤐:\
> 说一下收费，我现在在参加内测，标pro功能的都是可有可无，不影响日常使用的，即使不开会员照样用，就是换个颜色，增加服务器上限什么的
>
> 服务器上限开个分身就解决了，就是可能比麻烦
>
> MVP其实不影响使用，只不过就是字幕方面不能显示那个艺术体后续要是支持外部播放的外部播放完事
>
> 他当时MVP播放器啥都没加，没pro功能的时候我就开始用，使用起来没毛病

### 开发者QA

> Q：同一个播放环境，Emby客户端都能看，而yamby有些视频能看，有些视频播放报错？
>
> A：非 PRO 版本使用的是几乎未添加拓展的 EXO 播放器，只能使用硬解，无法使用软解。硬解效率高，但只能播放dsp等硬件设计支持的格式；软解效率低，但兼容性好。\
> 常见安卓端不支持硬解格式有：yuv444，h.264 10bit，rmvb等\
> 未来可开通 PRO 版本时使用 MPV 播放器，可以软硬解切换，这些格式便可以播放。
>
> Q：双语字幕重叠，样式错乱等ass字幕问题
>
> A：上文已说非 PRO 版本使用的是几乎未添加任何拓展的 EXO 播放器，所以只对ass字幕有最基础的支持，mpv使用的libass可以解决这些问题 来源
>
> Q：Emby 客户端不也是 EXO 播放器吗为什么它没有这些问题？
>
> A：EXO 播放器作为一个开源库，可玩性很高，Emby 客户端中的 EXO 经过长时间魔改已经十分完善

<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

### 下载地址

<table data-view="cards"><thead><tr><th></th><th></th><th></th><th data-hidden data-card-cover data-type="files"></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td></td><td>官方Telegram频道</td><td></td><td><a href="../../.gitbook/assets/image (5).png">image (5).png</a></td><td><a href="https://t.me/yamby_release">https://t.me/yamby_release</a></td></tr><tr><td></td><td>123云盘</td><td></td><td><a href="../../.gitbook/assets/image (6).png">image (6).png</a></td><td><a href="https://www.123pan.com/s/eIAZjv-f6V1H.html">https://www.123pan.com/s/eIAZjv-f6V1H.html</a></td></tr></tbody></table>
