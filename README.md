# endeavouros-workplace-setup

[EndeavourOS](https://endeavouros.com/) workplace setup with ansible.

## Installation

```bash
# 1. Update EndeavourOS
sudo pacman -Suy

# 2. Reboot after updating all packages
sudo reboot

# 3. Install ansible
sudo pacman -Sy ansible

# 4. Download the install.yml
wget https://github.com/neikei/endeavouros-workplace-setup/install.yml

# 5. Run the installation
ansible-playbook install.yml --ask-become-pass
```

## Included software

- CLI-Tools (vim, git, lsof, nmap, tree, snap)
- Visual Studio Code
- Keepass
- Chromium
- Spotify
- Docker
