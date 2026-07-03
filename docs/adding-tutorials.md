# Adding Tutorials

新增教程时推荐按主题建立独立目录：

```text
tutorials/
  pi06/
    index.html
    support.js
    figures/
      fig1-example.jpg
  wam-dreamzero/
    index.html
    support.js
```

步骤：

1. 在 `tutorials/` 下创建主题目录，例如 `tutorials/pi06/`。
2. 把导出的 HTML 命名为 `index.html`。
3. 如果页面依赖 `support.js`、`figures/` 或其他相对资源，把它们放在同一个主题目录内。
4. 在顶层 `index.html` 增加一张课程卡片，链接到 `./tutorials/<topic>/`。
5. 提交并推送到新仓库的 `main` 和 `gh-pages` 分支，GitHub Pages 会从 `gh-pages` 自动重新发布。

这种结构的好处是每个导出的 HTML 都可以保持自己的相对路径，不容易互相影响。
