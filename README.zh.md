# 中国历法数据集 · 总索引

**简体中文 ｜ [繁體中文](README.zh-Hant.md) ｜ [English](README.md) ｜ [日本語](README.ja.md) ｜ [한국어](README.ko.md)**

[![ORCID](https://img.shields.io/badge/ORCID-0009--0002--7650--833X-a6ce39.svg)](https://orcid.org/0009-0002-7650-833X) [![OpenAlex](https://img.shields.io/badge/OpenAlex-A5151908354-ff6f00.svg)](https://openalex.org/A5151908354) [![Site](https://img.shields.io/badge/site-kuangchujia.com-blue.svg)](https://kuangchujia.com) [![Data: CC BY 4.0](https://img.shields.io/badge/Data-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> **本仓是「中国历法」系列公开数据集的总入口。只做索引与互链，不存放数据本体。**
> 数据本体在各自子仓与 Zenodo，下载与引用请前往子仓。引用一律用 **Zenodo 概念 DOI**——它永久指向最新版本。

---

## 一、数据集一览

| # | 数据集 | 层次 | 规模 | Zenodo 概念 DOI | 许可 | 仓库 |
|:--:|:---|:---|:---|:---|:---|:---|
| 1 | **中国历法公共数据集**<br>二十四节气交节时刻 · 历代历法改革年表 · 干支纪日对照表 | **数值层**<br>「数是多少」 | A1 二十四节气交节时刻 **3,672** 条（公元 1900—2052，精确到秒）<br>A2 历代历法改革年表 **52** 部<br>A3 干支纪日对照表 **55,883** 天（1900-01-01 — 2052-12-31，逐日） | [10.5281/zenodo.22788686](https://doi.org/10.5281/zenodo.22788686) | CC BY 4.0 | [chinese-calendar-dataset](https://github.com/Kuangchujia/chinese-calendar-dataset) |
| 2 | **中国历法与古天文学术语对照表**（中英双语） | **概念层**<br>「词指什么」 | 主表 **279** 条术语 / **19** 组 / **25** 个二级子类<br>中文页与英文页逐条对拍 **279/279** 一致<br>另附二十八宿距星三源对照（28 行）与二十八宿星官星数（28 行） | [10.5281/zenodo.23028692](https://doi.org/10.5281/zenodo.23028692) | CC BY 4.0 | [chinese-calendar-glossary](https://github.com/Kuangchujia/chinese-calendar-glossary) |

**两件互为配套**：第 1 件给「数是多少」，第 2 件给「词指什么」。二者各自独立成仓、各自独立成篇，可单独引用，也可并为一套引用。

两件均另出**机器可读件**（`README_AI_AGENT.md` 与 schema.org 语义件），供 AI Agent 与 LLM 爬虫取用同一批事实的结构化声明。

---

## 二、配套软件

| 项目 | 说明 | Zenodo 概念 DOI | 许可 | 仓库 |
|:---|:---|:---|:---|:---|
| **astro-forecast** | 中国古天文历法**离线预计算引擎**（Skyfield ＋ JPL DE421）＋ WordPress 发布插件。二十四节气、日月食、行星合冲留逆、流星雨、日出日落与晨昏蒙影等，纯离线计算。 | [10.5281/zenodo.22950007](https://doi.org/10.5281/zenodo.22950007) | MIT | [astro-forecast](https://github.com/Kuangchujia/astro-forecast) |

第 1 件的数值即由此引擎自算而成，算法与代码完全公开、可复算。

---

## 三、为什么一律引「概念 DOI」

Zenodo 每一条记录有两个号：

| 号 | 性质 | 行为 |
|:---|:---|:---|
| **概念 DOI（concept DOI）** | 合集级 | **永久指向该合集的最新版本** |
| 版本 DOI（version DOI） | 记录级 | 固定在某一版，新版本发布后**不会跟着走** |

因此本索引一律只公布**概念 DOI**。日后数据集出新版本，同一串号照旧可用，不会停在旧版。

---

## 四、使用边界

- 两件数据集收录的均为**历法事实**（时刻、年表、对照表）与**术语对应关系**，不含任何推断、断语、吉凶宜忌或个体指向。
- 术语表第十九组「术数择日」只收**术语名与其界定**，不含任何择日方法或用法说明。
- 引用具体节气时刻时，宜同时注明**中国科学院紫金山天文台**《中国天文年历》／《日历资料》（依 GB/T 33661-2017《农历的编算和颁行》）；本数据集为独立的第二来源，用于复算与长跨度查询。
- 历代历法改革年表为**编纂表**，非原始文献；引用具体年份前请查考异表。
- 术语表的英文定译为**工作定译**，不主张排他。

---

## 五、作者与授权

| 项 | 地址 |
|:---|:---|
| **作者** | 邝楚嘉（Chujia Kuang / 嘉言一得） |
| **ORCID iD** | [0009-0002-7650-833X](https://orcid.org/0009-0002-7650-833X) |
| **OpenAlex** | [A5151908354](https://openalex.org/A5151908354) |
| **总入口 / 校验页** | <https://kuangchujia.com> |
| **OSF 项目（开放研究镜像）** | <https://osf.io/3wvkh/> |

- **数据**（第 1、2 件）采用 **Creative Commons Attribution 4.0 International（CC BY 4.0）**，可自由使用、复制、修改、分发（含商业用途），条件是署名。术语对照关系属通用数表性质；释义为作者原创表述。
- **软件**（第 2 节）采用 **MIT License**。

---

## 六、修订记录

| 日期 | 版本 | 说明 |
|:---|:---|:---|
| 2026-09-29 | 1.0.0 | 首次建立：收录中国历法公共数据集（数值层）与中国历法与古天文学术语对照表（概念层）两件，另录配套软件 astro-forecast。全部对外引用口径统一为 **Zenodo 概念 DOI**。 |
| 2026-10-07 | 1.1.0 | 五语版（**简体中文／繁體中文／English／日本語／한국어**）：README 出五个语种，各件题头置语言切换行。原置于 `README.md` 的中文版移入 `README.zh.md`；`README.md` 改置英文版，与系列内其余各仓体例对齐。**数据、DOI、许可均未变。** |
