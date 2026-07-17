# 行知旅行 EdgeOne 静态版

这是行知旅行给腾讯云 EdgeOne Pages 准备的纯静态发布仓库。

它不依赖 Next、Vinext、Cloudflare Workers，也没有服务端接口；适合先在国内访问环境里试水。

## EdgeOne Pages 配置

- 框架预设：Other
- 根目录：./
- 安装命令：npm install
- 构建命令：npm run build
- 输出目录：out
- Node.js：22.11.0

## 本地构建

```bash
npm install
npm run build
```