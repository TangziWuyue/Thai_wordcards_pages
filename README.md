# Thai_wordcards_pages

泰语组合练习（泰语拼读练习器）网页版的 **GitHub Pages 部署仓库**。

- 线上地址：<https://tangziwuyue.github.io/Thai_wordcards_pages/>
- 内容由主仓库 [`TangziWuyue/Thai_wordcards`](https://github.com/TangziWuyue/Thai_wordcards) 的 `docs/` 目录同步而来（`node web/build-standalone.mjs` 生成后 rsync），**不要在这个仓库里手改**。
- 这里只放静态产物：两个页面（练习 / 教学）、样式与脚本、打包字体、词典数据（按需加载）、以及全部音频（27,509 条单词 + 2,132 条音节）。

同步方式（在主仓库里）：

```bash
node tools/sync-pages.mjs   # 把 docs/ 同步到本仓库并提交推送
```
