# Simple extension boards for Olimex GateMate A1 EVB FPGA Board

```
Extensions should be stackable, so you can use 3 extension at once.
Limit for each extension is set by 500mA resetable fuse on the extension board.
This limit of StepUP is currently 400mA if board is using 3V3 or 5V.
```

### adcIO

#### Simple ADC input

```
MAX40079 are wide band, low-noise, low-input bias
current operational amplifiers that offer rail-to-rail outputs
and single-supply operation from 2.7V to 5.5V. These low-
noise amps draw 2.2mA of quiescent supply current per
amplifier. This family of amplifiers offers ultra-low distortion
(0.0002% THD+N), as well as low input voltage-noise
density (4.2nV/√Hz) and low input current-noise density
(0.5fA/√Hz). The low input bias current of 0.3pA (typ) and
low noise(4.5nV/√Hz), together with the wide bandwidth,
provides excellent performance for transimpedance (TIA)
and imaging applications
```

![adcIO](/pic/adcIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/adcIO/adcIO.pdf)

[adcIO Request](https://github.com/chili-chips-ba/openCologne/issues/5)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### camIO

#### CSI input/ DSI output

```
Raspberry Pi compatible pinout for CSI or DSI.
4 data lines connected.
Two data lines have P and N LP pin connected.
Clock has P LP pin connected.
There are placeholders for on board termination with 100 ohm resistors.
```

![camIO](/pic/camIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/camIO/camIO.pdf)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### dualIO

```
Olimex extension to dual PMOD
We are using LSF0108PWR voltage level translator with 3.3V on PMOD side. 
You can two single or one dual PMOD board that works with 3V3.
```

![dualIO](/pic/dualIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/dualTranslation/dualTranslation.pdf)

[dualIO Request](https://github.com/chili-chips-ba/openCologne/issues/44)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### dviIO

```
As on ULX3S we have DVI in/out extension we decided to try if it will work on GateMate
```

![dviIO](/pic/dviIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/dvi/dvi.pdf)

[dviIO Request](https://github.com/chili-chips-ba/openCologne/issues/46)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### ethIO

```
The Realtek RTL8211E-VB-CG/RTL8211E-VL-CG/RTL8211EG-VB-CG are highly integrated Ethernet
transceivers that comply with 10Base-T, 100Base-TX, and 1000Base-T IEEE 802.3 standards. They
provide all the necessary physical layer functions to transmit and receive Ethernet packets over CAT.5 UTP
cable.
The RTL8211E-VB(VL)/RTL8211EG-VB uses state-of-the-art DSP technology and an Analog Front End
(AFE) to enable high-speed data transmission and reception over UTP cable. Functions such as Crossover
Detection & Auto-Correction, polarity correction, adaptive equalization, cross-talk cancellation, echo
cancellation, timing recovery, and error correction are implemented in the
RTL8211E-VB(VL)/RTL8211EG-VB to provide robust transmission and reception capabilities at
10Mbps, 100Mbps, or 1000Mbps.
Data transfer between MAC and PHY is via the Reduced Gigabit Media Independent Interface (RGMII) or
Gigabit Media Independent Interface (GMII) for 1000Base-T, 10Base-T, and 100Base-TX. The
RTL8211E-VB and RTL8211EG-VB support 3.3V or 2.5V signaling for RGMII/GMII. The
RTL8211E-VL supports 1.5/1.8V signaling for RGMII
```

![ethIO](/pic/ethIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/ethIO/ethIO.pdf)

[ethIO Request](https://github.com/chili-chips-ba/openCologne/issues/40)

This project schematic is from this repository

https://github.com/rishivg/IO-SDR

Board routing is also partially copied

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### eduIO

```
While working with Olimex GateMateA1-EVB, we realized that there was only one push-button at user disposal, whereas our TetriSaraj game needed five. Similarly the number of user LEDs is inadequate for debugging (@TsvetanUsunov, take note).

We believe that many other examples would also benefit from a richer complement of LEDs and buttons, and recommend providing a PMOD with an 8-bit bank of each.

Given that this problem is due to GateMate somewhat lower I/O count compared to FPGAs in the same category (@DadoCCAG, take note), these 16 additional lines should come from a GPIO expander based on 1-Wire protocol, and would therefore consume only one FPGA I/O pin for the gain of 16 (or more) slow user I/Os.

To enable this new PMOD hardware, we shall within this project develop RTL for 1-Wire Controller.

PCA9535 is very popular and also available on LCSC and this is just simple extension where we can test 1-Wire Controller.
```

![eduIO](/pic/eduIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/eduIO/eduIO.pdf)

[eduIO Request](https://github.com/chili-chips-ba/openCologne/issues/6)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### MikroBusIO

```
Community request

Along with Dual Pmod - MikroBus allows lot of different boards to be tested..

https://www.mikroe.com/mikrobus

More about this open standard:

https://download.mikroe.com/documents/standards/mikrobus/mikrobus-standard-specification-v200.pdf
```

![MikroBusIO](/pic/MikroBusIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/MikroBusIO/MikroBusIO.pdf)

[MikroBusIO Request](https://github.com/chili-chips-ba/openCologne/issues/48)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### pwrIO

```
Automation, industrial control and robotics projects need to drive motors and actuators. FPGA outputs typically don't have enough current and voltage capability to drive them directly.

While there are many application-specific ICs custom-tuned for a specific load, we are hereby seeking an array of generic power drivers for educational projects, which:

    students can directly drive from FPGA
    and externally connect into a topology of choice (H-Bridge, D-Class Amp, BLDC and AC motor driver, Servos, etc.).

That's to facilitate labs on this subject. While Digilent has a PMOD along these lines, ours should come with more channels and higher power capability:

    https://digilent.com/reference/pmod/pmodoc1/start
    https://digilent.com/reference/pmod/pmodod1/start
    https://digilent.com/reference/pmod/pmodhb5/start

We have also added placeholder for 2 Encoder input's
```

![pwrIO](/pic/pwrIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/pwrIO/pwrIO.pdf)

[pwrIO Request](https://github.com/chili-chips-ba/openCologne/issues/42)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### simpleIO

```
We needed a controller board for ChiliChipsBa TetriSaraj.
On this simple design we have used Joypad with one aditional button.
On this board we also have I2S audio, and 8 LEDs for debugging purposes. 
```

![simpleIO](/pic/SimpleIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/GamePad_I2S_audio_Buttons/KiCad/GamePad_I2S_audio.pdf)

[simpleIO Request](https://github.com/chili-chips-ba/openCologne/issues/9)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [x] assemble PCB
- [x] design confirmed working

### tmrIO

```
ULX3S RTC feature is very cool and unique. But, since not needed for many use-cases, we believe it is better to offer it as an add-on PMOD card.

As Digilent already has such a card:

    https://digilent.com/reference/pmod/pmodrtcc/start
    ours could also come with a relay that allows turning on/off a 2 Amp / 250V consumer. The availability of a power switch would open the RTC to a whole new set of apps without needing additional PMODs

On this board we have I2C RTC chip and two relays that can handle 250V/3A
```

![tmrIO](/pic/tmrIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/tmrIO/tmrIO.pdf)

[tmrIO Request](https://github.com/chili-chips-ba/openCologne/issues/40)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### usbIO

```
USB2.0 is affordable and ubiquitous, with peripherals ranging from HIDs to webcams, and more. However, FPGAs typically don't have a good way of direct interfacing to USB (with a notable exception of Gowin LittleBee lineup). This proposal is to bridge that gap.

We have not seen a similar PMOD on the market. The reason is that it is hard to transfer 480Mbps over a PMOD. Should we manage to do it, we would directly play into the market segment occupied by SPI Camera modules like these:

    https://www.arducam.com/spi-arduino-camera

Our PMOD could be based on one of the following technologies:

    https://www.gowinsemi.com/en/market/featured_detail/13 -- LittleBee FPGA would make it easier to transport 480Mbps over PMOD
    https://verisilicon.com/en/IPPortfolio/USB2PHY
    https://www.ti.com/lit/ds/symlink/tusb1210.pdf

Granted, there are chips that convert USB to SPI, but they are limited to 12Mbps (aka "Full Speed), thus not suitable for cameras.
```

![usbIO](/pic/usbIO.png)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/USB/USB.pdf)

[usbIO Request](https://github.com/chili-chips-ba/openCologne/issues/43)

- [x] Schematic
- [x] PCB
- [x] order PCB
- [ ] assemble PCB
- [ ] design confirmed working

### Olimex Extension template

```
If you want to design your own board, you can use this template!
```

![templateIO](/pic/templateIO.png)

[templateIO folder](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/tree/main/extension_template)

[Schematic](https://github.com/intergalaktik/Extension_Boards_for_Olimex_GateMate/blob/main/extension_template/extension_template.pdf)

## Work on this boards is financed by NLnet foundation

![NLnet](https://nlnet.nl/logo/banner.png)

![NGIEntrust](https://nlnet.nl/image/logos/NGI0Entrust_tag.svg)

This project was funded through the NGI0 Entrust Fund, a fund established by NLnet with financial support from the European Commission's Next Generation Internet programme, under the aegis of DG Communications Networks, Content and Technology under grant agreement No 101069594.

This project is done in partnership with Chili.CHIPS.ba

https://www.chili-chips.xyz/

https://nlnet.nl/project/openCologne/

https://github.com/chili-chips-ba/openCologne

## Check up our blogposts

https://intergalaktik.eu/news

## Contact us

Discord: https://discord.gg/qwMUk6W
