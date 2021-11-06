# Ubuntu Commands

Before Running Any Command You Need To Run
- `sudo apt update`

# Curl
### Install
- `sudo aot install curl`

# PHP
### Install 7.4
- `sudo apt install php-fpm`

Once the installation is completed, the FPM service will start automatically. To check the status of the service, run
- `systemctl status php7.4-fpm` 


### Link
https://linuxize.com/post/how-to-install-php-on-ubuntu-20-04

# Composer
### Install
- `curl -sS https://getcomposer.org/installer -o composer-setup.php` 
- `sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer`

### Link
https://www.digitalocean.com/community/tutorials/how-to-install-and-use-composer-on-ubuntu-20-04


# Valet
### Install
- `sudo apt-get install network-manager libnss3-tools jq xsel`
- `composer global require cpriego/valet-linux`
- `test -d ~/.composer && bash ~/.composer/vendor/bin/valet install || bash ~/.config/composer/vendor/bin/valet install` 

### Link
- https://www.susantokun.com/cara-install-laravel-valet-di-linux/
- https://cpriego.github.io/valet-linux/faq

# Mysql-Server 
### Install
`sudo apt install mysql-server -y`

### After Install
Run\
`sudo mysql`
Update Password
`ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'P@ssw0rd';`\
Flush\
`FLUSH PRIVILEGES;`
Exit
`exit`

### Link
https://www.youtube.com/watch?v=cyNLSlL-BXQ&t=244s

# phpmyadmin 
### Install
`sudo apt install phpmyadmin php-mbstring php-zip php-gd php-json php-curl`\
Then Set Mysql application Password
### Link
`https://www.digitalocean.com/community/tutorials/how-to-install-and-secure-phpmyadmin-on-ubuntu-20-04`

### Symlink
`ln -s /usr/share/phpmyadmin /var/www/phpmyadmin`

### Link
https://gist.github.com/MnMTech/2cb40b6bf892c22eac26

# Node Js 
### Install

`curl -sL https://deb.nodesource.com/setup_12.x | sudo -E bash -`

`sudo apt install nodejs`

### Link
https://linuxize.com/post/how-to-install-node-js-on-ubuntu-18.04/



### Update
`sudo n latest`

### Fix PATH:

`sudo apt-get install --reinstall nodejs-legacy     # fix /usr/bin/node`

https://askubuntu.com/questions/426750/how-can-i-update-my-nodejs-to-the-latest-version



  # oh-my-zsh
  ### Uinstall

  `.oh-my-zsh`\
  `ls`\
  `tools`\
  `ls`\
  `sh uninstall.sh`\
  `y`

### Link
`https://www.youtube.com/watch?v=L1gRxcykSb8`



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