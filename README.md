# 链接转二维码

一个单页 HTML 小工具：输入链接，自动生成二维码，支持下载为 PNG 图片。

## 功能

- 输入任意链接（支持不带 `https://`，会自动补全）
- 一键生成二维码
- 支持下载二维码为 PNG 图片
- 支持回车键快速生成

## 本地使用

用浏览器直接打开 `index.html`，或使用本地服务器：

```bash
# Python 3
python3 -m http.server 8080

# 然后访问 http://localhost:8080
```

## 部署到 GitHub Pages

1. 在 GitHub 新建仓库（例如 `url-to-qrcode`）
2. 将本目录下的 `index.html` 和 `README.md` 推送到仓库
3. 打开仓库 **Settings → Pages**
4. **Source** 选择 **Deploy from a branch**
5. **Branch** 选择 `main`（或 `master`），目录选 **/ (root)**，保存
6. 几分钟后访问：`https://你的用户名.github.io/仓库名/`

例如：`https://username.github.io/url-to-qrcode/`

## 技术

- 纯 HTML + CSS + JavaScript，无构建步骤
- 使用 [QRCode.js](https://github.com/davidshimjs/qrcodejs)（CDN）生成二维码
