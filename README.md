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
      - chromium
      - code
      - geary
      - git
      - keepassxc
      - lsof
      - nmap
      - nmon
      - pdfsam
      - tree
      - vim
    aur_packages:
      - acroread
      - seafile-client-git
      - signal-desktop
      - spotify
    snap_packages:
      - ""
    unneeded_packages:
      - ""
    install_docker: true
```
