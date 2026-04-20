# 小组讨论知识库

> 小组讨论录音整理 — 计算机网络 + 宇宙学基础

🖥 **在线访问**：https://xz-freshman.github.io/group-discussion-wiki/

---

## 内容导航

### 📖 摘要
- [第七周讨论完整摘要](summaries/第七周讨论.md)

### 🧠 概念整理
- [计算机网络基础](concepts/计算机网络基础.md) — MAC 地址、集线器、交换机、路由器、IP、DNS、HTTP/HTTPS、无线安全
- [可观测宇宙的膨胀历史](concepts/可观测宇宙的膨胀历史.md) — Scale Factor、暗能量、红移、CMB、Hubble Tension
- [FRW 度规与宇宙学方程](concepts/FRW%20度规与宇宙学方程.md) — 度规形式、弗里德曼方程、曲率参数
- [哈勃常数与 Hubble Tension](concepts/哈勃常数与%20Hubble%20Tension.md) — H₀ 测量的两套方法及宇宙学最大难题

### ❓ Q&A
- [高价值提问与回答摘录](qa/Q&A%20摘录.md)

---

## 技术栈

- 框架：[MkDocs](https://www.mkdocs.org/) + [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- 托管：[GitHub Pages](https://pages.github.com/)（自动构建发布）
- 源码管理：[GitHub Actions](https://github.com/features/actions)

## 本地开发

```bash
# 安装依赖
pip install mkdocs-material

# 启动本地预览
mkdocs serve

# 构建静态网站
mkdocs build --strict
```

## 部署流程

每次 `git push` 到 `main` 分支后，GitHub Actions 会自动完成构建和发布。

详细操作说明见 [UPDATE.md](UPDATE.md)。

---

*由余川整理维护，基于小组讨论录音转文字生成*
