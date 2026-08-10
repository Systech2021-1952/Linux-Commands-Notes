# Linux Privilege Escalation Cheat Shee
### Commands Explained – Pentesting & Teaching Edition


## 1. System & User Enumeration

` id `
> Shows your current user ID (UID), group ID (GID), and group memberships. This helps you understand what privileges you already have.

` whoami `
> Displays the username you are currently operating as. Useful to confirm your current access level.

` groups `
> Lists all groups your user belongs to. Membership in privileged groups such as sudo or docker can lead to root access.

` uname -a `
> Displays kernel version, system architecture, and OS details. This information is critical for identifying kernel-based privilege escalation exploits.

` sudo -l `
> Lists commands the current user is allowed to run with  sudo . Misconfigured sudo rules are one of the most common privilege escalation vectors.  


## 2. SUID / SGID Binaries

` find / -perm -4000 -type f 2>/dev/null `
> Finds files with the SUID bit set. These binaries run with the file owner’s privileges (often root)
and are prime escalation targets.

` find / -perm -2000 -type f 2>/dev/null `
> Finds SGID binaries, which execute with the file’s group privileges rather than the user’s.

` strings /path/to/suid_binary `
> Extracts readable strings from a binary. This can reveal hardcoded paths, commands, or insecure function calls

## 3. Writable Files & Directories

` find / -writable -type d 2>/dev/null `
> Lists directories you can write to. Writable directories owned or used by root may allow script or
file injection.

` find / -writable -type f 2>/dev/null `
> Finds writable files. Modifying scripts or configuration files executed by root can lead to
escalation.

` ls -la /etc `
> Checks permissions on system configuration files. Misconfigured permissions may expose
credentials or allow tampering

## 4. Cron Jobs & Scheduled Tasks

` crontab -l `
> Displays cron jobs scheduled for the current user.

` cat /etc/crontab `
> Shows system-wide cron jobs. If a root cron job executes a writable script, it can be hijacked.

` ls -la /etc/cron* `
> Lists cron directories to identify scheduled tasks and potential permission issues.

## 5. Environment Variables




