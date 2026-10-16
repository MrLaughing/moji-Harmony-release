# 墨集 HarmonyOS

剪藏与笔记 · 墨集 HarmonyOS 客户端

这里是墨集 HarmonyOS 的官方安装包发布仓库。源码保存在私有仓库，本仓库仅用于公开发布经过正式签名的 HAP 与 SHA-256 校验文件。

## 下载与安装

前往 [Releases](https://github.com/MrLaughing/moji-Harmony-release/releases/latest) 下载最新版：

- 下载名称类似 `moji-harmony-x.x.x.hap` 的安装包。
- 安装前可使用同名 `.sha256` 文件核对安装包完整性。
- 安装包使用 AGC 发布证书与发布 Profile 签名，只有 Profile 中已登记的设备可以安装。
- 在设备上开启开发者模式后，用 DevEco Studio 命令行工具里的 `hdc` 安装：

  ```bash
  hdc install -r moji-harmony-x.x.x.hap
  ```

- 更换签名密钥会导致无法覆盖安装，需要先卸载再安装。
- 首次从调试版切换到正式版时，需要先完成 WebDAV 同步、卸载调试版，再安装正式版。

## 数据安全

卸载应用会删除设备上的本地数据。切换安装版本或设备前，请先确认 WebDAV 同步完成。

作者：冀缘巧豫