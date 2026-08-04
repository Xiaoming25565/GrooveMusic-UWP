# 简介

Groove音乐的不更新版本，在Windows11 22H2及以上版本可以和新媒体播放器共存,在Windows10中似乎可以因为签名、发布者不同而不会安装Groove音乐

# 有提示：

> [!IMPORTANT]
> 所有内容资源 _(包括但不限于应用、音频、图片等)_ 版权归 Microsoft 所有。  
> 本软件仅学习交流使用，请勿用于用于商业用途。如有侵权，请发 Issue 提出。  
> 使用此应用即代表您同意 [Microsoft 软件许可条款](https://go.microsoft.com/fwlink/?LinkID=524989)及 [Microsoft 隐私政策](https://go.microsoft.com/fwlink/?LinkID=521839)。

# 下载

* [20112-x64位安装包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove64.appx) 

* [20112-简体中文语言包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove-zh-hans.appx)

* [18052-x64位安装包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove64.appx)

* [18052-简体中文语言包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove-zh-hans.appx)

# 安装说明

在Windows中，默认我们只能安装微软商店或者是受信任的开发者应用程序，所以需要先安装证书，而证书

1. 右键点击 x64 / 语言包 的 ```appx``` 安装包，点击属性，切换到"数字签名"选项卡。双击签名列表中的"强力花调皮"。在弹出的"数字签名详细信息"窗口中点击"查看证书"，再点击"安装证书"。

2. 在"证书导入向导"中：

"存储位置"选"本地计算机"，下一步。（开启UAC时需要同意UAC权限请求）

选择"将所有的证书都放入下列存储"，点击"浏览"，选择"受信任的根证书颁发机构"，确定，下一步，继续完成证书导入。

3. 双击 x64 的 ```appx``` 安装包安装。

4.简体中文语言包，点击“Groove简体中文语言包.appx”，点击重新安装即可

# 已知问题

18052版本不能在Windows11浅色模式下使用（不会解决该问题，这是老版本UWP应用不适配Windows11风格，请安装20112版本）

# 解决问题

~~2019.20112.10111.0的版本在Windows10上无法使用，使用2019.20112.10111.0的版本可以考虑LTSC或者是补全补丁后关闭Windows Update~~本问题通过修改英文发布者和签名实现成功

# 灵感

* [网易云音乐不更新版本（提供了修改方式）](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack)

* [获取UWP的地方](https://store.rg-adguard.net/#google_vignette)

* [原版下载链接(新版媒体播放器)](https://apps.microsoft.com/detail/9WZDNCRFJ3PT?hl=zh-cn&gl=CN&ocid=pdpshare)
