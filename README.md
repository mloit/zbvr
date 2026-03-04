# Vintage AM Radio Inspired Offline MP3 Player PCB

***Complete PCB design files and documentation coming soon!***

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

The first step to building your own will be to get your hands on a bare PCB. PCB's can currently be ordered from our [Community project at PCBWay][1]. This is currently the preferred route as we do earn a small commission on every board ordered from there to help support the project (anything earned on the PCB's is shared between Zion and myself). Also please note that if you plan to resell the PCB's we ask that you fill out a [license application][7] on Zion's project site.

For the components you can use this [list at DigiKey][2] as a starting point. The list includes everything except the speakers, RP2040-Zero, and push-button, for the basic configuration of the PCB. Details on a more complete configuration for external power and a battery will be provided in the near future.

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

---

## Project Links:

- [Full Project Homepage][3]
- [Project Discord][6]
- [3D Print Files][4] (MakerWorld)
- [PCB Boards][1] (PCBWay)
- [Components][2] (DigiKey)
- [Zion Brock's YouTube][5]

---

[![alt text][cc-by-nc-sa]](./LICENSE.txt)


[cc-by-nc-sa]: ./assets/by-nc-sa.png "CC-BY-NC-SA"
[sch]: ./assets/zbvr-pwb-v1-a-sch.png "ZBVR-PWB-V1-A Schematic"
[pcb]: ./assets/zbvr-pcb-v1-a-render.png "Rendering of fully populated ZBVR-PCB-V1-A"
[front]: ./assets/ZBVR-PCB-V1-A-Front-Final.png "Top/Component Side of PCB"
[back]: ./assets/ZBVR-PCB-V1-A-Back-Final.png "Bottom/Solder Side of PCB"
[1]: https://www.pcbway.com/project/shareproject/Simple_low_fi_offline_MP3_player_for_the_Zion_Brock_vintage_radio_official_PCB_664cb836.html
[2]: https://www.digikey.com/en/mylists/list/7UZQIHX73I
[3]: https://www.zionbrock.com/radio
[4]: https://makerworld.com/en/models/2163838-my-vintage-radio-offline-am-style-music-player
[5]: https://www.youtube.com/@zionbrock/videos
[6]: https://discord.gg/p7cJ7csKEd
[7]: https://www.zionbrock.com/radio-license
