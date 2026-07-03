# AI Learning Tutorials

中文 AI 交互式教学页面集合，用来托管 Transformer、VLA、WAM、机器人论文等主题的可视化教程。

## 在线学习

GitHub Pages:

https://heliang-pu.github.io/ai-learning-tutorials/

当前已发布：

- [Transformer 完全图解](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/transformer/)
- [π0 论文交互教学](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/pi0/)
- [π0.5 论文交互教学](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/pi05/)
- [Ego-Pi 论文交互教学](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/ego-pi/)
- [WAM DreamZero 论文交互教学](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/wam-dreamzero/)
- [π0.6 论文交互教学](https://heliang-pu.github.io/ai-learning-tutorials/tutorials/pi06/)

## 目录结构

```text
.
├── index.html
├── tutorials/
│   ├── transformer/
│   │   ├── index.html
│   │   └── support.js
│   ├── pi0/
│   │   ├── index.html
│   │   ├── support.js
│   │   └── figures/
│   │       ├── pi0-fig5-robots.jpg
│   │       └── pi0-fig6-tasks.jpg
│   ├── pi05/
│   │   ├── index.html
│   │   └── support.js
│   ├── ego-pi/
│   │   ├── index.html
│   │   └── support.js
│   ├── wam-dreamzero/
│   │   ├── index.html
│   │   └── support.js
│   └── pi06/
│       ├── index.html
│       ├── support.js
│       └── figures/
│           ├── fig1-recap-overview.jpg
│           └── ...
└── docs/
    └── adding-tutorials.md
```

约定：

- 顶层 `index.html` 是教程集合首页。
- 每个主题一个目录，例如 `tutorials/transformer/`、`tutorials/pi06/`、`tutorials/wam-dreamzero/`。
- 每个主题目录内放自己的 `index.html` 和导出依赖文件，便于直接从 Claude/其他工具导出的 HTML 迁移过来。

## 本地预览

```bash
python3 -m http.server 8000
```

然后打开：

http://localhost:8000/

页面会从 CDN 加载 React、ReactDOM、Babel 和 Google Fonts，因此首次打开需要联网。
