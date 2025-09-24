# Warp Tools

一款专为 Warp 终端设计的 Windows 账户管理工具，基于 Python + PySide6 开发。

## 📌 项目信息

- **应用名称**：Warp Tools  
- **当前版本**：v1.3.0    
- **开发语言**：Python 3.9+  
- **GUI框架**：PySide6 (Qt for Python)  
- **目标平台**：Windows 10/11  
- **架构模式**：MVC (Model-View-Controller)  

## ✨ 功能特性

### 📊 仪表盘 (Dashboard)
- 显示当前 Warp 账户信息（邮箱、用户ID、令牌状态、过期时间）
- 实时展示订阅套餐类型（Free/Trial Pro/Pro/Premium）
- 显示使用量和额度信息（带进度条）
- 显示机器码和 Warp 客户端版本
- 支持一键保存当前账户到数据库
- 支持刷新账户信息

### 👥 账户管理 (Account Management)
- 完整的账户 CRUD 操作（增删改查）
- 账户列表展示（邮箱、套餐、使用量、到期时间）
- 快速切换 Warp 账户（自动处理进程关闭）
- 批量导入/导出 JSON 格式账户数据
- 批量刷新账户令牌
- 自动刷新过期的 ID Token
- 智能重复检测，避免数据冗余
- 账户搜索和筛选功能

### 🔑 获取令牌 (Token Acquisition)
- 三步式工作流程：生成链接 → 获取令牌 → 保存账号
- 支持从 URL 自动提取 refresh_token
- 自动获取账户订阅信息
- 自动计算令牌过期时间
- 步骤式引导界面，操作简单

### 🎭 匿名注册 (Anonymous Register)
- 无需邮箱即可注册账号
- 系统自动生成虚拟邮箱（格式：anonymous_随机6位@warp.dev）
- 一键快速创建匿名账号
- 实时显示注册过程日志
- 自动获取账号额度信息
- IP限制提醒（每小时限一个账号）

### 💾 配置备份 (Config Backup)
- 一键备份 Warp 配置文件（dev.warp.Warp-User）
- 快速还原历史备份
- 备份列表管理（显示时间、大小）
- 删除指定备份
- 进程状态安全检查

### 🔧 工具箱 (Tools)
- **账户清理**：删除本地用户配置文件
- **重置机器码**：修改注册表 ExperimentId（需管理员权限）
- **应用重置**：完全清除 Warp 数据和注册表（不可逆）
- **进程管理**：自动检测并终止 Warp 进程
- **操作日志**：实时显示执行过程

### 🎨 界面设计
- 无边框窗口设计，自定义标题栏
- 深色/浅色主题自动切换
- 可折叠侧边栏导航（展开/收缩）
- 现代化视觉效果（渐变背景、圆角卡片、阴影效果）
- 响应式布局设计

## 📋 常见问题

### Q: 为什么需要关闭 Warp 才能切换账户？
A: 因为需要修改 Warp 的本地配置文件，Warp 运行时会锁定这些文件。

### Q: 重置机器码有什么作用？
A: 可以解决某些账户限制问题，但可能需要重新激活某些软件。

### Q: 备份文件保存在哪里？
A: 备份文件保存在 `%APPDATA%\WarpTools\backups\` 目录下。

### Q: 如何获取匿名Token？
A: 点击"匿名注册"菜单，生成新的匿名Token即可。

### Q: 支持哪些 Windows 版本？
A: 支持 Windows 10/11 及以上版本。

## 🚀 联系方式

- Telegram: [https://t.me/gacjie](https://t.me/gacjie)
- GitHub: [https://github.com/gacjie](https://github.com/gacjie)
- 关注 Telegram 频道获取最新更新

## 🌟 致谢

- PySide6 团队
- 所有贡献者

---

**如果这个项目对你有帮助，请给个 ⭐ Star 支持一下！**

> 本项目仅供学习和研究使用，请遵守相关法律法规
