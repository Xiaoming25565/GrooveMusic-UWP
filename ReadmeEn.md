[中文](https://github.com/Xiaoming25565/GrooveMusic-UWP/blob/master/README.md) | English
# Introduction

This is a non-updating Groove Music build. On Windows 11 22H2 and later, it can coexist with the new Media Player, provided the Media Player has not been uninstalled. On Windows 10, it may appear to work in some cases, depending on the signature and publisher, but compatibility is not guaranteed.

<img width="1916" height="1030" alt="image" src="https://github.com/user-attachments/assets/cf18bf14-0bad-4031-a47a-16efaaef18e5" />


# Important Notice

> [!IMPORTANT]
> All resources (including but not limited to the application, audio, images, and other content) are copyrighted by Microsoft.
> This software is provided only for learning and communication purposes. Do not use it commercially. If any infringement is involved, please open an Issue.
> By using this application, you agree to the [Microsoft Software License Terms](https://go.microsoft.com/fwlink/?LinkID=524989) and [Microsoft Privacy Statement](https://go.microsoft.com/fwlink/?LinkID=521839).

# Please Note

* In 2025, user clinasama uploaded [their GrooveMusicUWP package](https://github.com/clinasama/GrooveMusicUWP-). That build is designed to coexist with the newer Media Player, while this repository's build is a removal/replacement-type build rather than a coexistence build.

* The 18052 package should not have been labeled as MSIX. It can actually be installed on Windows.Desktop (x64) 10.0.14393.0 and later versions; the original manifest `A.......t.xaml` specifies `TargetDeviceFamily Name="Windows.Desktop" MinVersion="10.0.14393.0" MaxVersionTested="10.0.18362.0"`.

# Downloads

* [20112 x64 installer](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/20112Groove64.appx)

* [20112 Start tile-modified installer, extraction code: `c3q5`](https://wwbud.lanzouc.com/iVvmR4gyzq1c)

* [18052 x64 installer](https://raw.githubusercontent.com/Xiaoming25565/GrooveMusic-UWP/refs/heads/master/18052Groove64.appx)

# Installation

Windows normally permits installation only from the Microsoft Store or from apps signed by a trusted developer. Therefore, you must first install the certificate.

1. Right-click the x64 or language-package `.appx` installer and open **Properties**. Switch to the **Digital Signatures** tab, then double-click the signature entry named `~~强力花调皮~~ Xiaoming25565`. In the **Digital Signature Details** dialog, open the certificate details and select **View Certificate**.

2. In the **Certificate Import Wizard**:

   - Select **Local Machine** as the store location and click **Next**. If UAC is enabled, approve the UAC prompt.
   - Select **Place all certificates in the following store**, click **Browse**, select **Trusted Root Certification Authorities**, then confirm and complete the wizard.

3. Double-click the x64 `.appx` installer to install it.

4. For the Simplified Chinese language package, open `20112Groove-zh-hans.appx` or `18052Groove-zh-hans.appx` and click **Reinstall**.

# Known Issues

1. After installing the Chinese language package, Start may still display “Groove Music.” On Windows 11, right-click “Groove Music” or “Groove 音乐” in Start, open **App settings**, scroll down to **Repair**, and click **Repair**. This attempts to repair the Start-menu display language and should not affect application data.

   * Open Start and find **Groove Music** (you can search for `Groove` if needed).
   * Right-click the app and select **App settings**.
   * Scroll to the **Reset** section.
   * Click **Repair**.

2. Start tiles for Groove may not update on Windows 10 DEV 21390 or Windows 11 when using ExplorerPatcher.
   * Download the [20112 tile-modified installer](https://wwbud.lanzouc.com/iVvmR4gyzq1c), extraction code: `c3q5`.

# System-Level Issues (Not Fixed by Me)

* The 18052 build cannot be used with Windows 11 Light mode. As an older UWP application, it is not compatible with the Windows 11 visual style. Windows 11 users should install the 20112 build.

* Windows 11 25H2 may display the issue shown below:

<img width="1211" height="935" alt="image" src="https://github.com/user-attachments/assets/784e371b-d814-475e-90b2-b158e08e7020" />

# Fixes

~~The 2019.20112.10111.0 version could not run on Windows 10. Users of that version could consider LTSC or install missing patches and disable Windows Update.~~ This issue has been resolved by modifying the English publisher and signature configuration.

# Inspiration

* [NetEase Cloud Music non-updating version (includes modification instructions)](https://github.com/JasonWei512/NetEase-Cloud-Music-UWP-Repack)

* [Where to obtain UWP packages](https://store.rg-adguard.net/#google_vignette)

* [Official/original download link (new Media Player)](https://apps.microsoft.com/detail/9WZDNCRFJ3PT?hl=zh-cn&gl=CN&ocid=pdpshare)
