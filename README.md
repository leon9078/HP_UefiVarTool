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
FSX: #Where X is the index of the FAT partition where the in.txt file resides.
uvt < in.txt

Ctrl+Alt+Del to Reboot!!!

Laptop: HP 15da-1000nl<br/>
BIOS Vendor: Insyde<br/>
BIOS Version: F.47<br/>
BIOS Release Date: 12/25/2023