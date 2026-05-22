---
title: "GitHub: The Extension That Opened the Vault"
description: "TLDR and impact summary for the GitHub internal repository breach caused by a malicious VS Code extension installed by a GitHub developer."
tags:
  - github
  - vscode
  - supply-chain
  - breach
  - malware
  - extension
author: Andras Bacsai
authorTwitter: heyandras
date: "2026-05-20T00:08:00.000Z"
image: /assets/github-malicious-extension-repo-breach.jpg
category: security
isNew: false
---

---

Source:

- [GitHub: statement on the incident](https://x.com/github/status/2056884788179726685?s=46)

---

__tldr: A GitHub developer installed a malicious VS Code extension, giving attackers access to GitHub's internal infrastructure. Around 3,800 private repositories were accessed. GitHub says only internal repos are confirmed affected so far and will contact customers if external repos are found to be impacted. Investigation is ongoing.__

## What we know

- A malicious VS Code extension was installed by a GitHub developer.
- Attackers used the access to reach **~3,800 private repositories**.
- So far only GitHub's internal repositories are confirmed impacted.
- GitHub says they will contact customers if any external repositories are found to be affected.
- A detailed report will be published once the investigation is complete.

## What to do

- Watch for official communications from GitHub — verify any emails or messages about this incident before taking action, as phishing attempts are likely.
- Review access logs for any GitHub-hosted private repositories your organization owns.
- Rotate credentials and tokens associated with GitHub if you suspect your repos may be in scope.
- Monitor [GitHub's official channels](https://x.com/github) for updates as the investigation progresses.
