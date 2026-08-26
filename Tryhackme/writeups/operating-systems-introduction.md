# Operating Systems: Introduction

## Room Info
- Path: Pre-Security > Operating Systems Basics > Operating Systems: Introduction
- Status: ✅ Completed

## What is an OS?
An operating system is core software that stands between the user
and hardware. It acts like a central manager that manages every
process of the computer.

## System Privilege Layers
OS works in 2 layers:
- **Kernel Layer** — Has full access to hardware, core of the OS
- **User Interface Layer** — Works in a limited space, interacts with user

## OS Duties
- **File Management** — Files organize karna, add karna, delete karna
  and manage permissions to access them
- **Process Management** — Manages which task gets how much CPU time,
  helps in multitasking
- **Memory Management** — Allocates memory to tasks, takes it back
  when task is complete
- **User Management** — Manages user data, authentication and
  permissions for different users
- **Device Management** — Manages external devices and combines
  hardware and software together

## OS Security
Before firewalls and antivirus, OS itself has security parameters:
- **Authentication** — Verifies original user with ID and password
- **Permissions** — Controls what users can access
- **Isolation** — Keeps processes separate from each other
- **System Protection** — Protects core system files

## OS Interface
Two types of interfaces:
- **GUI (Graphical User Interface)** — Visual, beginner friendly
- **CLI (Command Line Interface)** — Terminal based, faster and more
  powerful but requires knowledge of commands

## Types of Operating Systems

| Type | Purpose | Examples |
|------|---------|---------|
| Desktop OS | Personal computers, daily work, gaming, content creation | Windows 10/11, macOS, Ubuntu, Kali Linux |
| Mobile OS | Mobile phones and tablets | Android, iOS |
| Server OS | Web hosting, database, backend, cloud services | Windows Server, Ubuntu Server, Debian, CentOS |
| Embedded/IoT | Smart TVs, IoT devices, routers | OpenWrt, Ubuntu Core |
| Real-Time OS | Critical systems needing exact time response — medical devices, aircraft, industrial robots | FreeRTOS, QNX |
| Virtual/Cloud | Lab machines, containers, cloud environments | Ubuntu LTS, Amazon Linux, Alpine Linux |

## Why So Many Operating Systems?
Different tasks need different types of OS:
- Some need accuracy
- Some need fast processing
- Some need simple interface
- Some need high security
That is why we have multiple operating systems for different use cases.

## How This Connects to Real SOC Work
- SOC Analysts work on multiple OS types daily
- Linux CLI is essential for log analysis and investigation
- Understanding OS layers helps identify privilege escalation attacks
- OS security parameters are first line of defense before firewalls
