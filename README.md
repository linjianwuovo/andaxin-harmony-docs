# 安大信（鸿蒙端）隐私文档

现有公开地址：

- 隐私政策：https://andaxin-privacy-5uoh87tmjoi.qoder.zone/privacy.html
- 用户协议：https://andaxin-privacy-5uoh87tmjoi.qoder.zone/terms.html

根目录的 `index.md` 和 `terms.md` 保留原有迁移跳转。应用继续使用上面的独立站点地址。

## 文档与发布目录

- `_source/privacy.md`：隐私政策正文，与鸿蒙应用仓库 `docs/privacy.md` 同步，更新及生效日期为 2026-11-21。
- `site/privacy.html`：对应的完整静态隐私页，包含按账号保存本地头像、撤回同意后的清理，以及报修照片在确认提交后上传等说明。
- `site/terms.html`：保留现有公开用户协议正文，将原样式内联以免发布时遗漏CSS；协议正文不变。
- `site/index.html`：站点入口，跳转至隐私政策并保留两份文档链接。

发布时将 `site/` 作为静态站点根目录，沿用当前 Qoder 项目和域名；不要把仓库根目录当作该站点源，也不要改变原隐私/协议路径。

仓库提交与 GitHub Pages 构建不会自动更新上述 Qoder 地址。完成 Qoder 发布后，应重新打开现有地址，核对 2026-11-21 日期、头像本地保存与报修确认上传说明，以及用户协议链接。

## 应用版本关联

本轮政策与鸿蒙应用 0.1.39（versionCode 40，源码提交 `50d4d701a723820d9e75fae4f08a7720eb3a3e6a`）保持一致；具体收集、使用及权限范围以政策正文为准。
