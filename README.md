# endeavouros-workplace-setup

[EndeavourOS](https://endeavouros.com/) workplace setup with ansible.

## Installation

```bash
# 1. Update all installed packages
sudo pacman -Syu

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
#     - eos-update-notifier # No longer needed since 2019.12.03 release
    aur_packages:
      - acroread
      - seafile-client-git
      - spotify
      - signal-desktop
    snap_packages:
      - ""
    unneeded_packages:
      - "" # kalu # No longer needed since 2019.12.03 release
    install_docker: true
```
