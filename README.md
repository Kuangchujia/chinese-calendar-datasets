# Chinese Calendar Datasets · Index

**[简体中文](README.zh.md) ｜ [繁體中文](README.zh-Hant.md) ｜ English ｜ [日本語](README.ja.md) ｜ [한국어](README.ko.md)**

[![ORCID](https://img.shields.io/badge/ORCID-0009--0002--7650--833X-a6ce39.svg)](https://orcid.org/0009-0002-7650-833X) [![OpenAlex](https://img.shields.io/badge/OpenAlex-A5151908354-ff6f00.svg)](https://openalex.org/A5151908354) [![Site](https://img.shields.io/badge/site-kuangchujia.com-blue.svg)](https://kuangchujia.com) [![Data: CC BY 4.0](https://img.shields.io/badge/Data-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)

> **This repository is the umbrella entry point to the "Chinese Calendar" open dataset series. It indexes and cross-links only — no data itself is stored here.**
> The data lives in the sub-repositories and on Zenodo; please go there to download and cite. Always cite the **Zenodo concept DOI** — it points permanently to the latest version.

---

## I. The datasets at a glance

| # | Dataset | Layer | Scale | Zenodo concept DOI | Licence | Repository |
|:--:|:---|:---|:---|:---|:---|:---|
| 1 | **Chinese Calendar Open Datasets**<br>Instants of the twenty-four solar terms · Chronology of historical calendar reforms · Sexagenary day table | **Numerical layer**<br>"what the numbers are" | A1 solar-term instants **3,672** entries (CE 1900—2052, precise to the second)<br>A2 chronology of calendar reforms **52** calendars<br>A3 sexagenary day table **55,883** days (1900-01-01 — 2052-12-31, day by day) | [10.5281/zenodo.22788686](https://doi.org/10.5281/zenodo.22788686) | CC BY 4.0 | [chinese-calendar-dataset](https://github.com/Kuangchujia/chinese-calendar-dataset) |
| 2 | **Glossary of Chinese Calendrics and Traditional Uranography** (Chinese–English) | **Conceptual layer**<br>"what the words mean" | main table **279** terms / **19** groups / **25** second-level classes<br>Chinese and English pages matched term by term, **279/279** in agreement<br>plus two appendices — the determinative stars of the 28 lunar mansions in three-source comparison (28 rows), and star-official counts of the 28 lunar mansions (28 rows) | [10.5281/zenodo.23028692](https://doi.org/10.5281/zenodo.23028692) | CC BY 4.0 | [chinese-calendar-glossary](https://github.com/Kuangchujia/chinese-calendar-glossary) |

**The two are companions**: the first gives "what the numbers are", the second gives "what the words mean". Each stands as its own repository and its own citable work; they may be cited separately or as a set.

Both also ship a **machine-readable edition** (`README_AI_AGENT.md` and a schema.org semantic file), so that AI agents and LLM crawlers can take up structured statements of the same facts.

---

## II. Companion software

| Project | Description | Zenodo concept DOI | Licence | Repository |
|:---|:---|:---|:---|:---|
| **astro-forecast** | An **offline pre-computation engine** for Chinese historical astronomy and calendrics (Skyfield + JPL DE421), plus a WordPress publishing plugin. Solar terms, eclipses, planetary conjunctions / oppositions / stations / retrogradations, meteor showers, sunrise and sunset, twilight — all computed fully offline. | [10.5281/zenodo.22950007](https://doi.org/10.5281/zenodo.22950007) | MIT | [astro-forecast](https://github.com/Kuangchujia/astro-forecast) |

The figures in dataset 1 are computed by this engine; the algorithm and the code are fully public and reproducible.

---

## III. Why only concept DOIs are cited

Every Zenodo record carries two identifiers:

| Identifier | Level | Behaviour |
|:---|:---|:---|
| **Concept DOI** | collection | **permanently points to the latest version of that collection** |
| Version DOI | record | fixed to one version; when a new version is released it **does not follow along** |

This index therefore publishes **concept DOIs only**. When a dataset gains a new version, the same string keeps working and never stalls at an old release.

---

## IV. Scope and limits

- Both datasets contain **calendrical facts** (instants, chronologies, correspondence tables) and **term correspondences** only. They contain no inference, no verdict, no auspicious-or-inauspicious guidance, and nothing directed at any individual.
- Group 19 of the glossary, "divination and day-selection", records **term names and their definitions only**, with no day-selection method or usage instructions.
- When citing a particular solar-term instant, please also cite the **Purple Mountain Observatory, Chinese Academy of Sciences** — *Chinese Astronomical Almanac* / *Calendar Data* (under GB/T 33661-2017 *Calculation and promulgation of the Chinese calendar*). This dataset is an independent second source, for re-computation and long-span queries.
- The chronology of calendar reforms is a **compiled table**, not a primary document; consult the variant table before citing any particular year.
- The glossary's English renderings are **working translations** and claim no exclusivity.

---

## V. Author and licence

| Item | Address |
|:---|:---|
| **Author** | Chujia Kuang (邝楚嘉 / pen name Jiayan Yide 嘉言一得) |
| **ORCID iD** | [0009-0002-7650-833X](https://orcid.org/0009-0002-7650-833X) |
| **OpenAlex** | [A5151908354](https://openalex.org/A5151908354) |
| **Umbrella entry point / verification hub** | <https://kuangchujia.com> |
| **OSF project (open research mirror)** | <https://osf.io/3sz95/> |

- **The data** (datasets 1 and 2) is released under **Creative Commons Attribution 4.0 International (CC BY 4.0)** — free to use, copy, modify and distribute, including commercially, on condition of attribution. The term correspondences are of the nature of a general table of data; the definitions are the author's original wording.
- **The software** (section II) is released under the **MIT License**.

---

## VI. Revision history

| Date | Version | Notes |
|:---|:---|:---|
| 2026-09-29 | 1.0.0 | First established: indexing the Chinese Calendar Open Datasets (numerical layer) and the Glossary of Chinese Calendrics and Traditional Uranography (conceptual layer), with the companion software astro-forecast. All outward citation unified on **Zenodo concept DOIs**. |
| 2026-10-07 | 1.1.0 | Five-language edition (**Simplified Chinese / Traditional Chinese / English / Japanese / Korean**): the README now ships in five languages with a language switcher at the head of each file. The Chinese edition previously held in `README.md` has been carried over to `README.zh.md`; `README.md` now holds the English edition, aligned with the other repositories of the series. **No data, DOI or licence changed.** |
