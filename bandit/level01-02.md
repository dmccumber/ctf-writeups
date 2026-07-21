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
Once I gained access to the machine, I ran a quick LS command to list the contents of the current directory. I found the file that was in question. I attempted to run a cat command on the file and didn't have much success due to the terminal not interpretting it as STDIN instead of a file name. Therefore, I had to change my approach and use the relative path of the file inside of the directory.

```bash
cat ./-
```

## Solution Summary
The cat ./- command provided the password for the next level inside of the "-" file in plaintext.

**Flag:** `REDACTED`

## Key Takeaway / Blue-Team Relevance
Files that are named using a hyphen "-" are relevant to blue teamers because they are used by attackers to potentially confuse the command line due to option injection, or can be used for exploitation purposes.

Therefore, it is important to do what we did in this lab by either using the relative path or using the double dash parameter when running commands when dealing with suspicious files.

## Portfolio Angle
We should also keep this type of thing in mind when writing automation scripts, and should always validate filenames and their associated inputs. 
