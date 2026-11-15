# 论文修改与审稿意见回复

[English](README.md)

本 Codex 技能用于协助整理期刊返修材料、撰写逐点回复，并核对回复信与标记版手稿中的修改位置。

## 主要功能

- 整理编辑决定信、审稿意见和 PDF 中的批注。
- 保留审稿意见原文，撰写有依据、语气得体的逐点回复。
- 核对回复中声称的修改是否真实存在于标记版手稿中。
- 在指定的 Word 修订显示模式下核对页码和行号。
- 根据编辑要求检查 clean 版、marked 版、图件和其他提交材料。
- 提醒用户补充缺失数据，标出无法核实的结论或修改。

## 安装

将仓库克隆到 Codex 技能目录：

```powershell
git clone https://github.com/scli317/manuscript-revision-and-reviewer-response.git "$env:USERPROFILE\.codex\skills\manuscript-revision-and-reviewer-response"
```

如果同名技能已经存在，请先备份或更新已有目录，不要直接覆盖。若安装后技能未立即显示，可重启 Codex 或刷新技能列表。

## 使用方法

调用 `$manuscript-revision-and-reviewer-response`，并提供与任务有关的编辑决定信、审稿意见、原始手稿、最新标记版手稿和支撑数据。例如：

> 使用 $manuscript-revision-and-reviewer-response 撰写逐点回复，并根据显示所有修订的标记版手稿逐项核对页码和行号。

只需提供本次任务所需的文件。技能会遵循期刊编辑要求和用户指定的工作范围，不会将尚未核实的数据或修改当作已完成的工作。

## 文件说明

- `SKILL.md`：技能主文件及工作流程。
- `agents/openai.yaml`：Codex 中的显示信息。
- `references/response-templates.md`：编辑回信及逐点回复模板。
- `references/marked-line-numbering.md`：标记版手稿行号和 PDF 批注核对方法。

页码和行号受最终文件、Word 排版和修订显示模式影响；修改内容或页面发生变化后应重新核对。
