# HP_UefiVarTool
Put scriptable file with hidden UEFI variables to modify

Download "UEFI Shell" from here: [UEFI Shell](https://archlinux.org/packages/extra/any/edk2-shell/download/).<br/>
Extract the ".tar.zst" file.<br/>
Rename "usr\share\edk2-shell\x64\Shell_Full.efi" to "BOOTx64.efi".<br/>

* Copy "in.txt" to the root of a FAT16 / FAT32 USB drive.<br/>
* Create EFI/BOOT/ folder and copy "BOOTx64.efi" file there.<br/>
* Create EFI/TOOLS/ folder and copy "uvt.efi" file there.<br/>

You can take "uvt.efi" from [UefiVarTool](https://github.com/GeographicCone/UefiVarTool/releases/latest). All credits goes to [GeographicCone](https://github.com/GeographicCone) for this amazing tool!

After booting the UEFI Shell, type:
uvt < FS0:\in.txt

[BIOS_F48.img] (https://mega.nz/file/KdxSxQTY#nA_iRcF88m88zpmpzwJBP916X0rnWhAs8CKXbi6JZ9A)
[BIOS_F48.vhd] (https://mega.nz/file/qERFjQSa#g1HbqP-_EMlnqdnwUsjW0N8XwYGLfFFfb_GdXr5_qFM)

Use BIOS_F48.img in Linux/macOS or BIOS_F48.vhd in Windows in order to create a bootable USB BIOS recovery flash drive.
After created, insert the USB flash drive to the laptop. Connect the charger and shut down the PC. Hold down Win+B. While holding this combination, press and hold for 3 seconds the Power button, then release, but keep holding the Win+B combination. Release them when you hear the fans going full speed. It will start doing the recovery process.

Laptop: HP 15da-1000nl<br/>
BIOS Vendor: Insyde<br/>
BIOS Version: F.48<br/>
BIOS Release Date: 04/26/2024
