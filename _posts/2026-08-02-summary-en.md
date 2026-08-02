---
layout: default
title: "Horizon Summary: 2026-08-02 (EN)"
date: 2026-08-02
lang: en
---

> From 29 items, 1 important content pieces were selected

---

1. [Bor: Open-Source Real-Time Policy Management for Linux Desktops](#item-1) ⭐️ 8.0/10

---

<a id="item-1"></a>
## [Bor: Open-Source Real-Time Policy Management for Linux Desktops](https://getbor.dev/blog/2026-08-02-bor-v080-release/) ⭐️ 8.0/10

Bor v0.8 was released, adding support for Thunderbird, Microsoft Edge for Business, and FirewallD zones. The system streams desktop policies to Linux clients in real time over mTLS/gRPC instead of using polling. It fills a long-standing gap in open-source Linux desktop management, giving sysadmins a centralized alternative to manual configuration or proprietary tools like Microsoft Intune. Real-time policy streaming could also reduce configuration drift on managed workstations. The architecture uses a lightweight Go agent and a central server, with new policy types in v0.8 for Thunderbird, Edge for Business, and FirewallD zones. Existing supported policies include Firefox, Chrome, KDE, dconf, polkit, and package management.

hackernews · eniac111 · Aug 2, 09:06 · [Discussion](https://news.ycombinator.com/item?id=49142569)

**Background**: Linux desktop management traditionally relies on manual scripting or per-machine configuration, with few centralized open-source options. dconf is the low-level configuration system used by GNOME, polkit is a system-wide authorization framework, and FirewallD provides dynamically managed firewall zones for network access control. By streaming policies over mTLS/gRPC, Bor aims to enforce settings continuously rather than at fixed intervals.

<details><summary>References</summary>
<ul>
<li><a href="https://en.wikipedia.org/wiki/Dconf">dconf - Wikipedia</a></li>
<li><a href="https://manpages.ubuntu.com/manpages/trusty/man8/polkit.8.html">Ubuntu Manpage: polkit - Authorization Framework</a></li>
<li><a href="https://firewalld.org/documentation/zone/">Documentation - Zone | firewalld</a></li>

</ul>
</details>

**Discussion**: Reactions were generally positive, with commenters asking about support for Cinnamon, custom script execution, and integration with identity providers like Authentik. Others questioned the choice of mTLS over SSH, the handling of configuration drift without polling, and how Bor compares to existing tools or System76's Cosmic Sync.

**Tags**: `#Linux`, `#Policy Management`, `#Open Source`, `#Desktop Management`, `#DevOps`

---