
## 📀 ISO Creation (Windows Server 2019 / Windows 10/11)

This section documents the entire ISO creation workflow using PowerShell, including:

- Running the PowerShell script
- Generating the ISO
- Verifying ISO output
- Uploading ISO to ESXi

## 🔧 Step 1 — Run PowerShell ISO Creation Script

Screenshot: 01_powershell_iso_creation.png

This screenshot shows all executed commands, including:

- Mounting WIM

- Injecting drivers (if any)

- Creating bootable media

- Using oscdimg to build the ISO

## 📂 Step 2 — ESXi ISO Generated Successfully

Screenshot: 02_iso_generated.png

This confirms the ISO was created in the output folder.
The file should look like:

WindowsServer2019_Custom.iso

## 💿 Step 3 — Bootable Media Created

Screenshot: 03_iso_media_created.png

Shows the bootable ISO is created and is ready for installation, proving the process completed successfully.
