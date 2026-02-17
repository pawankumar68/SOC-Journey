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
