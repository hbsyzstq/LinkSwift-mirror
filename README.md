# LinkSwift 镜像

[LinkSwift](https://github.com/hmjz100/LinkSwift)（网盘直链下载助手改版）用户脚本的个人镜像，用于备份与稳定安装源。

- 当前版本：**v1.1.3**（正式版，同步于 2026-10-24）
- 文件：[`LinkSwift.user.js`](./LinkSwift.user.js)
- 许可：AGPL-3.0-or-later（见 [LICENSE](./LICENSE)）

## 上游

| 项 | 值 |
| --- | --- |
| 原项目 | 网盘直链下载助手（作者 油小猴，<https://github.com/syhyz1990/baiduyun>） |
| 改版作者 | Hmjz100（<https://github.com/hmjz100/LinkSwift>） |
| 官方发布渠道 | GitHub、Gitee、脚本猫（ID 1604）、OpenUserJS |

本仓库不含任何修改，仅为原样备份。问题反馈请去上游 Issues，这里不受理。

## 安装

用 Tampermonkey / 脚本猫打开下面的链接即可（需以 `.user.js` 结尾才会被识别为脚本）：

```
https://raw.githubusercontent.com/hbsyzstq/LinkSwift-mirror/main/LinkSwift.user.js
```

或把 `LinkSwift.user.js` 拖进脚本管理器仪表盘。

> 实测：部分网络下 GitHub raw 链接不会被篡改猴拦截成安装页（会当纯文本显示），遇到就改用官方脚本猫源
> `https://scriptcat.org/scripts/code/1604/LinkSwift.user.js`。

## 说明

- 通过各网盘**公开 API** 获取直链，不破解限速；网盘页面需保持登录状态。
- 支持：百度网盘 / 阿里云盘 / 中国移动云盘 / 天翼云盘 / 迅雷云盘 / 夸克网盘 / UC 网盘 / 123 云盘。
- 运行时从 unpkg 加载 jQuery、SweetAlert2 11、js-md5、js-sha256，首次使用需能访问 unpkg。
- 脚本头未声明 `@updateURL`/`@downloadURL`，从哪个地址安装就从哪个地址检查更新。
