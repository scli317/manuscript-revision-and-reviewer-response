# Verifying marked-manuscript page and line references

## View-dependent numbering

The line numbers in Word are a rendered property, not stable paragraph identifiers. Showing all revisions can add deleted text, expand lines or pages, and change the line numbers relative to “No Markup” / final content. In this user's workflow, use the view matching **all tracked revisions shown**, unless the user or journal explicitly indicates another view. A previous case produced page 10, line 182 and page 33, line 488 in all-markup view; the no-markup view showed different numbers. These are examples only, never fixed offsets.

1. Identify the exact latest marked DOCX, its timestamp and the user's requested Word/WPS view. If the file is being edited, account for unsaved changes: do not overwrite or rely on an older disk copy as if current.
2. Render or inspect the manuscript in the specified view with Word's actual page and line numbering. If using Word `ExportAsFixedFormat`, verify that the export includes tracked revisions: use the document-with-markup item and show revisions, not the default content-only export. Confirm the displayed page and anchor text or equation match the user-provided screenshot or a known reference. Tool enum values may differ; verify the resulting output, not just settings.
3. Map each response to the specific changed passage, not merely a related section heading. Identify the actual page and line, including equations or captions that fall between numbered text lines. Distinguish changes from background context; if a cited response says an explanation was added but it is absent, flag it rather than inventing a line.
4. Update references only. Preserve comments, reply prose, headings, paragraph and run formatting, and the user's edits. If the user supplied an example of the desired wording, follow it. Save separately if the original is open or overwrite risks user edits.
5. Reopen outputs; verify every updated reference against the same rendered view, and spot-check final layout. Document the view and source revision used. Recompute all affected references after a manuscript content or pagination change.

## PDF annotations

Use annotation contents rather than only visible text extraction. Verify the highlighted selection and match printed manuscript pagination separately from the PDF's one-based page number. Annotation numbers are working labels, not proof of reviewer numbering. When two comments target the same passage, retain both unless the user explicitly combines them.
