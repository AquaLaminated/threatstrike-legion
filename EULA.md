# ThreatStrike Legion - End User License Agreement

**Effective date:** 2026-05-26
**Licensor:** ThreatStrike ("Licensor")
**Software:** ThreatStrike Legion and any updates, patches, documentation, and
related materials ("Software")

PLEASE READ THIS AGREEMENT CAREFULLY. BY DOWNLOADING, INSTALLING, OR USING
THE SOFTWARE YOU AGREE TO BE BOUND BY THIS AGREEMENT. IF YOU DO NOT AGREE,
DO NOT INSTALL OR USE THE SOFTWARE.

## 1. Grant of License

Subject to your compliance with this Agreement and payment of any applicable
fees, Licensor grants you a limited, non-exclusive, non-transferable,
non-sublicensable, revocable license to install and use one (1) copy of the
Software on devices you personally own and control, solely for your own
internal use, for the term you have paid for (perpetual unless otherwise
specified at the time of purchase).

## 2. Restrictions

You will not, and will not permit any third party to:

(a) copy, distribute, sublicense, sell, rent, lease, or otherwise transfer
    the Software or any access to it;
(b) modify, translate, adapt, or create derivative works of the Software;
(c) reverse engineer, decompile, disassemble, or attempt to derive the
    source code of the Software, except (and only to the extent) such
    restriction is expressly prohibited by applicable law;
(d) remove, obscure, or alter any proprietary or attribution notices in the
    Software;
(e) use the Software, in whole or in part, to build or improve a competing
    product or service;
(f) use the Software to perform any activity that violates any applicable
    law, regulation, or third-party right, including without limitation
    unauthorized access to any computer system, network, account, or device.

## 3. Authorized use; your representations

The Software is a dual-use computer security testing tool. You represent
and warrant, on each occasion you use the Software, that:

(a) you will only use the Software to assess computer systems and networks
    that you own or for which you have obtained explicit prior written
    authorization to test;
(b) you are solely responsible for ensuring your use complies with all
    applicable laws, including without limitation the U.S. Computer Fraud
    and Abuse Act (18 U.S.C. § 1030), the Wiretap Act, the Stored
    Communications Act, the U.K. Computer Misuse Act 1990, the EU NIS2
    Directive, and any other laws of any jurisdiction in which you or your
    target operates;
(c) you are at least 18 years old (or the age of majority where you live)
    and have the legal capacity to enter into this Agreement.

Some categories of tooling bundled with or invoked by the Software carry
additional category-specific legal risk that you acknowledge and accept
by using them:

(i)   **Wireless capture tools** (for example, aircrack-ng, airodump-ng,
      hcxdumptool, wifite, bettercap, bluetoothctl) can intercept wireless
      transmissions you are not a party to. In many jurisdictions this
      engages wiretap or interception statutes (in the United States,
      18 U.S.C. § 2511) regardless of whether the captured traffic is
      encrypted. Use these tools only on networks you own or are
      explicitly authorized to test.
(ii)  **Digital-forensics tools** (for example, volatility3, sleuthkit,
      plaso, chainsaw, hayabusa) may operate on data that, if later
      introduced in legal proceedings, must satisfy chain-of-custody,
      integrity, and admissibility requirements. Licensor makes no
      representation that the Software's handling of artifacts satisfies
      any such requirements; you are responsible for your forensic
      process and documentation.
(iii) **Exploitation frameworks and offensive payloads** (for example,
      metasploit, impacket, evil-winrm, sqlmap) may be subject to export
      controls under U.S. or other regulations. See §11 (Export Controls).

## 4. Ownership

The Software is licensed, not sold. Licensor and its licensors retain all
right, title, and interest in and to the Software, including all
intellectual property rights. Nothing in this Agreement grants you any
ownership rights in the Software.

## 5. Third-party components

