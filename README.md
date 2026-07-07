# agent-team-frontend

Agent Platform 前端：React + Vite + TypeScript。

## 本地开发

```bash
npm install
npm run dev
```

默认通过 Vite proxy 将 `/api` 转发到 `http://127.0.0.1:8000`。

## Vercel 部署

1. 在 Vercel 导入本仓库，Framework Preset 选 **Vite**。
2. Build Command: `npm run build`，Output Directory: `dist`。
3. 在 Vercel 项目设置中添加 **Rewrite**，将 `/api/*` 代理到你的后端域名；或在构建前配置环境变量指向后端 API 基址（需配合前端代码调整）。
4. 生产环境需后端开启 CORS / Cookie（`AUTH_COOKIE_SECURE=true`，SameSite 与前后端域名一致）。

## 构建

```bash
npm run build
npm run preview
```
