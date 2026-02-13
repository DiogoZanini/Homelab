# Troubleshooting
Problems encountered and their solutions

### Driver name clash. Another driver with the same name as the one being registered exists. (VERR_PDM_USB_NAME_CLASH)
- **Problem:** Driver corrupted and duplicated in the host system;
- **Solution:** <details><summary>Reinstall and remove all data.</summary>

- Uninstall Virtualbox;
- Remove `C:\Program Files\Oracle\VirtualBox` and `C:\Windows\System32\drivers\VBox*`;
- Reboot system;
- Install [VirtualBox](https://www.virtualbox.org/) 
</details>