# Implementation

## Installation
Download the `.tar.gz` from latest release at Fondroid/clash_for_windows_pkg, and save it in, say, ~/Desktop.
Unzip and rename the destination folder to `clash` by typing in terminal
```sh
tar -zxf Clash.for.Windows-*-x64-linux.tar.gz
mv Clash.for.Windows-*-x64-linux clash
```
Move `clash` to /opt by typing in terminal
```sh
sudo mv clash /opt
```
Installation completed.

## Initiation
Launch Clash by typing in terminal
```sh
cd opt/clash
.cfw
```
When the GUI pops out, select on `Profiles`, type in your profile URL, and click `Download`.
After download completed, click on the downloaded `.yaml` and setup the `Proxies` to finish initiation.

## Launch
Launch Clash by typing in terminal
```sh
cd opt/clash
.cfw
```
When the GUI pops out, select on `General` and switch on `Start with Linux`.
