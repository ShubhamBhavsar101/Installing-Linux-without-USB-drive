
# Installing Linux without USB Drive

Install Ubuntu without a USB drive.

### 1. Create Partition
- Create an 8GB partition
- Format as FAT32

### 2. Copy ISO
- Mount Ubuntu ISO
- Copy contents to the root of the new partition

### 3. Set Partition as EFI

Open CMD as administrator:

```
diskpart

list disk
sel disk [NUMBER]

list part
sel part [NUMBER]

help set
set id=[EFI PARTITION VALUE]
```

### 4. Boot into Installer
- Reboot
- Enter BIOS (Del key on MSI)
- Select "UEFI OS" in the Boot menu

Linux installer should start.

