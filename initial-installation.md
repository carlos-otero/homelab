Updates
Edit /etc/apt/sources.list

Proxmox Version 6.X
deb http://ftp.us.debian.org/debian buster main contrib

deb http://ftp.us.debian.org/debian buster-updates main contrib

# security updates
deb http://security.debian.org buster/updates main contrib

# not for production use
deb http://download.proxmox.com/debian buster pve-no-subscription
Proxmox Version 7.X
(for a full guide on Proxmox 7, please see this link)

deb http://ftp.debian.org/debian bullseye main contrib

deb http://ftp.debian.org/debian bullseye-updates main contrib

# security updates
deb http://security.debian.org/debian-security bullseye-security main contrib

# PVE pve-no-subscription repository provided by proxmox.com,
# NOT recommended for production use
deb http://download.proxmox.com/debian/pve bullseye pve-no-subscription
Edit /etc/apt/sources.list.d/pve-enterprise.list

# deb https://enterprise.proxmox.com/debian/pve buster pve-enterprise
Run

apt-get update
apt dist-upgrade
reboot
