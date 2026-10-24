# Thai_wordcards_pages

泰语组合练习（泰语拼读练习器）网页版的 **GitHub Pages 部署仓库**。

- 线上地址：<https://tangziwuyue.github.io/Thai_wordcards_pages/>
- 内容由主仓库 [`TangziWuyue/Thai_wordcards`](https://github.com/TangziWuyue/Thai_wordcards) 的 `docs/` 目录同步而来（`node web/build-standalone.mjs` 生成后 `node tools/sync-pages.mjs`），**不要在这个仓库里手改**。
- **只保留页面真正要用的文件，不镜像主项目**：
  - 两个页面 + 它们加载的 CSS/JS（`index.html`、`tutorial.html`、`style.css`、`app.js`、`rules.js`、`dict.js`、`audio.js`、`seg.js`、`tour.js`、`pagefx.js`、教学页那 4 个文件）；
  - `fonts/`：88 个 woff2，全部被 `fonts.css` / `fonts-cjk.css` 引用（无冗余）；
  - `data/`：`audio.js`（发音清单）、`dict.js`（词典数据）、`common.js` / `syllable-index.js` / `drop-words.js`（抽词与音节反查）；
  - `audio/`：27,509 条单词音频 + `syl/v1/` 2,132 条音节音频（页面按需加载，**这是体积的主体，但缺一条就少一个发音**）；
  - `.nojekyll`：让 Pages 不做 Jekyll 处理。
- **不包含**主项目的源码/工具/测试/报告（`web/` 之外的 `tools/`、`tests/`、`reports/` 等），也不放 `使用说明.txt`（那是发单文件版用的）。

同步方式（在主仓库里）：

```bash
node tools/sync-pages.mjs   # 把 docs/ 同步到本仓库并提交推送
```
