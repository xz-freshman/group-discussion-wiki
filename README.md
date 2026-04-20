# 小组讨论知识库

小组讨论录音整理后的知识库网站，基于 MkDocs + Material 主题生成。

## 内容

- 计算机网络基础（MAC、IP、交换机、路由器、子网、DNS 等）
- 可观测宇宙的膨胀历史（Scale Factor、暗能量、CMB、Hubble Tension）
- FRW 度规与宇宙学方程
- 哈勃常数与 Hubble Tension

## 本地开发

```bash
mkdocs serve
```

访问 `http://localhost:8000`（或你本机当前启动服务时显示的端口）

## 发布

推送到 GitHub 仓库 `xz-freshman/group-discussion-wiki` 后，GitHub Actions 会自动构建并发布到 GitHub Pages。

文件更新后重新 push 即可自动更新网站。