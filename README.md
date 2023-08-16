# Moonchatbot
Moonchatbot是一个关于ChatGPT的程序.

## 部署

**Docker**

本地部署:

```shell
docker build -t chatgpt-ui .
docker run -d -e OPENAI_API_KEY=xxxxxxxx -p 80:3000 chatgpt-ui
```

公共容器部署:

```shell
docker pull jupiterjackson/chatgpt-ui:latest
docker run -d -e OPENAI_API_KEY=xxxxxxxx -p 80:3000 jupiterjackson/chatgpt-ui
```

## 本地运行

**1. 下载仓库**

```bash
git clone https://github.com/jupiterjackson/moonchatbot.git
```

**2. 安装依赖**

```bash
npm i
```

**3. 设置OpenAI API Key**

创建一个名为 .env.local 的文件在根目录，然后填入你的OpenAI API Key:

```bash
OPENAI_API_KEY=YOUR_KEY
```

**4. 运行程序**

```bash
npm run dev
```

## 参考

参考 [链接](https://github.com/mckaywrigley/chatbot-ui/tree/main ).