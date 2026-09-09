<p align="center">
  <img src="assets/hero.svg" alt="Kcoof Toolkit — Recon to report, one pipeline" width="780">
</p>

<h3 align="center">Cybersecurity Engineer · CEH · M.Tech<br>Offensive Security &amp; AI Automation — Saudi Arabia</h3>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Kcoof&label=profile+views&color=22c55e&style=flat-square" alt="profile views">
  <a href="https://github.com/Kcoof?tab=repositories"><img src="https://img.shields.io/badge/repos-security--tooling-22C55E?style=flat-square&labelColor=0F172A" alt="security tooling"></a>
  <img src="https://img.shields.io/badge/CEH-certified-22C55E?style=flat-square&labelColor=0F172A" alt="CEH">
  <img src="https://img.shields.io/badge/M.Tech-degree-475569?style=flat-square&labelColor=0F172A" alt="M.Tech">
  <img src="https://img.shields.io/badge/focus-web%20security%20·%20bug%20bounty%20·%20AI%20automation-94A3B8?style=flat-square&labelColor=0F172A" alt="focus">
</p>

---

## 🛡️ The Bug Bounty Toolkit

An end-to-end recon → scan → report pipeline. Four stages, one command each:

| Stage | Tool | What it does | Command |
|:-:|:-|:-|:-|
| **01 — RECON** | [**SUBenum**](https://github.com/Kcoof/SUBenum) | 5 passive sources, DNS bruteforce with wildcard detection, alive-host probing | `subenum -d target.com -probe` |
| **02 — FILTER** | [**xss**](https://github.com/Kcoof/Xss) | Mass reflection pre-filter across huge URL lists at machine speed | `xss -l urls.txt -o hits.txt` |
| **03 — SCAN** | [**secscan**](https://github.com/Kcoof/security-scanner) | Context-aware XSS, 3-mode SQLi, CORS, CRLF, open redirect, blind OOB via Interactsh | `secscan subs-alive.txt --oob` |
| **04 — REPORT** | findings | HTML dashboard + HackerOne-ready Markdown with CWE and remediation | `start dashboard.html` |

**Also in the kit:** [wordlist](https://github.com/Kcoof/wordlist) — 1M+ curated entries (subdomains, parameters, paths) wired in via `-w` and `--params-file` · [SentinelDork](https://github.com/Kcoof/sentineldork) — AI-assisted dorking recon with a serverless-secured GLM proxy.

<details>
<summary><b>📊 secscan detection coverage</b></summary>

| Check | Severity | CWE |
|---|---|---|
| Reflected XSS (context-aware: body / attribute / JS / comment) | High | CWE-79 |
| SQLi — error-based (MySQL, PostgreSQL, MSSQL, Oracle, SQLite) | Critical | CWE-89 |
| SQLi — boolean-based blind (response diffing) | Critical | CWE-89 |
| SQLi — time-based blind (real latency measurement) | Critical | CWE-89 |
| DOM XSS via headless Chromium (`--dom`) | High | CWE-79 |
| Open redirect (Location header + client-side) | Medium | CWE-601 |
| CORS misconfiguration (Origin reflection, null, subdomain tricks) | Med–High | CWE-942 |
| CRLF injection (params + path) | Medium | CWE-93 |
| Host header / X-Forwarded-Host injection | Medium | CWE-644 |
| Clickjacking, cookie flags, security headers | Low–Med | CWE-1021/1004/693 |
| Out-of-band callbacks — blind SSRF/SQLi/XSS via Interactsh | High | CWE-918 |

</details>

---

## 🔐 What I Do

- **Offensive security** — web app pentesting, OWASP Top 10, SQLi/XSS, auth & business-logic flaws, API security
- **Security tooling** — Python & Go: scanners, recon automation, pipeline integrations
- **AI automation** — LLM-assisted analysis, vision extraction, agent architecture for security workflows

Currently targeting senior cybersecurity roles in KSA while building next-generation tooling under **SamTechnology**.

---

## 🎓 Certifications & Learning

- 🛡️ Certified Ethical Hacker (CEH)
- 🎓 Master of Technology (M.Tech)
- 📚 Preparing: CISSP · ISO 27001 · CISM

---

## 📊 GitHub

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Kcoof&show_icons=true&hide_border=true&bg_color=0F172A&title_color=22C55E&icon_color=22C55E&text_color=F8FAFC" alt="Kcoof's GitHub stats" height="165">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Kcoof&layout=compact&hide_border=true&bg_color=0F172A&title_color=22C55E&text_color=F8FAFC&langs_count=8" alt="top languages" height="165">
</p>

---

## 🌍 Vision

Cybersecurity is evolving beyond manual testing — the future belongs to AI-augmented pentesting, intelligent vulnerability reasoning, and continuous adaptive security.

**My mission: engineer systems that think like attackers — but operate at machine speed.**

> ⚠️ All tooling is for **authorized security testing only** — programs you're registered with, or targets with written permission. Scope enforcement and rate limiting are built in; respecting each program's policy is on you.
