# 纽北赛道地图 Vue3 版本

这是原始纽博格林赛道地图项目的 Vue3 转换版本，移除了 PHP 依赖，使用纯前端技术栈。

## 技术栈

- Vue 3 (Composition API)
- Vite (构建工具)
- 原始 CSS 样式保持不变

## 安装和运行

1. 安装依赖：

```bash
npm install
```

2. 开发模式运行：

```bash
npm run dev
```

3. 构建生产版本：

```bash
npm run build
```

4. 预览构建结果：

```bash
npm run preview
```

## 主要变更

### 从 PHP 到 Vue3 的转换：

1. **服务端逻辑移除**：

   - 移除了 PHP 的语言检测逻辑，改为客户端 JavaScript 实现
   - 移除了 PHP 的资源路径配置，使用 Vite 的静态资源处理

2. **Vue2 到 Vue3 升级**：

   - 使用 Composition API 替代 Options API
   - 更新了响应式数据的声明方式
   - 优化了事件处理和生命周期钩子

3. **模块化改进**：

   - 将弯道数据提取到单独的 JavaScript 模块
   - 创建可复用的组件结构

4. **现代构建工具**：
   - 使用 Vite 替代传统的打包方式
   - 支持热模块替换(HMR)
   - 更快的开发服务器启动速度

## 项目结构

```
vue3-version/
├── public/
│   └── assets/          # 静态资源
├── src/
│   ├── assets/          # CSS等资源
│   ├── data/            # 弯道数据
│   ├── App.vue          # 主组件
│   └── main.js          # 入口文件
├── index.html           # HTML模板
├── package.json         # 项目配置
└── vite.config.js       # Vite配置
```

## 特性保持

- 保持了原项目的所有视觉效果和交互功能
- 支持中英文切换
- 保持了响应式设计
- 保留了深色模式支持
- 所有弯道信息和图片展示功能完整保留

## 与原版对比

### 优势：

- 无需 PHP 服务器，可部署到任何静态托管服务
- 更快的开发体验
- 现代化的构建流程
- 更好的代码组织结构

### 兼容性：

- 保持了原有的用户体验
- CSS 样式基本保持不变
- 所有功能特性得到保留
