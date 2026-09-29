# Vintage AM Radio Inspired Offline MP3 Player PCB

***Complete PCB design files and documentation coming soon!***

## Announcements 

- ***NEW:*** [26.0.2 firmware](https://github.com/mloit/zbvr-firmware) (Latest release available on the [Releases page](https://github.com/mloit/zbvr-firmware/releases/latest))

- ***New:*** [Big Speaker Option](./docs/Big%20Speaker%20Assembly%20Guide.md)

- ***New*** BOM's for PCB upgrade and battery module (see below)

- ***Coming Soon:*** Battery module PCB and assembly guides

---

Want to support my efforts? Feel free to [Buy me a Coffee][support]
---

## Docs
- [PCB Assembly Guide](./docs/PCB%20Assembly%20Guide.md)

- [Wiring Harness Assembly Guide](./docs/Wiring%20Harness%20Assembly%20Guide.md)


## Errata
A number of boards have been exhibiting a problem when turning on the radio via the potentiometer, the connection to Thonny (or other serial terminal) is lost. This appears to be due to a dip in voltage as a result of the inrush current to charg up the amplifier circuit. To address this I recommend soldering a 100uF electrolytic (Digikey: 1189-2195-ND, or similar) between the 5V and Gnd pins of the GPIO connector (J10) located between the RP-Zero and the DFPlayer

---
## The PCB
![alt text][pcb]

### Schematic 
(Click Image for PDF)
[![alt text][sch]](./assets/zbvr-pwb-v1-a-sch.pdf)


### Top/Component Side of PCB:
![alt text][front]

### Bottom/Solder Side of PCB:
![alt text][back]


---

## Building your own

The first step to building your own will be to get your hands on a bare PCB. PCB's can currently be ordered from our [Community project at PCBWay][pcbway]. This is currently the preferred route as we do earn a small commission on every board ordered from there to help support the project (anything earned on the PCB's is shared between Zion and myself). Also please note that if you plan to resell the PCB's we ask that you fill out a [license application][zion-lic] on Zion's project site.

For the components you can use this [list at DigiKey][dk-pcb] as a starting point. The list includes everything except the speakers, RP2040-Zero, and push-button, for the basic configuration of the PCB. Details on a more complete configuration for external power and a battery will be provided in the near future.

In terms of the 3D printed parts, for the PCB version you want to print the "Shell Normal - with button" version of the shell, from the "Shells" 3MF profile. From the "Mounts" 3MF profile you want to print the "Circuit Board Mount (PCB Version)" plate. (Optionally, if building for the "Big Speaker Option", you would print that mount instead)  All other radio parts (except for the back plate, see next section) are common, and the same for any version of the device. You may optionally print the "Soldering Aids" 3MF for some jigs and tools to make assembling the PCB a bit easier.

#### Radio Back Plate

Depending on which verion of the PCB you are plannning to build/use the back plate changes. The "Standard" version is powered by USB, while the "Full" version used with the battery option requires an external DC power supply. (The full version can be used without the battery, but still requires the external DC supply) The Full version is not compatable with being powered over USB, as such 2 versions of the back plate have been designed. One with the USB opening for the "Standard" buikd, and one with a hole for the external DC suppply for the "Full" version. Please be sure to print the correct version of the back plate for the version of the PCB you are going to assemble. 

- Standard PCB Build: "Back Plate for PCB Version"
- Full PCB Build: "Back Plate for PCB Battery Version"

#### Battery & Big Speaker Options

Note that the "Big Speaker Option" profile I have here currently does not have mounts for the battery module. I will be updating this soon to add the mounting points. If building now, I recommend using Hook and Loop (Velcro) adhesive fastener strips to attach he battery module to the back of the speaker shell. All versions of the PCB here support the big speaker, so no changes are required on the PCB itself.

Note the BOM's for the battery do NOT include teh external DC supplpy, as it will depend on your region. The requrements are 10W or more power, 9-12V. 5.5mm barrel with 2.1mm pin, centre positive.

