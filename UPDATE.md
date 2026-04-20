# 更新操作指南

本文档说明如何向知识库添加新内容并发布更新。

---

## 目录结构

```
mkdocs/
├── docs/                    ← 所有页面内容
│   ├── index.md             ← 首页
│   ├── concepts/            ← 概念页（按主题）
│   ├── summaries/           ← 讨论摘要
│   └── qa/                  ← 问答摘录
├── mkdocs.yml               ← 站点配置（导航结构）
├── .github/workflows/deploy.yml  ← 自动部署配置
└── UPDATE.md               ← 本文档
```

---

## 更新步骤

### Step 1：编辑内容

在 `docs/` 下对应目录中添加或修改 `.md` 文件：

| 场景 | 操作位置 |
|------|---------|
| 新增概念页 | `docs/concepts/你的概念标题.md` |
| 新增摘要页 | `docs/summaries/第X周讨论.md` |
| 新增 Q&A | `docs/qa/Q&A_摘录.md`（追加内容）|
| 修改导航结构 | 编辑 `mkdocs.yml` 的 `nav:` 部分 |

### Step 2：本地预览（推荐）

```bash
cd /root/.openclaw/workspace/小组讨论/mkdocs
mkdocs serve
```

打开 `http://localhost:8000` 检查页面效果。

### Step 3：提交到 GitHub

```bash
git add .
git commit -m "描述本次更新的内容"
git push
```

### Step 4：等待自动发布

- GitHub Actions 会自动检测到 push，开始构建
- 约 1–2 分钟后，网站自动更新
- 访问：https://xz-freshman.github.io/group-discussion-wiki/

---

## 修改 mkdocs.yml 导航

如果新增了页面，需要在 `mkdocs.yml` 的 `nav:` 部分加入对应条目，例如：

```yaml
nav:
  - 首页: index.md
  - 摘要:
    - summaries/第七周讨论.md
  - 概念:
    - concepts/计算机网络基础.md
    - concepts/新概念页.md    # ← 新增的页面
```

导航会自动根据文件名生成侧边栏和菜单。

---

## 本地构建（不依赖 GitHub）

```bash
mkdocs build --strict
```

构建产物会生成在 `site/` 目录（已在 `.gitignore` 中，不会被提交）。

---

## 常见问题

**Q：push 后网站没更新？**
检查 GitHub → Actions 标签页，看构建是否成功。失败的话点击工作流查看错误信息。

**Q：本地 mkdocs serve 显示正常，但 GitHub 上样式不对？**
可能是 Material 主题在 GitHub Pages 的加载顺序问题，尝试 `mkdocs build --strict` 重新构建确认无报错。

**Q：想添加新的内容分类？**
在 `docs/` 下新建目录（如 `docs/topics/`），然后在 `mkdocs.yml` 的 `nav:` 中加入对应条目即可。
