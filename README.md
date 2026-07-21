# CTF & Wargame Write-Ups

Hands-on write-ups from [OverTheWire: Bandit](https://overthewire.org/wargames/bandit/) and [picoCTF](https://picoctf.org/), documenting my approach to Linux fundamentals, privilege escalation, web exploitation, and forensics challenges as part of my cybersecurity training.

> **Note:** Flags are redacted throughout. These write-ups focus on methodology, tools, and reasoning — not answers — in line with each platform's community guidelines.

## About Me

I'm working toward a SOC Analyst / IT Security role with a blue-team focus, currently pursuing CompTIA Security+. This repo is part of a broader portfolio that includes [Sigma detection rules, incident response reports, and threat-hunt write-ups](#) *(link your other portfolio repo here)*.

## Skills Demonstrated

| Area | Challenges |
|---|---|
| Linux fundamentals & file system navigation | Bandit 0–15 |
| Privilege escalation techniques | Bandit 15+ |
| SUID/permissions exploitation | Bandit (various) |
| Cryptography & encoding | picoCTF – Cryptography |
| Forensics & file analysis | picoCTF – Forensics |
| Web exploitation basics | picoCTF – Web Exploitation |
| Binary exploitation fundamentals | picoCTF – Binary Exploitation |

## Bandit Write-Ups

| Level | Topic | Write-Up |
|---|---|---|
| 0 → 1 | SSH basics | [level00-01.md](bandit/level00-01.md) |
| 1 → 2 | Reading a File Named "-" | [level01-02.md](bandit/level01-02.md) |
| 2 → 3 | Filename containing spaces  | [level02-03.md](bandit/level02-03.md) |
| ... | ... | *(add new rows as you go)* |

## picoCTF Write-Ups

| Category | Challenge | Write-Up |
|---|---|---|
| General Skills | Example challenge | [example-challenge.md](picoctf/category-general-skills/example-challenge.md) |
| Forensics | ... | *(add as you go)* |
| Web Exploitation | ... | *(add as you go)* |
| Cryptography | ... | *(add as you go)* |

## Structure

```
ctf-writeups/
├── bandit/
├── picoctf/
│   ├── category-general-skills/
│   ├── category-forensics/
│   ├── category-web-exploitation/
│   └── category-cryptography/
└── assets/screenshots/
```

Each write-up follows a consistent format: objective, recon, approach, commands used, key takeaway, and blue-team relevance (where applicable). See [WRITEUP_TEMPLATE.md](WRITEUP_TEMPLATE.md).
