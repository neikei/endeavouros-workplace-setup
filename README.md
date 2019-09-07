# endeavouros-workplace-setup

Quick and dirty testing of arch as workplace...

1. sudo pacman -Suy && reboot
2. sudo pacman -Sy ansible
3. wget https://github.com/neikei/endeavouros-workplace-setup/install.yml
4. ansible-playbook install.yml --ask-become-pass
