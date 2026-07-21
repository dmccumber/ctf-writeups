# Bandit – Level 1 → 2

**Category:** Linux Fundamentals
**Difficulty:** Easy
**Tools used:** e.g. `ssh`, `find`, `strings`, `netcat`

## Objective
The objective of this room is to find the password of the next level that is stored in a file called "-"

## Recon
Connected using SSH with the credentials that I found in the previous level, and then listed the home directory contents to find the required file. 

```bash
ssh bandit1@bandit.labs.overthewire.org -p 2220
ls 
```

## Approach
Once I gained access to the machine, I ran a quick LS command to list the contents of the current directory. I found the file that was in question. I attempted to run a cat command on the file and didn't have much success due to the terminal not interpretting it as a file name. Therefore, I had to change my approach and use the relative path of the file inside of the directory.

```bash
cat - 
cat ./-
```

## Solution Summary
The cat ./- command provided the password for the next level inside of the "-" file in plaintext.

**Flag:** `REDACTED`

## Key Takeaway / Blue-Team Relevance
Trivial here, but it's the foundation for everything else: comfortable SSH usage and file navigation are prerequisites for log review, live response on remote hosts, and jump-box work in a SOC.

## Portfolio Angle
Establishes baseline Linux/SSH fluency that later Bandit levels build on (file permissions, SUID binaries, cron jobs, and privilege escalation).
