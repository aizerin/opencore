# HW Info
- CPU: Intel Core i3-9100F
- MTB: GIGABYTE Z370M-D3H (F12 bios)
- RAM: Patriot Viper Steel Series 16GB KIT DDR4 3000Mhz CL16
- SSD: Crucial MX500 500GB M.2 2280 SSD
- GPU: SAPPHIRE PULSE Radeon RX 580 OC 8G
- WIFI+BLUETOOTH: BCM94360CD + PCIE adapter 
- Screen: LG 27UK850

## misc fixes
- fix preview : https://www.tonymacx86.com/threads/rough-guide-fix-for-finder-preview-not-working-on-mojave-10-14-1.264398/ 

## F12 bios fix

https://www.tonymacx86.com/threads/success-b1s-mac-mini-killer-with-macos-mojave-i7-8700-gigabyte-z370n-rx560-16gb-ram.260337/page-51#post-1934546

1. Make a boot USB flash drive with your current EFI folder.
2. Download bootx64.efi and copy it to EFI/Boot/.
This is some kind of alternative bootloader that starts with the command line. Here we will modify hidden BIOS settings.

3. Update BIOS to F12 (only F12!)
4. Reboot and hold F12 to boot from your USB Flash drive. Now you should see this command line.
5. Now enter
Code:
setup_var 0x5A4 0x0
Code:
setup_var 0x507 0x1


NOTE: maybe this may be better solution (https://www.tonymacx86.com/threads/fix-for-boot-hangs-after-bios-update-acpi-patch.275091/)

TODO: test F13 bios

## misc links

https://www.tonymacx86.com/threads/solved-hide-boot-clover-from-efi.169641/

https://github.com/tkrotoff/Gigabyte-GA-Z77-DS3H-rev1.1-Hackintosh#prevent-os-x-from-mounting-a-volume

https://github.com/littlegtplr/Hackintosh-Clover-folder-for-Coffee-Lake-builds

https://github.com/omnitrix9991/Hackintosh-Z370M-D3H-OpenCore-with-DSDT

not needed so far: https://www.tonymacx86.com/threads/applehda-realtek-audio-guide.234732/