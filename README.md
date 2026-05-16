# 🎵 YesPlayMusic 网易云登录助手

一个纯静态网页工具，帮助你在 **YesPlayMusic** 无法正常登录网易云音乐账号时，安全地从网页版提取 Cookie 并注入到 YesPlayMusic 中，恢复完整功能。

> 🔐 **完全本地运行，Cookie 不上传任何服务器，安全可靠。**
>
> 🤖 **本项目由 [DeepSeek AI](https://www.deepseek.com/) 生成**
>
> 🌐 **在线使用地址：[https://yesplay.hxrch.top](https://yesplay.hxrch.top)**

---

## 📖 背景

YesPlayMusic 是一款优秀的第三方网易云音乐播放器，但有时会遇到无法登录网易云账号的问题。此问题的讨论和原始解决方案来自 [YesPlayMusic Issue #2398](https://github.com/qier222/YesPlayMusic/issues/2398)，由 [LuorixDev](https://github.com/LuorixDev) 提供了基于 Cookie 注入的解决方案。

本项目将该方案封装为一个友好的可视化网页工具，用户无需手动编辑脚本代码，只需粘贴 Cookie 即可自动生成注入脚本，进一步降低了操作门槛。

---

## 🚀 使用方法

### 第一步：获取网易云音乐 Cookie

1. 打开 [网易云音乐网页版](https://music.163.com/) 并**确保已登录成功**。
2. 按 `F12` 打开开发者工具，切换到 **Network（网络）** 标签页。
3. 刷新页面，在请求列表中找到任意一个以 `weblog` 开头的请求。
4. 点击该请求，在右侧 **Headers（标头）** 中找到 **Cookie** 字段，**完整复制**其值（值可能很长，请确保完整复制）。

### 第二步：生成注入脚本

5. 打开本工具页面：[https://yesplay.hxrch.top](https://yesplay.hxrch.top)
6. 将复制的 Cookie 粘贴到文本框中。
7. 点击 **⚡ 生成注入脚本** 按钮。
8. 点击 **📋 复制脚本** 将生成的完整脚本复制到剪贴板。

### 第三步：注入 YesPlayMusic

9. 打开你的 YesPlayMusic 页面。
10. 按 `F12` 打开开发者工具，切换到 **Console（控制台）** 标签页。
11. 粘贴脚本并按下 `Enter` 运行。
12. 脚本会自动处理 Cookie 和 localStorage，约 1 秒后自动刷新页面 —— **登录成功！** 🎉

---

## ✨ 特性

- 🔒 **纯前端处理**：Cookie 仅在本地浏览器中处理，绝不发送到任何服务器
- 🎨 **美观界面**：毛玻璃风格设计，清晰的操作引导
- ⚡ **一键生成**：自动将你的 Cookie 嵌入脚本，无需手动编辑
- 📋 **一键复制**：生成后可直接复制到剪贴板
- 📱 **响应式设计**：适配桌面端和移动端浏览器
- 🤖 **AI 驱动开发**：由 DeepSeek AI 辅助完成前端开发

---

## 🛠️ 技术栈

- 纯静态 HTML / CSS / JavaScript
- 无需任何依赖或构建工具
- 可部署至 GitHub Pages 等静态网页托管平台，通过自定义域名访问

---

## 📦 部署

### 在线使用

直接访问 **[https://yesplay.hxrch.top](https://yesplay.hxrch.top)** 即可使用。

### 本地使用

下载 `index.html` 文件，用浏览器直接打开即可，无需任何服务器环境。

### 自行部署

1. Fork 本仓库
2. 进入仓库 **Settings → Pages**
3. 选择部署分支（如 `main`）和目录（`/ (root)`）
4. （可选）在 Settings → Pages 中配置自定义域名
5. 保存后即可访问

---

## ⚠️ 注意事项

- Cookie 是敏感信息，**请勿将其分享给他人或粘贴到不可信的网站**。
- 本工具完全在浏览器本地运行，**不会存储、上传或记录你的 Cookie**。
- Cookie 有效期通常为 15 天左右，过期后需重新获取并注入。
- 如果登录失败，请检查：
  - 是否复制了**完整的** Cookie 字符串
  - 网易云网页版是否处于**已登录**状态
  - Cookie 是否已过期

---

## 🙏 致谢

- **原始解决方案**：[LuorixDev](https://github.com/LuorixDev) 在 [YesPlayMusic Issue #2398](https://github.com/qier222/YesPlayMusic/issues/2398) 中提供的 Cookie 注入脚本
- 推荐搭配 [AMLL-YesPlayMusic-Sync](https://github.com/LuorixDev/AMLL-YesPlayMusic-Sync) 使用，获得逐字歌词和更炫酷的歌词特效
- 本项目由 **DeepSeek AI** 辅助生成

---

## 📄 许可证

本项目基于 [MIT License](LICENSE) 开源。

---

## ⭐ 支持

如果这个工具帮助到了你，欢迎给仓库点个 Star ⭐！

有问题或建议？欢迎提交 [Issue](../../issues) 或前往原始讨论 [Issue #2398](https://github.com/qier222/YesPlayMusic/issues/2398) 查看详情。
