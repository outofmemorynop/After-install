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

  At first, edit the file:
  ```
  sudo gedit /etc/apt/sources.list
  ```
  
