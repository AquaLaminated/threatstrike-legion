# Security policy

## Reporting a vulnerability

If you believe you've found a security vulnerability in ThreatStrike Legion,
please report it privately to:

**security@threatstrike.ai**

PGP key available on request.

**Please don't** open a public GitHub issue for security reports. Public
disclosure before a fix is shipped puts other users at risk.

## What to include

- A description of the issue and its impact.
- Steps to reproduce.
- The affected version (visible in **Settings → About** inside the app).
- Your OS and version.
- Any logs, screenshots, or PoC code that helps.

## What to expect

- **Acknowledgement** within 72 hours.
- **Triage** (severity assessment + tentative fix timeline) within 7 days.
- **Fix** shipped in a point release with a credit to you in the release
  notes, unless you'd prefer to stay anonymous.

## Scope

In scope:
- The shipped ThreatStrike Legion binary (current and one previous version).

Out of scope:
- Third-party tools the app invokes (`nmap`, `ffuf`, `hydra`, etc.) - report
  those upstream.
- Third-party AI providers (Anthropic, OpenAI, Google) - report to them.
- Issues that require an attacker to already have local root on the user's
  machine.

## Bounty

No formal bounty program yet. For high-impact reports we may offer a free
license or store credit. We'll be straight with you about what we can offer.
