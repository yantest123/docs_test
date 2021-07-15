title: Krescue - take full control you khadas device
---

## What is krescue

Krescue is an extremely small (21mb) operating system that you can boot directly from a micro-SD card or your EMMC. It is a “Swiss Army knife”, and you can use it to perform a variety of low-level SBC maintenance tasks. Most notable of which are backing-up your EMMC by dumping a raw-compressed .img.gz, and rapidly installing a new OS via flashing a .img.gz back into the EMMC.  Krescue can download and install OS images directly from the web via wired Ethernet.

## Install Krescue by mirco SD card

### Means of preparation
1. A mirco SD card.
2. HDMI display，and a keyboard or a khadas remote control.
3. One of VIM1/2/3 or Edge-V
4. A PC that can be use to make the startup disk.

### Make Krescue startup disk
#### burning tool : Etcher
[Etcher](https://www.balena.io/etcher/) is an easy-to-use burning tool with good compatibility and simple operation interface. We choose this tool as the burning tool for krecure to SD card.

#### downloads Krescue images
THe Krescue images can be downloads in [there](https://dl.khadas.com/Firmware/Krescue/dump/),change you board's version.
![Kerscure_downloads](/krescue/images/vim1/Krescue_downloads.png)

#### Make the startup disk
Insert the mircosd card into the PC. Burn the downloaded image into SD card.
![Make_Krescue](/krescue/images/vim1/HowtoUseEtcher.png)


### Run
Insert the SD card into the board, connect HDMI and enter the [upgrade mode](/linux/vim3/HowtoBootIntoUpgradeMode.html),You can see that the following figure shows the successful startup of kerscure.
![boot Krescue](/krescue/images/vim1/krescue_boot.jpg)

## Install Krescue by Internet

### Means of preparation
1. A mirco SD card.
2. HDMI display，and a keyboard or a khadas remote control.
3. One of VIM1/2/3 or Edge-V which was run with a buntu firmware

### Install by Internet
1. Insert the SD card into the board, and confirm the node of the SD card, generally `/dev/mmcblk0` or `/dev/mmcblk1`. Remember the name of the node.
2. Open the terminal and run the command:
```
$ curl -sfL dl.khadas.com/.mega | sh -s - -l
```
You can see the list with firmware
![krescue firmware list](/krescue/images/vim1/krescue_list.png)
```
$ curl -sfL dl.khadas.com/.mega | sh -s - [BOARD_ID] > /dev/mmcblk0 (或者`/dev/mmcblk1`)
```
Note: When the system applies for -y parameter for "unsafe writing", the path of SD card is wrong. In this case, forced writing will be written in EMMC, resulting in the failure to run other firmware.
After the burning is completed, the image is written to the SD card. At this time, you can enter [upgrade mode] (/linux/vim3/HowtoBootIntoUpgradeMode.html) to start krecure.

## Use krescue

1. Backup and restore
With option 4, the firmware of EMMC on the board can be packed and stored in SD card. Option 3 allows you to restore the system in the SD card to the EMMC. SD card can save more than one system, put the raw.img.xz file directly under the dumps file in the SD card.

2. View board information
With the device info in option 2, you can view board configuration and other related information.

3. KBI
With option 7, the KBI of the board can be controlled.

4. Shell terminal
Select option c to start the shell terminal.

5. games
Select option 9 to kill time during mirror backup or restore.

6. others
With option 1, you can enter wizard mode;
Select option a to reboot/poweroff;
Other functions can view the related help through readme docs in option b.


## Notes

1. Select the firmware corresponding to your board model during burning. Vim3 and vim3l are different boards
2. Install and use krecure through the network. The firmware on the board is required to be Ubuntu firmware

## Mores 

What krecure can do is not only the parts mentioned in the document, but also the basic functions. For more functions, please refer to the following
https://youtu.be/ER4BOJUhoYU
https://youtu.be/vvpkbhnyhZY
https://forum.khadas.com/t/krescue-take-full-control-of-your-vim-device/5945
