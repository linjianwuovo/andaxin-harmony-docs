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

`site/` 是自包含的静态站点目录，页面及内联样式可独立作为静态站点根目录使用。当前 GitHub Pages 沿用 legacy 发布方式，从 `main` 分支的仓库根目录自动发布，因此官方页面保留上述 `/site/privacy.html` 和 `/site/terms.html` 路径。

更新推送到 `main` 后由现有 GitHub Pages 流程自动发布，无需另建部署工作流，也不再依赖旧 Qoder 项目或域名。发布后应重新打开上述官方地址，核对 2026-11-21 日期、头像本地保存与报修确认上传说明，以及用户协议链接。

## 应用版本关联

现有文档基线与鸿蒙应用 0.1.39（versionCode 40，源码提交 `50d4d701a723820d9e75fae4f08a7720eb3a3e6a`）保持一致；具体收集、使用及权限范围以政策正文为准。

计划在鸿蒙应用 0.1.40 中关联上述官方 GitHub Pages 地址；版本发布状态以最终核验结果为准。
