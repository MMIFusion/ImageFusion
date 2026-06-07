<a id="top"></a>

# 🌈 Image Fusion Papers

> **多模态信息融合** 公众号 · 图像融合论文持续追踪库
>
> 每篇论文的完整信息只在 `<VENUE>/<YEAR>.md` 中维护，本页只做导航。

![Papers](https://img.shields.io/badge/Papers-62-blue.svg)
![Venues](https://img.shields.io/badge/Venues-4-orange.svg)
![Latest](https://img.shields.io/badge/Latest-2026-brightgreen.svg)

---

## 🏛️ 会议

| Venue | 论文数 | 年份 |
|---|---|---|
| [CVPR](./CVPR/README.md) | 17 | [2026](./CVPR/2026.md) |
| [AAAI](./AAAI/README.md) | 15 | [2026](./AAAI/2026.md) |
| [ICCV](./ICCV/README.md) | 11 | [2025](./ICCV/2025.md) |

## 📚 期刊

| Venue | 论文数 | 年份 |
|---|---|---|
| [TPAMI](./TPAMI/README.md) | 19 | [2026](./TPAMI/2026.md) |

---

## 📂 结构说明

```
ImageFusion/
├── README.md         ← 本页：顶层导航
├── CVPR/
│   ├── README.md     ← CVPR 总览（年份索引 + 一行式列表）
│   └── 2026.md       ← 论文详情（标题、作者、单位、链接、摘要）
├── AAAI/
│   ├── README.md     ← AAAI 总览（年份索引 + 一行式列表）
│   └── 2026.md       ← 论文详情（标题、作者、单位、链接、摘要）
├── ICCV/
│   ├── README.md
│   └── 2025.md
└── TPAMI/
    ├── README.md
    └── 2026.md
```

- **顶层 README**：列出所有已收录的会议与期刊。
- **`<VENUE>/README.md`**：该 venue 的年份索引与全部论文一行式列表。
- **`<VENUE>/<YEAR>.md`**：论文详情卡片，唯一信息源。

## 🏷️ 字段约定

每条论文卡片包含：

| 字段 | 含义 |
|---|---|
| **Task** | 任务标签（VIF / MEF / MIF / Diffusion / Unified 等） |
| **Authors** | 作者列表，源专辑未列出时显式标注 |
| **Affiliations** | 主要作者单位 |
| **Session / Paper ID** | 会议 session 编号或期刊 paper ID |
| **Links** | 📄 论文 · 💻 代码 · 🔍 Scholar 检索（缺论文链接时的兜底） |
| **Code** | 作者代码状态；公开则在 Links 给出，未公开时显式标注 |
| **摘要 / Abstract** | 中文摘要（折叠展开） |

## 🔄 持续更新

每期公众号专辑发布后：

1. 在对应 `<VENUE>/<YEAR>.md` 末尾追加论文卡片；
2. 同步更新该 venue 的 `README.md`；
3. 在本页"会议 / 期刊"表更新论文数与年份；
4. 推送时 commit 信息统一写：`微信公众号：多模态信息融合`。

## 📮 公众号

**多模态信息融合** · 持续分享图像融合方向的最新论文与解读。

[⬆ 回到顶部](#top)
