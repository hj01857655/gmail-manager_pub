# Gmail Manager

基于 Tauri 2 + React + Rust 的桌面 Gmail 客户端。

## 功能

- 📬 邮件管理（收件箱、已发送、草稿、垃圾箱、归档等）
- 👥 多账号支持（添加、切换、管理多个 Gmail 账号）
- ⭐ 星标管理
- 📝 撰写和发送邮件
- 📎 附件支持
- 🗑️ 删除和归档邮件
- 🔐 Google OAuth2 安全认证
- 🔄 Token 自动刷新
- 🌓 深色/浅色主题切换
- ⚙️ 可自定义设置（阅读窗格、邮件密度等）

## 技术栈

- **前端**：React 18 + Tailwind CSS + Lucide Icons
- **后端**：Rust + Tauri 2
- **协议**：IMAP/SMTP over OAuth2

## 安装

从 [Releases](https://github.com/hj01857655/gmail-manager/releases) 下载最新版本。

## 开发

### 前置要求

- Node.js 18+
- Rust 1.70+
- [Tauri CLI](https://v2.tauri.app/start/prerequisites/)

### 配置 OAuth

1. 前往 [Google Cloud Console](https://console.cloud.google.com/)
2. 创建项目并启用 Gmail API
3. 创建 OAuth 2.0 凭据（桌面应用类型）
4. 复制 `src-tauri/.env.example` 为 `src-tauri/.env`
5. 填入 `CLIENT_ID` 和 `CLIENT_SECRET`

### 运行

```bash
npm install
npm run tauri dev
```

### 构建

```bash
npm run tauri build
```

## 许可证

MIT

## 作者

[@hj01857655](https://github.com/hj01857655)
