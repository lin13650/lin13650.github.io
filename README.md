# 林露茜 · 个人主页（GitHub Pages 版）

> 纯静态单页站点：HTML + CSS + 原生 JavaScript，零依赖。
> 本仓库可直接上传到 GitHub 并在 Settings → Pages 发布。

## 文件结构（GitHub Pages 根目录 = 仓库根目录）

```
.
├── index.html                  # 单页主页（首页 / 项目 / 证书 / 未来 四页切换 + 画廊 + PDF 预览）
├── assets/                     # 图片与 PDF（WebP 压缩 + 短文件名，适合上传）
│   ├── fluid-visualizer.jpg    # 1) 流体声纹可视化器封面
│   ├── site-screenshot.webp    # 2) 个人网页 · 首页截图
│   ├── workflow-screenshot.webp# 2) AI 工作流 · 自动化看板
│   ├── ppt-visual-preview.webp # 3) PPT 模板库 · 视觉效果预览
│   ├── ppt-templates.pdf       # 3) PPT 模板合集 · 完整 PDF
│   ├── tank-screenshot.webp    # 4) 坦克大战 · 游戏截图
│   ├── cert-junior.webp        # 阿里巴巴人工智能训练师（初级）
│   └── cert-senior.webp        # 阿里巴巴人工智能训练师（高级）
├── README.md
└── .gitignore
```

## 本地运行

直接双击 `index.html` 打开；或：

```bash
# Python 3
python -m http.server 8899
# 访问 http://localhost:8899
```

## 发布到 GitHub Pages

1. 把本文件夹内所有文件上传到 GitHub 仓库根目录（`index.html` 必须在仓库根，不能再套一层子目录）。
2. 仓库 → Settings → Pages → Build and deployment → Branch 选择 `main` 或 `master`，目录选 `/ (root)`。
3. 等待 1~2 分钟即可在 `https://<你的用户名>.github.io/<仓库名>/` 访问。

> 若部署后出现中文乱码，仓库根已附带 `.nojekyll` 空文件（避免 Jekyll 解析），GitHub Pages 会按 UTF-8 提供 HTML。

## 图片体积优化结果

总计：3886 KB → 约 557 KB（节省约 85.6%），全部文件均低于 GitHub 单文件 100 MB 硬限制、50 MB 警告阈值，可直接在网页端拖拽上传。
