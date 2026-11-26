# Security Policy

This policy covers DEX MACHINA // WIN and applies in the same way to every module of the DEX MACHINA project.

DEX MACHINA is built to analyze applications that may be hostile by design. Every file it opens must be treated as untrusted input, which makes the security of the tool itself a priority. If you find a way to make DEX MACHINA work against the person using it, we want to hear about it.

## Supported versions

DEX MACHINA is under active development. Until version 1.0, only the latest release receives security fixes. Once 1.0 is published, this section will list the supported release lines.

## Reporting a vulnerability

Please do not report security vulnerabilities through public issues, pull requests or discussions.

The preferred channel is GitHub's private vulnerability reporting: open the Security tab of this repository and click "Report a vulnerability". Your report stays private between you and the maintainer until a fix is published. If you cannot use GitHub, write to security@dexmachina.dev.

A useful report describes the affected module and version, the type of vulnerability, and the steps needed to reproduce it. If the issue is triggered by a crafted file, please describe how it is built or attach a minimal proof of concept, rather than a real malicious application. Tell us what an attacker could achieve in practice, for instance code execution on the analyst's machine or files written outside the output directory.

## What to expect

DEX MACHINA is maintained by an independent developer, so timelines are best effort but taken seriously. You will receive an acknowledgment within 7 days, and a first assessment of the issue within 14 days. We will keep you informed while the fix is being prepared, and we will agree with you on a disclosure date.

We follow coordinated disclosure. We ask you to keep the vulnerability confidential until a fix is released, or for 90 days after your report, whichever comes first. If a fix needs more time, we will explain why and agree on a new date with you.

Once the fix is out, we publish a GitHub Security Advisory and request a CVE when the impact justifies it. Reporters are credited by name or handle in the advisory, unless they prefer to remain anonymous. DEX MACHINA does not run a paid bug bounty program.

## Scope

The following issues are in scope, and we especially welcome them:

- code execution, file write or file read on the analyst's machine triggered by an analyzed file
- path traversal and zip slip during the extraction of packages such as APK, XAPK, IPA, MSI or DEB
- XML external entity attacks and other parsing flaws in manifests, property lists or metadata
- decompression bombs and inputs causing uncontrolled resource consumption
- escape from the isolation used during dynamic analysis
- injection of scripts or active content into generated reports
- leaks of local data, credentials or analysis results outside the expected output

The following issues are out of scope:

- vulnerabilities found in third-party applications analyzed with DEX MACHINA, which must be reported to their own developers
- vulnerabilities in dependencies that cannot be triggered through DEX MACHINA, which should be reported upstream
- attacks that require the analyst to run DEX MACHINA with a deliberately modified configuration or with elevated privileges against the documentation
- social engineering, and attacks against the project's website or hosting providers that do not involve DEX MACHINA itself

## Safe harbor

We will not take legal action against anyone who researches and reports vulnerabilities in good faith and in line with this policy. Good faith means testing only on your own systems and with files you are allowed to use, avoiding any harm to users or third parties, and giving us a reasonable time to fix the issue before any public disclosure.

Thank you for helping keep DEX MACHINA and its users safe.
