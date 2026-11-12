# 简体中文改编版说明 / Simplified Chinese adaptation notice

本仓库是 [academic-research-skills](https://github.com/Imbad0202/academic-research-skills)（作者 Cheng-I Wu，许可证 CC BY-NC 4.0）的改编版本，基于上游提交 `6d93886`（v3.24.2 之后的 main）。

This repository is an adaptation of [academic-research-skills](https://github.com/Imbad0202/academic-research-skills) by Cheng-I Wu, licensed under [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/). It is based on upstream commit `6d93886` (main after v3.24.2). The original work and this adaptation are for non-commercial use only. The original author does not endorse this adaptation.

## 改动内容 / Changes

- **文献回顾形式提醒（review-form note, #921）**：把繁体中文提醒文本改为简体中文（中国大陆用词，如“系统综述”“范围综述”“默认”“项目”），标题改为 `Note text (Simplified Chinese)`；中文对话（简体或繁体）都显示简体文本。正本 `shared/references/review_form_note.md` 与 `deep-research/SKILL.md`、`academic-paper/SKILL.md` 两个副本同步修改。
- `scripts/check_review_form_note_sync.py` 及其测试改为校验简体文本（选项标签、中立句、排序用词）。测试中一处 Windows 路径分隔符问题顺带修正。
- `deep-research`、`academic-paper`、`academic-paper-reviewer` 的 SKILL.md：模式选择表、示例提示改为简体；新增 `**简体中文**` 触发词行（保留原繁体触发词，繁体输入仍可触发）。
- Socratic mentor agents、`plan_mode_protocol.md`：在繁体输入示例旁补充简体示例。
- 繁转简（OpenCC t2s + 人工用词修正）：两个 `mode_selection_guide.md`、`writing_quality_check.md`、`equator_reporting_guidelines.md`、`socratic_questioning_framework.md`、LaTeX 模板注释、`academic-paper/examples/chinese_paper_example.md`。

## 未改动的繁体内容 / Left unchanged on purpose

- 专有名词：台湾期刊名（`top_journals_by_field.md`）、法规名称《人體研究法》及其引用（IRB 相关 registry 与文档）。
- 繁体 APA 引用规范示例（`apa7_chinese_citation_guide.md`、`citation_compliance_agent.md`）。
- Python 脚本里 `zh-TW` 语言的报告字符串与用于识别繁体输入的正则（改动会影响上游的 zh-TW 输出和检测）。
- `README.zh-TW.md`、`docs/*.zh-TW.md`、CHANGELOG、tests、evals、audits、examples 等开发与文档文件。
- `academic-paper` 的默认摘要语言对仍是 `zh-tw-en`（上游没有 zh-CN 语言对）。
