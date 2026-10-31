# MailBinder Local 0.1.3 - reviewed Windows evaluation edition

Turn an existing EML folder tree into one indexed PDF with bookmarks, optional attachment pages, source originals and processing reports. Runs locally on Windows 10/11 x64.

## Downloads

- `MailBinder-Local-0.1.3-trial-win-x64.zip`: up to 25 EML files per run, evaluation footer, evaluation-only license. Extract the entire ZIP before running `MailBinder.Local.Trial.exe`.
- `MailBinder-Sample-EML-0.1.2.zip`: the unchanged 12-message fictional input kit, also used for 0.1.3 checks. It is input data, not an app or a source-code release.
- `SHA256SUMS.txt`: SHA-256 checksums for these two ZIPs. Paid full build and source code are not distributed here.

## Changes

- Detect characters absent from the embedded PDF font. Affected email pages show a review note; errors.csv and manifest warnings include `text_glyph_missing`. Binder title/preparer/footer issues are reported at binder level. Source bytes are preserved where successfully snapshotted/extracted. This adds reporting, NOT universal Unicode, emoji or complex-script shaping support.
- Custom app/window icon; compact native language picker and Browse buttons.
- Fixed Generate/Cancel/Open PDF action bar, scrollable long notices and startup fit to the display work area.
- Retain the multipart body, skipped-link, attachment-path and manifest-warning corrections in 0.1.2. Version 0.1.1 remains withdrawn.

## Review and limits

76 Core/UI automated tests passed, plus 10 packaging guard tests. Codex and Claude independently cross-reviewed the release and frozen ZIPs. Final ZIPs were unpacked and run through actual Windows workflows: successful generation, trial limit, cancellation, source byte comparisons, trial footer and missing-glyph reporting.

These checks do not establish every input/machine configuration or actual OS 125%/150%/mixed-monitor rendering, and are not a zero-bug or security guarantee. Review output against sources. Development used substantial AI assistance; the app is not an AI service and does not upload message content.

EML files only; no MSG/PST/OST/MBOX, mailbox login/export, OCR, Office conversion, original HTML layout or legal/archival certification. Full build: up to 500 EML; trial: 25. Both: 1 GiB raw input, 100 MiB per EML/decoded attachment, 2,000 PDF pages, 1,000,000 UTF-16 rendered body characters per email. See the included README for image limits and complete scope.

This build is unsigned. SmartScreen or your organization's policy may block it. Do not disable protections to run it. Checksums confirm file consistency, not safety.

[Product details, real fictional sample output and optional purchase](https://dynamis-software.ms-sugar.chatgpt.site/mailbinder-local). Contact: work421398840@gmail.com; do not send confidential messages or attachments.
