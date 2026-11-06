# 月亮故事屋app

安卓离线睡前故事机。本仓库是固定的APK发布及应用内更新来源。

**当前正式版本：1.2.0（versionCode 3）**

- [下载最新APK](https://github.com/fuqiang12138/moon-story-house-app/releases/latest/download/moonstory.apk)
- [查看最新版本与更新说明](https://github.com/fuqiang12138/moon-story-house-app/releases/latest)
- [机器可读的版本信息](https://github.com/fuqiang12138/moon-story-house-app/releases/latest/download/update.json)

## 手机如何更新

先手动覆盖安装一次1.2.0，保留原有故事库和设置。之后打开App会检查GitHub新版，也可以进入“设置 → 检查软件更新”。发现新版后，在App内下载，下载完成校验后点击安装，并在系统安装页面确认。

首次使用App内安装，需要在系统设置中允许“月亮故事屋”安装应用。检查、下载更新需要手机能访问GitHub；故事播放仍然可以离线使用。App未打开时不发送厂商推送通知。

## 故事功能

20篇原创动物冒险睡前故事、100种中文音色、0.65–1.50倍语速。默认“暖月女声”的20篇未修改故事附带完整音频；其他音色及自编故事首次准备整篇，之后复用。支持编辑、新增、收藏、导入导出、定时停止和夜间模式。

## 以后持续在这个项目发布

每次使用原签名构建新版，提高versionCode，在本仓库创建对应的正式Release并标记为Latest，上传以下资产：

1. `moonstory.apk`：签名后的完整安卓安装包。
2. `update.json`：同一安装包对应的版本号、更新说明、字节数、SHA256、最低安卓版本及下载链接。
3. `SHA256SUMS.txt`：供人工核对的文件校验和。

APK链接应绑定该版本的具体标签，例如 `releases/download/v1.2.0/moonstory.apk`。App始终读取固定的 `releases/latest/download/update.json`，所以以后的新版本无需修改手机端更新地址。根目录的update.json保留一份当前版本资料便于查看，App以Release资产为准。

这里只存公开发布资料。签名私钥及包含私钥的开发源码压缩包由维护者另行保管，不上传本仓库。

## 本版验证范围

已完成编译、原签名校验、版本及更新元数据检查、下载完整性/取消/损坏恢复测试、设置入口和既有故事功能逻辑检查。尚未在小米15真机验证安装授权及系统安装界面的全过程。
