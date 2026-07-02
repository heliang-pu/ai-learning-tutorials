# Transformer 交互式教学

一个面向初学者的 Transformer 中文交互式图解教程。

内容从一句话进入模型开始，逐步拆解分词与嵌入、位置编码、注意力机制、多头注意力、Transformer Block、训练、生成采样以及模型家族全景。

## 在线学习

GitHub Pages 发布后可直接在浏览器中访问：

https://heliang-pu.github.io/transformer-interactive-tutorial/

## 本地预览

```bash
python3 -m http.server 8000
```

然后打开：

http://localhost:8000/

## 文件说明

- `index.html`：教程主页面。
- `support.js`：交互组件运行时依赖。

页面会从 CDN 加载 React、ReactDOM、Babel 和 Google Fonts，因此首次打开需要联网。

Last updated: 2026-07-02
