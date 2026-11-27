# v2rayNG

A V2Ray client for Android, support [Xray core](https://github.com/XTLS/Xray-core) and [v2fly core](https://github.com/v2fly/v2ray-core)

> **🧹 去广告纯净版 / Ad-free Mod** \
> 本版本移除了原版的推广/广告入口，「检查更新」与下载均指向本仓库，并自动跟随上游发布最新**正式版**与**预发布版**。 \
> Promotion/ad entries removed; update-check & downloads point to this repo; auto-synced with upstream **stable** & **pre-releases**.

[![API](https://img.shields.io/badge/API-24%2B-yellow.svg?style=flat)](https://developer.android.com/about/versions/lollipop)
[![Kotlin Version](https://img.shields.io/badge/Kotlin-2.4.0-blue.svg)](https://kotlinlang.org)
[![GitHub commit activity](https://img.shields.io/github/commit-activity/m/LOVECHEN/v2rayNG-mod)](https://github.com/LOVECHEN/v2rayNG-mod/commits/master)
[![GitHub Releases](https://img.shields.io/github/downloads/LOVECHEN/v2rayNG-mod/latest/total?logo=github)](https://github.com/LOVECHEN/v2rayNG-mod/releases)

---

## Download / 下载

Download the latest release here:

在这里下载最新版本：

[https://github.com/LOVECHEN/v2rayNG-mod/releases](https://github.com/LOVECHEN/v2rayNG-mod/releases)

> [!TIP]
> v2rayNG is the mobile version. For the desktop version, please visit the v2rayN \
> v2rayNG 是手机版，电脑版请访问 v2rayN
>
> https://github.com/LOVECHEN/v2rayN-mod

---

### Geoip and Geosite

- geoip.dat and geosite.dat files are in `Android/data/com.v2ray.ang/files/assets` (path may differ on some Android device)
- download feature will get enhanced version in this [repo](https://github.com/Loyalsoldier/v2ray-rules-dat) (note: it needs a working proxy)
- latest official [domain list](https://github.com/Loyalsoldier/v2ray-rules-dat) and [ip list](https://github.com/Loyalsoldier/geoip) can be imported manually
- possible to use a third-party dat file in the same folder, like [h2y](https://guide.v2fly.org/routing/sitedata.html#%E5%A4%96%E7%BD%AE%E7%9A%84%E5%9F%9F%E5%90%8D%E6%96%87%E4%BB%B6)

More in our [wiki](https://github.com/LOVECHEN/v2rayNG-mod/wiki)

### Geoip 与 Geosite

- geoip.dat 和 geosite.dat 文件位于 `Android/data/com.v2ray.ang/files/assets`（部分设备路径可能不同）
- 下载功能将获取该 [仓库](https://github.com/Loyalsoldier/v2ray-rules-dat) 中的增强版本（注意：此功能需要一个可用的代理）
- 最新官方 [域名列表](https://github.com/Loyalsoldier/v2ray-rules-dat) 和 [IP 列表](https://github.com/Loyalsoldier/geoip) 可手动导入
- 也可在同一文件夹中使用第三方 dat 文件，例如 [h2y](https://guide.v2fly.org/routing/sitedata.html#%E5%A4%96%E7%BD%AE%E7%9A%84%E5%9F%9F%E5%90%8D%E6%96%87%E4%BB%B6)

更多内容请见我们的 [wiki](https://github.com/LOVECHEN/v2rayNG-mod/wiki)

---

## Development guide / 开发指南

### Note

- Android project under the V2rayNG folder can be compiled directly in Android Studio, or using the Gradle wrapper. But the v2ray core inside the aar is (probably) outdated.
- The aar can be compiled from the Golang project [AndroidLibV2rayLite](https://github.com/2dust/AndroidLibV2rayLite) or [AndroidLibXrayLite](https://github.com/2dust/AndroidLibXrayLite). For a quick start, read the guides for [Go Mobile](https://github.com/golang/go/wiki/Mobile) and [Makefiles for Go Developers](https://tutorialedge.net/golang/makefiles-for-go-developers/).
- v2rayNG can run on Android Emulators. For WSA, VPN permission needs to be granted via `appops set [package name] ACTIVATE_VPN allow`.

### 提示

- V2rayNG 文件夹下的 Android 项目可直接在 Android Studio 中编译，或使用 Gradle wrapper 编译。但 aar 内置的 v2ray core（可能）已过时。
- aar 可由 Golang 项目 [AndroidLibV2rayLite](https://github.com/2dust/AndroidLibV2rayLite) 或 [AndroidLibXrayLite](https://github.com/2dust/AndroidLibXrayLite) 编译而成。快速入门可参考 [Go Mobile](https://github.com/golang/go/wiki/Mobile) 指南和 [Makefiles for Go Developers](https://tutorialedge.net/golang/makefiles-for-go-developers/)。
- v2rayNG 可在 Android 模拟器上运行。对于 WSA，需要通过 `appops set [package name] ACTIVATE_VPN allow` 授予 VPN 权限。
