# Ubuntu Commands

Before Running Any Command You Need To Run\
`sudo apt update`

# Curl
### Install
`sudo aot install curl`

# PHP
### Install 7.4
`sudo apt install php-fpm`

Once the installation is completed, the FPM service will start automatically. To check the status of the service, run\
`systemctl status php7.4-fpm`


# Composer
### Install
First\
`curl -sS https://getcomposer.org/installer -o composer-setup.php`\
Then\
`sudo php composer-setup.php --install-dir=/usr/local/bin --filename=composer`

### Link
https://linuxize.com/post/how-to-install-php-on-ubuntu-20-04

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