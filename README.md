# markify 官网

[markify](https://github.com/lifedever/markify) 产品官网 —— 纯静态站点，自动部署到 GitHub Pages。

> 这是**公开**仓库，只含营销官网。app 源码在**私有**仓库 `markify-app`，不公开。

## 技术

- 纯静态 HTML/CSS/JS，无构建步骤、无框架。
- 字体自托管（JetBrains Mono + Hanken Grotesk，OFL，`assets/fonts/`），不依赖任何 CDN。
- 视觉与 app 一致（青柠绿 + JetBrains Mono + 深色）。

## 本地预览

直接用浏览器打开 `index.html` 即可；或起一个静态服务器：

```bash
python3 -m http.server 8080   # 然后访问 http://localhost:8080
```

## 部署

push 到 `main` → GitHub Actions（`.github/workflows/deploy.yml`）自动发布到 GitHub Pages，无需构建。

需在仓库 **Settings → Pages → Build and deployment → Source** 选 **GitHub Actions**（仅首次）。

## 待填占位

- 闲鱼店铺链接：`index.html` 中 `[data-xianyu]`
- macOS 下载地址：`index.html` 中 `[data-download]`（随 app 发版更新）
