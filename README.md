# 卡沃 CardVault 官网

[![Deploy GitHub Pages](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml/badge.svg)](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml)

这是卡沃（CardVault）的产品介绍网站。卡沃是一款完全离线运行的 iOS 卡片保险箱，用于在当前设备上安全保存和取用身份证、银行卡的结构化信息及正反面照片。

- 产品网站：[marc-ing.github.io/card-vault-home](https://marc-ing.github.io/card-vault-home/)

> 卡沃目前处于 1.0 发布候选版本的真机验证与 App Store 提交准备阶段。

## 直接预览

这是一个纯静态网站，不需要安装 Node.js，也不需要执行构建命令。

直接双击仓库根目录中的 [`index.html`](index.html)，即可使用浏览器打开完整页面。

## 文件结构

```text
index.html                         # 产品介绍页面
privacy/index.html                 # 隐私政策
support/index.html                 # 帮助与支持
styles.css                        # 页面样式与移动端适配
app-icon.png                      # 来自 iOS 工程的正式 App Icon
.github/workflows/pages.yml       # GitHub Pages 自动部署
```

## 产品原则

- 无需账号，不提供服务端登录。
- 不发起网络请求，不上传卡片内容。
- 拍摄、OCR、加密、保存和取用全部在设备上完成。
- 卡片字段及照片使用 AES-GCM 加密存储。
- 支持系统认证或 6 位 App 独立密码。
- 敏感字段默认遮挡，复制内容仅限本机并限时失效。

## GitHub Pages 部署

仓库中的 [`.github/workflows/pages.yml`](.github/workflows/pages.yml) 会直接发布静态文件，不需要安装依赖或生成构建产物。

首次启用时：

1. 打开仓库的 **Settings → Pages**。
2. 在 **Build and deployment** 中将 **Source** 设为 **GitHub Actions**。
3. 将更改推送到 `main` 分支。
4. 等待 **Deploy GitHub Pages** 工作流完成。
5. 访问 <https://marc-ing.github.io/card-vault-home/>。

以后每次推送到 `main`，页面都会自动更新。

## 公开页面

- [产品介绍](https://marc-ing.github.io/card-vault-home/)
- [隐私政策](https://marc-ing.github.io/card-vault-home/privacy/)
- [帮助与支持](https://marc-ing.github.io/card-vault-home/support/)

产品代码和内部开发文档保存在私有仓库中，不作为公开网站入口。

## License

当前未声明开源许可证。未经明确授权，请勿将仓库内容视为可自由再分发的软件。
