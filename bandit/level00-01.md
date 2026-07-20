# Bandit – Level 0 → 1

**Category:** Linux Fundamentals
**Difficulty:** Easy
**Tools used:** `ssh`, `cat`, `ls`

## Objective
Log into the Bandit game server via SSH and locate the password for the next level, stored in a file called `readme` in the home directory.

## Recon
Connected via SSH using the credentials provided on the Bandit level 0 page, then listed the home directory contents.

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
ls -la
```

## Approach
The home directory contained a single file, `readme`. Printed its contents directly since no unusual permissions or naming were involved at this level.

```bash
cat readme
```

## Solution Summary
The password for the next level was stored in plaintext inside `readme` in the home directory.

**Flag:** `REDACTED`

## Key Takeaway / Blue-Team Relevance
Trivial here, but it's the foundation for everything else: comfortable SSH usage and file navigation are prerequisites for log review, live response on remote hosts, and jump-box work in a SOC.

## Portfolio Angle
Establishes baseline Linux/SSH fluency that later Bandit levels build on (file permissions, SUID binaries, cron jobs, and privilege escalation).
