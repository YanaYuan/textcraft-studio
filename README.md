# TextCraft Studio / 美页秀秀

🚀 **AI驱动的PPT页面生成器** - 科幻风格的智能内容创作平台

## ✨ 功能特色

- 🤖 **AI智能生成**：基于OpenAI GPT-4，将文本内容转换为精美PPT页面
- 🎨 **智能配图模式**：自动生成高质量配图，支持多种视觉风格
- 📝 **纯文字模式**：专注内容，简洁高效的文本展示
- � **双语支持**：完整的中英文界面和内容支持
- 🎭 **科幻风格UI**：独特的科幻风格界面设计，带有动态效果
- ⚡ **智能进度条**：7阶段AI处理状态显示，减缓用户等待焦虑
- 🎯 **Demo案例**：内置电动汽车技术方案和故宫介绍样例
- 📥 支持下载生成的HTML文件
- 🔗 支持在新窗口打开预览

## 技术栈

- **前端**: HTML5, CSS3, JavaScript (ES6+)
- **后端**: Node.js, Express.js
- **AI服务**: Azure OpenAI GPT-4o
- **依赖**: axios, cors, dotenv

## 安装和运行

1. 安装依赖：
```bash
npm install
```

2. 配置环境变量（已在.env文件中配置）：
- Azure OpenAI 端点
- API密钥
- 部署名称
- API版本

3. 启动服务器：
```bash
npm start
```

4. 打开浏览器访问：
```
http://localhost:3000
```

## 使用说明

1. 在左侧文本框中输入任意内容
2. 点击"生成精美网页"按钮
3. 等待AI处理（通常需要几秒钟）
4. 在右侧预览生成的网页
5. 可以下载HTML文件或在新窗口打开

## API接口

### POST /api/generate-webpage
生成网页内容

**请求体**:
```json
{
  "text": "要转换的文本内容"
}
```

**响应**:
```json
{
  "success": true,
  "html": "生成的HTML内容"
}
```

### GET /api/health
检查服务器状态

**响应**:
```json
{
  "status": "OK",
  "timestamp": "2025-06-28T..."
}
```

## 注意事项

- 确保Azure OpenAI服务可用
- 输入文本不要过长，建议在1000字以内
- 生成的HTML内容在iframe中预览，确保安全性
- 支持快捷键Ctrl+Enter快速提交

## 许可证

MIT License
