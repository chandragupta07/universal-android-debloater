# Universal Android Debloater GUI
**DISCLAIMER**: Use at your own risk. I am not responsible for anything that could happen to your phone. 

<img src="/resources/screenshots/v0.5.0.png" width="850" alt="uad_screenshot">

**This software is still in an early stage of development. Check out the issues, and feel free to contribute!**

## Summary
This is a complete rewrite in Rust of the [UAD project](https://gitlab.com/W1nst0n/universal-android-debloater), which aims to improve privacy and battery performance by removing unnecessary and obscure system apps. This can also contribute to improve security by reducing [the attack surface](https://en.wikipedia.org/wiki/Attack_surface). 

Packages are as well documented as possible in order to provide a better understanding of what you can delete or not. The worst thing which could happen is removing an essential system package needed during boot causing then an unfortunate bootloop. After about 5 failed system boots, the phone will automatically reboot in recovery mode and you'll have to perform a FACTORY RESET. So make a backup first!

In any case, you can NOT brick your device with this software! That's the main thing, right?

## Features 
* [X] Uninstall/Disable and Restore/Enable system packages
* [X] Multi-user support (e.g apps in work profiles)
* [X] Export/Import your selection in `uad_exported_selection.txt`
* [X] Multi-device support: you can connect multiple phones at the same time
* [X] All your actions are logged so you never forget what you've done 

NB : System apps cannot really be uninstalled without root (see the [FAQ](https://gitlab.com/W1nst0n/universal-android-debloater-rs/-/wikis/FAQ))

## Universal debloat lists 
* [X] GFAM (Google/Facebook/Amazon/Microsoft)
* [X] AOSP
* [X] Manufacturers (OEM)
* [X] Mobile carriers
* [X] Qualcomm / Mediatek / Miscellaneous

## Manufacturers debloat lists
* [ ] Archos
* [X] Asus
* [ ] Blackberry
* [ ] Gionee
* [X] LG
* [X] Google
* [X] Fairphone
* [ ] HTC
* [X] Huawei
* [X] Motorola
* [X] Nokia
* [X] OnePlus
* [X] Oppo  
* [X] Samsung
* [X] Sony
* [ ] TCL
* [ ] Wiko
* [X] Xiaomi
* [ ] ZTE

## Mobile carriers debloat lists
|   Country       | Carriers                          |
|-----------------|-----------------------------------|
| France          | Orange, SFR, Free, Bouygues       |
| USA             | T-Mobile, Verizon, Sprint, AT&T   |  
| Germany         | Telekom                           |
| UK              | EE                                |



# 📱 Common Android Bloatware Packages by Manufacturer

> ⚠️ **Disclaimer:** Removing some packages might break essential functions. Always **back up your data** before uninstalling system apps.

---

## 🧩 Universal (AOSP / Google / Meta / Microsoft / Amazon)

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Google Chrome | `com.android.chrome` | Optional; can use other browsers. |
| Google Maps | `com.google.android.apps.maps` | Optional. |
| Google Photos | `com.google.android.apps.photos` | Cloud sync app. |
| Google Assistant | `com.google.android.apps.googleassistant` | Optional. |
| YouTube | `com.google.android.youtube` | Replace with NewPipe. |
| YouTube Music | `com.google.android.apps.youtube.music` | Optional. |
| Gmail | `com.google.android.gm` | Optional. |
| Drive | `com.google.android.apps.docs` | Optional. |
| Play Movies | `com.google.android.videos` | Optional. |
| Facebook | `com.facebook.katana` | Optional. |
| Facebook Services | `com.facebook.services` | Optional. |
| Instagram | `com.instagram.android` | Optional. |
| LinkedIn | `com.linkedin.android` | Optional. |
| Microsoft Office | `com.microsoft.office.officehubrow` | Optional. |
| Amazon Shopping | `com.amazon.mShop.android.shopping` | Optional. |
| Alexa | `com.amazon.dee.app` | Optional. |
| Prime Video | `com.amazon.avod.thirdpartyclient` | Optional. |

---

## 📱 Samsung

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Bixby Home | `com.samsung.android.app.spage` | Optional. |
| Bixby Voice | `com.samsung.android.bixby.voiceinput` | Optional. |
| AR Emoji | `com.samsung.android.aremoji` | Optional. |
| Samsung Free | `com.samsung.android.app.spage` | Optional. |
| Samsung Pay | `com.samsung.android.spay` | Optional. |
| Samsung Health | `com.samsung.android.app.shealth` | Optional. |
| Galaxy Store | `com.sec.android.app.samsungapps` | Optional. |
| Game Launcher | `com.samsung.android.game.gamehome` | Optional. |
| Samsung Members | `com.samsung.android.voc` | Optional. |
| Global Goals | `com.samsung.sree` | Optional. |

---

## 📱 Xiaomi / MIUI

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| GetApps | `com.xiaomi.mipicks` | Xiaomi app store. |
| Mi Video | `com.miui.videoplayer` | Optional. |
| Mi Browser | `com.android.browser` | Optional. |
| Mi Community | `com.mi.global.bbs` | Optional. |
| Analytics | `com.miui.analytics` | Recommended to remove. |
| Mi Cloud | `com.miui.cloudservice` | Optional. |
| Mi Pay | `com.mipay.wallet.in` | Optional. |
| Screen Recorder | `com.miui.screenrecorder` | Optional. |
| Compass | `com.miui.compass` | Optional. |
| Weather | `com.miui.weather2` | Optional. |

---

## 📱 OnePlus / Oppo / Realme

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Clone Phone | `com.coloros.backuprestore` | Optional. |
| Game Space | `com.coloros.gamespace` | Optional. |
| HeyTap Cloud | `com.heytap.cloud` | Optional. |
| ORoaming | `com.redteamobile.roaming` | Optional. |
| App Market | `com.heytap.market` | Optional. |
| Smart Sidebar | `com.coloros.smartsidebar` | Optional. |
| Weather | `com.coloros.weather2` | Optional. |

---

## 📱 Huawei / Honor

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| HiCare | `com.huawei.phoneservice` | Optional. |
| AppGallery | `com.huawei.appmarket` | Optional. |
| Huawei Assistant | `com.huawei.intelligent` | Optional. |
| Huawei Wallet | `com.huawei.wallet` | Optional. |
| Themes | `com.huawei.android.thememanager` | Optional. |
| Cloud | `com.huawei.hicloud` | Optional. |
| Tips | `com.huawei.tips` | Optional. |

---

## 📱 Motorola

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Moto Help | `com.motorola.help` | Optional. |
| Moto Display | `com.motorola.motodisplay` | Optional. |
| Moto Voice | `com.motorola.audiomonitor` | Optional. |
| Moto App Launcher | `com.motorola.launcher3` | Optional. |

---

## 📱 Nokia (HMD Global)

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| My Phone | `com.evenwell.MyPhone` | Optional. |
| Email | `com.evenwell.Email` | Optional. |
| Evenwell Services | `com.evenwell.*` | Privacy concern; optional. |

---

## 📱 Sony

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| AR Effect | `com.sonymobile.areffect` | Optional. |
| Xperia Lounge | `com.sonymobile.xperialounge.services` | Optional. |
| Sketch | `com.sonymobile.sketch` | Optional. |
| Weather | `com.sonymobile.weather` | Optional. |
| What’s New | `com.sonymobile.advancedwidget.entrance` | Optional. |

---

## 📱 LG

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| SmartWorld | `com.lge.appbox.client` | Optional. |
| QuickMemo+ | `com.lge.qmemoplus` | Optional. |
| LG Health | `com.lge.lifetracker` | Optional. |
| Smart Doctor | `com.lge.sdoupdate` | Optional. |
| Smart Cleaning | `com.lge.smartcleaning` | Optional. |

---

## 📱 Asus

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| ZenUI Services | `com.asus.services` | Optional. |
| Game Genie | `com.asus.gamewidget` | Optional. |
| Mobile Manager | `com.asus.mobilemanager` | Optional. |
| Themes | `com.asus.themes` | Optional. |

---

## 📱 Fairphone

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Fairphone Updater | `org.fairphone.updater` | Keep if you use official OS updates. |
| Fairphone Services | `com.fairphone.myfairphone` | Optional. |

---

## 📱 Oppo / Vivo / Realme Common Packages

| App Name | Package Name | Notes |
|-----------|---------------|-------|
| Hot Apps | `com.oppo.market` | Optional. |
| Hot Games | `com.heytap.huangyan` | Optional. |
| Smart Assistant | `com.coloros.assistant` | Optional. |
| Weather | `com.coloros.weather2` | Optional. |

---

## Mobile carriers debloat lists
|   Country       | Carriers                          |
|-----------------|-----------------------------------|
| France          | Orange, SFR, Free, Bouygues       |
| USA             | T-Mobile, Verizon, Sprint, AT&T   |  
| Germany         | Telekom                           |
| UK              | EE                                |


## How to use it 
- **Read the [FAQ](https://github.com/0x192/universal-android-debloater/wiki/FAQ)!**
- **Do a proper backup of your data! You can never be too careful!**
- Enable *Developer Options* on your smartphone.
- Turn on *USB Debugging* from the developer panel.
- From the settings, disconnect from any OEM accounts (when you delete an OEM account package it could lock you on the lockscreen because the phone can't associate your identity anymore)
- Install ADB:
  <p>
  <details>
  <summary>LINUX</summary>

  - Install *Android platform tools* on your PC :

  Debian Base:
  ```bash
  $ sudo apt install android-sdk-platform-tools
  ```
  Arch-Linux Base:
  ```bash
  $ sudo pacman -S android-tools
  ```
  Red Hat Base:
  ```bash
  $ sudo yum install android-tools
  ```
  OpenSUSE Base:
  ```bash
  $ sudo zypper install android-tools
  ```
  </details>
  </p>

  <p>
  <details>
  <summary>MAC OS</summary>

  - Install [Homebrew](https://brew.sh/)
  - Install *Android platform tools*
    ```bash
    $ brew install android-platform-tools
    ```
  </details>
  </p>

  <p>
  <details>
  <summary>WINDOWS</summary>

  - Download [android platform tools](https://dl.google.com/android/repository/platform-tools-latest-windows.zip) and unzip it somewhere. [Add the folder to your PATH](https://www.architectryan.com/2018/03/17/add-to-the-path-on-windows-10/).

  - [Install USB drivers for your device](https://developer.android.com/studio/run/oem-usb#Drivers)
  - Check your device is detected:
    ```batch
    > adb devices
    ```
  </details>
  </p>


- Download the latest release of UAD GUI for your Operating System [here](https://github.com/0x192/universal-android-debloater/releases). Take the `opengl` version only if the default version (with a Vulkan backend) doesn't launch.

**NOTE:** Chinese phones users may need to use the AOSP list for removing some stock apps because those Chinese manufacturers (especially Xiaomi and Huawei) have been using the name of AOSP packages for their own (modified & closed-source) apps.

**IMPORTANT NOTE:** You will have to run this software whenever your OEM pushes an update to your phone as some *uninstalled* system apps could be reinstalled.

## How to contribute

Hey-hey-hey! Don't go away so fast! This is a community project. That means I need you! I'm sure you want to make this project better anyway.

==> [How to contribute](https://github.com/0x192/universal-android-debloater/wiki)

## Special thanks

- [@mawilms](https://github.com/mawilms) for his LotRO plugin manager ([Lembas](https://github.com/mawilms/lembas)) which helped me a lot to understand how to use the [Iced](https://github.com/hecrj/iced) GUI library.
- [@casperstorm](https://github.com/casperstorm) for the UI/UX inspiration.
