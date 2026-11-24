# githubio — Leon 个人主页 (changchun-zhou.github.io)

- Jekyll (academicpages)；remote `git@github.com:changchun-zhou/changchun-zhou.github.io.git`，分支 main。
- 主内容：`_pages/about.md`；头像/favicon：`_config.yml` avatar + `_includes/head/custom.html`（换头像必同步重生成 favicon 并把 `?v=` +1）。
- Chip Gallery 大图 `images/chips_platform.jpg` 由 `_harness/build_chip_gallery.py` 重生成。
- harness 产物（截图证据、脚本、QA）进 `_harness/`；旧图标等归档在 `backup/`。
- `*-LAPTOP-790P2OGK.*` 是 OneDrive 冲突副本，未跟踪，勿提交。
- **push = 公开发布**：commit 可直接做，push 前需 Leon 确认（除非本轮已明确授权）。
- ISSCC27 禁令已解除（AP 于 2026-11-23 发布）：Fornax(34.6)/LYRA(34.2) 两篇均为 Session 34 Highlight（证据 `_harness/ISSCC27_Session34_Highlights_*.png`） 已上主页；缩略图由 `_harness/build_isscc27_cards.py <AP.pdf>` 从 AP 裁生成。die photo/S1/highlight 外数字仍等 2027-02-17 报告后再放。
