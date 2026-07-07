# Render 部署指南

## 方式一：Docker 部署（推荐）

1. 注册 [Render.com](https://render.com)（用 GitHub 账号登录）
2. 点击 **New +** → **Web Service**
3. 连接你的 GitHub 仓库
4. Render 自动检测 Dockerfile，点击 **Create Web Service**
5. 等待 3-5 分钟构建完成
6. 获得永久 URL：`https://bagua-api.onrender.com`

## 方式二：直接从 Git URL 部署

1. Render 上点 **New +** → **Web Service**
2. 选择 **Deploy from Git repository**
3. 粘贴仓库 URL
4. 其余同上

## 环境变量（可选）

在 Render Dashboard → Environment 中添加：
- `ANTHROPIC_API_KEY` - Anthropic API Key
- `DEEPSEEK_API_KEY` - DeepSeek API Key
- `OPENAI_API_KEY` - OpenAI API Key

## 注意事项

- 免费计划：512 MB RAM，每月 750 小时
- 15 分钟无请求会自动休眠，下次请求会唤醒（约 30 秒冷启动）
- 建议在 Render Dashboard 设置 Uptime Monitor 防止休眠
