# 麻薯的知识星球 - 开发规范

## 🎯 项目概述
- **项目名称**: 麻薯的知识星球
- **域名**: mashubushimao.tech
- **GitHub**: https://github.com/wangqiannudt/mashubushimao
- **代码管理员**: 麻薯 🐱

## 📋 代码管理员职责

### 1. 代码管理
- 版本控制（Git）
- 代码审查
- 分支管理
- 提交规范

### 2. 测试
- 功能测试
- API 测试
- 兼容性测试
- 回归测试

### 3. 部署
- 本地测试环境
- 生产环境部署
- 服务监控
- 故障恢复

### 4. 上线流程
- 代码审查
- 测试通过
- 版本打标
- 推送生产
- 监控验证

## 🔄 开发工作流

```
需求 → 开发 → 测试 → 提交 → 推送 → 部署 → 监控
```

### 提交规范
```
feat:     新功能
fix:      Bug修复
docs:     文档更新
style:    样式调整
refactor: 代码重构
test:     测试相关
chore:    构建/工具
```

### 分支策略
```
master    - 生产分支（稳定）
develop   - 开发分支
feature/* - 功能分支
hotfix/*  - 紧急修复
```

## 📦 环境配置

### 生产环境
- **服务器**: 43.159.55.246
- **Web目录**: /var/www/html/
- **API目录**: /var/www/api/
- **数据库**: /var/www/data/mashu.db

### 服务状态
- nginx: 80端口
- API: 3001端口（内网）
- 反向代理: /api/ → 127.0.0.1:3001

## ✅ 测试清单

### 功能测试
- [ ] 首页访问
- [ ] 用户注册
- [ ] 用户登录
- [ ] 登录状态保持
- [ ] 管理后台访问
- [ ] 知识库页面

### API测试
- [ ] /api/health
- [ ] /api/auth/register
- [ ] /api/auth/login
- [ ] /api/auth/verify
- [ ] /api/admin/stats
- [ ] /api/admin/users

### 兼容性测试
- [ ] Chrome
- [ ] Firefox
- [ ] Safari
- [ ] 移动端

## 🚀 部署命令

```bash
# 拉取最新代码
cd /var/www/html && git pull

# 重启API服务
pkill -f "node server.js"
cd /var/www/api && nohup node server.js > /tmp/api.log 2>&1 &

# 重载nginx
nginx -s reload

# 检查服务状态
curl http://localhost/api/health
```

## 📊 版本历史

| 版本 | 日期 | 描述 |
|------|------|------|
| v1.1.0 | 2026-03-06 | 重构首页布局，模块化设计 |
| v1.0.0 | 2026-03-06 | 初始化项目 |

---

*代码管理员: 麻薯 🐱*
*最后更新: 2026-03-06*
