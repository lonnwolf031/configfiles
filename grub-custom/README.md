CONFIGFILES
==============

Grub configurations for my i5 laptop to avoid freeze bug and skip Grub menu at start

- config file is /etc/default/grub
When adjusting another setup:
- The line that needs to be adjusted to make this work is to add:

GRUB_FORCE_HIDDEN_MENU="true"

- 31_hold_shift script belongs in /etc/grub.d/

After edit, add GRUB_FORCE_HIDDEN_MENU="true" to /etc/default/grub and re-run grub-mkconfig (generally, grub-mkconfig -o /boot/grub/grub.cfg   OR    sudo update-grub
