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
