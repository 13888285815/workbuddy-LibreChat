# 🎯 LibreChat 一键部署到 Render（免费）

## ✅ 已完成
- [x] GitHub 仓库：https://github.com/13888285815/workbuddy-LibreChat
- [x] render.yaml 配置文件（已优化）
- [x] MongoDB Atlas 连接串已配置

## 📋 你需要做的（5分钟）

### 第1步：注册/登录 Render
1. 打开：**https://dashboard.render.com**
2. 点击 **"Get Started"**
3. 选择 **"GitHub"** 登录（最简单）

### 第2步：授权 GitHub
1. 弹出 GitHub 授权窗口
2. 点击 **"Authorize Render"**
3. 选择要授权的仓库：☑️ **workbuddy-LibreChat**

### 第3步：创建 Blueprint 部署
1. 在 Render Dashboard 点击 **"New +"**
2. 选择 **"Blueprint"**
3. 点击 **"Import from GitHub"**
4. 选择仓库：**13888285815/workbuddy-LibreChat**
5. Render 会自动检测 `render.yaml` 文件
6. 点击 **"Apply"** 开始部署

### 第4步：等待部署
⏱️ 等待 **3-5 分钟**，看到绿色 ✅ 即部署成功

### 第5步：获取公开地址
部署成功后，Render 会生成公开 URL：
```
https://librechat-xxxx.onrender.com
```
**点击这个链接即可访问！**

---

## 🎉 恭喜！
任何人都可以通过这个链接访问 LibreChat，无需安装任何东西！

---

## ⚠️ 注意事项

### 休眠问题
- Render 免费版 15 分钟无访问会休眠
- 下次访问时需要等待 30-60 秒唤醒
- 如果需要永不休眠，需要升级付费版

### 数据安全
- 数据存储在你的 MongoDB Atlas 数据库中
- 定期备份 MongoDB 以防丢失

---

## 🔧 如果遇到问题

### 问题1：Build 失败
检查 `.env` 配置是否正确，确保 `MONGO_URI` 格式正确

### 问题2：页面空白
检查 `DOMAIN_CLIENT` 和 `DOMAIN_SERVER` 是否设置正确

### 问题3：无法登录/注册
确保 `JWT_SECRET` 和其他密钥已生成（render.yaml 中配置了自动生成）

---

## 📞 需要帮助？
随时回来问我！
