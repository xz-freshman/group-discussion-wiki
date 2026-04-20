# 小组讨论知识库

> 把零散讨论整理成可检索、可复习、可持续扩展的知识站点。

---

## 👋 第一次来？先走这条路线

!!! info "推荐阅读顺序"
    **1. 先看摘要**：快速知道这次讨论讲了什么  
    **2. 再看概念页**：按主题系统学习  
    **3. 最后看 Q&A**：用问题检验自己是否真的理解

<div class="grid cards" markdown>

-   :material-file-document-outline: **先看摘要**

    快速把握本次讨论的主题结构、主讲内容和整体脉络。

    [进入摘要](summaries/index.md){ .md-button .md-button--primary }

-   :material-book-open-variant: **系统学概念**

    按主题整理的知识页，适合顺着逻辑往下读。

    [进入概念整理](concepts/index.md){ .md-button .md-button--primary }

-   :material-help-circle-outline: **用 Q&A 自测**

    从讨论里提炼出的高价值问题，适合查漏补缺。

    [进入 Q&A](qa/index.md){ .md-button .md-button--primary }

</div>

---

## 🗺 导航地图

| 我现在想做什么 | 应该去哪里 |
|---|---|
| 快速知道这次讨论讲了什么 | [摘要](summaries/index.md) |
| 系统学习计算机网络部分 | [概念 → 计算机网络基础](concepts/计算机网络基础.md) |
| 系统学习宇宙学部分 | [概念 → 宇宙学相关页面](concepts/index.md) |
| 直接找某个问题的答案 | [Q&A](qa/index.md) |

---

## 📚 这站里有什么

=== "💻 计算机网络"

    重点讲互联网为什么是“层层叠加”的：

    - MAC 地址和 IP 地址分别解决什么问题
    - Hub / Switch / Router 的角色区别
    - 子网、网关、DNS、HTTP/HTTPS 的逻辑关系
    - 无线网络为什么更危险

    [计算机网络基础](concepts/计算机网络基础.md){ .md-button }

=== "🌌 宇宙学"

    重点讲宇宙膨胀的物理图景：

    - 为什么可观测宇宙半径不是简单的 \(c/H_0\)
    - 尺度因子、暗能量、CMB、暴涨分别是什么
    - FRW 度规与宇宙学方程在描述什么
    - Hubble Tension 为什么是前沿难题

    - [可观测宇宙的膨胀历史](concepts/可观测宇宙的膨胀历史.md)
    - [FRW 度规与宇宙学方程](concepts/FRW%20度规与宇宙学方程.md)
    - [哈勃常数与 Hubble Tension](concepts/哈勃常数与%20Hubble%20Tension.md)

=== "❓ Q&A"

    适合快速回顾、考前翻阅、或者看到一个问题想立刻找答案。

    [Q&A 摘录](qa/Q&A%20摘录.md){ .md-button }

---

## 🆕 最近更新

- 重构首页与分组页，减少“纯列表式”导航造成的混乱
- 清理站内链接，统一成 MkDocs 可跳转路径
- 优化 Q&A 页面结构，增强可读性与检索性

---

## 🔧 维护者说明

??? warning "仅维护者需要看"
    本站基于 **MkDocs + Material for MkDocs**，部署在 **GitHub Pages**。

    常规更新流程：

    1. 修改 `docs/` 下对应页面
    2. 本地运行 `mkdocs build --strict`
    3. `git add . && git commit -m "描述" && git push`

    详细见：[UPDATE.md](UPDATE.md)

---

*由余川整理维护 · 基于小组讨论录音转文字生成*
