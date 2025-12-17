# Gmail Manager

基于 Tauri 2 + React + Rust 的桌面 Gmail 管理工具。

## 功能

- 📬 邮件列表浏览（收件箱、已发送、草稿、垃圾箱等）
- ⭐ 星标管理
- 📝 撰写和发送邮件
- 📎 附件下载
- 🗑️ 删除和归档邮件
- 🔐 Google OAuth2 认证

## 开发

### 前置要求

- Node.js 18+
- Rust 1.70+
- [Tauri CLI](https://v2.tauri.app/start/prerequisites/)

### 配置 OAuth

1. 前往 [Google Cloud Console](https://console.cloud.google.com/)
2. 创建项目并启用 Gmail API
3. 创建 OAuth 2.0 凭据（桌面应用类型）
4. 将 `CLIENT_ID` 和 `CLIENT_SECRET` 填入 `src-tauri/src/oauth.rs`

### 运行

```bash
npm install
npm run tauri dev
```

### 构建

```bash
npm run tauri build
```

## 技术栈

- 前端：React 18 + Tailwind CSS + Lucide Icons
- 后端：Rust + Tauri 2
- API：Gmail REST API
