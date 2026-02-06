# 链接转二维码

一个单页 HTML 小工具：输入链接，自动生成二维码，支持下载为 PNG 图片。

## 功能

- 输入任意链接（支持不带 `https://`，会自动补全）
- 一键生成二维码
- 支持下载二维码为 PNG 图片
- 支持回车键快速生成

## 线上使用：https://josiczhou.github.io/link2qrcode/
## 本地使用

用浏览器直接打开 `index.html`，或使用本地服务器：

```bash
# Python 3
python3 -m http.server 8080

# 然后访问 http://localhost:8080
```

## 技术

- 纯 HTML + CSS + JavaScript，无构建步骤
- 使用 [QRCode.js](https://github.com/davidshimjs/qrcodejs)（CDN）生成二维码
