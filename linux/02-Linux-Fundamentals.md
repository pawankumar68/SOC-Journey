# 02 – Linux Basic Commands
This file covers essential Linux commands required for file creation, editing, and system information tasks.
---
## touch
Creates a new empty file or updates the timestamp of an existing file.
Example:
touch filename.txt
touch file1.txt file2.txt
What I Observed:
- `touch filename.txt` creates a blank file instantly if it does not exist.
- Running `touch` on an existing file only updates its last-modified timestamp without changing the content.

Why Blue Team Cares:
- Used to quickly create placeholder or log files during investigations.
- Unexpected timestamp changes on files can indicate tampering during forensic analysis.
---
## nano
A simple, beginner-friendly text editor that runs inside the terminal.
Example:
nano filename.txt
nano /etc/hosts
What I Observed:
- Opens the file directly in the terminal for editing.
- Keyboard shortcuts are shown at the bottom: Ctrl+O to save, Ctrl+X to exit.
- Does not require a graphical interface — works over SSH and remote sessions.

Why Blue Team Cares:
- Used to edit configuration files or write investigation notes directly in the terminal.
- Helpful when modifying firewall rules, host files, or scripts during incident response.
---
## rmdir
Removes an empty directory.
Example:
rmdir foldername
rmdir test_folder
What I Observed:
- Only works on directories that are completely empty.
- If the directory contains files, it throws an error — use rm -r for non-empty directories instead.

Why Blue Team Cares:
- Used to clean up empty investigation directories after work is complete.
- Safer than rm -r as it cannot accidentally delete files inside a folder.
---
## cp
Copies files or directories from one location to another.
Example:
cp file.txt backup.txt
cp file.txt /home/user/Documents/
cp -r folder1/ folder2/
What I Observed:
- `cp file.txt backup.txt` creates an exact copy with a new name in the same location.
- `cp -r` is required to copy entire directories recursively.
- The original file remains untouched after copying.

Why Blue Team Cares:
- Essential for creating backups of log files before analysis.
- Used to preserve original evidence files while working on copies during investigations.
---
## wc
Counts lines, words, and characters in a file.
Example:
wc file.txt
wc -l file.txt
wc -w file.txt
What I Observed:
- Default output shows three numbers: line count, word count, and byte count.
- `wc -l` shows only the number of lines — very useful for large log files.
- `wc -w` shows only word count.

Why Blue Team Cares:
- Used to quickly measure the size of log files.
- Helps verify if a log file has been truncated or unexpectedly modified (sudden drop in line count can be suspicious).
- Can be combined with grep to count occurrences: grep "Failed" auth.log | wc -l
---
## date
Displays the current system date and time.
Example:
date
date +"%Y-%m-%d"
date +"%H:%M:%S"
What I Observed:
- Running `date` alone prints the full current date, time, timezone, and day of the week.
- Custom formats can be used with + to extract specific parts like year, month, or time only.

Why Blue Team Cares:
- Used to verify system time accuracy — attackers sometimes alter system time to confuse log timestamps.
- Important for correlating events across multiple systems during incident investigation.
- Time discrepancies between systems can indicate tampering or misconfiguration.
---
## cal
Displays a calendar in the terminal.
Example:
cal
cal 2025
cal 07 2025
What I Observed:
- `cal` alone shows the current month's calendar with today's date highlighted.
- `cal 2025` displays the full year calendar.
- `cal 07 2025` shows a specific month and year.

Why Blue Team Cares:
- Useful for quickly cross-referencing dates during timeline analysis of an incident.
- Helps verify the day of the week for specific event dates when reviewing historical logs.
---
