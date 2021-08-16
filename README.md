# 映画云盘使用手册

本手册专为 [**映画云盘**](https://disk.onji.cn/) 编写，收录了云盘相关的各种问题。

本手册正文包含：
[云盘相关](#云盘相关)、
[注册](#注册)、
[登录](#登录)、
[安全](#安全)、
[常见问题](#常见问题)、
[进阶问题](#进阶问题)、
[充值购买](#充值购买)
七部分，除此之外，正文之后还有[隐藏福利](#隐藏福利)。
遇到问题请优先查询本手册，或者 [Google](https://www.google.com/)，
在自己尝试解决问题却无法解决后，请咨询客服，描述问题请参考 [提问的智慧](https://github.com/ryanhanwu/How-To-Ask-Questions-The-Smart-Way)，仅在此处提醒，若是本手册所包含的内容，客服有权不予回答，后续不再提示，周知。
本手册并不完全，如果遇到好的问题，您可以提 [issues](https://github.com/W-W336/YINGHUA/issues)，我们会在判断后有选择地进行修改，如果您有好的想法欢迎PR。

在使用中，请善用网页搜索，电脑端可使用 Ctrl+F 打开网页搜索，手机端请在网页菜单中自行寻找网页搜索。

## 声明：
本文全程在 [纯纯写作](https://writer.drakeet.com/) 进行编辑完成.<br>
一个令人感到安心、拥有历史记录、段间距、多重防止文章丢失功能，和许多写作辅助的编辑器。<br>

本文参考了 [Ayaginu-Sue](https://github.com/Ayaginu-Sue) 编写的 [纯纯写作使用手册](https://github.com/Ayaginu-Sue/purewriter).<br>
一份非常详尽以及清晰明了的用户使用手册。<br>

内容按照 [中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines/blob/master/README.zh-CN.md) 进行排版，以保证内容的可读性。

## 目录

<!-- TOC -->

- [云盘相关](#云盘相关)
    - [云盘运营](#云盘运营)
    - [云盘收费](#云盘收费)
    - [云盘规则](#云盘规则)
- [注册](#注册)
    - [注册注意事项](#注册注意事项)
    - [注册邮件找不到](#注册邮件找不到)
- [登录](#登录)
    - [登陆方式](#登陆方式)
    - [登陆出现的问题](#登陆出现的问题)
        - [Backend is not running!](#Backend-is-not-running)
        - [提示用户邮箱或密码错误](#提示用户邮箱或密码错误)
        - [登录提示“参数错误”](#登录提示参数错误)
- [安全](#安全)
    - [绑定第三方账号（目前仅支持 QQ）](#绑定第三方账号目前仅支持-QQ)
    - [解绑 QQ 账号](#解绑-QQ-账号)
    - [忘记密码及密码修改](#忘记密码及密码修改)
        - [登陆账号前](#登陆账号前)
        - [登陆账号后](#登陆账号后)
    - [外部认证器](#外部认证器)
    - [两步验证](#两步验证)
- [常见问题](#常见问题)
    - [文件列表展示方式](#文件列表展示方式)
    - [寻找对应类型文件](#寻找对应类型文件)
    - [文件排序](#文件排序)
    - [黑暗模式的开启](#黑暗模式的开启)
    - [主题配色修改](#主题配色修改)
    - [收起侧边栏](#收起侧边栏)
    - [数字 UID](#数字-UID)
    - [字母 UID](#字母-UID)
    - [注册时间](#注册时间)
    - [积分查询](#积分查询)
    - [用户组到期时间](#用户组到期时间)
    - [修改头像](#修改头像)
- [进阶问题](#进阶问题)
    - [打包下载](#打包下载)
    - [在线解压缩功能](#在线解压缩功能)
    - [WebDAV 使用指南](#WebDAV-使用指南)
        - [何谓 WebDAV?](#何谓-WebDAV)
        - [WebDAV 功能的网页配置](#WebDAV-功能的网页配置)
        - [WebDAV 功能的本地配置](#WebDAV-功能的本地配置)
        - [WebDAV 账号管理](#WebDAV-账号管理)
        - [WebDAV 设置](#WebDAV-设置)
    - [上传问题](#上传问题)
        - [上传组件还未加载完成](#上传组件还未加载完成)
        - [上传失败](#上传失败)
        - [文件夹上传](#文件夹上传)
        - [单文件上传大小](#单文件上传大小)
    - [离线下载](#离线下载)
        - [怎么进行离线下载](#怎么进行离线下载)
        - [是否支持选择文件下载](#是否支持选择文件下载)
        - [下载出错](#下载出错)
        - [离线文件存储路径](#离线文件存储路径)
        - [磁力转换](#磁力转换)
        - [为什么有的磁力链离线速度很慢？](#为什么有的磁力链离线速度很慢)
        - [添加离线下载任务后显示“未知”](#添加离线下载任务后显示未知)
        - [文件转存失败](#文件转存失败)
        - [任务添加成功却看不到任务](#任务添加成功却看不到任务)
        - [查看资源下载的事件](#查看资源下载的事件)
        - [很早的资源看不到记录](#很早的资源看不到记录)
        - [“转存处理中”是什么意思？](#转存处理中是什么意思)
        - [一直处于“已完成，转存处理中”](#一直处于已完成转存处理中)
        - [转存为什么比离线慢](#转存为什么比离线慢)
    - [分享管理](#分享管理)
        - [预览功能](#预览功能)
        - [管理预览功能](#管理预览功能)
        - [分享时忘记设置密码](#分享时忘记设置密码)
        - [取消分享](#取消分享)
        - [分享排序](#分享排序)
        - [分享后的资源在网盘删除](#分享后的资源在网盘删除)
    - [存储策略介绍](#存储策略介绍)
    - [存储策略切换](#存储策略切换)
    - [直链技术](#直链技术)
- [充值购买](#充值购买)
    - [如何购买网盘容量？](#如何购买网盘容量)
    - [如何购买网盘会员？](#如何购买网盘会员)
    - [如何购买网盘积分？](#如何购买网盘积分)
    - [积分购买比例？](#积分购买比例)
    - [会员目前都有什么挡位？](#会员目前都有什么挡位)
    - [激活码相关](#激活码相关)
        - [购买方式](#购买方式)
        - [激活方式](#激活方式)
        - [使用次数](#使用次数)
        - [激活码时效](#激活码时效)
        - [激活码可激活内容](#激活码可激活内容)
        - [是否支持非购买账号激活](#是否支持非购买账号激活)
        - [重复激活](#重复激活)
- [隐藏福利](#隐藏福利)

<!-- /TOC -->


# 云盘相关

## 云盘运营
有专人维护，保证云盘可以正常运行，保护用户的每一份**资料的安全**

## 云盘收费

   仅仅凭爱发电是走不远的，所以请在力所能及的范围内给予云盘支持，我们将会用捐助的钱来提升服务，形成良性循环。**当然**，您也不必担心，我们的基础服务是免费的，一般情况下足够普通用户使用，如果您需要提升服务质量，欢迎进行捐赠。

## 云盘规则

   云盘不是法外之地，请遵守当地法律法规，以及本站的相关规定。如果您使用我们的网盘，那我们将默认您同意我们的规则。







# 注册

## 注册注意事项
1. 本站采用邮箱注册方式，请提前自备邮箱。
2. 注册按钮在登录首页的右下角（提交时点击一次一般就可以了）。
3. 为保证用户的财产信息安全，建议使用常用邮箱，包括但不限于 `@qq.com` 、 `@gmail.com` 、 `@163.com`,不推荐使用临时邮箱。
4. 注册时请再三确定邮箱地址正确，若无法收到注册邮件 [请点击此处](#注册邮件找不到)
5. 请牢记您的密码，并尽可能的不要保留在不稳定的媒介上以及不信任的设备，包括但不限于网吧。
6. 使用一个未绑定已注册本站的 QQ 时，会以游客身份访问(提示该 QQ 未绑定任何账号)，此时可以点开左侧菜单栏进行注册。

## 注册邮件找不到

1. 去预注册的邮箱的垃圾邮件中寻找，可能被系统误判。
2. 检查邮箱地址是否正确。
3. 确认自己的网络连接，注册时建议使用稳定网络。
4. 使用常用邮箱注册而不是临时邮箱。
5. 反馈客服。






# 登录

## 登陆方式

- 绑定了第三方账号（目前仅支持 QQ ）后可以通过 QQ 登录。
- 注册邮箱登录

## 登陆出现的问题

### Backend is not running!

检查网络连接，重新尝试。

### 提示用户邮箱或密码错误

1. 检查邮箱地址是否正确。
2. 重新输入密码。
3. 取消网页自动填充，手动输入邮箱和密码。

### 登录提示“参数错误”

由浏览器**自动填充密码**导致，请手动输入密码登录即可










# 安全

## 绑定第三方账号（目前仅支持 QQ）

>电脑端：右上角个人设置--> QQ 账号-->按流程授权即可

>手机端：侧边栏个人设置--> QQ 账号-->按流程授权即可

## 解绑 QQ 账号

点击右上角齿轮即可查看及修改

## 忘记密码及密码修改

### 登陆账号前

>电脑端

点击登录框中的`忘记密码`一栏，输入网盘邮箱（需要找回密码的邮箱），然后点击`发送密码重置邮件`，在邮箱中查看邮件，进行密码的重置

>手机端

点击登录框中的`忘记密码`一栏，输入网盘邮箱（需要找回密码的邮箱），然后点击`发送密码重置邮件`，在邮箱中查看邮件，进行密码的重置

### 登陆账号后

>电脑端

点击右上角个人设置按钮，点击"登录密码"一栏，按提示流程点击授权即可

>手机端

在侧边栏选择个人设置，点击"登录密码"一栏，按提示流程点击授权即可

[邮件找不到？点击这里](#注册邮件找不到)

## 外部认证器

此功能后续开放，目前支持带有指纹功能的电脑
>电脑端：带有指纹解锁功能的可以尝试添加外部认证器

>手机端：点击后会显示此功能未开放（敬请期待，后续开放）

## 两步验证

>电脑端：点击右上角设置（`齿轮按钮`），安全隐私中`二步验证`按照提示进行操作即可

>手机端：侧边栏点击个人设置，安全隐私中`二步验证`按照提示进行操作即可






# 常见问题

## 文件列表展示方式

目前支持`小图标展示`、`大图标展示`、`列表展示`三种

>电脑端：

1.右上角点击“列表展示”按钮即可快速切换<br>
2.点击右上角设置（齿轮按钮）-->个性化栏目中“文件列表”按钮即可切换

>手机端：

1.右上角点击“列表展示”按钮即可快速切换<br>
2.侧边栏点击“个人设置”按钮，点击个性化栏目中“文件列表”按钮即可切换

## 寻找对应类型文件
切换到`我的文件`栏目，再次点击`我的文件`即可看到对应文件类型

## 文件排序
(目前支持 A-Z、Z-A、最早、最新、最小、最大六种)

>电脑端：右上角点击“排序方式”按钮即可快速切换

>手机端：右上角点击“排序方式”按钮即可快速切换
　
## 黑暗模式的开启

>电脑端：点击右上角设置（齿轮按钮）-->个性化-->黑暗模式

>手机端：侧边栏点击“个人设置”-->"个性化"-->黑暗模式

## 主题配色修改

（目前提供十种配色）
>电脑端在：点击右上角设置（`齿轮按钮`）-->`个性化`-->主题配色

>手机端：侧边栏点击`个人设置`-->`个性化`-->主题配色

## 收起侧边栏

点击左上角的`三条杠`即可开关


## 数字 UID

点击右上角齿轮即可查看

## 字母 UID

点击右上角头像-->个人主页

## 注册时间

点击右上角头像-->个人主页

## 积分查询

点击右上角齿轮即可查看

## 用户组到期时间

点击右上角齿轮即可查看

## 修改头像

点击右上角齿轮即可修改





  
# 进阶问题

## 打包下载

>VIP-月付:暂不支持

>SVIP-月付：在线打包下载：1 G 文件

>SVIP-年付：在线打包下载：2 G 文件

## 在线解压缩功能

>VIP-月付：在线解压/压缩：500 M 文件

>SVIP-月付：在线解压/压缩：1 G 文件

>SVIP-年付：在线解压/压缩：2 G 文件

## WebDAV 使用指南

### 何谓 WebDAV?

基于Web的分布式编写和版本控制（ WebDAV ）是超文本传输协议（ HTTP ）的扩展，有利于用户间协同编辑和管理存储在万维网服务器文档。

### WebDAV 功能的网页配置

![WebDAV功能的网页配置](https://github.com/W-W336/YINGHUA/blob/main/Remarks/WebDAV%E5%8A%9F%E8%83%BD%E7%9A%84%E7%BD%91%E9%A1%B5%E9%85%8D%E7%BD%AE.png) 

### WebDAV 功能的本地配置

![WebDAV 功能的本地配置](https://github.com/W-W336/YINGHUA/blob/main/Remarks/WebDAV%E5%8A%9F%E8%83%BD%E7%9A%84%E6%9C%AC%E5%9C%B0%E9%85%8D%E7%BD%AE.png) 

### WebDAV 账号管理

![WebDAV 账号管理](https://github.com/W-W336/YINGHUA/blob/main/Remarks/WebDAV%E8%B4%A6%E5%8F%B7%E7%AE%A1%E7%90%86.png)

### WebDAV 设置

点击右上角齿轮下拉即可查看及修改

## 上传问题

### 上传组件还未加载完成

稍等片刻即可，这不是云盘问题。

### 上传失败

部分命名关键字及后缀不支持上传，如有发现可以反馈客服。着急使用的话建议暂时重命名。

### 文件夹上传

支持整个文件夹上传，但其中部分文件会显示上传失败，请到预上传目录进行查看，有时是显示错误，尽管概率极低。

### 单文件上传大小

>VIP-月付：20 G

>SVIP-月付：25 G

>SVIP-年付：30 G

## 离线下载

### 怎么进行离线下载

侧边栏点击 `离线下载` 点击右下角加号 ➕，添加文件下载地址，支持HTTP(S)/FTP/磁力链，选择文件离线位置（即文件存储位置）。

### 是否支持选择文件下载

暂不支持

### 下载出错

当添加的磁力任务是冷门资源，没人做种。5分钟后依然没有网速将自动取消任务。请尝试更换另一条磁力。

### 离线文件存储路径

存储至用户自己定义的路径

### 磁力转换

https://www.qtoo;.net/tomagnet

- 使用[映画云盘](https://disk.onji.cn/)还将获得一条专属的线路

### 为什么有的磁力链离线速度很慢？

磁力链，离线速度跟文件热度以及做种人数，做种人的上传宽带有关。

### 添加离线下载任务后显示“未知”

通常是刚添加任务，即将开始下载，无视了它就可以了。

### 文件转存失败

请进入存放目录进行查看，资源或许已经转存完毕，也可以尝试再次下载，或者换一条链接进行离线，如果依旧不行，请联系客服，描述问题。

### 任务添加成功却看不到任务

点击`进项中`左侧的刷新按钮

### 查看资源下载的事件

点击目标资源即可查看，如果资源包含文件数较多，需要下滑查看。

### 很早的资源看不到记录

点击下方屏幕下方“加载更多按钮”等待加载完成即可查看

### “转存处理中”是什么意思？

此状态是服务器已将文件下载完毕，正在中转到后端存储。还需要继续等待。

### 一直处于“已完成，转存处理中”

尝试点击刷新按钮，如果依旧这样，建议找点其他事干，比如推荐网盘给好朋友，待会再来查看

### 转存为什么比离线慢

中转到微软OD，上传速度限制不是满速。

## 分享管理

### 预览功能

本网盘支持预览功能，在分享时可以选择是否支持预览

### 管理预览功能

>电脑端：侧边栏点击“我的分享”按钮，点击`预览`按钮（眼睛）即可开关

>手机端：侧边栏点击“我的分享”按钮，点击“预览”按钮（眼睛）即可开关

### 分享时忘记设置密码

侧边栏点击`我的分享`按钮，点击分享按钮（锁）即可开关是否加密会刷新`钥匙`按钮，点击即可查看密码

### 取消分享

侧边栏点击“我的分享”按钮，在刷新后的页面进行管理<br>
**注意**：没有二次确认按钮，点击即取消

### 分享排序

侧边栏点击“我的分享”按钮，在刷新后的页面右上角，选择排序方式

### 分享后的资源在网盘删除

对方访问你的分享相当于访问你的网盘此文件，如果网盘删除，则分享自动失效（删除资源时有二次确认）,请谨慎操作。

## 存储策略介绍

>V1-月付：香港

>V2-月付：香港 / 北京

>V3-年付：香港 / 北京

## 存储策略切换

> 电脑端：右击待转移文件，点击转移存储策略，选择即可。

> 手机端：长按待转移文件，点击转移存储策略，选择即可。
<br></br>
ps：部分敏感资源不要存储在 `CN` 策略内。

## 直链技术

本站支持直链




# 充值购买

## 如何购买网盘容量？

在右侧菜单列表选择`容量配额`按钮，接着选择`购买容量包`,选择`容量包`按钮即可购买

## 如何购买网盘会员？

在右侧菜单列表选择`容量配额`按钮，接着选择`购买容量包`,选择`会员`按钮即可购买

## 如何购买网盘积分？

在右侧菜单列表选择`容量配额`按钮，接着选择`购买容量包`,选择`积分充值`按钮即可购买

## 积分购买比例？

10：1，即您需要花费1元钱来购买10积分（没有上限）

## 会员目前都有什么挡位？

目前有三个档位：V1 月付、V2 月付、V3 年付


## 激活码相关


### 购买方式

激活码一般不需要购买，通过赠送或其他方式获得
        
### 激活方式

-. 「容量配额」中点击「使用激活码兑换」进行激活 </br>
-. 「容量配额」中点击「购买容量包」点击「使用激活码」

### 使用次数

每条仅支持激活一次

### 激活码时效

激活码不限时

### 激活码可激活内容

包括用户组（即会员），或云盘容量

### 是否支持非购买账号激活

任何账号都可以激活，不进行限制

### 重复激活

每条仅支持激活一次


# 隐藏福利


客服暗号获取 `1T` 容量
