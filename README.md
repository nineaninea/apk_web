# 📱 极速安卓浏览器 (Android 原生网页浏览器工程)

本项目是由 WebDroid 自动化生成的标准原生 Android 网页浏览器工程，采用 **Kotlin + AndroidX + 硬件加速 WebView** 架构。

---

## ⚡ 如何一键生成并下载 APK 安装包？

### 方式 1：GitHub Actions 免费云端打包（推荐！无需安装任何软件）
1. 在 GitHub 上新建一个仓库（公开或私有均可）。
2. 将解压出来的本项目所有文件上传/推送（Push）到该仓库的 `main` 分支。
3. 进入 GitHub 仓库上方的 **Actions** 选项卡。
4. 你会看到 **"🚀 Build Android APK"** 自动开始运行（大约 1~2 分钟）。
5. 编译完成后，在下方 **Artifacts** 处点击即可直接下载 **`极速安卓浏览器-v1.0.0.apk`** 安装到手机上！

---

### 方式 2：使用 Android Studio 编译打包
1. 下载并安装官方 [Android Studio](https://developer.android.com/studio)。
2. 选择 **Open Project**，打开解压后的本文件夹。
3. 等待 Gradle 依赖同步完成（底部进度条走完）。
4. 点击顶部菜单栏 **Build** -> **Build Bundle(s) / APK(s)** -> **Build APK(s)**。
5. 完成后右下角会弹出提示，点击 **locate** 即可在 `app/build/outputs/apk/debug/app-debug.apk` 找到生成的 APK 安装包。

---

### 方式 3：命令行一键编译 (Linux / macOS / Windows / Termux)
确保已安装 JDK 17 及 Android SDK，在项目根目录运行：
```bash
# Linux / macOS:
chmod +x gradlew
./gradlew assembleDebug

# Windows CMD / PowerShell:
gradlew.bat assembleDebug
```
生成的 APK 位于：`app/build/outputs/apk/debug/app-debug.apk`。

---

## 🛠️ 工程配置清单
- **应用名称**: 极速安卓浏览器
- **包名 (Package Name)**: `com.android.webdroid.browser`
- **版本号**: `1.0.0` (Code: 1)
- **默认首页**: `https://www.bing.com`
- **支持架构**: arm64-v8a, armeabi-v7a, x86_64
- **最低 Android 版本**: Android 7.0 (API 24)
- **目标 Android 版本**: Android 14+ (API 34)
