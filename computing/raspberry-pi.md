Raspberry pi
============


```bash
sudo apt-get update
sudo apt-get full-upgrade -y
# sudo apt-get dist-upgrade -y
sudo rpi-update

# https://www.tomshardware.com/uk/how-to/boot-raspberry-pi-4-usb
# TODO make this modify file with sed?
sudo nano /etc/default/rpi-eeprom-update
#FIRMWARE_RELEASE_STATUS value from "critical" to "stable."
sudo rpi-eeprom-update -d -a
vcgencmd bootloader_version



sudo apt-get remove -y \
    python-configparser \

sudo apt-get install -y \
    libffi-dev \
    libssl-dev \
    python3 \
    python3-pip \
    webbrowser \
    firefox-esr \
    gimp \
    p7zip \
    exfat-fuse exfat-utils \
    sshfs \
    dosbox \
    mame \
    chocolate-doom \

    # webbrowser (need to upgrade for recent chomium)

curl -sSL https://get.docker.com | sh
sudo usermod -aG docker pi
sudo pip3 -v install docker-compose

# vscode
. <( wget -O - https://code.headmelted.com/installers/apt.sh )
# vscode alternative manual install
# https://pimylifeup.com/raspberry-pi-visual-studio-code/

# screen tearing fix - https://www.youtube.com/watch?v=6xiRUyOF7fM
sudo mv /etc/xdg/autostart/xcompmgr.desktop /etc/xdg/autostart/xcompmgr.desktop.backup

# sudo raspi-config

ssh-keygen -t rsa

# https://peppe8o.com/fixed-connect-bluetooth-headphones-with-your-raspberry-pi/
sudo usermod -G bluetooth -a pi
sudo apt-get install bluealsa pulseaudio
sudo systemctl status bluetooth.service
# service will not be running
# OH GOD! .. this guide is huge ... maybe not today .. why is this now broken :(
```


* [Raspberry Pi SD Card Speed Test](https://www.raspberrypi.org/blog/sd-card-speed-test/)
* [card advice](https://ototo.fm/best-sd-card-for-raspberry-pi-3/)
    * Example (at time) [Class 10 16GB £3.26](https://www.amazon.co.uk/dp/B07YGZHSJS/)
* [USB3 Boot](https://www.tomshardware.com/uk/how-to/boot-raspberry-pi-4-usb) Firmware update June2020
    * [USB3 Storage](https://www.amazon.co.uk/gp/product/B07FD8H2KD/) £15

external hd


* Required (£79)
    * [HDMI Screen](https://www.amazon.co.uk/dp/B016UPDUBO/) £65
    * [Logitec Keyboard](https://www.amazon.co.uk/Logitech-Business-Keyboard-Windows-Linux/dp/B003ZY9Z40/) £9
    * [Logitex Mouse](https://www.amazon.co.uk/Logitech-Optical-Ambidextrous-Mouse-Windows/dp/B00AZKNPZC) £5
* Pi 4 B+ (£89)
    * [Pi 4](https://thepihut.com/collections/raspberry-pi/products/raspberry-pi-4-model-b) (£34 2GB £54 4GB or £74 8GB)
    * [Power](https://thepihut.com/collections/raspberry-pi-power-supplies/products/raspberry-pi-psu-uk) £8
    * [Heatsink Case](https://thepihut.com/collections/raspberry-pi-cases/products/aluminium-armour-heatsink-case-for-raspberry-pi-4) £12
    * [USB3 Storage 64GB](https://www.amazon.co.uk/gp/product/B07FD8H2KD/) £15
* Pi Zero W (£31)
    * [Raspberry Pi Zero W](https://www.raspberrypi.org/products/raspberry-pi-zero-w/) £10
    * [Pi Zero Clear Case + adaptors](https://www.amazon.co.uk/GeeekPi-Raspberry-Starter-Heatsink-Screwdriver/dp/B07MGFRHHR/) £7
    * [Micro USB Power](https://thepihut.com/collections/raspberry-pi-power-supplies/products/official-raspberry-pi-universal-power-supply) £9
    * [Micro USB hub](https://thepihut.com/products/usb-mini-hub-with-power-switch-otg-micro-usb) £5
    * Optional
        * [USB Audio](https://www.amazon.co.uk/NOWBOTUCH-External-Converter-Microphone-Headphone/dp/B0894WJRW9/) £9
        * [Ethernet + 3port hub](https://www.amazon.co.uk/Nllano-USB-A3-0-Ethernet-Adapter-Aluminum/dp/B073PVB9MM/) £13 (usb3? would that work?)


* [eBay removing listed for Raspberry Pi](https://twitter.com/lbhq/status/1323482627681198080) because they COULD be used as a computer


* [CutiPi](https://cutiepi.io/) - CutiePi is a Raspberry Pi 4 tablet that turns your project into an untethered adventure. Build and create wherever an idea strikes you. No wires, no external power, and no strings attached.

Pi5
===

* Screen blanking
    * [Labwc and screen blanking with wlopm #2279](https://github.com/labwc/labwc/issues/2279)
    * [Wlopm power mode](https://forums.raspberrypi.com/viewtopic.php?t=372383)
    * https://github.com/labwc/labwc/issues/2031
    * https://www.google.com/search?q=swayidle+wlopm+wont+stay+off
