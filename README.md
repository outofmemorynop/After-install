# After-install

## Main
- **Internet**

  At first, edit the second file:
  ```
  sudo vi /etc/init.d/local.autostart
  ```
  Insert the following commands:
  ```
  #!/bin/sh
  echo 65 > /proc/sys/net/ipv4/ip_default_ttl
  ```
  Second, run the following commands:
  ```
  sudo chmod +x /etc/init.d/local.autostart
  sudo update-rc.d local.autostart defaults 80
  ```
- **Update**

  Run the following command:
  ```
  sudo apt-get -y update && sudo apt-get -y upgrade
  ```
- **Unity shell**

  Run the following command:
  ```
  sudo apt-get -y install ubuntu-desktop
  ```
- **Microphone**

  Run the following command:
  ```
  sudo apt-get -y install pavucontrol
  ```
- **lzip**

  Run the following command:
  ```
  sudo apt -y install lzip
  ```
- **vim**

  Run the following command:
  ```
  sudo apt-get -y install vim
  ```
- **mc**

  Run the following command:
  ```
  sudo apt-get -y install mc
  ```
- **7z**

  Run the following command:
  ```
  sudo apt-get -y install p7zip-full
  ```
- **git**

  Run the following command:
  ```
  sudo apt-get -y install git
  ```
- **Unity tweak tool**

  Run the following commands:
  ```
  sudo add-apt-repository -y ppa:freyja-dev/unity-tweak-tool-daily
  sudo apt-get -y update && sudo apt-get -y install unity-tweak-tool
  ```
- **lm-sensors**

  Run the following command:
  ```
  sudo apt-get -y install lm-sensors
  ```
- **gparted**

  Run the following command:
  ```
  sudo apt-get -y install gparted
  ```
- **alien**

  Run the following command:
  ```
  sudo apt-get -y install alien dpkg-dev debhelper build-essential
  ```
- **alien**

  Run the following command:
  ```
  sudo apt-get -y install alien dpkg-dev debhelper build-essential
  ```
- **jnettop**

  Run the following command:
  ```
  sudo apt-get -y install jnettop
  ```
- **iotop**

  Run the following command:
  ```
  sudo apt-get -y install iotop
  ```
- **Automount**

  Edit the second file:
  ```
  sudo vim /etc/fstab
  ```
  Insert the following commands:
  ```
  #UUID=656F1E4238CD1A6E /media/vaddemgen/windows-files ntfs defaults 0 1
  UUID=4ef65469-6b62-433f-82b9-bde4d4bb2910 /media/vaddemgen/linux-files ext4 defaults 0 1
  UUID=fcb1c92f-a0a9-48db-9a08-71d5d5164b5f /media/vaddemgen/virtual ext4 defaults 0 1
  UUID=464c3f75-dd76-4bb5-b551-2ee0c4bec1a1 /media/vaddemgen/docs ext4 defaults 0
  ```
- **firewall**

  Run the following command:
  ```
  sudo apt-get -y install gufw
  ```
- **inxi**

  Run the following command:
  ```
  sudo apt-get -y install inxi
  ```
  Example of usage:
  ```
  inxi -b
  ```
- **aidax64**

  See [Linux Extension for AIDA64](http://www.aida64.com/linux-extension-aida64)
  File is located at directory ***/media/vaddemgen/linux-files/program-files/install/system/aida/*** as file **linuxextensionforaida64.tar.gz**
- **Freedoom**

  Run the following command:
  ```
  sudo apt-get -y install prboom
  ```
- **npm**

  Run the following command:
  ```
  sudo apt-get -y install npm
  ```
- **xclip**

  Run the following command:
  ```
  sudo apt-get -y install xclip
  ```
  Example of usage:
  ```
  xclip -sel clip < ~/.ssh/id_rsa.pub
  ```
- **fish**

  Run the following commands:
  ```
  sudo apt-add-repository ppa:fish-shell/release-2
  sudo apt-get update
  sudo apt-get -y install fish
  ```
- **PuTTY**

  See [PuTTY Download Page](http://www.chiark.greenend.org.uk/~sgtatham/putty/download.html)
- **npm**

  Run the following command:
  ```
  sudo apt-get -y install npm
  ```
- **Alarm clock**

  Run the following command:
  ```
  sudo apt-get install alarm-clock-applet
  ```
- **Nvidia**

  Run the following commands:
  ```
  sudo apt install nvidia-375 -y
  sudo apt install nvidia-375-dev -y
  sudo nvidia-xconfig
  ```

## Video
- **handbrake** - the open source video transcoder.
  See [handbrake](https://handbrake.fr).

## Image
- **darktable** - is an open source photography workflow application and raw developer
  See [darktable](http://www.darktable.org).
