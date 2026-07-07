# agent-team-frontend

Agent Platform 前端：React + Vite + TypeScript。

## Vercel 部署

1. 编辑 `vercel.json`，将 `YOUR-BACKEND.vercel.app` 换成后端域名（方式 A：Rewrite 代理，推荐）。
2. Framework Preset：**Vite**，Build `npm run build`，Output `dist`。
3. 方式 B 跨域：设置 `VITE_API_BASE_URL=https://你的后端.vercel.app` 并重新 deploy。

## 本地开发

```bash
npm install
npm run dev
```

本地通过 Vite proxy 将 `/api` 转发到 `http://127.0.0.1:8000`。
