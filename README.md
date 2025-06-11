# 纽北赛道地图 Vue 3.2 版本

这是一个使用 Vue 3.2 重新构建的纽博格林北环赛道互动地图项目。

## 原项目

原项目使用 PHP + Vue 2.6.11 构建，现已完全迁移到 Vue 3.2 + TypeScript + Composition API。

## 功能特点

- 🏁 **互动赛道地图**: 通过滚动或点击查看赛道上各个弯道
- 🌍 **双语支持**: 中文/英文切换
- 📱 **响应式设计**: 适配桌面和移动设备
- ⚡ **现代技术栈**: Vue 3.2 + TypeScript + Composition API
- 🎨 **精美界面**: 保持原有的视觉设计和交互体验

## 技术栈

- **框架**: Vue 3.2
- **语言**: TypeScript
- **构建工具**: Vite
- **状态管理**: Pinia
- **路由**: Vue Router 4
- **样式**: CSS + CSS Variables

## 项目结构

```
src/
├── App.vue                 # 主应用组件
├── main.ts                 # 应用入口
├── assets/                 # 静态资源
│   └── main.css           # 主样式文件
├── composables/           # 组合式函数
│   └── useTrackData.ts    # 赛道数据管理
├── components/            # 组件
├── router/                # 路由配置
└── stores/                # 状态管理
```

## 安装和运行

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run dev

# 构建生产版本
npm run build

# 预览生产版本
npm run preview
```

## 使用说明

1. **滚动交互**: 向下滚动页面来"驾驶"通过赛道
2. **点击弯道**: 点击弯道名称快速跳转到该位置
3. **语言切换**: 点击右上角的语言按钮切换中英文
4. **显示所有弯道**: 点击"显示所有"按钮查看所有弯道名称

## 特色

- 使用 Composition API 重构了原有的 Vue 2 Options API 代码
- 完全的 TypeScript 类型支持
- 更好的代码组织和复用性
- 保持了原有项目的所有交互功能和视觉效果

## 致谢

感谢原作者 JJ Ying 创造了这个优秀的交互式赛道地图项目。

## 许可证

本项目遵循原项目的许可证。
