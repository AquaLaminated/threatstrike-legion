# ThreatStrike Legion

**Pentest tools that don't live in a terminal.**

![ThreatStrike Legion - engagement overview](./gallery/01-overview.png)

Every tool you'd reach for on a Kali box, sitting in a real window with every
tool now able to be ran in a GUI. `nmap`, `ffuf`, `metasploit`, `trufflehog`,
`CloudFox`, `impacket`, `volatility3`, and 79 more (86 total: 69 offensive,
17 defensive). Run them by hand the way you always have, or hand an objective
to the built-in AI agent and let it drive. Same binaries either way. Same
flags. Same output. Just no terminal.

> 🌐 **Website:** https://www.threatstrike.ai
> 💳 **Get the app:** https://www.threatstrike.ai/pricing.html
> 📧 **Contact:** security@threatstrike.ai

---

## What it is

ThreatStrike Legion is a commercial desktop pentest workstation for **macOS**
and **Linux**. One download, runs entirely on your machine, no cloud, no
telemetry, no SaaS dashboard. The engagement data lives on your laptop and
nowhere else.

## What's in it

- **A GUI for the Kali toolset.** 86 tools across 15 categories ([full list](./TOOLS.md), 69 offensive, 17 defensive),
  each one a real form with the real flags exposed. Bundled wordlists,
  interface dropdowns, file pickers, the works.
- **An optional AI agent.** Type the objective in plain English; the agent
  drives the same forms autonomously, with interactive chat so you can ask
  follow-up questions about any output. Switch models on the fly from the
  agent, chat, and tool-output panels.
- **An engagement knowledge graph.** Every host, service, credential, vuln,
  web path, and screenshot lives in one typed SQLite tree. Severity colors,
  click-to-reveal vault, embedded evidence.
- **A credential vault.** Every secret is stored in a local file
  (`~/.strikedeck/license.json`, owner-only permissions). The credential-aware
  tool forms get a one-click vault picker. No more `creds.txt` on the desktop.
- **A report builder.** AI drafts the exec summary + per-vuln remediation +
  conclusion. Renders a polished HTML page or PDF (via WeasyPrint) with your
  screenshots embedded and credentials redacted.
- **Red team and blue team.** One toggle in the header flips the entire UI.
  Blue side ships defensive tools (Volatility3, YARA, Sigma, Chainsaw,
  Suricata, Zircolite, capa, floss) and an Analyst agent tuned for DFIR,
  hunting, and detection engineering.
- **Cloud attack surface.** A new Cloud category ships CloudFox, Prowler, and
  ScoutSuite for AWS / Azure / GCP enumeration and misconfiguration auditing.
- **Bring your own AI.** Claude (CLI subscription or API key), OpenAI,
  Gemini, or any local OpenAI-compatible endpoint (Ollama, LM Studio,
  vLLM, llama.cpp).
- **Bring your own MCP servers.** Paste a Burp, BloodHound, or custom
  MCP server config into Settings; the agent can call it next session.

## Get it

- **Download free (3-day trial):** [www.threatstrike.ai/pricing.html](https://www.threatstrike.ai/pricing.html), or grab the [latest release](https://github.com/AquaLaminated/threatstrike-legion/releases/latest) directly (macOS Apple Silicon + Intel, Linux `.deb` / `.AppImage` / `.rpm`).
- **Buy a license:** All plans are annual. Pay by card (Visa, Mastercard, Amex, Apple Pay, Google Pay) or crypto (BTC, XMR, LTC, ETH). Your key is emailed instantly.
  - **Personal** -- $99.99/year -- non-commercial use, up to 3 devices
  - **Consultant** -- $499.99/year -- paid client engagements, up to 3 devices
  - **Team** -- $1,999/year -- paid client engagements, up to 10 devices
- No accounts, no telemetry. The engagement data never leaves your machine.

## Requirements

- macOS 12 or later (Apple Silicon or Intel), or Debian 13 / Ubuntu 22+ / Kali.
- For the AI features: a Claude subscription (via Claude Code CLI) **or** an
  Anthropic / OpenAI / Gemini API key **or** any local OpenAI-compatible
  endpoint. Pick one in Settings.
- For PDF reports: WeasyPrint (one-click install from the in-app Setup tab).
- The Kali toolset itself can be installed in one click from the in-app Tool
  Status page; nothing extra to set up manually.

## Status

v0.6.1 is live. macOS and Linux installers are on the [releases page](https://github.com/AquaLaminated/threatstrike-legion/releases/latest), and the in-app updater ships new versions from there automatically.

## Reporting bugs / requesting features

Use the **Issues** tab on this repository.

For security vulnerabilities please follow [SECURITY.md](./SECURITY.md) - don't
open a public issue.

## Source code

This is the public landing repository. **The source code is not distributed.**
ThreatStrike Legion is closed-source commercial software; the binary is sold
under the terms in [LICENSE](./LICENSE) and the full EULA in [EULA.md](./EULA.md).

## Dual-use notice

ThreatStrike Legion is a computer security testing tool. **You are solely
responsible for the lawful use of this software.** By using it you represent
that you will only assess systems and networks you own or have explicit
written authorization to test. Unauthorized use may violate computer-fraud,
anti-hacking, wiretap, and export laws in many jurisdictions.

---

© 2026 ThreatStrike LLC. All rights reserved.
