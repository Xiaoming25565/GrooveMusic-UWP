# Introduction

This is an unofficial, non-updated version of Groove Music. On Windows 11 (22H2 and later) it can coexist with the new Media Player (provided you haven't uninstalled the new Media Player). On Windows 10 it may fail to run due to signature or publisher issues [...]

![screenshot](https://github.com/user-attachments/assets/cf18bf14-0bad-4031-a47a-16efaaef18e5)

# Important Notice

> [!IMPORTANT]
> All content resources (including but not limited to apps, audio, images, etc.) are Copyright Microsoft.  
> This software is provided for learning and communication purposes only. Do not use it for commercial purposes. If there is any infringement, please open an Issue.  
> By using this app you agree to the [Microsoft Software License Terms](https://go.microsoft.com/fwlink/?LinkID=524989) and the [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?LinkID=521839).

# Please note

* User clinasama uploaded his GrooveMusicUwp installer in 2025 ([clinasama/GrooveMusicUWP-](https://github.com/clinasama/GrooveMusicUWP-)). That one is a coexistence build; this repository only removes updates and does not include other changes [...]

* I mistakenly added msix for the 18052 build. In fact, the package requires Windows.Desktop (x64) 10.0.14393.0 or newer (the original manifest A.......t.xaml states TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.14393.0" MaxVersionTested=...).

# Downloads

* [20112 x64 installer](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove64.appx)

* [20112 Simplified Chinese language pack](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove-zh-hans.appx)

* [18052 x64 installer](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove64.appx)

* [18052 Simplified Chinese language pack](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove-zh-hans.appx)

# Installation

By default Windows only allows installing apps from the Microsoft Store or trusted developer-signed packages, so you need to install the certificate first.

1. Right-click the x64 installer or language pack (.appx), open Properties, go to the "Digital Signatures" tab. Double-click the signature entry named "~~强力花调皮~~ Xiaoming25565". In the "Digital Signature Details" dialog [...]

2. In the Certificate Import Wizard:

   - Select "Local Machine" as the Store Location, then Next. (UAC consent is required when UAC is enabled)
   - Choose "Place all certificates in the following store", click "Browse", select "Trusted Root Certification Authorities", confirm and proceed to complete the import.

3. Double-click the x64 .appx installer to install.

4. For the Simplified Chinese language pack, open the "Groove Simplified Chinese language pack.appx" and choose Reinstall.

# Known issues

1. After installing the Chinese language pack the Start menu may still show "Groove Music". Windows 11 users can right-click Groove Music in Start, choose App settings (screenshot below), scroll down and click "Repair" to fix this issue [...]

![screenshot](https://github.com/user-attachments/assets/77fcca97-44d5-44b3-9a81-1cdec07777a0)

![screenshot](https://github.com/user-attachments/assets/de26cb8f-2dbb-4fd4-8353-a4a3c368f9df)

# System-level issues (not fixed by me)

* The 18052 build cannot be used in Windows 11 Light theme — it is an older UWP app that doesn't match Windows 11 styling. Windows 11 users should install the 20112 build.

* Windows 11 25H2 may show the issue pictured below:

![screenshot](https://github.com/user-attachments/assets/784e371b-d814-475e-90b2-b158e04e7020)

# Fixes

~The 2019.20112.10111.0 version could not run on Windows 10. Users of that version might consider LTSC or installing missing patches and disabling Windows Update.~ This issue was resolved by modifying the English publisher and signature [...]

# Inspiration

* [NetEase Cloud Music - Non-updating version (includes modification instructions)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack)

* [Where to get UWP packages](https://store.rg-adguard.net/#google_vignette)

* [Original download (new Media Player)](https://apps.microsoft.com/detail/9WZDNCRFJ3PT?hl=zh-cn&gl=CN&ocid=pdpshare)
