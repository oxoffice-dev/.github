# Security policy

## Reporting a vulnerability

Please report security issues privately through GitHub's
[private vulnerability reporting](https://docs.github.com/en/code-security/security-advisories/guidance-on-reporting-and-writing-information-about-vulnerabilities/privately-reporting-a-security-vulnerability)
on the affected repository (Security tab, "Report a vulnerability"). Do not open a public issue.

We answer within a few days and publish an advisory with the fix.

## Supported versions

Only the latest release is supported. oxoffice is in 0.x, so fixes land in a new release rather than in
backports.

## Verifying a release

Every release carries `SHA256SUMS` and a signed build provenance. Check any downloaded file with:

```bash
sha256sum -c SHA256SUMS --ignore-missing
gh attestation verify <file> --repo oxoffice-dev/oxoffice
```
