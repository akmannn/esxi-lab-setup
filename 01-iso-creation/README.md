
## 📀 ISO Creation ESXi + USB NIC fling

This section documents the entire ISO creation workflow using PowerShell, including:

- Running the PowerShell script
- Generating the ISO
- Verifying ISO output
- Uploading ISO to ESXi

## 🔧 Step 1 — Run PowerShell ISO Creation Script

Screenshot:

<img width="1920" height="1080" alt="01_powershell_iso_creation png" src="https://github.com/user-attachments/assets/a4796e0a-e753-4120-b48f-50068ff71990" />

This screenshot shows all executed commands, including:

- Mounting WIM

- Injecting drivers

- Creating bootable ISO image

- Using oscdimg to build the ISO

## 📂 Step 2 — ESXi ISO Generated Successfully

Screenshot: <img width="1920" height="1080" alt="02_iso_generated png" src="https://github.com/user-attachments/assets/38562abf-2889-40d8-a115-796c4d78e2e0" />


This confirms the ISO was created in the output folder.
The file should look like:

WindowsServer2019_Custom.iso

## 💿 Step 3 — Bootable Media Created

Screenshots: <img width="569" height="759" alt="03_iso_media_created" src="https://github.com/user-attachments/assets/9971e421-9d70-4683-b36e-e58eab573f68" />

<img width="1920" height="1080" alt="Screenshot (1052)" src="https://github.com/user-attachments/assets/b47bbb5a-85f0-4989-8a8b-d1e65966d241" />

These screenshots shows the bootable ISO is created and is ready for installation, proving the process completed successfully.
