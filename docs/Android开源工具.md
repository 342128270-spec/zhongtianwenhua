# Android 开源工具 · 2026

> 22 个 Android 平台上真正可用的开源应用与工具。
> 星标、许可证、更新由 GitHub API 核实（2026-11-24）。

## 怎么读

| 列 | 含义 |
|---|---|
| 星标 | 社区规模 |
| 许可 | 能否商用与再分发 |
| 更新 | 最近推送年月 |

仓库地址：github.com/ 后接项目名。

---

## 一、系统与权限

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| termux/termux-app | 65.6k | NOASSERTION | 2026-11 | Android 上的终端与 Linux 环境 |
| f-droid/fdroidclient | 3.3k | GPL-3.0 | 2026-11 | 开源应用商店，无追踪 |
| whyorean/AuroraStore | 3.3k | GPL-3.0 | 2026-11 | Google Play 的匿名客户端 |
| topjohnwu/Magisk | 64.3k | GPL-3.0 | 2026-11 | 系统级 root 方案（需解锁） |
| tiann/KernelSU | 21.0k | GPL-3.0 | 2026-11 | 内核级 root，替代 Magisk |
| RikkaApps/Shizuku | 34.6k | Apache-2.0 | 2025-06 | 免 root 使用系统 API 权限 |
| ImranR98/Obtainium | 21.9k | GPL-3.0 | 2026-11 | 直接从 GitHub 更新应用 |
| Droid-ify/client | 7.8k | GPL-3.0 | 2026-11 | 现代化的 F-Droid 客户端 |


## 二、隐私与安全

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| beemdevelopment/Aegis | 13.6k | GPL-3.0 | 2026-09 | 双重验证码管理，可导出加密备份 |
| Kunzisoft/KeePassDX | 7.7k | GPL-3.0 | 2026-11 | 本地密码库，兼容 KeePass |
| bitwarden/android | 9.7k | GPL-3.0 | 2026-11 | 开源密码管理器官方客户端 |
| AdguardTeam/AdguardForAndroid | 2.0k | 自定义 | 2026-11 | 系统级广告拦截 |


## 三、通讯与阅读

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| TeamNewPipe/NewPipe | 40.9k | GPL-3.0 | 2026-11 | 无广告 YouTube 客户端 |
| AntennaPod/AntennaPod | 8.3k | GPL-3.0 | 2026-11 | 播客客户端，本地优先 |
| thunderbird/thunderbird-android | 14.3k | Apache-2.0 | 2026-11 | K-9 Mail，老牌开源邮箱 |
| ReadYouApp/ReadYou | 7.7k | GPL-3.0 | 2026-08 | Material 风格的 RSS 阅读器 |
| zhanghai/MaterialFiles | 9.5k | GPL-3.0 | 2026-10 | 文件管理器，支持 root/SMB |


## 四、生活与工具

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| osmandapp/OsmAnd | 6.2k | NOASSERTION | 2026-11 | 离线地图与导航，功能最全 |
| syncthing/syncthing-android | 4.3k | MPL-2.0 | 2024-12 | 点对点文件同步，无服务器 |
| JunkFood02/Seal | 31.0k | GPL-3.0 | 2026-09 | 视频下载器，基于 yt-dlp |
| LawnchairLauncher/lawnchair | 14.0k | NOASSERTION | 2026-11 | 类 Pixel 启动器 |
| videolan/vlc-android | 4.2k | GPL-2.0 | 2026-11 | 万能播放器 |

---

## 按场景选

| 你想做的事 | 用什么 |
|---|---|
| 手机上跑 Linux / 写脚本 | Termux（配 F-Droid 装） |
| 不想被 Google 追踪 | Aurora Store 装应用 + AdGuard 拦广告 |
| 自动更新 GitHub 上的应用 | Obtainium，填仓库地址即可 |
| 需要 root 但不想刷 Magisk | KernelSU（需内核支持）或 Shizuku（免 root） |
| 无广告看视频 | NewPipe，支持后台播放 |
| 地图要离线、要隐私 | OsmAnd，可整国下载 |
| 文件同步不上云 | Syncthing，点对点 |

## 注意

1. 开启 root（Magisk/KernelSU）会导致部分银行、支付类 App 拒绝运行，需隐藏或用备用机。
2. 解锁 Bootloader 会清空数据，操作前必须备份。
3. F-Droid 与 Google Play 版本不要混装同一应用，签名不同会冲突。
4. 侧载 APK 前核对签名与来源，第三方下载站常夹带广告 SDK。

本次核实收录 **22** 个项目。

_最后核实：2026-11-24_