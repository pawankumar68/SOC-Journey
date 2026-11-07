# Windows Basics

## Room Info
- Path: Pre-Security > Operating Systems Basics > Windows Basics
- Status: ✅ Completed

## Task 1 — Introduction
Introduced what Windows is and how it differs from other
operating systems.
- Early computers ran MS-DOS, a black screen where commands
  had to be typed
- Windows 1.0 (1985) added a graphical interface with windows,
  menus and mouse control on top of DOS

## Task 2 — Exploring the Windows Workspace

### Account Types
| Account | Purpose |
|---------|---------|
| Guest | Temporary access, minimal permissions, cannot change system settings |
| Standard | Everyday tasks like running apps and changing personal settings, no system-wide changes |
| Administrator | Full control: software installation, configuration changes, user management |

### Desktop vs Taskbar
- **Desktop** — the whole main screen where files, folders and
  shortcuts live
- **Taskbar** — thin strip at the bottom with important pinned
  applications, Start menu, Search, Task View, network/audio
  settings, date/time and notifications

## Task 3 — Configuring and Securing Windows
- Updating Windows
- Installing applications
- Uninstalling applications

Keeping Windows updated matters for security because updates
include patches for known vulnerabilities.

## How This Connects to Real SOC Work
- Attackers target Administrator accounts. A normal user suddenly
  becoming admin is a privilege escalation red flag
- Unpatched Windows systems are easy targets for known exploits
- Most enterprise endpoints a SOC analyst monitors run Windows
