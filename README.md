# NBTI

把 CatTI 和 MouTI 放进同一个仓库后的统一项目。

## 项目结构

```text
NBTI/
├─ cat-ti/
│  └─ index.html
├─ mou-ti/
│  └─ index.html
└─ index.html
```

## 约定后的发布流程

以后统一走这条链路：

1. 先在本地修改 `cat-ti/index.html` 或 `mou-ti/index.html`
2. 提交并推送到 GitHub 仓库 `NBTI`
3. 再由 Cloudflare Pages 从 GitHub 拉取并部署

## Cloudflare Pages 建议配置

### CatTI
- Repository: `hesumin/NBTI`
- Production branch: `main`
- Root directory: `cat-ti`
- Framework preset: `None`
- Build command: 留空
- Build output directory: `.`

### MouTI
- Repository: `hesumin/NBTI`
- Production branch: `main`
- Root directory: `mou-ti`
- Framework preset: `None`
- Build command: 留空
- Build output directory: `.`

## 页面入口

- CatTI: `cat-ti/index.html`
- MouTI: `mou-ti/index.html`
- 根目录导航页: `index.html`
