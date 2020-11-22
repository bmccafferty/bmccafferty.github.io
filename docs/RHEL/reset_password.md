# Reset root password RHEL 7/8

- Reboot to grub menu and press e to edit the boot line
- On the line marked linux at the end enter rd.break
- Press Ctrl and X to boot into the emergency shell
- mount -o remount,rw /sysroot
- chroot /sysroot
- passwd
- touch /.autorelabel
