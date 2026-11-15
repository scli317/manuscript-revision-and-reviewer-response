# Manuscript Revision and Reviewer Response

[中文说明](README.zh-CN.md)

A Codex skill for preparing and checking journal revisions, point-by-point reviewer responses, and marked manuscripts with traceable page and line references.

## What it helps with

- Organize editorial decisions, reviewer reports, and comments in annotated PDFs.
- Draft respectful, evidence-based responses while preserving each reviewer's wording.
- Reconcile response letters with actual revisions in the marked manuscript.
- Verify page and line references in the specified Word revision view.
- Check requested clean and marked documents, figures, and submission files against the editor's instructions.
- Flag missing data, unsupported claims, and changes that cannot be verified.

## Installation

Clone this repository into your Codex skills directory:

```powershell
git clone https://github.com/scli317/manuscript-revision-and-reviewer-response.git "$env:USERPROFILE\.codex\skills\manuscript-revision-and-reviewer-response"
```

If a skill with that name already exists, back it up or update it rather than cloning over it. Restart Codex or refresh its skill list if the skill does not immediately appear.

## Usage

Invoke `$manuscript-revision-and-reviewer-response` and provide the editor's decision letter, reviewer comments, the original manuscript, the latest marked manuscript, and any relevant supporting data. For example:

> Use $manuscript-revision-and-reviewer-response to draft point-by-point replies and verify each page and line reference against the marked manuscript with all revisions displayed.

Supply only the files relevant to your task. The skill follows the journal's instructions and your requested scope; it does not treat unverified manuscript changes or data as completed work.

## Repository contents

- `SKILL.md` — skill instructions and workflow.
- `agents/openai.yaml` — display metadata for Codex.
- `references/response-templates.md` — reusable editor-letter and point-by-point response templates.
- `references/marked-line-numbering.md` — guidance for checking marked-manuscript locations and PDF annotations.

Page and line numbers depend on the final document, Word layout, and revision-display settings. Review references again after pagination or content changes.
