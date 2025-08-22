# 一念 (Priospace)

<div align="center">
  <img src="./public/logo.png" alt="一念 Logo" width="120" height="120">
  
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

## 🚀 快速开始

### 环境要求
- Node.js >= 18.0.0
- npm >= 8.0.0 或 yarn >= 1.22.0
- Rust >= 1.70.0 (桌面应用开发)

### 安装依赖
```bash
# 克隆项目
git clone https://github.com/your-username/一念.git
cd 一念

# 安装依赖
npm install
# 或
yarn install
```

### 开发模式
```bash
# 启动Web开发服务器
npm run dev
# 或
yarn dev

# 启动Tauri桌面应用开发
npm run tauri dev
```

### 构建生产版本
```bash
# 构建Web应用
npm run build
# 或
yarn build

# 构建桌面应用
npm run tauri build
```

### 启动生产服务器
```bash
npm start
# 或
yarn start
```

## 📁 项目结构

```
一念/
├── app/                     # Next.js App Router
│   ├── api/                 # API路由
│   │   ├── chat/           # AI对话接口
│   │   └── reminder/       # 提醒相关接口
│   ├── globals.css         # 全局样式
│   ├── layout.js           # 根布局
│   └── page.js             # 主页面
├── components/              # React组件
│   ├── chat/               # 聊天相关组件
│   ├── summaries/          # 总结报告组件
│   ├── ui/                 # 基础UI组件
│   ├── yinian-modal.js     # 一念捕捉模态框
│   ├── task-list.js        # 任务列表组件
│   ├── habit-tracker.js    # 习惯跟踪器
│   ├── reminder-panel.js   # 提醒面板
│   └── timer-modal.js      # 番茄钟计时器
├── services/               # 服务层
│   ├── api.js              # API接口封装
│   └── dataManager.js      # 数据管理器
├── src-tauri/              # Tauri桌面应用
│   ├── src/                # Rust源码
│   ├── icons/              # 应用图标
│   └── tauri.conf.json     # Tauri配置
├── public/                 # 静态资源
├── lib/                    # 工具库
├── utils/                  # 工具函数
├── i18n/                   # 国际化配置
└── translations/           # 翻译文件
```

## 🎨 核心组件

### 主要功能组件
- **YinianModal**: 一念捕捉模态框，AI驱动的灵感记录
- **TaskList**: 智能任务列表，支持拖拽排序和实时编辑
- **HabitTracker**: 习惯跟踪器，可视化习惯养成进度
- **ChatInterface**: AI对话界面，与"念念"助手交互
- **ReminderPanel**: 智能提醒面板，个性化通知管理
- **TimerModal**: 番茄钟计时器，专注时间管理
- **SummaryNavigation**: 数据总结导航，周报月报生成

### UI组件系统
- **Button**: 多变体按钮组件
- **Card**: 卡片容器组件
- **Input/Textarea**: 表单输入组件
- **Select**: 下拉选择组件
- **Modal**: 模态框组件系统

## 🔌 API接口

### 任务管理
- `GET /api/tasks` - 获取任务列表
- `POST /api/tasks` - 创建新任务
- `PUT /api/tasks/:id` - 更新任务
- `DELETE /api/tasks/:id` - 删除任务

### 习惯跟踪
- `GET /api/habits` - 获取习惯列表
- `POST /api/habits` - 创建新习惯
- `PUT /api/habits/:id/status` - 更新习惯状态

### AI服务
- `POST /api/chat` - AI对话接口
- `POST /api/generate-tasks` - AI任务生成

### 用户系统
- `POST /api/auth/login` - 用户登录
- `GET /api/user/info` - 获取用户信息
- `GET /api/user/settings` - 获取用户设置

### 提醒系统
- `GET /api/reminder/messages` - 获取提醒消息
- `POST /api/reminder/settings` - 保存提醒设置

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

### 开发流程
1. Fork本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启Pull Request

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