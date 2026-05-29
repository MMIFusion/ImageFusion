<a id="top"></a>

# 多模态信息融合 | Image Fusion Papers

微信公众号：多模态信息融合 + : ）

本仓库用于持续整理图像融合方向的最新论文，覆盖顶会、顶刊与高质量预印本，重点记录论文题目、作者信息、作者单位、论文下载链接、代码链接、项目主页与公众号解读链接。每次提交并 push 到 GitHub 后，README 页面会自动展示最新内容，读者可收藏本仓库链接。

GitHub 入口：https://github.com/MMIFusion/ImageFusion

---

<a id="navigation"></a>

## 快速导航

- [最新更新](#latest-updates)
- [收录范围](#scope)
- [如何检索](#search-guide)
- [任务标签](#task-tags)
- [字段说明](#field-guide)
- [预印本与待接收论文](#preprints)
- [顶会论文](#conference-papers)
  - [CVPR](#cvpr)
  - [ICCV](#iccv)
  - [ECCV](#eccv)
  - [NeurIPS](#neurips)
  - [ICLR](#iclr)
  - [AAAI](#aaai)
  - [IJCAI](#ijcai)
  - [ACM MM](#acm-mm)
  - [Other Conferences](#other-conferences)
- [顶刊论文](#journal-papers)
  - [TPAMI](#tpami)
  - [TIP](#tip)
  - [TMM](#tmm)
  - [TNNLS](#tnnls)
  - [TCSVT](#tcsvt)
  - [Information Fusion](#information-fusion)
  - [Pattern Recognition](#pattern-recognition)
  - [Remote Sensing / TGRS / JSTARS](#remote-sensing-journals)
  - [Medical Image Analysis / TMI](#medical-journals)
  - [Other Journals](#other-journals)
- [论文条目模板](#paper-template)
- [更新流程](#update-workflow)
- [维护规范](#maintenance-guide)
- [扩展策略](#scaling-guide)

---

<a id="latest-updates"></a>

## 最新更新

> 建议按更新时间倒序维护。新论文加入对应会议或期刊章节后，在这里放一条简短索引，方便读者快速查看最近更新。

| Date | ID | Venue | Task | Title | Links |
|---|---|---|---|---|---|

[Back to top](#top)

---

<a id="scope"></a>

## 收录范围

本仓库优先收录与图像融合、多模态视觉融合、跨模态图像增强和融合感知任务相关的论文。

优先级建议：

1. 顶会与顶刊正式录用论文。
2. 有代码、项目主页、数据集或 benchmark 的高质量论文。
3. 与图像融合密切相关的 arXiv、OpenReview 或技术报告。
4. 与检测、分割、超分、低照度、遥感、医学影像等任务结合紧密的融合论文。

暂不建议收录：

1. 与图像融合关系较弱的通用多模态大模型论文。
2. 只有标题相关、但正文任务不属于融合方向的论文。
3. 无法确认来源、作者或下载链接的非正式资料。

[Back to top](#top)

---

<a id="search-guide"></a>

## 如何检索

推荐使用浏览器页面搜索：

- 按论文标题搜索：`Ctrl + F` / `Command + F` 后输入关键词。
- 按作者搜索：输入作者姓名，例如 `First Author`。
- 按单位搜索：输入学校、实验室或公司名称，例如 `University`, `CAS`, `Tencent`, `Huawei`。
- 按会议或期刊搜索：输入 `CVPR 2026`, `ICCV 2025`, `TPAMI 2026`。
- 按任务标签搜索：输入 `VIF`, `MEF`, `MFF`, `MIF`, `Pansharpening`, `HSI-MSI`。
- 按代码状态搜索：查看 `Code` 列是否存在 GitHub、官方项目页或 Papers with Code 链接。

建议每篇论文使用统一 ID：

```text
VENUE-YEAR-NUMBER
```

示例：

```text
CVPR-2026-001
TPAMI-2026-001
INFOFUSION-2026-001
```

[Back to top](#top)

---

<a id="task-tags"></a>

## 任务标签

| Tag | 中文方向 | 说明 |
|---|---|---|
| VIF | 红外与可见光图像融合 | Infrared and visible image fusion |
| MEF | 多曝光图像融合 | Multi-exposure image fusion |
| MFF | 多焦点图像融合 | Multi-focus image fusion |
| MIF | 医学图像融合 | Medical image fusion |
| Pansharpening | 全色锐化 | Panchromatic and multispectral image fusion |
| HSI-MSI | 高光谱与多光谱融合 | Hyperspectral and multispectral image fusion |
| RS-Fusion | 遥感图像融合 | Remote sensing image fusion |
| RGB-T | RGB-T 融合 | RGB and thermal fusion |
| RGB-D | RGB-D 融合 | RGB and depth fusion |
| SR-Fusion | 超分辨率融合 | Fusion for super-resolution or restoration |
| LL-Fusion | 低照度融合 | Fusion for low-light enhancement |
| Detection | 检测导向融合 | Fusion for object detection |
| Segmentation | 分割导向融合 | Fusion for semantic segmentation |
| Registration | 配准与融合 | Joint registration and fusion |
| Survey | 综述 | Survey, benchmark, dataset or evaluation paper |

[Back to top](#top)

---

<a id="field-guide"></a>

## 字段说明

| Field | 填写方式 | 示例 |
|---|---|---|
| ID | `VENUE-YEAR-NUMBER`，同一章节内递增 | `CVPR-2026-001` |
| Date | 加入仓库或论文公开日期 | `2026-05-29` |
| Venue / Journal | 会议、期刊或预印本来源 | `CVPR 2026`, `TPAMI 2026`, `arXiv 2026` |
| Title | 官方英文标题 | `Paper Title` |
| Authors | 作者列表，使用分号分隔 | `Author A; Author B; Author C` |
| Affiliations | 主要作者单位，使用分号分隔 | `University A; Institute B` |
| Task | 使用统一任务标签 | `VIF`, `MEF`, `MIF` |
| Paper | 官方论文、PDF、arXiv、OpenReview 或出版社页面 | `[PDF](paper-url)` |
| Code | 官方代码仓库；没有则填 `-` | `[Code](code-url)` |
| Project | 官方项目主页、Demo、数据集页；没有则填 `-` | `[Project](project-url)` |
| 公众号解读 | 对应公众号文章链接；未发布则填 `-` | `[解读](wechat-url)` |
| Notes | 一句话贡献点、关键词或检索辅助信息 | `Transformer, benchmark, low-light` |

[Back to top](#top)

---

<a id="preprints"></a>

## 预印本与待接收论文

> 适合先收录 arXiv、OpenReview、技术报告或已公开但尚未确认最终会议信息的论文。论文正式接收后，建议移动到对应会议或期刊章节。

| ID | Date | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

---

<a id="conference-papers"></a>

## 顶会论文

<a id="cvpr"></a>

### CVPR

<a id="cvpr-2026"></a>

#### CVPR 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

<a id="cvpr-2025"></a>

#### CVPR 2025

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="iccv"></a>

### ICCV

<a id="iccv-2025"></a>

#### ICCV 2025

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="eccv"></a>

### ECCV

<a id="eccv-2026"></a>

#### ECCV 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="neurips"></a>

### NeurIPS

<a id="neurips-2026"></a>

#### NeurIPS 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="iclr"></a>

### ICLR

<a id="iclr-2026"></a>

#### ICLR 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="aaai"></a>

### AAAI

<a id="aaai-2026"></a>

#### AAAI 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="ijcai"></a>

### IJCAI

<a id="ijcai-2026"></a>

#### IJCAI 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="acm-mm"></a>

### ACM MM

<a id="acmmm-2026"></a>

#### ACM MM 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="other-conferences"></a>

### Other Conferences

| ID | Venue | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

---

<a id="journal-papers"></a>

## 顶刊论文

<a id="tpami"></a>

### TPAMI

<a id="tpami-2026"></a>

#### TPAMI 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="tip"></a>

### TIP

<a id="tip-2026"></a>

#### TIP 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="tmm"></a>

### TMM

<a id="tmm-2026"></a>

#### TMM 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="tnnls"></a>

### TNNLS

<a id="tnnls-2026"></a>

#### TNNLS 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="tcsvt"></a>

### TCSVT

<a id="tcsvt-2026"></a>

#### TCSVT 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="information-fusion"></a>

### Information Fusion

<a id="infofusion-2026"></a>

#### Information Fusion 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="pattern-recognition"></a>

### Pattern Recognition

<a id="pr-2026"></a>

#### Pattern Recognition 2026

| ID | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="remote-sensing-journals"></a>

### Remote Sensing / TGRS / JSTARS

| ID | Journal | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="medical-journals"></a>

### Medical Image Analysis / TMI

| ID | Journal | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

<a id="other-journals"></a>

### Other Journals

| ID | Journal | Title | Authors | Affiliations | Task | Paper | Code | Project | 公众号解读 | Notes |
|---|---|---|---|---|---|---|---|---|---|---|

[Back to top](#top)

---

<a id="paper-template"></a>

## 论文条目模板

复制下面任意一行到对应会议或期刊章节后填写即可。

### 会议论文

```markdown
| <a id="cvpr-2026-001"></a>CVPR-2026-001 | Paper Title | Author A; Author B; Author C | Affiliation A; Affiliation B | VIF | [PDF](paper-url) | [Code](code-url) | [Project](project-url) | [解读](wechat-url) | Main idea / keywords |
```

### 预印本

```markdown
| <a id="arxiv-2026-001"></a>ARXIV-2026-001 | YYYY-MM-DD | Paper Title | Author A; Author B | Affiliation A; Affiliation B | VIF | [PDF](paper-url) | [Code](code-url) | [Project](project-url) | [解读](wechat-url) | Main idea / keywords |
```

### 期刊论文

```markdown
| <a id="tpami-2026-001"></a>TPAMI-2026-001 | Paper Title | Author A; Author B; Author C | Affiliation A; Affiliation B | VIF | [PDF](paper-url) | [Code](code-url) | [Project](project-url) | [解读](wechat-url) | Main idea / keywords |
```

### 最新更新索引

```markdown
| YYYY-MM-DD | [CVPR-2026-001](#cvpr-2026-001) | CVPR 2026 | VIF | Paper Title | [Paper](paper-url) / [Code](code-url) / [Project](project-url) / [解读](wechat-url) |
```

### 其他会议或其他期刊

```markdown
| <a id="conf-yyyy-001"></a>CONF-YYYY-001 | Conference YYYY | Paper Title | Author A; Author B | Affiliation A; Affiliation B | VIF | [PDF](paper-url) | [Code](code-url) | [Project](project-url) | [解读](wechat-url) | Main idea / keywords |
```

如果某个链接暂时没有，可以填：

```markdown
-
```

[Back to top](#top)

---

<a id="update-workflow"></a>

## 更新流程

每次新增论文，按下面顺序维护：

1. 判断论文归属：正式录用放入对应会议或期刊；未正式确认放入 [预印本与待接收论文](#preprints)。
2. 复制 [论文条目模板](#paper-template) 中合适的一行。
3. 生成唯一 ID，例如 `CVPR-2026-001`、`TPAMI-2026-001`、`ARXIV-2026-001`。
4. 在 ID 前写入同名小写锚点，例如 `<a id="cvpr-2026-001"></a>CVPR-2026-001`。
5. 填写标题、作者、单位、任务标签、论文链接、代码链接、项目主页、公众号解读和备注。
6. 在 [最新更新](#latest-updates) 添加一行，ID 链接到具体论文锚点。
7. 本地检查 README 显示无明显断行或表格错误。
8. 提交并推送到 GitHub。

常用命令：

```bash
git add README.md
git commit -m "Update image fusion paper list"
git push
```

[Back to top](#top)

---

<a id="maintenance-guide"></a>

## 维护规范

1. 新论文优先填入对应的会议或期刊年份章节。
2. 论文 ID 使用 `VENUE-YEAR-NUMBER`，同一章节内从 `001` 递增。
3. 每条论文 ID 建议写成 `<a id="venue-year-number"></a>VENUE-YEAR-NUMBER`，这样 [最新更新](#latest-updates) 可以直达具体条目。
4. `Title` 使用论文官方英文题目，避免自行缩写。
5. `Authors` 建议填写完整作者；作者过多时可写 `First Author et al.`，但公众号解读中建议补全。
6. `Affiliations` 建议填写主要作者单位，用分号分隔多个单位。
7. `Task` 使用 [任务标签](#task-tags) 中的统一写法，便于搜索。
8. `Paper` 优先放官方 PDF，其次放 arXiv、OpenReview、IEEE、CVF、ACM 或 Springer 页面。
9. `Code` 优先放官方 GitHub；没有代码时填 `-`，不要放无关复现仓库。
10. `Project` 放官方项目主页、Demo 页面或数据集页面；没有则填 `-`。
11. `公众号解读` 放对应文章链接；尚未发布时填 `-`。
12. `Notes` 用一句话写清贡献点、关键词或适合检索的短语。
13. 每次新增论文后，将该论文同步加入 [最新更新](#latest-updates)。
14. 表格单元格中不要直接出现竖线 `|`；如果论文标题或备注里必须出现，写成 `\|`，否则 GitHub 表格会断列。
15. 暂无内容的字段统一填 `-`，不要留空，后续检索和排版更稳定。

[Back to top](#top)

---

<a id="scaling-guide"></a>

## 扩展策略

当前阶段建议所有内容都维护在 `README.md` 中，优点是打开仓库即可浏览、跳转和检索，最适合公众号读者直接使用。

长期扩展时按下面规则处理：

1. 新增年份：在对应 venue 下新增 `#### VENUE YEAR` 小节，并复制同样的表头。
2. 新增会议：在 [顶会论文](#conference-papers) 下新增 `### Venue Name`，同时在 [快速导航](#navigation) 加入链接。
3. 新增期刊：在 [顶刊论文](#journal-papers) 下新增 `### Journal Name`，同时在 [快速导航](#navigation) 加入链接。
4. 论文数量增多后，仍保持一篇论文一行，不在 README 中写长摘要；长解读放到公众号文章。
5. `最新更新` 只保留最近一段时间或最近若干篇，完整列表仍以各会议、期刊章节为准。
6. 当 README 超过数百篇论文且 GitHub 页面明显加载变慢时，再考虑拆分 `papers/` 子文件；即使拆分，`README.md` 仍作为主导航入口。

[Back to top](#top)
