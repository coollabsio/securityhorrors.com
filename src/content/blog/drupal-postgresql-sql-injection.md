---
title: "Drupal: The Postgres Backdoor Query"
description: "TLDR and affected version summary for CVE-2026-9082, a SQL injection vulnerability in Drupal affecting PostgreSQL deployments."
tags:
  - drupal
  - postgresql
  - sql-injection
  - cve
  - vulnerability
author: Andras Bacsai
authorTwitter: heyandras
date: "2026-05-22T00:00:00.000Z"
image: /assets/drupal-postgresql-sql-injection.webp
category: security
isNew: false
---

---

Source:

- [Drupal: SA-CORE-2026-004](https://www.drupal.org/sa-core-2026-004)

---

__tldr: CVE-2026-9082 is a SQL injection vulnerability in Drupal that affects sites running on PostgreSQL. MySQL and MariaDB deployments are not impacted. Patches are available across all supported Drupal branches.__

## Affected versions

Affects only PostgreSQL deployments — MySQL/MariaDB not impacted.

| Branch | Affected | Upgrade to |
| --- | --- | --- |
| 11.3.x | 11.3.x | 11.3.10 |
| 11.2.x | 11.2.x | 11.2.12 |
| 11.1.x–11.0.x | 11.1.x–11.0.x | 11.1.10 |
| 10.6.x | 10.6.x | 10.6.9 |
| 10.5.x | 10.5.x | 10.5.10 |
| ≤10.4.x | ≤10.4.x | 10.4.10 |

## What to do

- If you run Drupal on PostgreSQL, upgrade to the patched version for your branch immediately.
- If you run Drupal on MySQL or MariaDB, you are not affected — but upgrading is still good practice.
- Review the [Drupal security advisory](https://www.drupal.org/sa-core-2026-004) for full details and upgrade instructions.
