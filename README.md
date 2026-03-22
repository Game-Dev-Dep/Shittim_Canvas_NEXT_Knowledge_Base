# Shittim Canvas NEXT · Knowledge Base / 知识库

## English

### What’s in this repo

This repository contains the **source** for the documentation website: Markdown/MDX pages, images, Docusaurus config, and English locale files. The published site is static HTML (built with `npm run build`).

Content areas include:

- **Features overview** — UI, docks, wallpaper mode, editor, music player, settings, etc.
- **Software & character updates** — full installers, patches, character packs.
- **FAQ** — common issues and troubleshooting.
- **About** — terms and contact.

Versioned snapshots live under `versioned_docs/` (e.g. `version-1.0.0`); the **current** Chinese docs are edited in `docs/`.

### Local development

```bash
npm install
npx docusaurus start
```

**English UI:** run with locale, for example:

```bash
yarn run start --locale en
```

### How to contribute

We welcome corrections, new FAQ entries, screenshots, and translation improvements.

1. **Fork** this repository and create a **branch** for your change (`fix/…`, `docs/…`, `i18n/…`, etc.).
2. **Edit the right place**
   - **Chinese (current):** `docs/` (and category files such as `docs/**/_category_.json` when adding sections).
   - **English:** mirror paths under `i18n/en/docusaurus-plugin-content-docs/current/` (and under `version-1.0.0/` in that tree if you maintain that release’s English copy).
   - **Frozen version** (e.g. 1.0.0): `versioned_docs/version-1.0.0/` for Chinese; keep in sync with your versioning policy.
3. **Assets:** put images next to the doc that uses them (e.g. `docs/功能总览/img/`) and use relative paths in Markdown.
4. **Check locally:** `npm run build` — the project is set to **throw** on broken links, so fix any reported broken anchors before opening a PR.
5. **Pull request:** describe what changed and why; link related issues if any.

**Style:** keep tone consistent with existing pages; for screenshots, prefer the same regions/UI as comparable docs. If you only update Chinese, note in the PR whether English should be updated separately.

**i18n:** after adding new user-facing strings in the theme, you may run `npm run write-translations` and merge the updated JSON under `i18n/en/` as needed.

---

## 中文

### 本仓库是什么

这里存放的是**文档网站**的源码：Markdown/MDX 正文、配图、Docusaurus 配置，以及英文站点的翻译文件。线上站点为静态页面，通过 `npm run build` 生成后部署。

文档大致包括：

- **功能总览** — 主界面、Dock、壁纸模式、编辑模式、音乐播放器、设置等。
- **软件与角色的更新** — 全量包、补丁包、角色包等说明。
- **常见问题** — 使用中的疑问与排错。
- **关于** — 使用条款、联系方式等。

**当前**中文文档在 `docs/` 下维护；历史版本快照在 `versioned_docs/`（例如 `version-1.0.0`）。

### 本地开发

```bash
npm install
npx docusaurus start
```

查看 **英文** 界面示例：

```bash
yarn run start --locale en
```

### 如何贡献

欢迎勘误、补充 FAQ、更新截图与完善翻译。

1. **Fork** 本仓库并新建**分支**（建议命名如 `fix/…`、`docs/…`、`i18n/…`）。
2. **改对路径**
   - **中文（当前）：** 编辑 `docs/`（新增分类时请同时维护对应的 `docs/**/_category_.json`）。
   - **英文：** 在 `i18n/en/docusaurus-plugin-content-docs/current/` 下保持与 `docs/` 对应的目录结构；若需维护某发行版的英文副本，同步修改 `i18n/en/.../version-1.0.0/` 中对应文件。
   - **已冻结的版本**（如 1.0.0）：中文在 `versioned_docs/version-1.0.0/`，是否修改请遵循项目的版本策略。
3. **图片：** 放在引用该图的文档旁（例如 `docs/功能总览/img/`），Markdown 里用相对路径引用。
4. **自检：** 执行 `npm run build`；项目对坏链为 **throw**，请在发起 PR 前修好报错中的链接。
5. **Pull Request：** 说明修改内容与原因；若有关联 issue 请附上链接。

**文风与素材：** 尽量与现有文档语气一致；截图尽量与同类文档的界面区域一致。若只改中文，可在 PR 中说明是否需要另起任务更新英文。

**国际化：** 若在主题或代码中新增需翻译的文案，可运行 `npm run write-translations`，并将 `i18n/en/` 下变更一并纳入提交。

---

## License / 许可证

This repository is licensed under **GNU General Public License v3.0** — see [`LICENSE`](./LICENSE).

本仓库以 **GNU 通用公共许可证第 3 版（GPL-3.0）** 授权，详见仓库根目录 [`LICENSE`](./LICENSE)。

For product-specific terms and disclaimers, see the **About** section on the documentation site (**关于** → 使用条款等).

产品相关的使用条款与声明，请以在线文档 **关于** 栏目为准。
