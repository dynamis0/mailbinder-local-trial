# MailBinder Local for Windows

Turn a folder of exported `.eml` email files into one indexed PDF binder, with nested bookmarks, attachment pages, original messages, and a processing report.

[Product, sample output, and purchase](https://dynamis-software.ms-sugar.chatgpt.site/mailbinder-local)

## Try it with your own files

The Windows x64 evaluation edition processes up to **25 EML files per run** and adds an evaluation notice to binder pages. It is licensed for evaluation only, not production or third-party service work. No account, payment card, mailbox access, or internet connection is needed to process files.

Download the ZIP from [Releases](https://github.com/dynamis0/mailbinder-local-trial/releases), extract all files to a new folder, then run `MailBinder.Local.Trial.exe`. Read the included quick-start instructions and check the SHA-256 download checksum in the release.

**Compatibility:** Windows 10/11 x64. The app is currently unsigned; SmartScreen or your organization's security policy may block it from running. Do not disable security protections. Evaluate it only where your software policy allows unsigned applications. A checksum confirms that your file matches the published download; it is not a security certification.

## What the app creates

- One continuous `Binder.pdf` with an index, folder bookmarks, message headers, and page numbers.
- Optional appended PDF/JPG/PNG attachment pages.
- Extracted attachments and a ZIP of original EML files.
- CSV and JSON manifests with source paths, SHA-256 hashes, statuses, and page ranges.
- An explicit errors report for failed or unsupported content.

## Know the limits before purchase

- **EML files only.** No PST, MSG, OST, MBOX, Outlook/Gmail sign-in, or mailbox export.
- The result is **one binder**, not a separate PDF for each email.
- HTML bodies are converted to readable plain text. Original HTML layout and inline-image placement are not preserved.
- Office, encrypted, and other unsupported attachments are not converted into PDF pages.
- The paid build supports up to 500 EML files per run, subject to file-size and 2,000-page safety limits.
- SHA-256 values help compare files; they do not certify authenticity or legal admissibility.
- English, Japanese, and Simplified Chinese interface.

## Samples and support

The product page links to a real generated sample binder and manifest. The sample uses fictional people, organizations, and `.invalid` addresses, including deliberate malformed-input test cases.

For compatibility or purchase questions: [happy421398840@gmail.com](mailto:happy421398840@gmail.com). Describe the file format and visible error first; do not send private email archives or credentials.

This repository distributes product information and the evaluation edition only. MailBinder Local is proprietary software; no source-code license is granted. The paid build and source code are not included.
