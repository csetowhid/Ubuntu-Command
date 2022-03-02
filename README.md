# Ubuntu Commands

Before Running Any Command You Need To Run

```
 sudo apt update
```
# Google Chrome
To install Google Chrome from the terminal, get the DEB file using the wget command:
```
wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb
```
Now you can use dpkg to install Chrome from the downloaded DEB file:
```
sudo dpkg -i google-chrome-stable_current_amd64.deb
```
Link
- [Install Google Chrome on Ubuntu](https://itsfoss.com/install-chrome-ubuntu)

# Install MPV

`sudo add-apt-repository ppa:mc3man/mpv-tests`\
`sudo apt-get update`\
`sudo apt install mpv`

### Link

https://launchpad.net/~mc3man/+archive/ubuntu/mpv-tests

# Install SMPlayer

`sudo add-apt-repository ppa:rvm/smplayer`\
 `sudo apt-get update`\
 `sudo apt-get install smplayer smplayer-themes smplayer-skins`

# Zoom

`sudo snap install zoom-client`

# Xtreme Download Manager

### Download

https://xtremedownloadmanager.com/#downloads

### Install

Go to the directory first & Extract: \
 Now run the installer script and follow the instrcution:\
 `sudo ./install.sh`

### Uninstall

To uninstall run /opt/xdman/uninstall.sh as root like this:\
 `sudo /opt/xdman/uninstall.sh`

### Link

https://itsfoss.com/xtreme-download-manager-install/

# Bijoy For Ubuntu

### Download

- [Download](https://www.techtdbangla.com/2020/05/best-bangla-typing-software-bijoy.html)

### Install

```
sudo apt-get install ibus-m17n
```

```
sudo chmod 777 /usr/share/m17n/
```

```
sudo chmod 777 /usr/share/m17n/icons
```

```
sudo chmod 777 /var/lib/dpkg/info/m17n-db.list
```

```
gedit /var/lib/dpkg/info/m17n-db.list
```

```
/usr/share/m17n/icons/bn-bijoyClassic.png
/usr/share/m17n/bn-bijoyClassic.mim
/usr/share/m17n/icons/bn-bijoyUnicode.png
/usr/share/m17n/bn-bijoyUnicode.mim
```

### Link

- [Best Bangla Typing Software](https://www.techtdbangla.com/2020/05/best-bangla-typing-software-bijoy.html)

# Journalctl Cache Clear
`journalctl --disk-usage`\
`sudo journalctl --rotate`
- Delete journal logs older than X days:\
`sudo journalctl --vacuum-time=2days`
- Delete log files until the disk space taken falls below the specified size:\
`sudo journalctl --vacuum-size=100M`
- Delete old logs and limit file number to X:\
`sudo journalctl --vacuum-files=5`


### Link
[Free up Disk Space – Clear Systemd Journal Logs in Ubuntu 20.04](https://ubuntuhandbook.org/index.php/2020/12/clear-systemd-journal-logs-ubuntu/)


# Drive Permission
### permission in create folder and file on hard drive
```
sudo chmod -R a+rwx /path/to/folder
```