---
title: "Chromium: The Tab That Never Really Closed"
description: "TLDR and details on a Chromium vulnerability allowing attackers to run JavaScript in the background even after the browser is closed."
tags:
  - chrome
  - chromium
  - vulnerability
  - javascript
author: Andras Bacsai
authorTwitter: heyandras
date: "2026-05-22T00:06:00.000Z"
image: /assets/chromium-background-js-after-close.webp
category: security
isNew: false
---

---

Source:

- [BleepingComputer: Google accidentally exposed details of unfixed Chromium flaw](https://www.bleepingcomputer.com/news/security/google-accidentally-exposed-details-of-unfixed-chromium-flaw/)

---

__tldr: A vulnerability in Chromium-based browsers allows attackers to run JavaScript in the background even after the browser is closed — just by visiting a specially crafted website. Reported to Google in late 2022, patched in January 2026, but researchers found in May 2026 that the fix is still incomplete.__

## Timeline

- **Late 2022:** Researcher privately reports the bug to Google.
- **January 2026:** Google patches the vulnerability.
- **May 2026:** Google publishes the bug report and public PoC.
- **May 2026:** Researchers discover the vulnerability is still not fully patched.

## Affected versions

- **Affected:** Chromium-based browser versions since 2022.
- **Status:** As of writing, the vulnerability is still not fully patched.

## What to do

- Be aware that closing your browser may not fully terminate all page-originated scripts.
- Monitor for Chromium/Chrome updates addressing this specific background execution flaw.
- Review the [BleepingComputer writeup](https://www.bleepingcomputer.com/news/security/google-accidentally-exposed-details-of-unfixed-chromium-flaw/) for full technical details and PoC information.
