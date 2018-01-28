# Headless Raspberry PI, no GUI

###### Get image

Download Raspbian Stretch Lite from https://www.raspberrypi.org/downloads/raspbian/.

###### Get right disk name

```
diskutil list
```

###### Unmount disk

```
diskutil unmountdisk /dev/disk2
```

###### Copy image to drive

```
sudo dd if=FILE.img of=/dev/disk2 bs=2m
```

###### Set up.

Hook the Pi up to a keyboard and monitor, start the Pi, and log in using the default username (_pi_) and password (_raspberry_).

Go to the setup menu

```
sudo raspi-config
```

And select `SSH` from the `Interfacing options` menu.

Install git...

```
sudo apt-get install git-core
```

... and install docker.

```
curl -sSL https://get.docker.com | sh
```