- Example for North America: [GlobTek WR9HD1333CCP-F(R6B)][dk-psu-us] (Digikey)

### Before you purchase components
The board is designed to support either the amplifier module from DigiKey, or the amplifier module originally demonstrated by Zion in his video, from Amazon. If you have already purchased components from Amazon, you can omit getting them from the list provided above. Note that if you are going with the Amazon Amplifier this affcts a few lines in the list. With the exception of the items mentioned earlier, this list here effectively replaces teh BOM currently on Zion's site.

#### If you have already purchased, or plan to use the amplifier module from Amazon

**Remove** the following 3 line items:
1. Line 2: DFR0119-O (PAM8403 Eval board) Digikey P/N: 1738-1041-ND
2. Line 26: PPTC041LFBN-RC (1x4 pos female header 2.54mm) Digikey P/N: S7002-ND
3. Line 27: PPTC061LFBN-RC (1x6 pos female header 2.54mm) Digikey P/N: S7004-ND

**Add** the following 2 items:
1. PPTC021LFBN-RC (1x2 pos female header 2.54mm) DigiKey P/N: S7000-ND - Quantity 3 per board
2. PPTC031LFBN-RC (1x3 pos female header 2.54mm) DigiKey P/N: S7001-ND - Quantity 1 per board

#### Notes on the BoM (Bill of Materials)

There are several bills of materials for the PCB, depending on which version you want to build, or are upgrading from one to the other. They all use the same base Radio PCB but are populated differently.

##### Standard Build (USB Powered)

If building the standard version fo the PCB, as featuerd in Zion's original videos about the PCB, you want to use this BOM. (Note that this version does not include support for the battery option)

- [Standard PCB Components][dk-pcb] (DigiKey)
- [Standard PCB Components Alternate][dk-pcb-alt] (DigiKey) -- for when you are using the amplifier from Amazon
- [Amplifier Module][amp] (Amazon) -- Optional/Alternate
- [RP2040-Zero][rp] (Amazon)

##### Full Build (External Powered or Battery Powered)

If you want your radio to be powered by an external DC supply, or be powered by the battery module use this BOM if building a new board. If upgrading an existing board, use the upgrade BOM below. Note that if planning to use the battery module, you need to also get the items in the "Battery Only" BOM below. Note while I have not amde an alternalte BOM for this version, you can make teh same changes as noted above if using the amplifier from Amazon.

- [Full PCB Components][dk-pcb-full] (DigiKey)
- [Amplifier Module][amp] (Amazon) -- Optional/Alternate
- [RP2040-Zero][rp] (Amazon)

**Note:** the BOM does NOT include teh external DC supplpy, as it will depend on your region. The requrements are 10W or more power, 9-12V. 5.5mm barrel with 2.1mm pin, centre positive.

- Example for North America: [GlobTek WR9HD1333CCP-F(R6B)][dk-psu-us] (Digikey)


##### Standard to Full Upgrade (with Battery)

This BOM contains only the components required to upgrade your PCB from the standard configuration to the full configuration, as well as the components for the battery module. Note if building more than one battery board, I recommend not purchasing the "PC4" battery holder on the Digikey BOM and instead ordering them on Amazon.

- [PCB Upgrade and Battery Parts][dk-pcb-upg] (DigiKey)
- [PC4 Battery holder][pc4] (Amazon)
- [Battery Charger Module][chg] (Amazon)
- [Battery Protection Module][prot] (Amazon)

**Note:** the BOM does NOT include teh external DC supplpy, as it will depend on your region. The requrements are 10W or more power, 9-12V. 5.5mm barrel with 2.1mm pin, centre positive.

- Example for North America: [GlobTek WR9HD1333CCP-F(R6B)][dk-psu-us] (Digikey)


##### Battery Only

