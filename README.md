# 麻薯的知识星球 - 项目文档

## 📁 项目结构

```
mashubushimao.tech/
├── index.html              # 首页
├── login.html              # 登录/注册
├── admin/                  # 管理后台
├── zhongcai/               # 智采观察
├── ai-news/                # AI 前沿观察
├── exam/                   # 智采学堂
├── docs/                   # 文档目录
├── assets/                 # 静态资源
│   ├── css/
│   │   ├── main.css        # 主样式
│   │   ├── components.css  # 组件样式
│   │   └── responsive.css  # 响应式
│   ├── js/
│   │   ├── main.js         # 主脚本
│   │   ├── auth.js         # 认证模块
│   │   └── utils.js        # 工具函数
│   └── images/             # 图片资源
└── api/                    # API 服务 (独立仓库)
```

## 🎨 设计系统

### 颜色变量
```css
--primary: #667eea;      /* 主色调 */
--primary-dark: #764ba2; /* 主色深 */
--bg-dark: #1a1a2e;      /* 深色背景 */
--bg-card: #16213e;      /* 卡片背景 */
--text-primary: #ffffff;  /* 主文字 */
--text-secondary: #888;   /* 次要文字 */
```

### 组件规范
- **按钮圆角**: 20-25px
- **卡片圆角**: 15-20px
- **导航高度**: 60px
- **间距基准**: 15px

## 📦 版本管理

### Git 工作流
- `master` - 生产分支
- `develop` - 开发分支
- `feature/*` - 功能分支

### 提交规范
- `feat:` 新功能
- `fix:` 修复
- `docs:` 文档
- `style:` 样式
- `refactor:` 重构

### 版本号规则
- 主版本号: 重大架构变更
- 次版本号: 新功能
- 修订号: Bug修复

## 🧪 测试清单

### 功能测试
- [ ] 用户注册
- [ ] 用户登录
- [ ] 登录状态保持
- [ ] 管理员权限
- [ ] 页面访问

### 兼容性测试
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] 移动端

### API 测试
- [ ] /api/auth/login
- [ ] /api/auth/register
- [ ] /api/auth/verify
- [ ] /api/admin/stats
- [ ] /api/admin/users

## 🚀 部署流程

1. 本地测试通过
2. Git commit
3. 推送到服务器
4. 重启服务

---

*版本: v1.0.0*
*更新时间: 2026-03-06*
