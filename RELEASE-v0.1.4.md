# MailBinder Local 0.1.4 - Windows evaluation edition

Turn an existing EML folder tree into one indexed PDF with bookmarks, optional attachment pages, copies of source EML files and processing reports. Runs locally on Windows 10/11 x64.

## Reporting correction

When attachment appending is enabled, an unsupported attachment now adds an `unsupported_for_binder` review warning to `errors.csv` and the GUI issue count. It is still extracted and listed in the manifest; the warning means it did not become a PDF page, not that the file was lost. Intentionally disabling appending remains `append_disabled`, not an issue.

In 0.1.3, this warning was visible in the manifest and the parent email's PDF review notes but could be omitted from `errors.csv` and the issue count. Check those records when reviewing older output. Older trial releases remain withdrawn as drafts with their files retained.

## Downloads

- `MailBinder-Local-0.1.4-trial-win-x64.zip`: up to 25 EML per run, evaluation footer, evaluation-only license. Extract the entire ZIP before running `MailBinder.Local.Trial.exe`.
- `MailBinder-Sample-EML-0.1.2.zip`: unchanged 12-message fictional input kit, also used in 0.1.4 tests. Input data only, not an application or source-code release.
- `SHA256SUMS.txt`: checksums for the two ZIPs. No paid full build, source code or private review metadata is distributed here.

## Checks and limits

79 Core/UI automated tests and 13 negative packaging guards passed. Codex and Claude cross-reviewed the exact ZIPs. Unpacked full/trial executables were run through supported/unsupported attachment jobs, deliberate append-off behavior, trial limit, cancellation and localized interface checks. Source-file and extracted-attachment bytes were compared; trial footers were checked on all sample pages.

These bounded checks are not a zero-bug or security guarantee. Actual OS high-DPI/mixed-monitor behavior, clean-machine installation and PDF-reader launch were not retested in this pass. Development used substantial AI assistance; the app itself is not an AI service and does not upload message content.

EML only; no MSG/PST/OST/MBOX, mailbox login/export, OCR, Office conversion, original HTML layout or legal/archival certification. Full edition: up to 500 EML; evaluation: 25. Both: 1 GiB raw input, 100 MiB per EML/decoded attachment, 2,000 pages, and 1,000,000 UTF-16 rendered body characters per email. Image and font/script limitations remain documented in the included README. Not every Unicode character or writing system is supported.

Unsigned Windows build: SmartScreen or organizational policy may block it. Do not disable security protections to run it. Checksums confirm file consistency, not safety certification. Review output against sources.

The full 0.1.4 build is available through the official website as an optional one-time purchase for JPY 980. This release provides the evaluation edition only; its download does not unlock or include the full build. [Product scope, purchase terms and contact](https://dynamis-software.ms-sugar.chatgpt.site/mailbinder-local). Contact: work421398840@gmail.com; do not send confidential messages or attachments.
