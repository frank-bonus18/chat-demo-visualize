# chat-demo-visualize

基于 DeepSeek 官方 [chat-demo v0.1.1](https://github.com/deepseek-ai/chat-demo)（MIT）改造的自包含网页版，在官方对话能力之上，把回复中的完整 HTML 文档围栏直接渲染成可交互卡片。

## 功能

- 回复里的完整 HTML 文档围栏渲染为可交互卡片（iframe srcdoc），卡片支持查看源码、放大全屏
- 自定义智能体：人设前置注入到请求 system 字段，支持快速模板
- 设置并入官方设置弹窗的第三个「可视化」标签页；配置与备份在官方「数据管理」页管理
- 输入/发送体验：停止生成（软停止）、草稿自动保存、输入框自适应高度、输入历史上下翻、失败自动重试、流式节流
- 所有 JS / CSS / 字体资源内联在单个 `index.html` 中，无本地相对路径依赖

## 使用

- 直接打开页面即可；API Key 在页面内填写，仅保存在当前浏览器的 `localStorage`，不会进入仓库或打包产物
- 运行时接口为 `https://api.deepseek.com`，需要联网

## 协议

保留官方包的 MIT LICENSE 与版权声明，随本仓库一并存放。
