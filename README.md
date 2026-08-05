中文 | [English](https://github.com/Xiaoming25565/GrooveMusic-UWP/blob/master/ReadmeEn.md)
# 简介

Groove音乐的不更新版本，在Windows11 22H2及以上版本可以和新媒体播放器（前提是别卸载新媒体播放器。）共存,在Windows10中似乎可以因为签名、发布者不同而不会安装Groove音乐

<img width="1916" height="1030" alt="image" src="https://github.com/user-attachments/assets/cf18bf14-0bad-4031-a47a-16efaaef18e5" />


# 有提示：

> [!IMPORTANT]
> 所有内容资源 _(包括但不限于应用、音频、图片等)_ 版权归 Microsoft 所有。  
> 本软件仅学习交流使用，请勿用于用于商业用途。如有侵权，请发 Issue 提出。  
> 使用此应用即代表您同意 [Microsoft 软件许可条款](https://go.microsoft.com/fwlink/?LinkID=524989)及 [Microsoft 隐私政策](https://go.microsoft.com/fwlink/?LinkID=521839)。

# 请注意

* 用户clinasama在2025年虽然已经上传了[他的GrooveMusicUwp的安装包(clinasama/GrooveMusicUWP-)](https://github.com/clinasama/GrooveMusicUWP-)，他这个是共存版，本版本只去更新,这两个是不同的修改方式

* 18052误添加msix,实际上是Windows.Desktop(x64)10.0.14393.0及以上版本才可以安装（在A.......t.xaml原话是TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.14393.0" MaxVersionTested="10.0.17035.0"）

# 下载

* [20112-x64位安装包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove64.appx) 

* [20112-简体中文语言包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove-zh-hans.appx)

* [18052-x64位安装包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove64.appx)

* [18052-简体中文语言包](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove-zh-hans.appx)

# 安装说明

在Windows中，默认我们只能安装微软商店或者是受信任的开发者应用程序，所以需要先安装证书，而证书

1. 右键点击 x64 / 语言包 的 ```appx``` 安装包，点击属性，切换到"数字签名"选项卡。双击签名列表中的"~~强力花调皮~~ Xiaoming25565"。在弹出的"数字签名详细信息"窗口中点击"查看证书"，再点击"安装证书"。

2. 在"证书导入向导"中：

"存储位置"选"本地计算机"，下一步。（开启UAC时需要同意UAC权限请求）

选择"将所有的证书都放入下列存储"，点击"浏览"，选择"受信任的根证书颁发机构"，确定，下一步，继续完成证书导入。

3. 双击 x64 的 ```appx``` 安装包安装。

4.简体中文语言包，点击“Groove简体中文语言包.appx”，点击重新安装即可

# 已知问题

1. 安装好中文语言包后在开始菜单还是Groove Music,Windows11用户可以在开始菜单右键Groove音乐点击应用设置（下图），下拉找到“修复”后点击后即可修复，Windows10目前没有解决方法
* 打开开始菜单，找到Groove Music（如果需要可以搜索“Groove”）。
* 右键点击应用，选择“应用设置”。
* 往下滚动到“重置”部分。
* 点击“修复”。这会尝试修复开始菜单显示语言，可能不会不影响你的应用数据。

# 系统性问题（不是我解决的）

* 18052版本不能在Windows11浅色模式下使用，这是老版本UWP应用不适配Windows11风格，Windows11请安装20112版本

* Windows11 25H2会出现下图问题

<img width="1211" height="935" alt="image" src="https://github.com/user-attachments/assets/784e371b-d814-475e-90b2-b158e04e7020" />

# 解决问题

~~2019.20112.10111.0的版本在Windows10上无法使用，使用2019.20112.10111.0的版本可以考虑LTSC或者是补全补丁后关闭Windows Update~~本问题通过修改英文发布者和签名实现成功

# 灵感

* [网易云音乐不更新版本（提供了修改方式）](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack)

* [获取UWP的地方](https://store.rg-adguard.net/#google_vignette)

* [原版下载链接(新版媒体播放器)](https://apps.microsoft.com/detail/9WZDNCRFJ3PT?hl=zh-cn&gl=CN&ocid=pdpshare)
