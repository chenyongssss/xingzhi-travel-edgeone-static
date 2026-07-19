# 行知旅行 EdgeOne 静态版

这是面向 EdgeOne Pages 的纯静态发布版本，根目录直接包含 `index.html`，不依赖 Next.js 构建、不需要服务端接口。

## 推荐部署

在 EdgeOne Pages 控制台导入仓库：

```text
仓库：chenyongssss/xingzhi-travel-edgeone-static
框架预设：Other
根目录：./
输出目录：./
安装命令：留空；如必填，使用 echo skip
构建命令：留空；如必填，使用 echo skip
```

## 使用 Token 自动部署

在 GitHub 仓库添加 Secret：

```text
EDGEONE_API_TOKEN=你的 EdgeOne API Token
```

然后运行：

```text
Actions → Deploy EdgeOne Static → Run workflow
```

## AI 深度定制

静态版先用于公开访问和体验验证。需要 AI 深度定制时，请部署支持服务端接口的版本，并在 EdgeOne 环境变量中配置：

```text
AI_BASE_URL=https://api.openai.com/v1
AI_API_KEY=你的模型密钥
AI_MODEL=gpt-4.1-mini
```

模型密钥只放在平台环境变量或 GitHub Secrets 中，不要写入代码或提交到仓库。
