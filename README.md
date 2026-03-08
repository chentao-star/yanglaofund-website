# 个人养老金产品名录网站

🌐 **在线访问**: https://yanglaofund.com

## 自动部署

本仓库使用 GitHub Actions 自动部署到阿里云服务器。

### 部署触发条件
- 推送代码到 `main` 分支时自动触发
- 修改 `index.html` 后会自动更新网站

### 所需 Secrets

需要在 GitHub 仓库 Settings → Secrets and variables → Actions 中添加：

| Secret 名称 | 值 |
|:---|:---|
| `SSH_PRIVATE_KEY` | （私钥内容，见下方） |
| `SERVER_IP` | `39.105.59.18` |
| `SERVER_USER` | `root` |

### SSH 私钥内容

复制以下内容添加到 SSH_PRIVATE_KEY：

-----BEGIN OPENSSH PRIVATE KEY-----
b3BlbnNzaC1rZXktdjEAAAAABG5vbmUAAAAEbm9uZQAAAAAAAAABAAAAMwAAAAtzc2gtZW
QyNTUxOQAAACCAVCQOI7v6z09b9PUsCOgStBFMzMElwAxxIO2oD1jT9AAAAKAIVvzECFb8
xAAAAAtzc2gtZWQyNTUxOQAAACCAVCQOI7v6z09b9PUsCOgStBFMzMElwAxxIO2oD1jT9A
AAAEBcXtdnQAOttgHxXoPeZeSXpFAZmosS4PA9f1KzWQO/24BUJA4ju/rPT1v09SwI6BK0
EUzMwSXADHEg7agPWNP0AAAAFmRlcGxveUB5YW5nbGFvZnVuZC5jb20BAgMEBQYH
-----END OPENSSH PRIVATE KEY-----

## 如何更新网站

1. 修改 `index.html` 文件
2. 提交并推送到 GitHub
3. GitHub Actions 会自动部署到服务器
4. 访问 https://yanglaofund.com 查看更新

## 服务器信息

- **IP**: 39.105.59.18
- **域名**: yanglaofund.com / www.yanglaofund.com
- **SSL**: Let's Encrypt 自动续期

---
Created by OpenClaw AI
