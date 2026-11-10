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

## 与 iPhone / iPad 同步书籍（0.3.0 起）

- Mac 和 iPhone / iPad 登录同一个 Apple ID，并在系统设置里打开 iCloud 云盘，书架里的 EPUB 会通过你自己的 iCloud 互相同步。
- 书籍只存在你的 iCloud 里，不会上传到 Ad Astra 服务器。
- 打开书架、导入新书后会自动同步，也可以点书架右上角的“Sync with iCloud”。
- 需要先在 iPhone / iPad 版 Ad Astra 里打开过一次 iCloud 书籍同步；否则 Mac 上书架会显示“仅本机”。
- 目前只同步书籍文件，阅读进度、笔记和书签不同步；在一台设备上删除书不会删除另一台上的书。

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

**Book sync with iPhone / iPad (0.3.0+):** with the same Apple ID and iCloud Drive
turned on, EPUB books sync through your own iCloud and are never uploaded to the
Ad Astra server. Sync runs when the bookshelf opens and after an import, or from
the "Sync with iCloud" button. iCloud book sync must have been used once in the
iPhone / iPad app first; otherwise the Mac shelf stays local. Only book files
sync: reading positions, notes and bookmarks do not, and deleting a book on one
device does not delete it on the other.

**Known limits:** no automatic updates; a few pages such as Sync Article open in
the browser instead of inside the app.
