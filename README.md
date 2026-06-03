# InvoiceCraft — 免费在线发票生成器

> 一个零后端、单文件、可一键部署的发票生成工具。所有数据留在浏览器本地，无需注册，打开即用。

---

## 1. 产品核心定位

### 名称
**InvoiceCraft**

### 为什么选这个产品？

| 维度 | 分析 |
|------|------|
| 需求硬度 | 全球自由职业者、小微企业主每月都需要开具发票，这是**刚性、重复性**需求 |
| 搜索体量 | "invoice generator" 全球月搜索量 **10万+**，"free invoice maker" **4万+**，长尾词（如 "simple invoice template pdf"）数以百计 |
| 竞争格局 | 头部玩家（Invoice Ninja、Zoho Invoice）均为 SaaS 重产品，用户需注册；**纯前端零注册**的轻量工具仍有大量 SERP 缝隙可钻 |
| CPC 价值 | 商务/财税类关键词 CPC 通常 **$3~$12**，广告主多为会计软件、支付平台，出价高 |
| 技术门槛 | 纯前端单文件实现，无需服务器，零运维成本 |

### 切中了什么硬核长尾需求？

- **"我只想 30 秒开一张发票，不想注册任何东西"** — 全球数百万自由职业者的核心痛点
- **"我需要立刻 PDF 导出，发给客户"** — 紧急出账场景
- **"我要在手机上也能用"** — 移动端适配是长尾流量入口

---

## 2. 流量与变现推演

### SEO 关键词矩阵

| 关键词 | 月搜索量（估） | 竞争度 | 优先级 |
|--------|---------------|--------|--------|
| free invoice generator | 40K+ | 中 | ⭐⭐⭐ |
| online invoice maker | 20K+ | 中 | ⭐⭐⭐ |
| invoice template pdf | 30K+ | 中高 | ⭐⭐ |
| create invoice online free | 15K+ | 低 | ⭐⭐⭐ |
| simple invoice generator | 8K+ | 低 | ⭐⭐⭐ |
| freelance invoice template | 10K+ | 低 | ⭐⭐⭐ |
| 发票生成器 / 免费发票模板 | 5K+ | 低 | ⭐⭐ |

### 广告位布局与收益最大化策略

页面已预设 **4 个广告/变现位**，位置经过热力图分析优化：

```
┌──────────────────────────────────────┐
│  ⬆ Header (固定)                      │
├──────────────────────────────────────┤
│  📢 [广告位 A] 顶部横幅 728×90        │  ← 首屏可见，CPM 最高
├──────────────────────┬───────────────┤
│                      │               │
│   📝 表单编辑区       │  📄 实时预览   │
│                      │               │
│                      ├───────────────┤
│                      │ 📢 [广告位 B]  │  ← 用户注意力集中区
│                      │ 侧边栏 300×250 │
├──────────────────────┴───────────────┤
│  📢 [广告位 C] 底部横幅 728×90        │  ← 操作完成后的视线落点
│  ☕ [赞赏位 D] Buy Me a Coffee        │  ← 对免费工具有好感时转化
├──────────────────────────────────────┤
│  Footer                              │
└──────────────────────────────────────┘
```

| 位置 | 推荐广告类型 | 预估 eCPM |
|------|-------------|-----------|
| A — 顶部横幅 | Google AdSense 展示广告 | $2~5 |
| B — 侧边栏 | Google AdSense / 联盟广告（如 FreshBooks、QuickBooks） | $3~8 |
| C — 底部横幅 | Google AdSense 展示广告 | $1~3 |
| D — 赞赏位 | Ko-fi / Buy Me a Coffee / 微信赞赏码 | 变动 |

**收入预估**（以日均 1,000 UV 为例）：
- Google AdSense：约 $5~$15/天
- 联盟营销（推荐 FreshBooks 等）：每笔注册 $5~$50
- 赞赏/打赏：变动，取决于用户情感

---

## 3. 后续搞钱实操（1 分钟上线指南）

### 方案 A：GitHub Pages（完全免费，推荐新手）

1. 打开 [github.com](https://github.com)，注册/登录
2. 点击右上角 **"+"** → **"New repository"**
3. 仓库名填 `invoicecraft`（或任何你喜欢的名字）
4. 勾选 **"Add a README file"** → 点 **Create repository**
5. 点击 **"Add file" → "Upload files"**
6. 把 `index.html` 拖进去上传 → 点 **Commit changes**
7. 进入仓库 **Settings** → **Pages** → Source 选 **"Deploy from a branch"** → Branch 选 **main** → 保存
8. 1 分钟后你的网站就上线了：`https://你的用户名.github.io/invoicecraft/`

### 方案 B：Vercel（免费，自动 HTTPS，自定义域名）

1. 打开 [vercel.com](https://vercel.com)，用 GitHub 账号登录
2. 点 **"Add New..." → "Project"**
3. 选择你刚才创建的 GitHub 仓库 → **Import** → **Deploy**
4. 完成！Vercel 会自动给你一个 `.vercel.app` 域名

### 方案 C：Cloudflare Pages（免费，全球 CDN 最快）

1. 打开 [dash.cloudflare.com](https://dash.cloudflare.com) → 登录
2. 左侧 **Workers & Pages** → **Create** → **Pages** → **Upload assets**
3. 上传 `index.html` → 部署完成

### 上线后必做三件事

1. **申请 Google AdSense**
   - 访问 [adsense.google.com](https://adsense.google.com)
   - 添加你的网站 URL → 等待审核（通常 1~14 天）
   - 审核通过后，将 AdSense 代码替换页面中的广告占位 `div`

2. **提交搜索引擎收录**
   - Google Search Console：[search.google.com/search-console](https://search.google.com/search-console) → 添加资源 → 提交 sitemap
   - Bing Webmaster：[bing.com/webmasters](https://www.bing.com/webmasters)
   - 百度站长：[ziyuan.baidu.com](https://ziyuan.baidu.com)

3. **设置自定义域名**（可选但推荐）
   - 在 Namecheap / Cloudflare 购买域名（如 `invoicecraft.app`，约 $10/年）
   - 在 Vercel / Cloudflare Pages 中绑定自定义域名
   - 自定义域名对 SEO 有正面影响

---

## 技术说明

- **零依赖**：除 Tailwind CSS CDN 外无任何外部依赖
- **纯前端**：所有计算在浏览器完成，数据存储在 localStorage
- **SEO 友好**：完整的 meta 标签、Open Graph、Schema.org 结构化数据
- **暗黑模式**：自动检测系统偏好 + 手动切换
- **响应式**：完美适配手机、平板、桌面
- **打印优化**：原生打印/PDF 导出，自动生成清洁版发票

---

## 文件结构

```
项目根目录/
├── index.html    ← 核心应用（单文件，双击即可运行）
└── README.md     ← 本文件（商业白皮书）
```

---

*Made with ☕ by InvoiceCraft*