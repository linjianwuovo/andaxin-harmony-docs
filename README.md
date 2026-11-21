# 安大信（鸿蒙端）隐私文档

官方发布平台为 GitHub Pages，公开地址：

- 隐私政策：https://linjianwuovo.github.io/andaxin-harmony-docs/site/privacy.html
- 用户协议：https://linjianwuovo.github.io/andaxin-harmony-docs/site/terms.html

根目录的 `index.md` 和 `terms.md` 分别直接跳转到上述官方页面，并保留可手动打开的链接。

## 文档与发布目录

- `_source/privacy.md`：隐私政策正文，与鸿蒙应用仓库 `docs/privacy.md` 同步，更新及生效日期为 2026-11-21。
- `site/privacy.html`：对应的完整静态隐私页，包含按账号保存本地头像、撤回同意后的清理，以及报修照片在确认提交后上传等说明。
- `site/terms.html`：保留现有公开用户协议正文，将原样式内联以免发布时遗漏CSS；协议正文不变。
- `site/index.html`：站点入口，跳转至隐私政策并保留两份文档链接。
- `site/harmony-update.json`：鸿蒙 `prerelease` 公开版本元数据，仅从已经发布、下载及哈希验收通过的 GitHub 附件生成；版本号、版本码、发布时间、发布地址及签名 HAP 的名称、URL、大小和 SHA-256 均公开，仓库及附件继续为 private。

`site/` 是自包含的静态站点目录，页面及内联样式可独立作为静态站点根目录使用。当前 GitHub Pages 沿用 legacy 发布方式，从 `main` 分支的仓库根目录自动发布，因此官方页面保留上述 `/site/privacy.html` 和 `/site/terms.html` 路径。

更新推送到 `main` 后由现有 GitHub Pages 流程自动发布，无需另建部署工作流，也不再依赖旧 Qoder 项目或域名。发布后应重新打开上述官方地址，核对 2026-11-21 日期、头像本地保存与报修确认上传说明，以及用户协议链接。

## 应用版本关联

公开版本文件的当前值以 `site/harmony-update.json` 为准。建立通道时先使用已经验收的 0.1.42（versionCode 43），后续仅在新版本附件验收通过后更新，不能预告不存在的安装包。

鸿蒙端从 0.1.43 起提供关于页手动检查入口。更新请求不携带学校身份或 GitHub 凭据；用户主动打开发布或安装包链接后由系统浏览器访问 GitHub，私有仓库下载需要访问权限，不自动安装。隐私政策增加更新托管及基础网络信息说明，应用门禁版本为 `2026-11-21-2`。

公开 JSON 使用 `schemaVersion: 1`、`platform: harmonyos`、`channel: prerelease`，包含 `versionCode`、`versionName`、`publishedAt`、`releaseUrl` 及 `signedHap`（`name`、`url`、`size`、`sha256`）；不含账号、设备信息、访问令牌或私有认证数据。
