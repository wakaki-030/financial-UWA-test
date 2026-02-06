# CRT Ledger — 真·可安装 PWA（无需编译）

这是一个完整的 PWA 静态站点：只要把整个文件夹上传到 **HTTPS** 的静态托管，就能在 Android 上“安装到主屏幕”，离线可用。

## 文件结构
- index.html （应用本体）
- manifest.webmanifest（PWA 清单）
- sw.js（离线缓存 Service Worker）
- icons/（图标）

## 最快部署方式（任选其一）
### A) GitHub Pages（免费）
1) 在 GitHub 新建仓库（public）
2) 把这些文件上传到仓库根目录
3) Settings → Pages → Deploy from branch → 选择 main / root
4) 等它生成一个 https://xxxx.github.io/xxxx/ 的网址
5) 用手机 Chrome 打开这个网址 → 右上角菜单 → “添加到主屏幕”

### B) Netlify / Vercel（免费）
- 新建静态站点，直接拖拽上传整个文件夹即可（必须 HTTPS）
- 用手机打开生成的 HTTPS 链接 → 添加到主屏幕

## 安装提示
- 必须在 **HTTPS** 或 localhost 上，PWA 才能安装与离线（这是浏览器安全规则）
- 首次打开后，随便点一下按钮即可激活音效（系统要求音频由用户手势触发）
