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
# Curl

### Install

```
sudo apt install curl
```

# PHP

### Install

```
sudo apt install php-fpm
```
### Install 7.4

```
sudo apt install php7.4-fpm
```

To check the status of the service, run

```
systemctl status php7.4-fpm
```

### Link

- [Visit Here](https://linuxize.com/post/how-to-install-php-on-ubuntu-20-04)

# Composer

### Install

```
curl -sS https://getcomposer.org/installer -o composer-setup.php
```

```
sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```

### Link

- [Visit Here](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04)

# Valet

### Install
```
sudo apt-get install php7.4-curl
```

```
sudo apt-get install network-manager libnss3-tools jq xsel
```

```
composer global require cpriego/valet-linux
```

```
test -d ~/.composer && bash ~/.composer/vendor/bin/valet install || bash ~/.config/composer/vendor/bin/valet install
```

### Link

- [Cara Install Laravel Valet di Linux](https://www.susantokun.com/cara-install-laravel-valet-di-linux/)
- [Valet Linux Faq](https://cpriego.github.io/valet-linux/faq)

# Mysql-Server

### Install

```
sudo apt install mysql-server -y
```

```
sudo mysql
```

### Update Password

```
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'P@ssw0rd';
```

```
FLUSH PRIVILEGES;
```

```
exit
```

### Link

- [Visit Here](https://www.youtube.com/watch?v=cyNLSlL-BXQ&t=244s)

# phpmyadmin

### Install

```
sudo apt install phpmyadmin php-mbstring php-zip php-gd php-json php-curl
```

### Link

- [How To Install and Secure phpMyAdmin on Ubuntu 20.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-20-04`)

### Symlink

```
ln -s /usr/share/phpmyadmin /var/www/phpmyadmin
```

### Link

- [Symlink Github](https://gist.github.com/MnMTech/2cb40b6bf892c22eac26)

# Node Js

### Install

```
curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -
```

```
sudo apt install nodejs
```

### Link

https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/

### Update

```
sudo n latest
```

### Fix PATH:

```
sudo apt-get install --reinstall nodejs-legacy     # fix /usr/bin/node
```

### Link

https://askubuntu.com/questions/426750/how-can-i-update-my-nodejs-to-the-latest-version

# oh-my-zsh

### Install

```
sudo apt install zsh
```

Make default shell

```
chsh -s $(which zsh)
```

Install

```
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

Install PowerLeve10K theme

```
git clone https://github.com/romkatv/powerlevel10k.git $ZSH_CUSTOM/themes/powerlevel10k
```

Download Plugins for autosuggestion and syntax highlighting

```
git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions
```

```
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting
```

Now edit `~/.zshrc` file to use the PowerLeve10K theme, Awesome

```
snap install micro --classic
```

```
micro ~/.zshrc
```

Find the `ZSH_THME` and replace it with

```
ZSH_THEME="powerlevel10k/powerlevel10k"
```

Now we will add plugins\
`plugins=(git)`

```
plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
```

Save And Exit. Then Set The Terminal Design

### Link

- [Make your terminal beautiful and fast with ZSH shell and PowerLevel10K](https://medium.com/@shivam1/make-your-terminal-beautiful-and-fast-with-zsh-shell-and-powerlevel10k-6484461c6efb)

### Install Meslo Nerd Font
- [powerlevel10k](https://github.com/romkatv/powerlevel10k)

Change Font From Terminal Preferences To
- MesloLGS NF Regular 
### Uninstall

`.oh-my-zsh`\
 `ls`\
 `tools`\
 `ls`\
 `sh uninstall.sh`\
 `y`

### Link

- [Uninstall Oh My Zsh from Kali Linux](https://www.youtube.com/watch?v=L1gRxcykSb8)

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