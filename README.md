# SenseNova Image Studio

这是一个单文件静态网页,用于接入商汤 SenseNova 公测期 OpenAI 兼容文生图接口。

## 使用方式

1. 打开 `index.html`。
2. 填写你在 SenseNova 控制台创建的 API Key。
3. 保持默认 Base URL: `https://token.sensenova.cn/v1`。
4. 输入提示词,选择模型、尺寸和张数。
5. 点击“开始生成”。

## GitHub Pages 部署

1. 在 GitHub 新建一个公开仓库,例如 `sensenova-image-studio`。
2. 上传 `index.html` 和 `README.md` 到仓库根目录。
3. 进入仓库的 `Settings` → `Pages`。
4. `Source` 选择 `Deploy from a branch`。
5. `Branch` 选择 `main` / `/root`,保存。
6. 等待 GitHub Pages 生成访问地址。

## 注意事项

- API Key 只保存在浏览器本地 `localStorage`,不会写入代码文件。
- 如果浏览器调用接口时出现 CORS 错误,需要增加一个后端代理或 Cloudflare Worker 转发请求。
- 不要把自己的 API Key 写进 `index.html` 后提交到 GitHub。
