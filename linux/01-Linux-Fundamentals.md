# 01 – Linux Basic Commands

This file covers essential Linux commands required for system navigation and basic investigation tasks.

---

## ls

Lists files and directories in the current location.

Example:
ls
ls -l
ls -a

What I Observed:
- `ls -l` shows file permissions, owner, size, and modification date.
- `ls -a` shows hidden files (files starting with .)

Why Blue Team Cares:
- Helps identify suspicious or hidden files.
- Useful during incident response to check unknown directories.

---

## cd

Changes the current directory.

Example:
cd foldername
cd ..
cd /

What I Observed:
- `cd ..` moves one level up.
- `cd /` takes you to the root directory.

Why Blue Team Cares:
- Used to navigate system directories during investigations.
- Important when accessing log locations like /var/log.

---

## pwd

Displays the current working directory.

Example:
pwd

Why Blue Team Cares:
- Ensures you know exactly where you are before executing commands.
- Prevents accidental modification of critical directories.

---

## mkdir

Creates a new directory.

Example:
mkdir test_folder

Why Blue Team Cares:
- Used to organize investigation files, scripts, and collected logs.

---

## rm

Removes files or directories.

Example:
rm file.txt
rm -r foldername

Important:
Use carefully. Deleting system files can cause damage.

Why Blue Team Cares:
- Used to remove malicious files after investigation.
- Must be handled carefully during incident response.

---

## mv

Moves or renames files and directories.

Example:
mv file1.txt file2.txt
mv file.txt /home/user/

Why Blue Team Cares:
- Helps organize evidence.
- Used to isolate suspicious files during analysis.

---

## cat

Displays the full content of a file.

Example:
cat test.txt

What I Observed:
- It prints all lines inside the file.
- Useful for quickly reading small files.

Why Blue Team Cares:
Used to read log files or configuration files during investigations.

---

## head

Displays the first 10 lines of a file by default.

Example:
head test.txt

What I Observed:
- Shows only the top portion of a file.
- Useful when the file is large.

Why Blue Team Cares:
Helps quickly check the beginning of log files for recent system events.

---

## tail

Displays the last 10 lines of a file by default.

Example:
tail test.txt

What I Observed:
- Shows the bottom portion of the file.
- Often used to monitor recent activity.

Why Blue Team Cares:
Useful for checking the latest log entries in files like /var/log/auth.log.

---

## grep

Searches for a specific word or pattern inside a file.

Example:
grep SOC test.txt

What I Observed:
- Displays only lines that match the searched word.
- Case-sensitive by default.

Why Blue Team Cares:
Very important for searching suspicious keywords in logs, such as failed login attempts or error messages.

