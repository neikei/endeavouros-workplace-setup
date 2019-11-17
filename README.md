# endeavouros-workplace-setup

[EndeavourOS](https://endeavouros.com/) workplace setup with ansible.

## Installation

```bash
# 1. Remove kalu and update all installed packages
sudo pacman -R kalu && sudo pacman -Syu

# 2. Install ansible
sudo pacman -S ansible

# 3. Download the install.yml
wget https://raw.githubusercontent.com/neikei/endeavouros-workplace-setup/master/install.yml

# 4. Run the installation
ansible-playbook install.yml --ask-become-pass
```

## Included software

- CLI-Tools
  - vim
  - git
  - lsof
  - nmap
  - tree
  - snap
- Visual Studio Code
- Seafile
- Chromium
- Acrobat Reader
- Spotify
- KeepassXC
- Docker
