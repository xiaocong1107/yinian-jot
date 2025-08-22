# 一念 (Priospace)

<div align="center">
  <img src="https://app.bornforai.cn/static/logo/logo.jpeg" alt="一念 Logo" width="120" height="120">
  
  **万事始于一念之间，快速记下每一个闪现的念头，将其演化成完整的现实计划**
  
  [![Next.js](https://img.shields.io/badge/Next.js-15.4.2-black?style=flat-square&logo=next.js)](https://nextjs.org/)
  [![React](https://img.shields.io/badge/React-19.1.0-blue?style=flat-square&logo=react)](https://reactjs.org/)
  [![TailwindCSS](https://img.shields.io/badge/TailwindCSS-3.4.17-38B2AC?style=flat-square&logo=tailwind-css)](https://tailwindcss.com/)
  [![Tauri](https://img.shields.io/badge/Tauri-2.7.1-FFC131?style=flat-square&logo=tauri)](https://tauri.app/)
  [![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)](./LICENSE)
</div>

## 📖 项目简介

一念是一款专注于将灵感转化为行动的个人效率工具。通过AI技术，帮助用户快速捕捉灵感、分解任务、规划路径、跟踪执行并提供智能提醒。项目由一位全栈独立开发者完整开发，集成了现代化的前端技术栈和智能化的用户体验设计。

## ✨ 核心功能

### 🎯 1. 一念捕捉
- 快速记录闪现的灵感和想法
- 支持文本、语音等多种输入形式
- 实时保存，不让任何有价值的念头溜走
- 智能分类和标签管理

### 🤖 2. AI分解
- 利用先进的AI技术自动分解复杂任务
- 将抽象想法转化为具体可执行的小步骤
- 智能优先级排序和时间估算
- 个性化的任务建议和优化

### 🗺️ 3. 路径规划
- 智能规划任务执行路径和时间安排
- 可视化的时间轴和甘特图展示
- 自动识别任务依赖关系
- 提供最优的行动方案和执行策略

### 📊 4. 执行跟踪
- 全程跟踪任务执行进度
- 实时统计和数据分析
- 可视化的完成情况展示
- 周报和月报自动生成
- 番茄钟计时器集成

### 🔔 5. 智能提醒
- 基于任务优先级和时间安排的个性化提醒
- 多种提醒方式：桌面通知、邮件、短信
- 智能学习用户习惯，优化提醒时机
- 与"念念"AI助手的对话式提醒交互

## 🛠️ 技术架构

### 前端技术栈
- **框架**: Next.js 15.4.2 (App Router)
- **UI库**: React 19.1.0
- **样式**: TailwindCSS 3.4.17 + CSS Variables
- **组件库**: Radix UI + 自定义组件系统
- **动画**: Framer Motion 12.23.6
- **图标**: Lucide React 0.525.0
- **主题**: next-themes (支持深色模式)
- **国际化**: next-intl 4.3.4

### 桌面应用
- **跨平台框架**: Tauri 2.7.1
- **Rust后端**: 高性能的原生桌面应用
- **窗口管理**: 自定义窗口大小和行为
- **系统集成**: 原生通知和系统托盘

### 开发工具
- **构建工具**: Next.js + PostCSS
- **代码高亮**: highlight.js 11.11.1
- **Markdown**: react-markdown 10.1.0
- **日期处理**: date-fns 4.1.0
- **用户引导**: driver.js 1.3.6
- **通知系统**: sonner 2.0.6

### 后端服务
- **API架构**: RESTful API
- **数据管理**: 智能缓存 + 后端API
- **AI集成**: 外部AI服务集成
- **用户认证**: JWT Token认证
- **数据同步**: 多设备数据同步


## 🌟 项目特色

### 🎯 用户体验
- **直观的界面设计**: 简洁现代的UI，符合用户直觉
- **流畅的动画效果**: Framer Motion驱动的丝滑交互
- **响应式设计**: 完美适配桌面和移动设备
- **深色模式支持**: 护眼的深色主题
- **新手引导系统**: driver.js驱动的交互式教程

### 🤖 AI智能化
- **智能任务分解**: AI自动将复杂目标拆分为可执行步骤
- **个性化建议**: 基于用户习惯的智能推荐
- **自然语言交互**: 与"念念"AI助手的对话式交互
- **智能提醒优化**: 机器学习优化的提醒时机

### 🔧 技术亮点
- **现代化技术栈**: 采用最新的React 19和Next.js 15
- **跨平台支持**: Web + 桌面应用双端覆盖
- **高性能优化**: 智能缓存和数据管理
- **类型安全**: TypeScript部分组件确保代码质量
- **模块化架构**: 组件化设计，易于维护和扩展

### 📊 数据可视化
- **进度追踪**: 实时的任务完成进度展示
- **统计报表**: 自动生成的周报和月报
- **习惯分析**: 可视化的习惯养成数据
- **时间管理**: 番茄钟和专注时间统计

## 🔒 隐私与安全

- **本地优先**: 敏感数据优先本地存储
- **加密传输**: HTTPS加密的数据传输
- **Token认证**: JWT安全认证机制
- **数据备份**: 支持数据导出和导入
- **隐私保护**: 严格的数据使用政策

## 🌍 部署方案

### Web应用部署
- **静态部署**: 支持Vercel、Netlify等平台
- **服务器部署**: Node.js服务器部署
- **Docker容器**: 容器化部署方案

### 桌面应用分发
- **Windows**: .msi安装包
- **macOS**: .dmg安装包
- **Linux**: .deb/.rpm包

## 🤝 贡献指南

欢迎提交Issue和Pull Request来改进这个项目！


### 代码规范
- 遵循ESLint配置
- 使用Prettier格式化代码
- 编写清晰的提交信息
- 添加必要的测试用例

## 📄 许可证

本项目采用 [MIT](LICENSE) 许可证。

## 👨‍💻 关于作者

这个项目由一位全栈独立开发者完整开发，涵盖了从前端UI设计、后端API开发、AI集成、桌面应用开发到部署运维的完整技术栈。项目体现了现代化Web开发的最佳实践和创新思维。

---

<div align="center">
  <p>如果这个项目对你有帮助，请给它一个 ⭐️</p>
  <p>让我们一起将每一个念头转化为现实！</p>
</div>