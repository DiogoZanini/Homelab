# Homelab
Index of my study infrastructure.

[**PT-BR**](./docs/README.pt-br.md)

![Homelab Diagram](./docs/homelab_network_diagram.png)

## Development Environment

### Host Machine
- [**VS Code IDE:**](https://github.com/DiogoZanini/VSCode-IDE-setup) VSCode setup for C, Python and SQLite development, extending CS50's workflow.

### pfSense (Oracle VirtualBox)
- [**Virtual Network Gateway:**](https://github.com/DiogoZanini/pfSense) Default gateway for the virtual lab network, handling routing and firewall rules.

### Kali Linux (Oracle VirtualBox)
- **Kali Linux Analyst Machine:** Kali Linux analyst virtual machine for security analysis of the homelab environment and CTF challenges on online study platforms.

### SanDisk USB Drive
- [**Tails Amnesic Incognito System:**](https://github.com/DiogoZanini/Portable-Linux-Tails) Personal setup and operational notes for an amnesic security environment on a USB drive. 

## Roadmap
- [x] Tails Amnesic Incognito System live on a USB drive;
- [x] Host Machine: VS Code IDE and Oracle VirtualBox;
- [x] pfSense virtual machine;
- [x] Kali Linux analyst virtual machine;
- [ ] Metasploitable vulnerable machines;
- [ ] OWASP Juice Shop vulnerable Web Server;
- [ ] SOC Laboratory.

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
