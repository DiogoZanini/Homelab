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

### Driver name clash. Another driver with the same name as the one being registered exists. (VERR_PDM_USB_NAME_CLASH)
- **Problem:** Driver corrupted and duplicated in the host system;
- **Solution:** <details><summary>Reinstall and remove all data.</summary>

- Uninstall Virtualbox;
- Remove `C:\Program Files\Oracle\VirtualBox` and `C:\Windows\System32\drivers\VBox*`;
- Reboot system;
- Install [VirtualBox](https://www.virtualbox.org/) 
</details>