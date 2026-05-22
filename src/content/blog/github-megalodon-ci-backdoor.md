---
title: "Megalodon: 5,561 Repos Swallowed in Six Hours"
description: "TLDR and details on the Megalodon supply chain attack mass-backdooring GitHub repositories via malicious CI/CD workflow commits."
tags:
  - github
  - supply-chain
  - ci
  - malware
  - github-actions
author: Andras Bacsai
authorTwitter: heyandras
date: "2026-05-22T00:09:00.000Z"
image: /assets/github-megalodon-ci-backdoor.jpg
category: security
isNew: true
---

---

Source:

- [SafeDep: Megalodon — Mass GitHub Repo Backdooring CI Workflows](https://safedep.io/megalodon-mass-github-repo-backdooring-ci-workflows/)

---

__tldr: A supply chain attack dubbed "Megalodon" is targeting GitHub repositories by injecting malicious commits into CI/CD workflows. Around 5,561 repositories were hit in a 6-hour window using fake bot accounts to push poisoned GitHub Actions pipelines that auto-run on pull requests.__

## What is happening

- Fake bot accounts (`build-bot`, `ci-bot`, `pipeline-bot`) are committing malicious workflow files directly into repositories.
- The attack targets GitHub Actions and CI pipelines configured to auto-run on PRs.
- Around **5,561 repositories** were affected within a single 6-hour window.
- The malicious workflows execute attacker-controlled code in the context of the target repository's CI environment — potentially leaking secrets, tokens, and build artifacts.

## What to do

- Audit your repository's recent commits — especially anything touching `.github/workflows/` from unfamiliar bot accounts.
- Review collaborator and outside contributor access for any unexpected accounts.
- Require approval for workflow runs from first-time contributors (`pull_request_target` is particularly dangerous).
- Rotate any secrets or tokens that may have been exposed through CI runs triggered by the malicious commits.
- Review the [SafeDep writeup](https://safedep.io/megalodon-mass-github-repo-backdooring-ci-workflows/) for IOCs and detection guidance.
