CONFIGFILES
==============

Grub configurations for my i5 laptop to avoid freeze bug and skip Grub menu at start

- config file should be in /etc/default/grub
- 31_hold_shift script belongs in /etc/grub.d/

After edit, add GRUB_FORCE_HIDDEN_MENU="true" to /etc/default/grub and re-run grub-mkconfig (generally, grub-mkconfig -o /boot/grub/grub.cfg or sudo update-grub
