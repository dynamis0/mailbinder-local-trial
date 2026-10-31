# MailBinder Local 0.1.1 - Windows evaluation edition

Create one indexed PDF binder from a nested folder of EML emails. Processing stays on your PC.

## Downloads

- **MailBinder-Local-0.1.1-trial-win-x64.zip**: the Windows x64 trial. Extract the entire ZIP, read the quick start, and run `MailBinder.Local.Trial.exe`. Up to 25 messages per job, with an evaluation footer. No signup or card.
- **MailBinder-Sample-EML-0.1.1.zip**: 12 fictional input messages within the trial limit. Use these to test the workflow without confidential files.
- **MailBinder-Local-0.1.1-sample-package.zip**: a real generated 28-message output package with PDF, manifests, errors report, and original fictional inputs. This is an output example, not the 12-message trial input set.
- **SHA256SUMS.txt**: verify downloaded ZIPs against these SHA-256 checksums.

## Changes

- Report email with no readable body in both the errors report and manifest.
- Validate physical output paths so directory junctions cannot place generated output inside the source tree.
- Update the cryptography dependency to a patched version.
- Show the correct 25-message limit consistently in the evaluation UI.

## Scope to check before use

EML input only. One combined PDF, not one PDF per email. HTML bodies are converted to readable plain text, without preserving original HTML layout or inline-image placement. Supported PDF/JPG/PNG attachments can be appended. No mailbox login, PST/MSG/MBOX import, OCR, or authenticity/legal-admissibility certification.

Windows 10/11 x64. The build is currently unsigned; Windows may show an unknown-publisher warning. Use it only if your organization's software policy allows unsigned apps. Do not disable security protections. Review generated files and the errors report before relying on the output.

The product is proprietary. Source code and the paid build are not included in this repository. [Product details, sample PDF and purchase](https://dynamis-software.ms-sugar.chatgpt.site/mailbinder-local).
