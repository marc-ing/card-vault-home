# CardVault · 卡沃

[![Deploy GitHub Pages](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml/badge.svg)](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml)

[English](#english) · [中文](#中文)

## English

CardVault is a privacy-first, fully offline card vault for iPhone. It keeps structured details and front/back images of identity documents and bank cards securely on the current device, so important information remains available without being uploaded to a server.

- Product website: [marc-ing.github.io/card-vault-home](https://marc-ing.github.io/card-vault-home/)
- Privacy policy: [marc-ing.github.io/card-vault-home/privacy](https://marc-ing.github.io/card-vault-home/privacy/)
- Help and support: [marc-ing.github.io/card-vault-home/support](https://marc-ing.github.io/card-vault-home/support/)

> CardVault 1.0 is currently undergoing release-candidate testing on physical devices and preparation for App Store submission.

### Preview locally

This is a pure static website. No Node.js installation, dependency setup, or build command is required.

Open [`index.html`](index.html) directly in a browser to preview the complete website.

### Project structure

```text
index.html                         # Product landing page
privacy/index.html                 # Privacy policy
support/index.html                 # Help and support
styles.css                         # Shared styles and responsive layout
app-icon.png                       # Official app icon from the iOS project
.github/workflows/pages.yml        # GitHub Pages deployment workflow
```

### Product principles

- No account or server-side sign-in is required.
- Card content is not uploaded, and the app does not depend on network requests.
- Capture, OCR, encryption, storage, and access all take place on the device.
- Card fields and images are encrypted with AES-GCM.
- Access can be protected by system authentication or a separate six-digit app passcode.
- Sensitive fields are concealed by default, and copied content stays local with a limited lifetime.

### Deploy with GitHub Pages

The [GitHub Actions workflow](.github/workflows/pages.yml) publishes the static files directly. No dependencies or generated build artifacts are needed.

For the initial setup:

1. Open **Settings → Pages** in the repository.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Push changes to the `main` branch.
4. Wait for the **Deploy GitHub Pages** workflow to finish.
5. Visit <https://marc-ing.github.io/card-vault-home/>.

Every later push to `main` will update the website automatically.

The CardVault application source code and internal development documentation are maintained privately and are not exposed through this public website.

### License

No open-source license is currently provided. Unless explicit permission is granted, do not treat the contents of this repository as freely redistributable software.

---

## 中文

卡沃（CardVault）是一款注重隐私、完全离线运行的 iPhone 卡片保险箱。它用于在当前设备上安全保存身份证件、银行卡的结构化信息及正反面照片，无需将重要信息上传至服务器。

- 产品网站：[marc-ing.github.io/card-vault-home](https://marc-ing.github.io/card-vault-home/)
- 隐私政策：[marc-ing.github.io/card-vault-home/privacy](https://marc-ing.github.io/card-vault-home/privacy/)
- 帮助与支持：[marc-ing.github.io/card-vault-home/support](https://marc-ing.github.io/card-vault-home/support/)

> 卡沃 1.0 目前处于发布候选版本的真机验证与 App Store 提交准备阶段。

### 本地预览

这是一个纯静态网站，不需要安装 Node.js、安装依赖或执行构建命令。

直接使用浏览器打开仓库根目录中的 [`index.html`](index.html)，即可预览完整网站。

### 项目结构

```text
index.html                         # 产品介绍页面
privacy/index.html                 # 隐私政策
support/index.html                 # 帮助与支持
styles.css                         # 共用样式与移动端适配
app-icon.png                       # 来自 iOS 工程的正式 App Icon
.github/workflows/pages.yml        # GitHub Pages 部署工作流
```

### 产品原则

- 无需账号，不提供服务端登录。
- 不上传卡片内容，应用不依赖网络请求。
- 拍摄、OCR、加密、保存和取用全部在设备上完成。
- 卡片字段及照片使用 AES-GCM 加密存储。
- 支持系统认证或六位 App 独立密码。
- 敏感字段默认遮挡，复制内容仅限本机并限时失效。

### 使用 GitHub Pages 部署

仓库中的 [GitHub Actions 工作流](.github/workflows/pages.yml) 会直接发布静态文件，不需要安装依赖或生成构建产物。

首次启用时：

1. 打开仓库的 **Settings → Pages**。
2. 在 **Build and deployment** 中将 **Source** 设为 **GitHub Actions**。
3. 将更改推送到 `main` 分支。
4. 等待 **Deploy GitHub Pages** 工作流完成。
5. 访问 <https://marc-ing.github.io/card-vault-home/>。

以后每次推送到 `main`，页面都会自动更新。

卡沃的应用源代码和内部开发文档保存在私有仓库中，不会通过这个公开网站对外提供。

### 许可证

当前未声明开源许可证。未经明确授权，请勿将仓库内容视为可自由再分发的软件。
