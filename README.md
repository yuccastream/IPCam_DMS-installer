# IPCam_DMS-installer
A simple helper script to install [IPCam_DMS](https://team.openipc.org/ipcam_dms/) in GNU/Linux

## Feature:
1. Supported GNU/Linux distributtions: Debian, Ubuntu, Elementary OS, Zorin OS, Linux Mint, Kali Linux, Fedora, RHEL, CentOS, IGOS Nusantara, Archlinux
2. Installs wine
3. Upgrades wine (from the distribution's repo) to a newer version (only for Fedora, RHEL, CentOS, IGN)
4. Menu entry in the application launcher
5. Latest IPCam_DMS from https://team.openipc.org/ipcam_dms/

## How to install:
Copy and paste this commands to your terminal:

1. `cd /tmp`
1. `git clone https://github.com/yuccastream/IPCam_DMS-installer.git`
1. `cd IPCam_DMS-installer`
1. `sudo ./ipcam_dms-setup install` **OR** `sudo bash ipcam_dms-setup install`

## Firewall setting:
On Fedora/CentOS/Redhat, if you experience neighbor discovery problems, open the port in the firewall

`firewall-cmd --permanent --add-port=5678/udp`

`firewall-cmd --reload`

## Icon cache in GTK based desktop:
Optional step for GTK based desktop, if the icon is not loaded or loaded with wrong size. Update icon cache with this command:

`gtk-update-icon-cache -f -t /usr/share/icons/hicolor`

## How to remove:
If you want to remove winbox, just run this command:

`sudo ./ipcam_dms-setup remove` **OR** `sudo ./ipcam_dms-setup remove`