This BOM contains just the DigiKey parts requred for the Battery Module and teh wiring to connect it to the main board. If upgrading follow the Upgrade BOM above instead. If building for the battery from the start, use the "Full Build" Bom above, and add the items in this BOM to your order as well. Note if building more than one battery board, I recommend not purchasing the "PC4" battery holder on the Digikey BOM and instead ordering them on Amazon.

- [Battery Module Parts][dk-bat] (DigiKey)
- [PC4 Battery holder][pc4] (Amazon)
- [Battery Charger Module][chg] (Amazon)
- [Battery Protection Module][prot] (Amazon)

---

## Project Links:

- [Full Project Homepage][zion-web]
- [PCB page on Zion's website][zion-build]
- [Project Discord][discord]
- [3D Print Files][zion-mw] (MakerWorld)
- [PCB Boards][pcbway] (PCBWay)
- [Standard PCB Components][dk-pcb] (DigiKey)
- [Standard PCB Components Alternate][dk-pcb-alt] (DigiKey) -- for when you are using the amplifier from Amazon
- [Full PCB Components][dk-pcb-full] (DigiKey)
- [PCB Upgrade Components][dk-pcb-upg] (DigiKey)
- [Battery Module Components][dk-bat] (DigiKey)
- [Zion Brock's YouTube][zion-yt]

---

Want to support my efforts? Feel free to [Buy me a Coffee][support]

[![alt text][cc-by-nc-sa]](./LICENSE.txt)


[cc-by-nc-sa]: ./assets/by-nc-sa.png "CC-BY-NC-SA"
[sch]: ./assets/zbvr-pwb-v1-a-sch.png "ZBVR-PWB-V1-A Schematic"
[pcb]: ./assets/zbvr-pcb-v1-a-render.png "Rendering of fully populated ZBVR-PCB-V1-A"
[front]: ./assets/ZBVR-PCB-V1-A-Front-Final.png "Top/Component Side of PCB"
[back]: ./assets/ZBVR-PCB-V1-A-Back-Final.png "Bottom/Solder Side of PCB"
[pcbway]: https://www.pcbway.com/project/shareproject/Simple_lo_fi_offline_MP3_player_for_the_Zion_Brock_vintage_radio_official_PCB_5a9d43d7.html
[dk-pcb]: https://www.digikey.com/en/mylists/list/7UZQIHX73I
[zion-web]: https://www.zionbrock.com/radio
[zion-mw]: https://makerworld.com/en/models/2163838-my-vintage-radio-offline-am-style-music-player
[zion-yt]: https://www.youtube.com/@zionbrock/videos
[discord]: https://discord.gg/p7cJ7csKEd
[zion-lic]: https://www.zionbrock.com/radio-license
[zion-build]: https://www.zionbrock.com/vintage-radio-circuit-board-pcb
[dk-pcb-alt]: https://www.digikey.com/en/mylists/list/B0VSUA3P00
[dk-pcb-full]: https://www.digikey.com/en/mylists/list/RAMKQWNZRU
[dk-pcb-upg]: https://www.digikey.com/en/mylists/list/QIRFQ48IGT
[dk-bat]: https://www.digikey.com/en/mylists/list/4W6Q9O6ATI
[dk-psu-us]: https://www.digikey.ca/en/products/detail/globtek-inc/WR9HD1333CCP-F-R6B/13245472
[rp]: https://www.amazon.com/dp/B0C5Q2V49P?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1
[amp]: https://www.amazon.com/HiLetgo%C2%AE-PAM8403-Digital-Amplifier-2-5-5V/dp/B00LODGV64/ref=sr_1_1_sspa?th=1
[pc4]: https://www.amazon.com/dp/B0B1JJZ363?ref=ppx_yo2ov_dt_b_fed_asin_title&th=1
[chg]: https://www.amazon.com/Bloepum-Charging-Management-Lithium-Battery/dp/B0FB8K6PVR
[prot]: https://www.amazon.com/dp/B0DDY32WF4?ref=ppx_yo2ov_dt_b_fed_asin_title
[support]: https://buymeacoffee.com/canadianavenger

