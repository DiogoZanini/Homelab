# Homelab
Index of my study infrastructure.

[**PT-BR**](./docs/README.pt-br.md)

![Homelab Diagram](./docs/homelab_network_diagram.png)

## Development Environment

### 🖥️ Host Environment 
- [**VS Code IDE:**](https://github.com/DiogoZanini/VSCode-IDE-setup) VSCode setup for C, Python and SQLite development, extending CS50's workflow.
- [**Tails Amnesic Incognito System:**](https://github.com/DiogoZanini/Portable-Linux-Tails) Personal setup and operational notes for an amnesic security environment on a USB drive.

### 🌐 Homelab Infrastructure
- [**pfSense:**](https://github.com/DiogoZanini/pfSense) Default gateway for the virtual lab network, handling routing and firewall rules.

### 🔴 Red Team / Analysis
- [**Kali Linux:**](https://github.com/DiogoZanini/Kali-Linux) Analyst virtual machine for security analysis of the homelab environment and CTF challenges on online study platforms.

## Roadmap

### 🖥️ Host Environment 
- [x] Host Machine: VS Code IDE + Oracle VirtualBox;
- [x] Tails Amnesic Incognito System (Bootable USB);

### 🌐 Homelab Infrastructure
- [x] pfSense VM (Firewall/Router);

### 🔴 Red Team / Analysis
- [x] Kali Linux VM (Security Analysis);

### 🎯 Attack Surface (Vulnerable Targets)

**Web Applications:**
- [ ] OWASP Juice Shop;
- [ ] DVWA (Damn Vulnerable Web Application);

**Vulnerable Systems:**
- [ ] Metasploitable;
- [ ] Metasploitable2;
- [ ] Metasploitable3-ub1404 (Ubuntu);
- [ ] Metasploitable3-win2k8 (Windows);

### 🪟 Windows Environment

**Active Directory Lab:**
- [ ] Windows Server 2025 + Active Directory;

**Workstations:**
- [ ] Windows 11 (Production);
- [ ] Windows 10;

**Legacy Systems (EOL):**
- [ ] Windows 7;
- [ ] Windows Vista;
- [ ] Windows XP;

**Malware Analysis (Isolated):**
- [ ] Windows 11 - Malware Analysis Lab (Snapshot)
  - Tools: Wireshark, IDA, x32dbg, x64dbg, ProcMon, ProcExp, Ghidra, DIE, HxD

### 🐧 Linux Environment
- [ ] Debian VM:
  - Snapshot: OWASP Juice Shop
  - Snapshot: DVWA

### 🔵 Blue Team / Detection
- [ ] SOC Laboratory;

## Troubleshooting
Common issues and their solutions.

[Full Troubleshooting Guide](./docs/TROUBLESHOOTING.md)

### Driver name clash (VERR_PDM_USB_NAME_CLASH)
- **Problem:** Corrupted/duplicated USB drivers after reinstall or update.
- **Solution:** Reinstall VirtualBox cleanly:
  1. Uninstall VirtualBox (accept removal of all network/USB components);
  2. Delete `C:\Program Files\Oracle\VirtualBox` and `C:\Windows\System32\drivers\VBox*`;
  3. Reboot;
  4. Reinstall from [virtualbox.org](https://www.virtualbox.org/).
