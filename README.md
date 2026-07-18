# SC26-17 · 五行日常

DaSE 2026 暑期学校 SC26-17 小组项目：将传统文化元素转化为每日色彩、衣橱与穿搭灵感的网页应用。

## 本地运行

建议使用 Node.js 20：

```bash
npm install
npm run dev
```

访问 `http://localhost:3000`。

## DeepSeek 配置

复制 `.env.example` 为 `.env.local`，再填写 DeepSeek 配置：

```env
DEEPSEEK_API_KEY=XXX_YOUR_DEEPSEEK_API_KEY_HERE
DEEPSEEK_MODEL=deepseek-chat
DEEPSEEK_BASE_URL=https://api.deepseek.com/v1
```

`.env.local` 不会被提交到 Git。首次生成后，应用会按出生资料、八字、衣橱与当天日期缓存结果；相同输入当天不会重复调用模型。
