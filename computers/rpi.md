# Installation » Raspberry PI

## Installing OS

1. Download « Raspian OS 64-bit Lite »
2. Burn with « Raspberry Pi Imager »
3. Add « SD Card » into « Raspberry Pi » device
4. Turn on device

## Overclock Pi

1. Overclock by these command
2. `sudo nano /boot/config.txt`
3. Find `#arm_freq=700`
4. Uncomment and change `800` to `1850`
5. Add above one line `over_voltage=5`
6. Run `sudo reboot`

## Turn off HDMI

1. Run `sudo tvservice -o`

## Disable Wi-Fi and Bluetooth

```bash
sudo apt install rfkill
sudo rfkill block wifi
sudo rfkill block bluetooth
sudo reboot
```

## Add dotfiles

```bash
cd ~
git init
git remote add origin https://github.com/dalisoft/dotfiles.git
git fetch && git checkout origin/master -ft
```

## Install Docker

1. Follow guides from <https://docs.docker.com/engine/install/debian/>
2. Run `sudo apt install docker docker-compose`
3. Follow guides from <https://docs.docker.com/engine/install/linux-postinstall/>

## SSH Authorised Keys

1. Run `mkdir ~/.ssh`
2. Run `touch ~/.ssh/authorized_keys`
3. Run `ssh-copy-id -i (find ~/.ssh -name rpi.pub) pi@192.168.100.$PI_IP`

## Increase Swap Size

1. Follow guides from <https://pimylifeup.com/raspberry-pi-swap-file>

## Enable TRIM

1. Run `sudo nano /etc/udev/rules.d/plextor-EX1-Trim.rules`
2. Add `ACTION=="add|change", ATTRS{idVendor}=="0bc2", ATTRS{idProduct}=="2312", SUBSYSTEM=="scsi_disk", ATTR{provisioning_mode}="unmap"`
3. Run `sudo reboot`
4. Run `sudo systemctl start fstrim.timer`
5. Run `sudo fstrim -v /`
