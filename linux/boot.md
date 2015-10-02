# Rescuing a non-booting grub2 on Linux

https://www.linux.com/learn/tutorials/776643-how-to-rescue-a-non-booting-grub-2-on-linux/

# Grub Not Appearing on Boot After Dual-Bootable Windows Upgrade

From an administrator command prompt in Windows run this command:

```
bcdedit /set {bootmgr} path \EFI\ubuntu\grubx64.efi
```

Grub should re-appear on your next reboot.
