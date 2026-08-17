# CardVault

[![Deploy GitHub Pages](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml/badge.svg)](https://github.com/marc-ing/card-vault-home/actions/workflows/pages.yml)

English · [简体中文](README.zh-CN.md)

CardVault is a privacy-first, fully offline card vault for iPhone. It keeps structured details and front/back images of identity documents and bank cards securely on the current device, so important information remains available without being uploaded to a server.

- Product website: [marc-ing.github.io/card-vault-home](https://marc-ing.github.io/card-vault-home/)
- Privacy policy: [marc-ing.github.io/card-vault-home/privacy](https://marc-ing.github.io/card-vault-home/privacy/)
- Help and support: [marc-ing.github.io/card-vault-home/support](https://marc-ing.github.io/card-vault-home/support/)

> CardVault 1.0 is currently undergoing release-candidate testing on physical devices and preparation for App Store submission.

## Preview locally

This is a pure static website. No Node.js installation, dependency setup, or build command is required.

Open [`index.html`](index.html) directly in a browser to preview the complete website.

## Project structure

```text
index.html                         # Product landing page
privacy/index.html                 # Privacy policy
support/index.html                 # Help and support
styles.css                         # Shared styles and responsive layout
app-icon.png                       # Official app icon from the iOS project
.github/workflows/pages.yml        # GitHub Pages deployment workflow
```

## Product principles

- No account or server-side sign-in is required.
- Card content is not uploaded, and the app does not depend on network requests.
- Capture, OCR, encryption, storage, and access all take place on the device.
- Card fields and images are encrypted with AES-GCM.
- Access can be protected by system authentication or a separate six-digit app passcode.
- Sensitive fields are concealed by default, and copied content stays local with a limited lifetime.

## Deploy with GitHub Pages

The [GitHub Actions workflow](.github/workflows/pages.yml) publishes the static files directly. No dependencies or generated build artifacts are needed.

For the initial setup:

1. Open **Settings → Pages** in the repository.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.
3. Push changes to the `main` branch.
4. Wait for the **Deploy GitHub Pages** workflow to finish.
5. Visit <https://marc-ing.github.io/card-vault-home/>.

Every later push to `main` will update the website automatically.

The CardVault application source code and internal development documentation are maintained privately and are not exposed through this public website.

## License

No open-source license is currently provided. Unless explicit permission is granted, do not treat the contents of this repository as freely redistributable software.
