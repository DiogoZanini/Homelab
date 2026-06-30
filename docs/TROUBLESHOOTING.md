# Troubleshooting
Problems encountered and their solutions

### Driver name clash (VERR_PDM_USB_NAME_CLASH)
- **Problem:** Corrupted/duplicated USB drivers after reinstall or update.
- **Solution:** Reinstall VirtualBox cleanly:
  1. Uninstall VirtualBox (accept removal of all network/USB components);
  2. Delete `C:\Program Files\Oracle\VirtualBox` and `C:\Windows\System32\drivers\VBox*`;
  3. Reboot;
  4. Reinstall from [virtualbox.org](https://www.virtualbox.org/).


### VitualBox - Critical Error (ERROR_SERVICE_DISABLED/0x80070422 (0x80070422))
- **Problem:** The following error message appears when opening VirtualBox: `"The VBoxSDS Windows service is disabled."` (Error code: `ERROR_SERVICE_DISABLED` / `0x80070422`).
- **Solution:** Enable VirtualBox System Service in `mscofig`:
  1. Press `Windows + R`, type `msconfig`, and press **Enter**;
  2. Go to **Services** tab;
  3. Check the **Hide all Microsoft services** box;
  4. Find and check **VirtualBox System Service**;
  5. Click **Apply** and then **OK**;
  6. Reboot the operating system.