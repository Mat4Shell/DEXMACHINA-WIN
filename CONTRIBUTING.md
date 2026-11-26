# Contributing to DEX MACHINA

Thank you for considering a contribution to DEX MACHINA. This document explains how the project works, what we expect from contributions, and how to get your changes merged. It applies to every module of the project: DEX MACHINA // DROID, // IOS, // WIN and // NIX.

## Before you start

DEX MACHINA is dual-licensed under the AGPL-3.0-or-later and a commercial license (see `LICENSING.md`). To make this possible, every contributor must sign the DEX MACHINA Contributor License Agreement (`CLA.md`) before their first pull request can be merged. You keep the ownership of your code, and you only sign once for all DEX MACHINA repositories. When you open your first pull request, a bot will ask you to post a short comment to sign it.

For anything larger than a bug fix or a small improvement, please open an issue first to discuss what you have in mind. It saves everyone time, and it avoids you spending hours on a change that does not fit the direction of the project.

## Responsible use

DEX MACHINA is a security analysis tool. Contributions must serve the analysis, understanding and defense of applications. We do not accept features whose main purpose is to facilitate piracy, the redistribution of paid applications, the bypass of licensing mechanisms, or attacks against third parties.

## Malware samples and test files

Never commit real malware, cracked applications or proprietary applications to any repository of the project, not even in a test folder or an archive. Test fixtures must be applications you built yourself for that purpose, or files whose license explicitly allows redistribution. When a test needs a known malicious sample, reference it by its SHA-256 hash and by the public dataset where it can be obtained, and make the test skip cleanly when the sample is not available locally.

## Reporting bugs

Open an issue with the version of DEX MACHINA you use, your operating system, the exact command or action that triggered the problem, and the full output or error. If the bug depends on a specific application, share its package name and hash rather than the file itself.

## Reporting security vulnerabilities

Do not open a public issue for a vulnerability in DEX MACHINA itself. Follow the process described in `SECURITY.md` and use GitHub's private vulnerability reporting, or write to security@dexmachina.dev.

## Development setup

Setup instructions are specific to each module and live in the `README.md` of its repository.

## Making changes

Work on a dedicated branch created from `main`, and keep each pull request focused on a single topic. Commit messages follow the Conventional Commits format (`feat:`, `fix:`, `docs:`, `refactor:`, `test:`...), which keeps the history readable and lets us generate changelogs automatically. Signed commits are strongly encouraged.

Every new feature or bug fix should come with tests, and the existing test suite must pass before review. If your change affects how the tool is used, update the documentation in the same pull request.

## Pull request review

A maintainer will review your pull request as soon as possible. Expect questions and change requests: they are part of the process, not a rejection. Once the CLA is signed, the checks are green and the review is approved, your contribution will be merged and your name will remain in the project history.

## Code of conduct

Everyone taking part in the project is expected to follow the `CODE_OF_CONDUCT.md`. Be respectful, assume good faith, and keep discussions technical.

Thank you for helping make DEX MACHINA better.
