# Install VCSA

## Table of contents

* [Setup BIOS for NEC Express Server](#Setup-BIOS-for-NEC-Express-Server)
* [Setup ESXi](#Setup-ESXi)
* [Deploy for VCSA install](#Deploy-for-VCSA-install)
* [Install VCSA](Install-VCSA)

## Setup BIOS for NEC Express Server

1. Power On Server.
1. Push button F2 in the boot sequence.
1. Choose `Boot` Menu.
1. Choose `UEFI` in HDD mode.
1. Select `Remote Media Device` for 1st boot.
1. Push button `Esc` and `Save and Exit`.

## Setup ESXi

1. Insert ESXi Install media ISO file in Express Scope.
1. Push button `connects` and `Save`.
1. Wait about 5 minutes for ESXi Install Media boot.
1. Push button `Enter` in Welcome installation page.
1. Push button `F11` in End User License Agreement page.
1. Choose Disk for ESXi install and push button `Enter` in Select a Disk to Install or Upgrade page.
1. Choose Install mode and push button `Enter` in ESXi install mode page. (Option)
1. Choose language and push button `Enter` in select a keyboard layout page.
1. Enter a root password and push button `Enter` in Enter a root password page.
1. Wait about 10 minutes for ESXi install.
1. Push button `Enter` in Installation Compleate page.
1. Rebooting...
1. Enter a root password.
1. Setup network settings.

## Deploy for VCSA install

1. Deploy on ESXi.
1. Setup network settings of Windows.
1. Check network connection.

## Install VCSA

### Requirement

* Available resolve DNS of VCSA.
* Work from windows on ESXi.

1. Execute VCSA installer.
1. Enter the necessary information.
