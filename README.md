# Snake Ransomware CTF Simulation 🐍💻

**Category:** Reverse Engineering / Malware Analysis   
---

## Overview

This is a **safe, educational simulation** inspired by a ransomware-style challenge.  
The program mimics a ransomware executable that:

- Appears as a classic Snake game.  
- Contains a hidden XOR-encrypted flag in memory.  
- Unlocks the flag when the player reaches **15 points** in the game.  

> ⚠️ **Important:** This project is completely safe. It does **not** encrypt or modify any files on your system. It is intended for learning **reverse engineering** and **malware analysis concepts** in a controlled environment.

---

## Features

- Terminal-based Snake game (ASCII graphics).  
- XOR-encrypted flag hidden in the binary.  
- `decrypt_key()` function simulates key derivation, similar to malware logic.  
- Flag reveals only after reaching a gameplay milestone (score ≥ 15).  

---

## Build Instructions

### Prerequisites

- GCC compiler (`gcc`)  
- POSIX-compatible terminal (Linux/macOS)

### Compile

```bash
git clone https://github.com/yeabsira-mihret/Snake-Ransomware-CTF
cd Snake-Ransomware-CTF
gcc -O2 -o snake_ctf rasomeware.c -Wall
```
Run
```bash
./snake_ctf
```
## Controls:

W / ↑: Move up
S / ↓: Move down
A / ←: Move left
D / →: Move right

Score at least 15 points to reveal the hidden flag.

---

## Educational Objectives

Reverse engineer binaries and understand how malware stores secrets.
Learn XOR encryption/decryption in memory.
Practice runtime key derivation and payload unlocking.
Develop basic terminal game programming skills in C.

---

## Flag

Once you reach the target score, the program reveals:
```bash
cxc{malware_is_fun!}
```
## License

This project is released under the MIT License.
Feel free to use, modify, and learn from it for educational purposes.

## Disclaimer

This project is safe and intended only for learning and practice.
Do not attempt to use it for malicious purposes.
