# Inside a Computer System

## Room Info
- Path: Pre-Security > Computer Fundamentals > Inside a Computer System
- Status: ✅ Completed

## Task 1 — Introduction
Before defending a system, you must understand it first.
Just like defending a castle — you need to know where it is,
what's inside, and who can access it.
A cybersecurity professional must understand the system
before they can protect it.

## Task 2 — Inside a Computer System

| Component | Purpose |
|-----------|---------|
| Motherboard | Skeleton of the computer — connects all components |
| RAM | Short term memory — stores data currently in use |
| SSD | Long term memory — faster, works on chips |
| HDD | Long term memory — slower, has moving parts, older technology |
| Network Adapter | Used to communicate with other computer systems |
| PSU (Power Supply Unit) | Supplies power to all components |
| Graphics Card | Handles and displays visuals |
| I/O Devices | Used to send or receive data (keyboard, mouse, monitor) |

## Task 3 — What Happens When You Press the Start Button?
1. Power button is pressed
2. PSU supplies power to all components
3. **BIOS or UEFI** starts — first software to run on a computer
   - BIOS = older systems
   - UEFI = modern systems (replacement of BIOS)
4. **POST (Power On Self Test)** runs — checks all components are working
5. Boot device is selected from boot list
6. OS loads from SSD/HDD
7. Booting begins

## How This Connects to Real SOC Work
- Understanding hardware helps identify unusual system behavior
- Knowing boot process helps detect bootkit malware
- Network adapter knowledge helps in traffic analysis
- RAM forensics is used in incident response to find malware in memory
