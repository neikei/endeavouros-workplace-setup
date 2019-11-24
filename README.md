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

```yaml
    pacman_packages:
      - vim
      - git
      - lsof
      - nmap
      - nmon
      - tree
      - code
      - keepass
      - chromium
      - eos-update-notifier # Fix: https://forum.endeavouros.com/t/pacman-5-2-1-1-cant-install/2268
    aur_packages:
      - acroread
      - seafile-client-git
      - spotify
      - signal-desktop
    snap_packages: ""
    unneeded_packages:
      - kalu # Fix: https://forum.endeavouros.com/t/pacman-5-2-1-1-cant-install/2268
    install_docker: true
```
