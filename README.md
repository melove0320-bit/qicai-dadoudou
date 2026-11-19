# 七彩打豆豆｜分享入口网页

纯静态宣传落地页，使用原生 HTML 与 CSS。无需构建、服务器、数据库、域名或第三方 API，可通过 GitHub Pages 免费托管。

## 文件

- `index.html`：响应式游戏介绍页。
- `assets/mini-program-code.png`：提供的永久小程序码原图副本。不要裁剪、重绘或压缩这张图片。

页面链接是展示介绍与小程序码的普通网页地址，不是微信官方 URL Link，也不保证点击网页就能自动唤起小游戏。访客可在微信中扫一扫，或长按识别小程序码进入游戏。

## 发布到 GitHub Pages

1. 登录 [GitHub](https://github.com/)，新建一个仓库，例如 `colorful-beans-landing`。公开仓库可直接使用 GitHub Pages 免费方案；不要勾选创建 README（本目录已有文件）。
2. 将本目录中的 `index.html`、`README.md` 和 `assets` 文件夹上传到仓库根目录，保持目录结构不变。也可以在本目录初始化 Git 并推送到新仓库：

   ```bash
   git init
   git add index.html README.md assets/mini-program-code.png
   git commit -m "Create game landing page"
   git branch -M main
   git remote add origin https://github.com/你的用户名/colorful-beans-landing.git
   git push -u origin main
   ```

3. 在仓库打开 **Settings → Pages**，在 **Build and deployment** 下将 **Source** 设为 **Deploy from a branch**，分支选 `main`、目录选 `/(root)`，保存。
4. 等待 Pages 部署完成。设置页会显示 HTTPS 访问地址，通常为 `https://你的用户名.github.io/colorful-beans-landing/`。若仓库名是 `你的用户名.github.io`，地址通常是 `https://你的用户名.github.io/`。
5. 更新网页时，修改相应文件并提交推送到 `main`；Pages 会自动重新部署。保留仓库名和账号不变，网页入口地址就保持不变。

## 本地预览

直接用浏览器打开 `index.html` 即可预览；图片通过相对路径 `assets/mini-program-code.png` 加载，适用于 GitHub Pages 的仓库子路径部署。

## 发布前检查

- 在手机与电脑浏览器打开部署地址，确认页面没有横向溢出且小程序码完整显示。
- 在微信中打开该 HTTPS 页面，尝试长按小程序码识别，或用另一台设备的微信扫一扫。
- GitHub Pages 只托管网页；小程序码本身是否有效由微信官方码决定。