The Software may include or depend on third-party open-source software
("Third-Party Components"), and may invoke third-party command-line
tools that you install separately, including but not limited to: network
scanners (for example nmap, masscan, rustscan); web reconnaissance and
fuzzers (for example ffuf, gobuster, nuclei, wpscan, sqlmap); authentication
and password tools (for example hydra, hashcat, john, crackmapexec,
evil-winrm, impacket, smbmap, smbclient); wireless capture tools (for
example aircrack-ng, airodump-ng, hcxdumptool, wifite, bettercap,
bluetoothctl); digital-forensics and incident-response tools (for example
volatility3, sleuthkit, plaso, chainsaw, hayabusa); network defense and
analysis tools (for example suricata, zeek, tshark); and malware-analysis
tools (for example clamscan, yara, capa, floss, ssdeep, exiftool); and
many others installed at your direction.

Use of Third-Party Components is governed by the terms of their respective
licenses, which are available with each tool or upon request. You are
solely responsible for installing, configuring, and using each tool in
compliance with its license and with all applicable laws. Licensor is not
responsible for the operation, output, or terms of any third-party tool
invoked by the Software, including any tool installed via the Software's
in-app installer.

## 6. AI services and data egress

The Software supports four AI engine modes, selected by you in Settings.
The choice you make determines what data leaves your device:

