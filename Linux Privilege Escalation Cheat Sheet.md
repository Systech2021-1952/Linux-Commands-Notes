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


2. SUID / SGID Binaries

` find / -perm -4000 -type f 2>/dev/null `
> Finds files with the SUID bit set. These binaries run with the file owner’s privileges (often root)
and are prime escalation targets.

` find / -perm -2000 -type f 2>/dev/null `
> Finds SGID binaries, which execute with the file’s group privileges rather than the user’s.

` strings /path/to/suid_binary `
> Extracts readable strings from a binary. This can reveal hardcoded paths, commands, or insecure function calls




