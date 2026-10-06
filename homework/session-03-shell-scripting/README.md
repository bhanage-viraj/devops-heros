# Session 3 — System information script

Student: `bhanage-viraj`  
Enrollment number: `ENROLLMENT-NUMBER-HERE` (replace this before you submit the form)

Script: [system_info.sh](system_info.sh)

It prints the date, hostname, username, and disk usage. It reads a name, enrollment number, and comment with `read -p`. It creates `student-output/`, touches `processes.log`, and redirects `ps aux` into that file.

## Command output

Captured on 6 Oct 2026 by piping answers into the script:

```text
Current date: Tue Oct  6 18:35:32 WITA 2026
Hostname: Virajs-MacBook-Pro-3.local
Username: bhanageviraj

Disk usage:
/dev/disk3s1s1   926Gi   13Gi   224Gi    6%   /

My name is bhanage-viraj
My enrollment number is ENROLLMENT-NUMBER-HERE
My comment is: Completed the system information script.

Created directory: student-output
Stored running processes in: student-output/processes.log
Process log line count: 1184
```

The full `df` listing from that run is in [script-output.txt](script-output.txt). The process log is generated locally and is gitignored, because a full process list from a laptop does not belong in a public repository. Run the script again and the file is recreated:

```bash
chmod +x system_info.sh
./system_info.sh
wc -l student-output/processes.log
```
