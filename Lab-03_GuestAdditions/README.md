# Lab 03 — Install VirtualBox Guest Additions (Windows 10)

## Goal
Install VirtualBox Guest Additions on the Windows 10 VM so features like:
- Better screen resizing (auto-resize)
- Shared clipboard
- Drag & Drop  
work correctly.

## Environment
- Host OS: Windows (Host PC)
- Hypervisor: Oracle VirtualBox
- Guest OS: Windows 10 (x64)

## Steps (what I did)
1. In the VM window, go to **Devices → Drag and Drop → Bidirectional** (optional but recommended).
2. Go to **Devices → Insert Guest Additions CD Image…**
3. In Windows (inside the VM), open **This PC** and open the **CD Drive: VirtualBox Guest Additions**
4. Run **VBoxWindowsAdditions-amd64.exe**
5. Click **Yes** on the UAC prompt.
6. Setup wizard:
   - **Next**
   - **Next** (install location)
   - **Install**
   - **Reboot now → Finish**

## Evidence (Screenshots)
![01 - Enable Drag & Drop Bidirectional](screenshots/01-enable-dragdrop-bidirectional.png)
![02 - Guest Additions CD shows](screenshots/02-guestadditions-cd-shows.png)
![03 - Run VBoxWindowsAdditions amd64](screenshots/03-run-vboxwindowsadditions-amd64.png)
![04 - UAC Yes](screenshots/04-uac-yes.png)
![05 - Setup Welcome](screenshots/05-setup-welcome-next.png)
![06 - Install Location](screenshots/06-setup-install-location.png)
![07 - Components Install](screenshots/07-setup-components-install.png)
![08 - Reboot Finish](screenshots/08-setup-reboot-finish.png)

## Verification
After reboot, confirm at least one of these works:
- Drag a file from host → VM
- Copy/paste text from host → VM
- VM screen resizes automatically when you resize the window
