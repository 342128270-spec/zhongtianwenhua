# Windows 开源工具 · 2026

> Windows 平台上真正好用、仍在维护的开源工具，26 个项目。
> 星标、许可证、更新时间由脚本通过 GitHub API 核实（2026-11-24）。

## 怎么读

| 列 | 含义 |
|---|---|
| 星标 | 社区规模 |
| 许可 | 能否商用与再分发 |
| 更新 | 最近推送年月 |

仓库地址：github.com/ 后接项目名。

---

## 一、系统增强

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| microsoft/PowerToys | 141.3k | MIT | 2026-11 | 微软官方系统增强套件，20+ 工具 |
| files-community/Files | 46.8k | MIT | 2026-11 | 现代化文件管理器，多标签 |
| microsoft/terminal | 105.5k | MIT | 2026-11 | Windows 终端，多标签/分屏 |
| Flow-Launcher/Flow.Launcher | 16.1k | MIT | 2026-11 | 快速启动器，插件生态丰富 |
| QL-Win/QuickLook | 25.9k | GPL-3.0 | 2026-11 | 空格预览文件，类 macOS |
| sabrogden/Ditto | 7.5k | GPL-3.0 | 2026-10 | 剪贴板历史管理 |
| AutoHotkey/AutoHotkey | 13.5k | GPL-2.0 | 2026-11 | 自动化脚本，改键/宏 |


## 二、包管理与开发环境

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| ScoopInstaller/Scoop | 24.8k | NOASSERTION | 2026-11 | 命令行包管理，免管理员 |
| chocolatey/choco | 11.6k | NOASSERTION | 2026-11 | 包管理器，软件源大 |
| microsoft/winget-cli | 26.6k | MIT | 2026-11 | 微软官方包管理器 |
| microsoft/WSL | 34.5k | MIT | 2026-11 | Windows 里的 Linux 子系统 |
| git-for-windows/git | 9.5k | NOASSERTION | 2026-11 | Git 官方 Windows 版 |


## 三、性能监控与诊断

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| winsiderss/systeminformer | 16.6k | MIT | 2026-11 | 进程/句柄/网络全面监控（Process Hacker 后继） |
| LibreHardwareMonitor/LibreHardwareMonitor | 9.4k | MPL-2.0 | 2026-11 | 硬件温度/电压/风扇监控 |
| cgsecurity/testdisk | 2.7k | GPL-2.0 | 2026-11 | 分区恢复与数据修复 |


## 四、安全与逆向

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| x64dbg/x64dbg | 50.4k | NOASSERTION | 2026-11 | Windows 调试器，逆向主力 |
| NationalSecurityAgency/ghidra | 101.2k | Apache-2.0 | 2026-11 | NSA 反编译套件（跨平台） |
| bleachbit/bleachbit | 7.6k | GPL-3.0 | 2026-11 | 系统清理与隐私擦除 |


## 五、备份与同步

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| restic/restic | 37.4k | BSD-2-Clause | 2026-11 | 去重加密备份，命令行 |
| duplicati/duplicati | 15.2k | NOASSERTION | 2026-11 | 图形化备份，支持云存储 |
| mRemoteNG/mRemoteNG | 11.2k | GPL-2.0 | 2026-11 | 多协议远程连接管理 |


## 六、中文与输入法

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| rime/weasel | 8.3k | GPL-3.0 | 2026-10 | 小狼毫输入法，高度可定制 |
| iDvel/rime-ice | 20.4k | GPL-3.0 | 2026-11 | 雾凇拼音：开箱即用的 Rime 配置 |


## 七、影音与工具

| 项目 | 星标 | 许可 | 更新 | 说明 |
|---|---:|---|---|---|
| mpv-player/mpv | 38.3k | NOASSERTION | 2026-11 | 极简高效播放器 |
| ShareX/ShareX | 41.3k | GPL-3.0 | 2026-11 | 截图/录屏/上传一条龙 |
| obsproject/obs-studio | 80.0k | GPL-2.0 | 2026-11 | 直播录制（跨平台） |

---

## 按场景选

| 你想做的事 | 用什么 |
|---|---|
| 新装系统后第一件事 | winget 或 Scoop 批量装软件 |
| 想要 mac 那种空格预览 | QuickLook |
| 窗口多开找文件慢 | Files（多标签） |
| 剪贴板经常覆盖 | Ditto，历史全留着 |
| 中文输入想自定义 | 小狼毫（Weasel）+ 雾凇拼音配置 |
| 查进程占用/句柄锁 | System Informer（原 Process Hacker） |
| 系统盘满了想深度清理 | BleachBit（谨慎，勾选前看清） |
| 做逆向分析 | x64dbg 动态 + Ghidra 静态 |

## 注意

1. 清理类工具会删文件，第一次用先只扫描不执行。BleachBit 勾错项可能清掉浏览器密码。
2. 注册表修改前先导出备份。第三方优化脚本风险高。
3. Scoop 与 Chocolatey 不要混用同一软件，否则升级会冲突。
4. 部分工具（如 WSL）需要开启虚拟化，在 BIOS 里确认已启用。

本次核实收录 **26** 个项目。

_最后核实：2026-11-24_