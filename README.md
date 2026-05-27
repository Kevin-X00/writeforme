# ✍ WriteForMe 手写助手

**你描述，我写。**

自然语言 → 手写文字生成器。PWA 应用，手机/电脑浏览器打开即用。

## 场景

| 你说 | 它写 |
|------|------|
| "发烧了请一天假" | 完整的请假条 |
| "想离职休息一段时间" | 正式辞职信 |
| "情人节卡片写什么" | 一段情书文字 |
| "通知大家明天开会" | 会议通知 |
| "把这段录音整理成笔记" | 结构化笔记 |

## 功能

- 🎯 **场景自动判断** — 识别请假/辞职/情书/通知等场景
- 🎨 **四种语气** — 正式/亲切/古风/简短
- 🖊 **手写体渲染** — 楷体排版，打印即用
- 📱 **PWA 应用** — 手机浏览器打开，可添加到桌面
- 💾 **本地存储** — API Key 和历史记录保存在浏览器
- 🖨 **一键打印** — 打印出纸质版直接手写签名
- 📋 **复制/保存** — 复制到剪贴板或下载

## 使用

### 在线版（推荐）
GitHub Pages 托管，无需安装：
→ [https://kevin-x00.github.io/writeforme](https://kevin-x00.github.io/writeforme)

### 手机使用
1. 浏览器打开链接
2. 点击「添加到主屏幕」（Safari）或「添加到桌面」（Chrome）
3. 像原生App一样使用

### 离线 CLI 版
```bash
npm install -g writeforme-cli
writeforme "请一天假"
```

## 隐私

- API Key 仅存储在浏览器 LocalStorage，不会发送到任何第三方
- 语音识别使用浏览器原生 Web Speech API，语音数据不会上传
- 所有历史记录仅保存在本地

## 技术

- 纯 HTML/CSS/JS 单页应用
- PWA（Service Worker + Manifest）
- Web Speech API（语音输入）
- OpenAI API（文案生成）
- 零后端依赖，GitHub Pages 免费托管

## License

MIT
