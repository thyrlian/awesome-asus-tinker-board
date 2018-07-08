# Awesome ASUS Tinker Board
A curated list of ASUS Tinker Board resources

![Tinker Board Logo](https://github.com/thyrlian/awesome-asus-tinker-board/blob/master/resources/images/tinker_board_logo.png)

**⚠ Warning**

I take no responsibility and I am not liable for any damage caused through use of this guide.

## Hardware

### Specifications

**ASUS Tinker Board**

| Component | Details |
| --- | --- |
| CPU | Rockchip Quad-Core RK3288 processor |
| Memory | 2GB Dual Channel DDR3 |
| Graphic | Integrated Graphics Processor<br/>ARM® Mali™-T764 GPU |
| Storage | Micro SD(TF) card slot |
| LAN | RTL GB LAN |
| Wireless Data Network | 802.11 b/g/n, Bluetooth V4.0 + EDR |
| Audio | RTL ALC4040 CODEC |
| USB Ports | 4 x USB 2.0 |
| Internal I/O Ports | **1 x 40-pin header :**<br/><ul><li>up to 28 x GPIO pins</li><li>up to 2 x SPI bus</li><li>up to 2 x I2C bus</li><li>up to 4 x UART</li><li>up to 2 x PWM</li><li>up to 1 x PCM/I2S</li><li>2 x 5V power pins</li><li>2 x 3.3V power pins</li><li>8 x ground pins</li></ul>**1 x 2-pin contact pin :**<br/><ul><li>1 x PWM</li><li>1 x S/PDIF</li></ul>**1 x 15-pin MIPI DSI**<br/>**1 x 15-pin MIPI CSI** |
| Accessories | Passive heatsink<br />User manual |
| Weight | 55g |
| Dimensions | 85.60mm x 56mm x 21mm |

### Power Supply

According to the quick start guide (first edition):
> 1 x Micro USB cable and a **5V/2A** USB power adapter with **LPS** marking

According to the ASUS Tinker Board official page's FAQ:
> Tinker Board supports **5V/1~2.5A** power input, but since the SoC’s performance is high, if the connected
peripheral required huge power demand from the board, it might cause the power supply issue.
Thus we strongly recommended to use the AC adaptor with **5V/2~2.5A** power rating, plus **LPS** marking.

**Battery** supply is also possible, as long as the power output is no less than **5V/1A**.

### Tested Compatible Components

| Category | Model Name |
| --- | --- |
| SD Card | Lexar® Professional 1000x microSDXC™ UHS-II (150MB/s) 64GB |
| Power Adapter | Samsung Travel Adaptor EP-TA10EWE 5.3V/2.0A |
| Case | akasa Pi ALUMINIUM CASE for Raspberry Pi (A-RA01-A1B) |
| Case | akasa Pi ALUMINIUM CASE for Raspberry Pi and Asus Tinker Board (A-RA02-A1B) |

### CSI Camera

* Prerequisite: TinkerOS v2.0+
* [How-to](https://tinkerboarding.co.uk/wiki/index.php?title=CSI-camera)

## Configuration

### Remote Connection

* SSH is enabled by default
* [How to set up VNC server](https://www.digitalocean.com/community/tutorials/how-to-set-up-vnc-server-on-debian-8)

## TinkerOS

A Debian-based distribution ensures a smooth and functional experience.

### Flash OS Image

1. Download [**Etcher**](https://etcher.io/) - a powerful cross-platform open source OS image flasher.
2. Download **TinkerOS**.
3. Uncompress the TinkerOS file, select the **.img** file in Etcher and flash it to the SD card.  (Don't worry about the FS format, Etcher will make it **FAT32** eventually.)

### Authentication

username: `linaro`

password: `linaro`

### Download

To check your OS version:
```shell
cat /proc/version
```

**Debian**

| Version | Release Date |
| --- | --- |
| [V2.0.7](http://dlcdnet.asus.com/pub/ASUS/mb/Embedded_IPC/TinkerBoard_S/20180622-tinker-board-linaro-stretch-alip-v2.0.7.img.zip) | 2018/06/28 |
| [V2.0.5](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/TInker_Board/2GB/20180222-tinker-board-linaro-stretch-alip-v2.0.5.img.zip) | 2018/03/20 |
| [V2.0.4](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20171115-tinker-board-linaro-stretch-alip-v2.0.4.zip) | 2017/12/11 |
| [V2.0.3 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170928-tinker-board-linaro-stretch-alip-v2.0.3.img.zip) | 2017/10/30 |
| [V2.0.1 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170817-tinker-board-linaro-stretch-alip-v2.0.1.img.zip) | 2017/08/21 |
| [V1.9 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170703-tinker-board-linaro-stretch-alip-v1.9.zip) | 2017/07/12 |
| [V1.8 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170417-tinker-board-linaro-stretch-alip-v1.8.zip) | 2017/04/18 |
| [V1.6 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170330-tinker-board-linaro-jessie-alip-v16.zip) | 2017/04/01 |
| [V1.4](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170223-tinker-board-linaro-jessie-alip-v14.zip) | 2017/03/10 |
| [V1.3](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/TinkerOS_Debian.zip) | 2017/02/07 |

**Android**

| Version | Release Date |
| --- | --- |
| [V13.13.0.74](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20180206-tinker-board-android-v13.13.0.74.img.zip) | 2018/03/02 |
| [V13.12.0.43](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20171115-tinker-board-android-marshmallow-userdebug-v1312043.zip) | 2017/12/11 |
| [V13.11.0.5 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170721tinkerboard-androidmarshmallow-userdebug-v131105.zip) | 2017/08/18 |
| [V13.11.0.2 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170419-tinkerboard-android-marshmallow-userdebug131102.zip) | 2017/04/20 |
| [V13.11.0.3 Beta](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170427-tinkerboardandroidmarshmallow-userdebug-v131103.zip) | 2017/04/28 |
| [V13.11.0.4](http://dlcdnet.asus.com/pub/ASUS/mb/Linux/Tinker_Board_2GB/20170511-tinker-board-android-marshmallow-userdebug-v131104.zip) | 2017/05/15 |

## Links

* [Official Page from ASUS](https://www.asus.com/Single-Board-Computer/Tinker-Board/)
* [Driver & Tools download page](https://www.asus.com/Single-Board-Computer/Tinker-Board/HelpDesk_Download/)

## Articles

* [First Impressions: Asus Tinkerboard and Docker](https://blog.alexellis.io/first-impressions-asus-tinkerboard/) by Docker Captain [Alex Ellis](https://github.com/alexellis)
