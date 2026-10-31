# MailBinder Local 0.1.2 - reviewed Windows evaluation edition

Create one indexed PDF binder from a nested folder of EML emails. Processing stays on your PC. This release replaces the withdrawn 0.1.1 build.

## Downloads

- `MailBinder-Local-0.1.2-trial-win-x64.zip`: Windows x64 evaluation build; up to 25 EML files per job, evaluation footer, evaluation-only license. Extract all files before running `MailBinder.Local.Trial.exe`.
- `MailBinder-Sample-EML-0.1.2.zip`: 12 fictional input messages within the trial limit.
- `MailBinder-Local-0.1.2-sample-package.zip`: real 28-message output, including deliberately malformed cases. It contains 50 PDF pages, manifests and explicit processing issues. It is an output example, not the 12-message trial input set.
- `SHA256SUMS.txt`: checksums of these public ZIPs. The paid full build and source code are not distributed here.

## Correctness fixes

- Preserve multiple readable MIME body fragments instead of silently dropping later fragments; report the combination.
- Fall back to substantive HTML when the plain-text alternative is empty.
- Do not follow filesystem reparse points; explicitly record paths skipped during a job.
- Keep manifest warnings consistent with body truncation and rendering failures.
- Prevent a message attachment from colliding with a nested message's attachment directory; report isolated copy failures.
- Explain when uncertain network aliases cannot be safely validated.

43 automated tests passed. The changes received independent cross-review, and final full/trial binaries were exercised through the Windows GUI using the original regression inputs. That is not a guarantee of zero bugs or security certification. Review the PDF, manifest and errors report before relying on output.

## Boundaries

Windows 10/11 x64. EML input only: no MSG/PST/MBOX, mailbox login or mailbox export. One combined PDF, not one PDF per message. HTML becomes readable plain text; original layout and inline-image placement are not preserved. PDF/JPG/PNG attachments can be appended. The full build allows 500 messages per run; both builds have a 1 GiB raw-input and 2,000-page batch limit, plus documented item/rendering limits.

The build is unsigned. SmartScreen or organizational security policy may prevent it from running. Do not disable security protections. Check software policy before downloading or buying. Checksums verify download consistency, not safety. Complex hostile PDFs can still consume substantial resources; do not treat the tool as an evidence-certification or malware-analysis system.

[Product details, real samples and current availability](https://dynamis-software.ms-sugar.chatgpt.site/mailbinder-local).