- **Claude** (via the Claude Code CLI or an Anthropic API key) - governed
  by Anthropic's Usage Policy
  (https://www.anthropic.com/legal/aup) and Consumer / Commercial Terms
  (https://www.anthropic.com/legal).
- **OpenAI / ChatGPT** (via an OpenAI API key) - governed by OpenAI's
  Terms of Use (https://openai.com/policies/terms-of-use/) and Usage
  Policies (https://openai.com/policies/usage-policies/).
- **Google Gemini** (via a Google AI Studio API key, using Google's
  OpenAI-compatible endpoint) - governed by Google's Generative AI Terms
  (https://policies.google.com/terms/generative-ai) and the Gemini API
  Additional Terms (https://ai.google.dev/gemini-api/terms).
- **Local LLM** (via any OpenAI-compatible endpoint you point the
  Software at, including Ollama, LM Studio, vLLM, or llama.cpp) -
  governed by the terms of whichever software and model you have
  installed locally (for example, https://ollama.com/legal/terms). When
  using a local model, no data leaves your device through the Software.

WHEN YOU SELECT A CLOUD AI ENGINE (Claude API, Claude CLI, OpenAI, or
Gemini), the Software transmits your engagement context to that provider
on each request. This may include: target hostnames, IP addresses,
service banners, command output, tool findings, and the text of any
prompt you send. Credentials stored in the OS keychain are not sent to
AI providers automatically, but their plaintext may appear in command
output that is sent. If your engagement scope or contract prohibits
sending engagement data to a third-party processor, choose the Local
LLM engine.

AI output is non-deterministic and may be incomplete, incorrect, or
fabricated ("hallucinated"). The Software's AI agent may misclassify
findings, miss vulnerabilities, suggest commands that fail or have
unintended effects, or generate report text that is factually wrong. You
must independently verify any AI-generated finding, command, or report
section before relying on it for any compliance, remediation,
notification, legal, or contractual purpose. Licensor disclaims all
responsibility for AI output content and for any third-party AI
service's availability, accuracy, latency, cost, billing, terms, or
data-handling practices. You are responsible for any fees a third-party
AI provider charges.

## 7. Warranty disclaimer

THE SOFTWARE IS PROVIDED "AS IS" AND "AS AVAILABLE," WITH ALL FAULTS,
AND WITHOUT WARRANTY OF ANY KIND. LICENSOR DISCLAIMS ALL WARRANTIES,
WHETHER EXPRESS, IMPLIED, OR STATUTORY, INCLUDING WITHOUT LIMITATION ANY
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, TITLE,
NON-INFRINGEMENT, ACCURACY, OR QUIET ENJOYMENT, AND ANY WARRANTIES
ARISING FROM COURSE OF DEALING, USAGE, OR TRADE PRACTICE. NO ADVICE OR
INFORMATION OBTAINED FROM LICENSOR OR THROUGH THE SOFTWARE WILL CREATE
ANY WARRANTY NOT EXPRESSLY STATED IN THIS AGREEMENT.

## 8. Limitation of liability

TO THE MAXIMUM EXTENT PERMITTED BY APPLICABLE LAW, IN NO EVENT WILL
LICENSOR BE LIABLE FOR ANY INDIRECT, INCIDENTAL, SPECIAL, CONSEQUENTIAL,
EXEMPLARY, OR PUNITIVE DAMAGES, INCLUDING WITHOUT LIMITATION LOST
PROFITS, LOST REVENUE, LOST DATA, BUSINESS INTERRUPTION, OR LOSS OF
GOODWILL, ARISING OUT OF OR RELATED TO THIS AGREEMENT OR YOUR USE OF (OR
INABILITY TO USE) THE SOFTWARE, WHETHER IN CONTRACT, TORT (INCLUDING
NEGLIGENCE), OR ANY OTHER LEGAL THEORY, AND EVEN IF LICENSOR HAS BEEN
ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.

LICENSOR'S TOTAL CUMULATIVE LIABILITY UNDER THIS AGREEMENT WILL NOT
EXCEED THE GREATER OF (A) THE TOTAL AMOUNT YOU PAID FOR THE SOFTWARE IN
THE TWELVE (12) MONTHS PRECEDING THE EVENT GIVING RISE TO LIABILITY, OR
(B) FIFTY U.S. DOLLARS (US $50).

Some jurisdictions do not allow the exclusion or limitation of certain
damages, so portions of this section may not apply to you.

## 9. Indemnification

You will defend, indemnify, and hold harmless Licensor and its
affiliates, officers, employees, and agents from and against any
third-party claim, demand, suit, or proceeding, and all related damages,
settlements, costs, and reasonable attorneys' fees, arising out of or
related to: (a) your use or misuse of the Software; (b) your violation
of this Agreement; or (c) your violation of any law or any right of any
third party in connection with your use of the Software.

## 10. Term and termination

This Agreement is effective on the date you first install or use the
Software and continues until terminated. Your rights under this
Agreement will terminate automatically and without notice if you
materially breach any of its terms. Upon termination, you must
immediately cease all use of the Software and destroy or delete all
copies in your possession or control. Sections 2, 4, 7, 8, 9, 11, and
12–14 survive termination.

## 11. Export controls and sanctions

The Software may be subject to United States export controls and trade
sanctions. You will comply with all applicable export and re-export
restrictions, including those of the U.S. Export Administration
Regulations (EAR) and the U.S. Office of Foreign Assets Control (OFAC).
You may not use, export, or re-export the Software to (or for use by) any
person, entity, or country that is subject to a U.S. or U.N. embargo,
sanctions list, or denied-party designation.

## 12. Governing law and venue

This Agreement is governed by the laws of the United States and the
state of the Licensor's primary residence, without regard to its
conflict-of-laws principles. The exclusive venue for any dispute arising
out of or relating to this Agreement will be the state or federal courts
located in that jurisdiction, and you consent to the personal
jurisdiction of those courts. The U.N. Convention on Contracts for the
International Sale of Goods does not apply.

## 13. Entire agreement; updates

This Agreement, together with any order form or invoice referencing it,
constitutes the entire agreement between you and Licensor regarding the
Software and supersedes all prior or contemporaneous agreements,
proposals, or representations, whether oral or written. Licensor may
update this Agreement from time to time by posting a revised version at
https://www.threatstrike.ai/eula.html; the revised Agreement will
apply to any new version of the Software you install or use after the
update.

## 14. Severability; assignment

If any provision of this Agreement is held to be unenforceable, that
provision will be modified only to the extent necessary to make it
enforceable, and the remaining provisions will continue in full force
and effect. You may not assign or transfer this Agreement or any rights
under it without Licensor's prior written consent. Licensor may freely
assign this Agreement.

## 15. Contact

Questions about this Agreement may be sent to: **security@threatstrike.ai**
