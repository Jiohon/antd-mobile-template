# Antd Mobile Template

基于 antd-mobile 的移动端应用模版，包含完整的路由、权限管理和开发工具链配置。

## 特性

- 🚀 基于 React 18 + TypeScript + Vite
- 📱 移动端优先的响应式设计
- 🎨 Antd Mobile UI 组件库
- 🛣️ React Router 路由管理
- 🔐 完整的权限管理系统
- 🗂️ Zustand 状态管理
- 🌐 Alova HTTP 请求封装
- 💅 Less 样式预处理器
- 📏 ESLint + Prettier 代码规范
- 🔧 完善的 TypeScript 配置
- 📦 PWA 支持

## 技术栈

- **框架**: React 18.2.0
- **构建工具**: Vite 5.0.0
- **语言**: TypeScript 5.2.2
- **UI 组件**: antd-mobile 5.36.1
- **路由**: react-router-dom 6.20.1
- **状态管理**: zustand 4.4.7
- **HTTP 客户端**: alova 3.0.9
- **样式**: Less 4.2.0
- **代码规范**: ESLint + Prettier

## 项目结构

```
src/
├── components/          # 公共组件
│   ├── AuthGuard/      # 认证守卫
│   └── Layout/         # 布局组件
├── pages/              # 页面组件
│   ├── Home/           # 首页
│   ├── Login/          # 登录页
│   ├── Profile/        # 个人中心
│   ├── Settings/       # 设置页
│   └── NotFound/       # 404页面
├── router/             # 路由配置
├── stores/             # 状态管理
├── types/              # 类型定义
├── utils/              # 工具函数
├── styles/             # 全局样式
└── main.tsx           # 应用入口
```

## 快速开始

### 安装依赖

```bash
npm install
```

### 启动开发服务器

```bash
npm run dev
```

### 构建生产版本

```bash
npm run build
```

### 预览构建结果

```bash
npm run preview
```

## 开发命令

- `npm run dev` - 启动开发服务器
- `npm run build` - 构建生产版本
- `npm run preview` - 预览构建结果
- `npm run lint` - 运行 ESLint 检查
- `npm run lint:fix` - 自动修复 ESLint 问题
- `npm run format` - 格式化代码
- `npm run type-check` - TypeScript 类型检查

## 功能特性

### 认证系统

- 登录/登出功能
- Token 自动刷新
- 路由权限控制
- 用户信息管理

### 路由管理

- 基于 React Router 的路由配置
- 路由守卫和权限验证
- 懒加载支持

### 状态管理

- 基于 Zustand 的轻量级状态管理
- 持久化存储支持
- TypeScript 类型安全

### UI 组件

- 完整的移动端 UI 组件
- 响应式设计
- 深色模式支持（可扩展）

### 开发工具

- 完善的 TypeScript 配置
- ESLint + Prettier 代码规范
- 路径别名支持
- 热重载开发体验

## 部署

### 传统部署

```bash
npm run build
# 将 dist 目录部署到服务器
```

### Docker 部署

```dockerfile
FROM nginx:alpine
COPY dist /usr/share/nginx/html
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]
```

### Vercel 部署

```bash
npm i -g vercel
vercel --prod
```

## 许可证

MIT License

## 贡献

欢迎提交 Issue 和 Pull Request！

## 更新日志

### v1.0.0 (2024-01-01)

- 初始版本发布
- 完整的移动端模版功能
- 认证和权限管理
- 开发工具链配置
