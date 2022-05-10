# Implementation

## Installation

Download the `.tar.gz` file from the [latest release][release-source] at `Fondroid/clash_for_windows_pkg`, and save it in, say, ~/Desktop.
Unzip and rename the destination folder to `clash` by typing in terminal
```sh
tar -zxf Clash.for.Windows-*-x64-linux.tar.gz
mv Clash.for.Windows-*-x64-linux clash
```
Move `clash` to `/opt` by typing in terminal
```sh
sudo mv clash /opt
```
Installation completed.

[release-source]:https://github.com/Fndroid/clash_for_windows_pkg/releases/latest

## Initiation

Launch Clash by typing in terminal
```sh
cd opt/clash
.cfw
```
When the GUI pops out, select on `Profiles`, type in your profile URL, and click `Download`.
After download completed, click on the downloaded `.yaml`.
Select on `General` and switch on `Allow LAN`, `IPv6` and `Start with Linux`.
Select on `Proxies` to set up the proxy rule.
Close the GUI and stop the command by pressing `Ctrl`+`Z`.

Setup the environment by typing in terminal
```sh
sudo chmod 666 /etc/environment
vi /etc/environment
```
Press `I` to enable editing and copy the following content into terminal with `Ctrl`+`Shift`+`V`
```sh
http_proxy=http://127.0.0.1:7890/
https_proxy=http://127.0.0.1:7890/
ftp_proxy=http://127.0.0.1:7890/
HTTP_PROXY=http://127.0.0.1:7890/
HTTPS_PROXY=http://127.0.0.1:7890/
FTP_PROXY=http://127.0.0.1:7890/
```
Press `Enter` and then press `Esc` to exit edting.
Press `Shift`+`;`, type `wq` and press `Enter` to save and quit. 
Finish environment setup by typing in terminal
```sh
sudo chmod 444 /etc/environment
```

## Launch and Pause

The Clash GUI pops up every time the Linux OS starts up.
Select on `Connection` and click `Pause` if you wish to pause the proxy.
Minimize the GUI windows instead of close it off when in use.

