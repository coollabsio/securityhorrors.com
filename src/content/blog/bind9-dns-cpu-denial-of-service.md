---
title: "BIND 9: Three Cracks in the Resolver Wall"
description: "TLDR and affected version summary for three BIND 9 DNS resolver vulnerabilities causing denial of service via high CPU usage."
tags:
  - bind
  - dns
  - vulnerability
  - denial-of-service
author: Andras Bacsai
authorTwitter: heyandras
date: "2026-05-22T00:03:00.000Z"
image: /assets/bind9-dns-cpu-denial-of-service.webp
category: security
isNew: false
---

---

Source:

- [ISC: CVE-2026-1519](https://kb.isc.org/docs/cve-2026-1519)

---

__tldr: Three vulnerabilities were disclosed in BIND 9, the widely-used DNS resolver. Some of these can cause denial of service through high CPU consumption. Patches are available — upgrade immediately if you run BIND in production.__

## Affected versions

| Branch | Affected | Upgrade to |
| --- | --- | --- |
| 9.11.x–9.16.x | 9.11.0–9.16.50 | — |
| 9.18.x | 9.18.0–9.18.46 | 9.18.47 |
| 9.20.x | 9.20.0–9.20.20 | 9.20.21 |
| 9.21.x | 9.21.0–9.21.19 | 9.21.20 |

## What to do

- Upgrade BIND 9 to a patched version (`9.18.47`, `9.20.21`, or `9.21.20`) immediately.
- If you cannot patch right away, monitor DNS resolver CPU usage for abnormal spikes.
- Review the [ISC advisory](https://kb.isc.org/docs/cve-2026-1519) for full details on each CVE and any available workarounds.
