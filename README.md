# Ad Astra for Mac

Ad Astra 的 Mac 桌面版。在这里下载安装包：
**[下载最新版本 / Download the latest release](https://github.com/tangbin90/adastra-mac/releases/latest)**

## 系统要求

- Apple 芯片的 Mac（M1 及更新机型），暂不支持 Intel Mac
- macOS 13 或更高版本
- 已有 Ad Astra 账号（服务地址 `https://www.catsdogs.site:8443`）

## 安装

1. 在 Releases 页面下载 `Ad-Astra-<版本>-mac-arm64.zip`，双击解压。
2. 把 `Ad Astra.app` 拖进“应用程序”文件夹。
3. 首次打开时系统会提示“无法验证开发者”，因为这个版本还没有经过 Apple 公证：
   - 打开“系统设置 → 隐私与安全性”，在页面下方找到 Ad Astra 的提示，点“仍要打开”。
   - 或者在终端运行：`xattr -dr com.apple.quarantine "/Applications/Ad Astra.app"`
4. 打开后点登录，应用会跳到浏览器完成登录，再自动回到应用。

## 已知限制

- 应用不会自动更新，新版本需要回到这里重新下载。
- “Sync Article”等少数页面暂时没有 Mac 版界面，应用内会提供按钮在浏览器中打开。

---

# English

The Mac desktop app for Ad Astra. Get the installer from
[Releases](https://github.com/tangbin90/adastra-mac/releases/latest).

**Requirements:** Apple silicon Mac (M1 or later; Intel is not supported), macOS 13+,
and an Ad Astra account on `https://www.catsdogs.site:8443`.

**Install:**

1. Download `Ad-Astra-<version>-mac-arm64.zip` and unzip it.
2. Move `Ad Astra.app` to Applications.
3. The app is not notarized by Apple yet, so macOS blocks the first launch. Open
   System Settings → Privacy & Security and choose "Open Anyway", or run
   `xattr -dr com.apple.quarantine "/Applications/Ad Astra.app"` in Terminal.
4. Sign in. The app finishes sign-in in your browser and then returns.

**Known limits:** no automatic updates; a few pages such as Sync Article open in
the browser instead of inside the app.
