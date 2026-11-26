# Arolu

Arolu 对冲套利系统的签名安装包发布仓库。安装包、签名和版本清单都在 [Releases → packages](https://github.com/Delukang/arolu-go-release/releases/tag/packages)。

## 安装要求

- 干净的 Ubuntu 24.04 x86_64 服务器
- 开放 TCP 80、443 端口
- 以管理员（root）身份在私有 SSH 终端中运行

## 安装命令

```bash
curl -fsSL https://github.com/Delukang/arolu-go-release/releases/download/packages/install.sh | sudo sh
```

安装脚本会先核对安装包的签名和摘要，再准备数据库、申请 HTTPS 证书并启动服务。首次登录资料和恢复码只在终端中显示；之后也可以运行 `sudo /usr/libexec/arolu-maintenance show-login` 查看。

## 升级

安装完成后，后续升级都在网页“设置 → 系统与服务 → 版本与更新”中完成，不需要再次运行安装命令。
