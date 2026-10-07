# 中國曆法數據集 · 總索引

**[简体中文](README.zh.md) ｜ 繁體中文 ｜ [English](README.md) ｜ [日本語](README.ja.md) ｜ [한국어](README.ko.md)**

[![ORCID](https://img.shields.io/badge/ORCID-0009--0002--7650--833X-a6ce39.svg)](https://orcid.org/0009-0002-7650-833X) [![OpenAlex](https://img.shields.io/badge/OpenAlex-A5151908354-ff6f00.svg)](https://openalex.org/A5151908354) [![Site](https://img.shields.io/badge/site-kuangchujia.com-blue.svg)](https://kuangchujia.com) [![Data: CC BY 4.0](https://img.shields.io/badge/Data-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> **本倉是「中國曆法」系列公開數據集的總入口。只做索引與互鏈，不存放數據本體。**
> 數據本體在各自子倉與 Zenodo，下載與引用請前往子倉。引用一律用 **Zenodo 概念 DOI**——它永久指向最新版本。

---

## 一、數據集一覽

| # | 數據集 | 層次 | 規模 | Zenodo 概念 DOI | 許可 | 倉庫 |
|:--:|:---|:---|:---|:---|:---|:---|
| 1 | **中國曆法公共數據集**<br>二十四節氣交節時刻 · 歷代曆法改革年表 · 干支紀日對照表 | **數值層**<br>「數是多少」 | A1 二十四節氣交節時刻 **3,672** 條（公元 1900—2052，精確到秒）<br>A2 歷代曆法改革年表 **52** 部<br>A3 干支紀日對照表 **55,883** 天（1900-01-01 — 2052-12-31，逐日） | [10.5281/zenodo.22788686](https://doi.org/10.5281/zenodo.22788686) | CC BY 4.0 | [chinese-calendar-dataset](https://github.com/Kuangchujia/chinese-calendar-dataset) |
| 2 | **中國曆法與古天文學術語對照表**（中英雙語） | **概念層**<br>「詞指什麼」 | 主表 **279** 條術語 / **19** 組 / **25** 個二級子類<br>中文頁與英文頁逐條對拍 **279/279** 一致<br>另附二十八宿距星三源對照（28 行）與二十八宿星官星數（28 行） | [10.5281/zenodo.23028692](https://doi.org/10.5281/zenodo.23028692) | CC BY 4.0 | [chinese-calendar-glossary](https://github.com/Kuangchujia/chinese-calendar-glossary) |

**兩件互為配套**：第 1 件給「數是多少」，第 2 件給「詞指什麼」。二者各自獨立成倉、各自獨立成篇，可單獨引用，也可併為一套引用。

兩件均另出**機器可讀件**（`README_AI_AGENT.md` 與 schema.org 語義件），供 AI Agent 與 LLM 爬蟲取用同一批事實的結構化聲明。

---

## 二、配套軟件

| 項目 | 說明 | Zenodo 概念 DOI | 許可 | 倉庫 |
|:---|:---|:---|:---|:---|
| **astro-forecast** | 中國古天文曆法**離線預計算引擎**（Skyfield ＋ JPL DE421）＋ WordPress 發佈插件。二十四節氣、日月食、行星合衝留逆、流星雨、日出日落與晨昏蒙影等，純離線計算。 | [10.5281/zenodo.22950007](https://doi.org/10.5281/zenodo.22950007) | MIT | [astro-forecast](https://github.com/Kuangchujia/astro-forecast) |

第 1 件的數值即由此引擎自算而成，算法與代碼完全公開、可復算。

---

## 三、為什麼一律引「概念 DOI」

Zenodo 每一條記錄有兩個號：

| 號 | 性質 | 行為 |
|:---|:---|:---|
| **概念 DOI（concept DOI）** | 合集級 | **永久指向該合集的最新版本** |
| 版本 DOI（version DOI） | 記錄級 | 固定在某一版，新版本發佈後**不會跟著走** |

因此本索引一律只公佈**概念 DOI**。日後數據集出新版本，同一串號照舊可用，不會停在舊版。

---

## 四、使用邊界

- 兩件數據集收錄的均為**曆法事實**（時刻、年表、對照表）與**術語對應關係**，不含任何推斷、斷語、吉凶宜忌或個體指向。
- 術語表第十九組「術數擇日」只收**術語名與其界定**，不含任何擇日方法或用法說明。
- 引用具體節氣時刻時，宜同時註明**中國科學院紫金山天文臺**《中國天文年曆》／《日曆資料》（依 GB/T 33661-2017《農曆的編算和頒行》）；本數據集為獨立的第二來源，用於復算與長跨度查詢。
- 歷代曆法改革年表為**編纂表**，非原始文獻；引用具體年份前請查考異表。
- 術語表的英文定譯為**工作定譯**，不主張排他。

---

## 五、作者與授權

| 項 | 地址 |
|:---|:---|
| **作者** | 鄺楚嘉（Chujia Kuang / 嘉言一得） |
| **ORCID iD** | [0009-0002-7650-833X](https://orcid.org/0009-0002-7650-833X) |
| **OpenAlex** | [A5151908354](https://openalex.org/A5151908354) |
| **總入口 / 校驗頁** | <https://kuangchujia.com> |

- **數據**（第 1、2 件）採用 **Creative Commons Attribution 4.0 International（CC BY 4.0）**，可自由使用、複製、修改、分發（含商業用途），條件是署名。術語對照關係屬通用數表性質；釋義為作者原創表述。
- **軟件**（第 2 節）採用 **MIT License**。

---

## 六、修訂記錄

| 日期 | 版本 | 說明 |
|:---|:---|:---|
| 2026-09-29 | 1.0.0 | 首次建立：收錄中國曆法公共數據集（數值層）與中國曆法與古天文學術語對照表（概念層）兩件，另錄配套軟件 astro-forecast。全部對外引用口徑統一為 **Zenodo 概念 DOI**。 |
| 2026-10-07 | 1.1.0 | 五語版（**簡體中文／繁體中文／English／日本語／한국어**）：README 出五個語種，各件題頭置語言切換行。原置於 `README.md` 的中文版移入 `README.zh.md`；`README.md` 改置英文版，與系列內其餘各倉體例對齊。**數據、DOI、許可均未變。** |
