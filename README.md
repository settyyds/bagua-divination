# ☯ 八卦推演系统

传统中国命理学 x 多模型 AI 全栈融合平台

[![Deploy to Render](https://render.com/images/deploy-to-render-button.svg)](https://render.com/deploy?repo=https://github.com/settyyds/bagua-divination)

---

## 一键部署到 Render

点击 Deploy to Render 按钮，自动检测 Dockerfile 并部署。
免费计划 512MB RAM，15分钟无请求会休眠。

## 本地运行

```bash
pip install -r requirements.txt
python -m uvicorn main:app --host 0.0.0.0 --port 8888
```

API: http://localhost:8888/docs

## 模块

- 八字 | 六爻 | 紫微 | 奇门 | 风水 | 择日 | 知识库