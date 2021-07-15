title: Edge Beginners Guide
---

## Edge
![image](/android/images/edge/docs_edge_labels.jpg)

<ul class="nav nav-tabs" id="myTab" role="tablist">
  <li class="nav-item" role="presentation">
    <a class="nav-link active" id="front-tab" data-toggle="tab" href="#front-edge" role="tab" aria-controls="front" aria-selected="true">Front(Blue)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="back-tab" data-toggle="tab" href="#back-edge" role="tab" aria-controls="back" aria-selected="false">BACK(RED)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="button-tab" data-toggle="tab" href="#button-edge" role="tab" aria-controls="button" aria-selected="false">BUTTONS</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="led-tab" data-toggle="tab" href="#led-edge" role="tab" aria-controls="led" aria-selected="false">Indicator LEDs</a>
  </li>
</ul>
<div class="tab-content" id="myTabContent">
<div class="tab-pane fade show active" id="front-edge" role="tabpanel" aria-labelledby="front-tab">

||Component|Purpose|
|---:|:---|:---|
|1|USB-A|USB 3.0 speeds|
|2|USB-C|USB 3.0, Display Port v1.2, with 5-[20V](https://www.khadas.com/product-page/usb-c-24w-adapter) input (USB power delivery), can be used for [upgrading the OS](/android/edge/UpgradeViaUSBCable.html)|
|3|HDMI 2.0|Type-A Female, up to 4K@60Hz, HDCP 2.2|
|4|USB-C|USB-C port with 5-[20V](https://www.khadas.com/product-page/usb-c-24w-adapter) input (USB power delivery)|
|5|USB-A|USB 2.0 speeds|
|6|Fan Header|4-wire [fan](https://www.khadas.com/product-page/3705-cooling-fan) header utilising pulse width modulation|
|7|Reset Button|Force reboot your Edge in the event of a system freeze|
|8|Function Button|Press this 3 times in 2 seconds to [enter MaskROM mode](/android/edge/HowtoBootIntoUpgradeMode.html)|
|9|Power Button|This button turns on your Edge|
|A|314-Pin Gold Fingers|For docking with expansion boards such as the [Captain](https://www.khadas.com/product-page/captain-carrier-board)|
|B|I-Pex [Wi-Fi](/android/edge/HowToConnectWifi.html) / Bluetooth Connector|Connect Wi-Fi / Bluetooth antennas|
|C|I-Pex Wi-Fi / [Bluetooth](/android/edge/HowToSetupBluetooth.html) Connector|Connect Wi-Fi / Bluetooth antennas|

</div>
<div class="tab-pane fade" id="back-edge" role="tabpanel" aria-labelledby="back-tab">

||Component|Purpose|
|---:|:---|:---| 
|1|Li-Po Battery Connector|For connecting Lithium Polymer batteries|
|2|Secondary Wi-Fi / Bluetooth Pad|Extra pad for mounting Wi-Fi / Bluetooth antennas|
|3|Secondary Wi-Fi / Bluetooth Pad|Extra pad for mounting Wi-Fi / Bluetooth antennas|
|4|M2x4 Mounting Point|For mounting a [heatsink](https://www.khadas.com/product-page/edge-heatsink) or [carrier board](https://www.khadas.com/product-page/captain-carrier-board)|
|5|FPC Connector B|10-Pins, 0.5mm Pitch, USB, I2S(8ch), I2C, MCU IOs|
|6|FPC Connector A|10-Pins, 0.5mm Pitch, UART, I2C, SPI, SDMMC, ADC, PWM, IOs. To add GPIO, use [Edge IO](https://www.khadas.com/product-page/edge-io)|
|7|M-Register|Allows the EMMC to [enter MaskROM mode](/android/edge/HowtoBootIntoUpgradeMode.html)|

</div>
<div class="tab-pane fade" id="button-edge" role="tabpanel" aria-labelledby="button-tab">

|Reset|Function|Power|Purpose|
|:---:|:---:|:---:|:---|
|x|||Force Reboot Edge|
||x||[Enter Upgrade Mode (TST)](/android/edge/HowtoBootIntoUpgradeMode.html)|
|||x|Power On/Wake Up Edge|
|x||x|[Enter Upgrade Mode (KEYS)](/android/edge/HowtoBootIntoUpgradeMode.html)|

</div>
<div class="tab-pane fade" id="led-edge" role="tabpanel" aria-labelledby="led-tab">

|Colour|Behaviour|Meaning|
|---:|:---:|:---|
|Blue|OFF|Power source disconnected|
||Solid ON|Power source connected, SBC turned off|
|White|OFF|SBC turned off|
||Solid ON|SBC turned on|
|Red|None|None|

The above behaviours are default out-of-the-box, and can be altered by a user. For example the white LED can be made to blink or breathe. For more information on how to program them via your favourite OS (each OS is different), please consult with experts at [forum.khadas.com](https://forum.khadas.com).

</div>
</div> 


## Edge-V
![image](/android/images/edge/docs_edge_v_labels.jpg)

<ul class="nav nav-tabs" id="myTab" role="tablist">
  <li class="nav-item" role="presentation">
    <a class="nav-link active" id="front-tab" data-toggle="tab" href="#front-edgev" role="tab" aria-controls="front" aria-selected="true">Front(Blue)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="back-tab" data-toggle="tab" href="#back-edgev" role="tab" aria-controls="back" aria-selected="false">BACK(RED)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="button-tab" data-toggle="tab" href="#button-edgev" role="tab" aria-controls="button" aria-selected="false">BUTTONS</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="led-tab" data-toggle="tab" href="#led-edgev" role="tab" aria-controls="led" aria-selected="false">Indicator LEDs</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="gpio-tab" data-toggle="tab" href="#gpio-edgev" role="tab" aria-controls="gpio" aria-selected="false">GPIO Pinout</a>
  </li>
</ul>
<div class="tab-content" id="myTabContent">
<div class="tab-pane fade show active" id="front-edgev" role="tabpanel" aria-labelledby="front-tab">

||Component|Purpose|
|---:|:---|:---|
|1|USB-A|USB 3.0, blue colour|
|2|RJ-45|Gigabit Ethernet with [Wake-On-LAN (WOL)](/android/edge/HowtoUseWol.html)|
|3|HDMI|Type-A Female, up to 4K@60Hz, HDCP 2.2|
|4|USB-C|USB 3.0, Display Port v1.2, can be used for [upgrading the OS](/android/edge/UpgradeViaUSBCable.html)|
|5|USB-A|USB 2.0, black colour|
|6|Fan Header|4-wire [fan](https://www.khadas.com/product-page/3705-cooling-fan) header utilising pulse width modulation|
|7|Reset Button|Force reboot your Edge-V in the event of a system freeze|
|8|Function Button|Press this 3 times in 2 seconds to [enter MaskROM mode](/android/edge/HowtoBootIntoUpgradeMode.html)|
|9|Power Button|This button turns on your Edge-V|
|A|RTC Battery Header|Header for attaching a battery for the real time clock|
|B|[40-Pin GPIO](/android/edge/EdgeVGPIOPinout.html)|Learn how to access GPIO [here](/android/edge/HowToAccessGpio.html), or use it to add a [Toneboard](https://www.khadas.com/product-page/tone-board)|
|C|Gesture Sensor|Control your Edge-V with a hand-wave|
|D|Infrared Module|2-channel infrared receiver for use with [Khadas IR remote](https://www.khadas.com/product-page/ir-remote)|
|E|LEDs|Status indicator LEDs|
|F|I-Pex [Wi-Fi](/android/edge/HowToConnectWifi.html) / [Bluetooth](/android/edge/HowToSetupBluetooth.html) Connector|Wi-Fi / BT Antenna connector|
|G|I-Pex [Wi-Fi](/android/edge/HowToConnectWifi.html) / [Bluetooth](/android/edge/HowToSetupBluetooth.html) Connector|Wi-Fi / BT Antenna connector|

</div>
<div class="tab-pane fade" id="back-edgev" role="tabpanel" aria-labelledby="back-tab">

||Component|Purpose|
|---:|:---|:---|
|1|Li-Po Battery Connector|Connect a [Lithium Polymer battery](https://www.khadas.com/product-page/lipo-battery) with the [Juice Board](https://www.khadas.com/product-page/juice-board)|
|2|USB-C|USB-C port that accepts 5-[20V](https://www.khadas.com/product-page/usb-c-24w-adapter) power input (USB power delivery)|
|3|[Micro-SD Card Slot](/android/edge/UpgradeViaTFBurningCard.html)|Boot alternative OSes via a Micro-SD card, or just for extra storage|
|4|M.2 Socket (PCI-E 2.1)|Connect 2280 NVMe SSDS at 4-lane speed with [M2X Extension](https://www.khadas.com/product-page/m2x-extension-board)|
|5|E-DP Display|For connecting to external displays via E-DP|
|6|M2x4 Mounting Point|For mounting to [cases](https://www.khadas.com/product-page/diy-case) and [heatsinks](https://www.khadas.com/product-page/new-vim-heatsink)|
|7|Touch Panel|For accepting [touch-input](/android/edge/ConnectLcd.html)|
|8|MIPI-TX|MIPI-DSI header for connecting [LCD screens](/android/edge/ConnectLcd.html)|
|9|MIPI-RX|For connecting to [MIPI-CSI cameras](https://www.khadas.com/product-page/imx214-13mp-camera)|
|A|MIPI-RX/TX|Configurable, connect to [MIPI-CSI cameras](https://www.khadas.com/product-page/imx214-13mp-camera) or MIPI-DSI displays|
|B|M-Register|Another way for entering [upgrade mode](/android/edge/HowtoBootIntoUpgradeMode.html)|

</div>
<div class="tab-pane fade" id="button-edgev" role="tabpanel" aria-labelledby="button-tab">

|Reset|Function|Power|Purpose|
|:---:|:---:|:---:|:---|
|x|||Force Reboot Edge-V|
||x||[Enter Upgrade Mode (TST)](/android/edge/HowtoBootIntoUpgradeMode.html)|
|||x|Power On/Wake Up Edge-V|
|x||x|[Enter Upgrade Mode (KEYS)](/android/edge/HowtoBootIntoUpgradeMode.html)|

</div>
<div class="tab-pane fade" id="led-edgev" role="tabpanel" aria-labelledby="led-tab">

|Colour|Behaviour|Meaning|
|---:|:---:|:---|
|Blue|OFF|Power source disconnected|
||Solid ON|Power source connected, SBC turned off|
|White|OFF|SBC turned off|
||Solid ON|SBC turned on|
|Red|None|None|

The above behaviours are default out-of-the-box, and can be altered by a user. For example the white LED can be made to blink or breathe. For more information on how to program them via your favourite OS (each OS is different), please consult with experts at [forum.khadas.com](https://forum.khadas.com).

</div>
<div class="tab-pane fade" id="gpio-vim" role="tabpanel" aria-labelledby="gpio-tab">

SIGNAL| PIN|PIN|SIGNAL
---|:---|:---|:---
5V|1|21|GND
5V|2|22|SPI3_RXD/I2C0_SCK/GPIO1_C0
HOST1_DM|3|23|SPI3_TXD/I2C0_SDA/GPIO1_B7
HOST1_DP|4|24|GND
GND|5|25|I2C2_SCL/GPIO2_A1
MCU_TX|6|26|I2C2_SDA/GPIO2_A0
MCU_NRST|7|27|3.3V
MCU_SWIM|8|28|GND
GND|9|29|I2S0_SCLK/GPIO3_D0
ADC_IN2|10|30|I2S_CLK/GPIO4_A0
1.8V|11|31|I2S0_SDO0/GPIO3_D7
ADC_IN3|12|32|2S0_LRCK_TX/GPIO3_D2
SPDIF/GPIO3_C0|13|33|I2S0_SDI0/GPIO3_D3
GND|14|34|GND
SPI3_CS/GPIO1_C2|15|35|I2S0_SDI3SDO1/GPIO3_D6
SPI3_CLK/GPIO1_C1|16|36|2S0_SDI2SDO2/GPIO3_D5
GND|17|37|I2S0_SDI1SDO3/GPIO3_D4
Linux_RX|18|38|I2S0_LRCK_RX/GPIO3_D1
Linux_TX|19|39|MCU_PA1
3.3V|20|40|GND

</div>
</div>


## Captain
![image](/android/images/edge/docs_captain_labels.jpg)

<ul class="nav nav-tabs" id="myTab" role="tablist">
  <li class="nav-item" role="presentation">
    <a class="nav-link active" id="front-tab" data-toggle="tab" href="#front-captain" role="tab" aria-controls="front" aria-selected="true">Front(Blue)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="back-tab" data-toggle="tab" href="#back-captain" role="tab" aria-controls="back" aria-selected="false">BACK(RED)</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="button-tab" data-toggle="tab" href="#button-captain" role="tab" aria-controls="button" aria-selected="false">BUTTONS</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="led-tab" data-toggle="tab" href="#led-captain" role="tab" aria-controls="led" aria-selected="false">Indicator LEDs</a>
  </li>
  <li class="nav-item" role="presentation">
    <a class="nav-link" id="gpio-tab" data-toggle="tab" href="#gpio-captain" role="tab" aria-controls="gpio" aria-selected="false">GPIO Pinout</a>
  </li>
</ul>
<div class="tab-content" id="myTabContent">
<div class="tab-pane fade show active" id="front-captain" role="tabpanel" aria-labelledby="front-tab">

||Component|Purpose|
|---:|:---|:---|
|1|RK3399 SoC Heat Spreader|Metallic layer for reducing heat concentration|
|2|RJ-45|Gigabit Ethernet port with [Wake-On-LAN (WOL)](/android/edge/HowtoUseWol.html)|
|3|[40-Pin GPIO](/android/edge/CaptainGPIOPinout.html)|Learn how to access the GPIO [here](/android/edge/HowToAccessGpio.html)|
|4|RTC Header|For connecting an external button battery for the real-time clock|
|5|Reset Button|Forcefully reboot Edge+Captain if your system freezes|
|6|12V DC Barrel Jack|Alternative [12V DC power input](https://www.khadas.com/product-page/captain-12v-adapter), see [power priority](/android/edge/EdgeCaptainPowerPriority.html)|
|7|Micro-SD Card Slot|Boot additional OSes via [Micro-SD](/android/edge/UpgradeViaTFBurningCard.html), or just for extra storage|
|8|Buzzer|Produces simple sounds|
|9|Gesture Sensor|Control your Edge+Captain with a hand-wave|
|A|IR Receiver|2-channel infrared module, for use with the [Khadas IR remote](https://www.khadas.com/product-page/ir-remote)|
|B|Right Game Pad|For games, use with the [Kap Case](https://www.khadas.com/product-page/kap-case)|
|C|Left Game Pad|For games, use with the [Kap Case](https://www.khadas.com/product-page/kap-case)|
|D|USIC|Legacy USB-bus, unpopular|
|E|E-DP Display|For connecting to external displays via E-DP|
|F|Touch Panel|For accepting [touch-input](/android/edge/ConnectLcd.html)|
|G|MIPI-TX|MIPI-DSI header for connecting [LCD screens](/android/edge/ConnectLcd.html)|
|H|MIPI-RX/TX|Configurable MIPI-CSI/DSI header|
|I|MIPI-RX|For connecting to [MIPI-CSI cameras](https://www.khadas.com/product-page/imx214-13mp-camera)|
|J|3.5mm Audio Jack|Audio output, works with the [Kap Case](https://www.khadas.com/product-page/kap-case)|
|K|Function Button|For entering [upgrade mode](/android/edge/HowtoBootIntoUpgradeMode.html)|
|L|Microphone|Audio input|
|M|MXM3 Connector|For docking with the [Edge](https://www.khadas.com/product-page/edge)|
|N|[Wi-Fi](/android/edge/HowToConnectWifi.html) / [Bluetooth](/android/edge/HowToSetupBluetooth.html) Chip Antenna|Wi-Fi and BT antenna|
|O|[Wi-Fi](/android/edge/HowToConnectWifi.html) / [Bluetooth](/android/edge/HowToSetupBluetooth.html) Chip Antenna|Wi-Fi and BT antenna|
|P|M3 Clearance Hole|For mounting and cases, such as the [Kap Case](https://www.khadas.com/product-page/kap-case)|
|Q|M2 Threaded Stand-Off|For mounting the [Edge](https://www.khadas.com/product-page/edge)|

</div>
<div class="tab-pane fade" id="back-captain" role="tabpanel" aria-labelledby="back-tab">

||Component|Purpose|
|---:|:---|:---|
|1|[M.2 Socket (PCI-E 2.1)](/android/edge/ListOfCompatibleNVMeSSDs.html)|Connect directly to 2280 NVMe SSDs|
|2|External Speaker & DMIC Input FPC Connector|Connecting to an external speaker| 
|3|[M.2 2280 Stand-Off (M2 Threaded)](/android/edge/ListOfCompatibleNVMeSSDs.html)|Boss for securing an SSD to the Captain|
|4|Lithium Polymer Battery Connector|Add a [2-Cell Li-Po battery](https://www.khadas.com/product-page/lipo-battery) for portable usage, see [power priority](/android/edge/EdgeCaptainPowerPriority.html)|
|5|Right Function Button|User programmable button|
|6|Left Function Button|User programmable button|

</div>
<div class="tab-pane fade" id="button-captain" role="tabpanel" aria-labelledby="button-tab">

|Reset|Function|Left Gamepad|Right Gamepad|Left Function|Right Function|Purpose|
|:---:|:---:|:---:|:---:|:---:|:---:|:---|
|x||||||Force reboot Edge+Captain if the system freezes|
||x|||||[Enter Upgrade Mode (TST)](/android/edge/HowtoBootIntoUpgradeMode.html)|
|||x||||User programmable button|
||||x|||User programmable button|
|||||x||User programmable button|
||||||x|User programmable button|

</div>
<div class="tab-pane fade" id="led-captain" role="tabpanel" aria-labelledby="led-tab">

|Colour|Behaviour|Meaning|
|---:|:---:|:---|
|Blue|OFF|Power source disconnected|
||Solid ON|Power source connected, SBC turned off|
|White|OFF|SBC turned off|
||Solid ON|SBC turned on|
|Red|None|None|

The above behaviours are default out-of-the-box, and can be altered by a user. For example the white LED can be made to blink or breathe. For more information on how to program them via your favourite OS (each OS is different), please consult with experts at [forum.khadas.com](https://forum.khadas.com).

</div>
<div class="tab-pane fade" id="gpio-vim" role="tabpanel" aria-labelledby="gpio-tab">

SIGNAL| PIN|PIN|SIGNAL
---|:---|:---|:---
5V|1|21|GND
5V|2|22|SPI3_RXD/I2C0_SCK/GPIO1_C0
HOST1_DM|3|23|SPI3_TXD/I2C0_SDA/GPIO1_B7
HOST1_DP|4|24|GND
GND|5|25|I2C2_SCL/GPIO2_A1
MCU_TX|6|26|I2C2_SDA/GPIO2_A0
MCU_NRST|7|27|3.3V
MCU_SWIM|8|28|GND
GND|9|29|I2S0_SCLK/GPIO3_D0
ADC_IN2|10|30|I2S_CLK/GPIO4_A0
1.8V|11|31|I2S0_SDO0/GPIO3_D7
ADC_IN3|12|32|2S0_LRCK_TX/GPIO3_D2
SPDIF/GPIO3_C0|13|33|I2S0_SDI0/GPIO3_D3
GND|14|34|GND
SPI3_CS/GPIO1_C2|15|35|I2S0_SDI3SDO1/GPIO3_D6
SPI3_CLK/GPIO1_C1|16|36|2S0_SDI2SDO2/GPIO3_D5
GND|17|37|I2S0_SDI1SDO3/GPIO3_D4
Linux_RX|18|38|I2S0_LRCK_RX/GPIO3_D1
Linux_TX|19|39|MCU_PA1
3.3V|20|40|GND

</div>
</div>

## Captain + Edge
![image](/android/images/edge/docs_captain_with_edge_labels.jpg)

* Front (Yellow)
||Component|Purpose|
|---:|:---|:---|
|1|[314-Pin "Edge Connector"](https://www.khadas.com/product-page/edge)|Data and power interface between Edge & Captain|
|2|RockChip RK3399 SoC|x2 1.8GHz A72, x4 1.5GHz A53|
|3|M2x4 Screw|Use M2 screws to secure to the Captain|
|4|[USB-C Power Delivery (5-20V)](/android/edge/EdgeCaptainPowerPriority.html)|USB-C power input|
|5|[USB-C (3.0 + Display Port)](/android/edge/UpgradeViaUSBCable.html)|USB-C power input, and display port output|
|6|USB-A|USB 3.0 speed|
|7|USB-A|USB 2.0 speed|
|9|HDMI|HDMI 2.0 and CEC|

## Edge Power Supply
Although your Edge SBC is compatible with various types of power supplies, these are the recommended specs for the best performance-output and stability.

![image](/android/images/edge/usb-c_adapter_24w_2.jpg)

1. Khadas USB-C 24W Power Adapter (USB Power Delivery)
2. Khadas USB-C Cable (Male-to-Male)

{% note info Tip %}
These items are now available at Khadas Shop
{% endnote %}

**Learn More:**
* [Edge+Captain Power Priority](/android/edge/EdgeCaptainPowerPriority.html)
* [Khadas Edge Specifications](https://khadas.com/edge)
* [Khadas Edge Accessories](https://www.khadas.com/edge-add-ons)

## Displays & User Input
These items are useful when you need to connect your Edge SBC to an external display + keyboard mouse + remote control, for use as a desktop computer or media center. *Edge series SBCs have USB-C display-port capability, which allows them to connect directly to Type-C enabled 4K monitors, to exchange power, data, video, and audio over a single cable.*

1. 4K HDMI 2.0 Cable
2. HDMI-Compatible 1080P/4K Monitor w/ USB Type-C
3. Wireless USB Keyboard + Mouse
4. CEC-Compatible Remote Control

**Learn More:**
* [Khadas Shop - HDMI Cable](https://www.khadas.com/product-page/hdmi-cable)
* [Khadas Shop - Remote Control](https://www.khadas.com/product-page/ir-remote)
* [Amazon - LG 4K Monitor w/ USB Type-C](https://www.amazon.com/LG-27UD88-W-LED-Lit-Monitor-Type-C/dp/B01CDYB0QS/ref=sr_1_7?ie=UTF8&qid=1543993886&sr=8-7&keywords=usb-c+compatible+monitor)
* [Amazon - Wireless Keyboard + Mouse](https://www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Delectronics&field-keywords=wireless+keyboard+and+mouse&rh=n%3A172282%2Ck%3Awireless+keyboard+and+mouse)


{% note info Note %}
Please do not attach multiple cables with large heads that interfere with each other, as that may bend or twist the connectors, and this will cause intermittent connectivity issues after some time.
{% endnote %}

## Making Bootable / Burning SD-Cards / Thumbdrives
These items are useful when you want to upgrade your Edge SBC's operating system via SD-Card or Thumbdrive (Burning Cards). Or if you want to run operating systems that can only be run from external media (Booting Cards) like LibreELEC.

1. 8GB or Larger, SD-Card
2. SD-Card Reader
3. Laptop / Desktop PC
4. 8GB or Larger, USB-Thumbdrive (U-Disk)

**Learn More:**
* [Booting Card Vs Burning Card](/android/edge/BootingCardVsBurningCard.html)
* [Upgrade Using SD-Card](/android/edge/UpgradeViaTFBurningCard.html)
* [Boot From External Media](/android/vim2/BootFromExtMedia.html)
* [Enter Upgrade Mode](/android/edge/HowtoBootIntoUpgradeMode.html)

{% note info Tip %}
* **eMMC image** should be burned directly to the eMMC using a USB-C data cable, from a Ubuntu or Windows Host. It must not be burned into an SD-Card. For Example: Android and Ubuntu distributions containing the `EMMC` mark.
* **SD/USB image** should be copied into an SD-Card, before that card is then used to reformat the eMMC storage with a new OS. For Example: Armbian, Ubuntu distributions containing the `SD_USB` mark, as well as LibreELEC and CoreELEC.
* In order to bootup from **SD/USB images**, you need Android (V180209 or newer) or Ubuntu (V180531 or newer) running on your eMMC with Multi-Boot activated.
{% endnote %}

## Upgrading eMMC Operating System Using USB-C Cable
You'll need these items if you want to use your laptop or desktop PC to upgrade your Edge SBC's operating system stored in its eMMC storage. For example, changing the bootup operating system from Android to Ubuntu, or installing a more exotic 3rd-party OS.

1. USB-A to USB-C Data Cable (Legacy Computers)
2. USB-C to USB-C Data Cable (Modern Computers)
3. Laptop / Desktop PC

**Learn More:**
* [Upgrade Using USB-C Cable](/android/edge/UpgradeViaUSBCable.html)
* [Boot Into Upgrade Mode](/android/edge/HowtoBootIntoUpgradeMode.html)

**Firmware Images:**
* [Android OS](/android/edge/FirmwareAndroid.html)
* [Ubuntu OS](/android/edge/FirmwareUbuntu.html)

## Watching Movies, Expanding Internal eMMC Storage
These items are useful if you wish to use your Edge-V or Edge+Captain SBC as a media center, for storing/downloading large movie files. A microSDXC UHS-I card is expensive, but its also fast enough for 4K video playback. An external NVMe M.2 socket SSD will also be large enough to contain your entire media library.

1. NVMe PCIe M.2 2280 SSD
2. *microSDXC UHS-I* SD-Card

**Learn More:**
* [Amazon - Samsung 970 EVO NVMe SSD](https://www.amazon.com/Samsung-970-EVO-500GB-MZ-V7E500BW/dp/B07BN4NJ2J/ref=sr_1_3?ie=UTF8&qid=1543993490&sr=8-3&keywords=samsung+m.2+ssd)
* [Amazon - microSDXC UHS-I SD-Card](https://www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Daps&field-keywords=microSDXC+UHS-I&rh=i%3Aaps%2Ck%3AmicroSDXC+UHS-I)

## Software Development / Advanced Crash Recovery
*Edge series SBCs are equipped with "Terry's Smart Tweezers" for crash recovery without the need for conductive metal tweezers, even when the bootloader is damaged.* Extreme cases of crash-recovery will require you to use the MRegister to reset your Edge SBC. A USB Serial Debug Tool is also useful for developers debugging complex software issues. 

1. Your Fingers (For resetting a dead SBC via Terry's Smart Tweezers)
2. Conductive Metal Tweezers (For resetting a dead SBC via MRegister)
3. USB Serial Debug Tool (For diagnosing software/hardware issues)

**Learn More:**
* [Terry's Smart Tweezers](/android/edge/HowtoBootIntoUpgradeMode.html)
* [MRegister Upgrade Mode](/android/edge/HowtoBootIntoUpgradeMode.html)
* [Amazon - Metal Tweezers](https://www.amazon.com/s/ref=nb_sb_noss_2?url=search-alias%3Daps&field-keywords=metal+tweezers)
* [Amazon - USB Serial Debug Tool](https://www.amazon.com/s/ref=nb_sb_noss?url=search-alias%3Daps&field-keywords=usb+serial+debug+tool&rh=i%3Aaps%2Ck%3Ausb+serial+debug+tool)

## Edge Website
For more information, please see our website, read more documentation, or visit our forum.
* [Khadas Edge Homepage](https://www.khadas.com/edge)
* [Khadas Edge Forum](https://forum.khadas.com/c/Khadas-Edge)
