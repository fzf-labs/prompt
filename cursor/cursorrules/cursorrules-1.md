# 项目背景
这是一个基于 Nextjs 的支持多语言的博客 Web 应用程序，使用 Nextjs 框架编写。

# 编码标准
- 使用函数式组件和 Hooks，避免类组件
- 变量声明优先使用 const，而不是 let
- 变量和函数名使用 camelCase 规范，组件名使用 PascalCase

# 首选的库和框架

- 使用 Next.js 进行导航
- 使用 next-intl 做国际化
- 使用 tailwind 进行 CSS-in-JS 样式设计

# 文件结构
- components: 可复用的 UI 组件
- app/[locale]: 支持多语言的 nextjs 页面
- data/blog: 多语言的博客文件 
- app/api: API 服务函数

# 性能优化指南
- 对纯函数组件使用 React.memo
- 路由组件实现懒加载
- 优化 useEffect 依赖，防止不必要的重新渲染

# 测试要求
- 使用 Jest 和 React Testing Library 编写单元测试
- 测试覆盖率应至少达到 80%
- 对 UI 组件使用快照测试 (Snapshot Testing)

# 文档规范
- 使用 JSDoc 格式编写函数和组件的注释
- 组件必须包含 PropTypes 验证
- 每个主要目录必须包含 README.md 文件
- 同时提供英语和中文版本的 README.md 文件

# 错误处理
- 使用 try/catch 块处理异步操作
- 实现全局错误边界组件