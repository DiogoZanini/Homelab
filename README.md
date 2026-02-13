# Homelab
Index of my study infrastructure.

[**PT-BR**](./docs/README.pt-br.md)

## Development Environment
### Host Machine
- **IDE:** [VS Code IDE Setup](https://github.com/DiogoZanini/VSCode-IDE-setup).

### pfSense [Oracle VirtualBox]
- **Virtual Network Gateway:** Default gateway for the virtual lab network, handling routing and firewall rules.

### SanDisk USB Drive
- **Tails Amnesic Incognito System:** [Portable Linux Tails](https://github.com/DiogoZanini/Portable-Linux-Tails).

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