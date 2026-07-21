# [Platform] – [Level/Challenge Name]

**Category:** e.g. Privilege Escalation / Forensics / Web Exploitation
**Difficulty:** Easy / Medium / Hard
**Tools used:** e.g. `ssh`, `find`, `strings`, `netcat`

## Objective
One or two sentences: what does this level/challenge ask you to do?

## Recon
What did you observe first? (file listing, service banners, hints in challenge description, permissions, etc.)

```bash
# commands used during recon
```

## Approach
Walk through your reasoning step by step — this is the part recruiters actually read. Explain *why* you tried something, not just what you typed.

```bash
# key commands, redact any flag output
```

## Solution Summary
Brief recap of the technique that worked (e.g. "SUID binary allowed reading a file owned by the next-level user").

**Flag:** `REDACTED`

## Key Takeaway / Blue-Team Relevance
How does this technique show up in real environments? What would you look for as a defender to detect or prevent this? (e.g. "This SUID misconfiguration is exactly what auditing tools like `linpeas` or a scheduled `find / -perm -4000` check would catch.")

## Portfolio Angle
One line on how this connects to a broader skill (e.g. "Same privilege-escalation logic applies to Linux persistence checks during incident response.")
