# Big Speaker Assembly Guide

![alt text][begin]


So you build the [radio with the PCB][1], but wanted bigger sound from it. This guide is here to help with that. I've designed a new mount and enclosure for a 3.5in car speaker that is fairly inexpensive, and fairly easy to obtain. The solution here isn't perfect, but sounds quite good. The only real downside is that the PCB needs to be mounted on the mount and the potentiometer plugged in before the speaker can be mounted. (you may want to have the LED connected as well beforehand) 

[1]: https://www.zionbrock.com/radio
[begin]: ./assets/speaker/BigSoundRear.jpg "Assembled Speaker and Mount"

---

## Materials

- 1x 3D Printed speaker mount and enclosure
	- [All Parts 3MF](/assets/speaker/big-speaker.3mf) 
	- [All Parts STL/ZIP](/assets/speaker/big-speaker.zip)
	- Individual STL files
		- 1x [Mount](/assets/speaker/mount-big-spkr.stl)
		- 1x [Speaker Cup](/assets/speaker/GRS-3AS-4-cup.stl)
		- 1x [Face Ring](/assets/speaker/GRS-3AS-4-ring.stl)
- 6x M3 Threaded heat-set insert nuts
	- [Maker World M3x5x4](https://ca.store.bambulab.com/products/round-threaded-brass-heat-insert-nut) AB012
	- [CNC Kitchen M3x5x4](https://cnckitchen.store/products/made-for-voron-gewindeeinsatz-threaded-insert-m3x5x4-100-stk-pcs)
- 2x M3x6 SHCS (Socket Head Cap Screws) - for mounting assembly in radio
	- [Maker World M3x6 SHCS](https://ca.store.bambulab.com/products/m3-socket-head-cap-machine-screws-shcs-1) AA036
- 2x M3x10 SHCS (Socket Head Cap Screws) - attaching speaker to mount
	- [Maker World M3x10 SHCS](https://ca.store.bambulab.com/products/m3-socket-head-cap-machine-screws-shcs-1) AA159
- 2x M3x8 BHCS (Button Head Cap Screws) - attaching ring to cup
	- [Maker World M3x8 BHCS](https://ca.store.bambulab.com/products/m3-button-head-cap-machine-screws-bhcs) AA058
- 4x BT2x6 SHCSST (Socket Head Cap Screw Self Tapping) - Attaching PCB to mount
	- [Maker World BT2x6 SHCS](https://ca.store.bambulab.com/products/bt2-socket-head-cap-self-tapping-screws-shcs-new) AA093
	- [Maker World BT2x6 BHCS](https://ca.store.bambulab.com/products/bt2-button-head-cap-self-tapping-screw-bhcs) AA128 (Old Button Head Version) 
- 1x GRS 3AS-4 3.5in automotive replacement speaker 4 ohm 15 Watts
	- [Parts Express](https://www.parts-express.com/GRS-3AS-4-3-1-2-Car-Replacement-Speaker-4-Ohm-292-452?quantity=1) (USA)
	- [Solen Online](https://www.solen.ca/en/products/GRS-3AS-4-87mm-Car-Replacement-Speaker-4-Ohm) (Canada)
	- [Sound Imports](https://www.soundimports.eu/en/grs-3as-4.html) (Europe)
- 1x JST PHR-2 - PH Series 2mm pitch 2 pin housing
	- Not needed if salvaging from old speaker
	- [Digikey 455-1165-ND](https://www.digikey.com/short/q53mh2v7)
	- [Mouser 306-PHR-2PP](https://mou.sr/4vBqxXr)
- 1x JST ASPHSPH24K305 - PH Series crimped 12in 24AWG lead
	- Not needed if salvaging from old speaker
	- [Digikey 455-3083-ND](https://www.digikey.com/short/qd985ztp)
	- [Mouser 306-ASPHSPH24K305](https://mou.sr/48MVWfJ)

***Note:*** *If salvaging the wire and connector from an old speaker, be sure to cut as close to the speaker as possible, you want to end up with at least 6in of wire from the cut end to the connector.*

### Additional Required Materials

- Solder

### Optional Materials

- Sealant or Glue
	- Hot Glue
	- Silicone
	- Epoxy 

## Tools
### Required Tools

- Soldering Iron
- Wire Cutters
- Wire Strippers

### Optional Tools

- Hot Glue Gun

---

## Assembly

### Mount Preparation

We'll start by installing the heat-set insert nuts

1. Install the heat-set nuts into the bottom of the mount as shown.<br>![alt text][nut1]
2. Install the heat-set nuts into the speaker cup as shown.<br>![alt text][nut2]


[nut1]: ./assets/speaker/NutBase.jpg "Locations for heat inserts in mount base"
[nut2]: ./assets/speaker/NutCup.jpg "Locations for heat inserts in speaker cup"

### Speaker Preparation

![alt text][wir1]

Next we need to add wire leads to the speaker

1. Fold and cut the 12in wire lead in half to produce two 6in wire leads, each with a crimp on one end.
2. Strip the bare end of the wire exposing 3-5mm of the bare wire.<br>![alt text][wir2]
3. Tin the stripped wire ends with some solder.<br>![alt text][wir3]
4. Solder the leads to the speaker.I find it easiest to solder to the base of the terminals where there is solder already.<br>![alt text][wir4]
5. Insert the positive lead into pin 2 of the connector housing. *(Note: polarity is not strictly important here as we only have one speaker)*<br>![alt text][wir5]
6. Insert the negative lead into pin 1 of the connector housing.<br>![alt text][wir6]

[wir1]: ./assets/speaker/WiringParts.jpg "Speaker wiring parts"
[wir2]: ./assets/speaker/CutWire.jpg "Cut and stripped wire leads"
[wir3]: ./assets/speaker/TinWire.jpg "Tinned leads"
[wir4]: ./assets/speaker/SolderedWire.jpg "Wires soldered to speaker"
[wir5]: ./assets/speaker/InsertPos.jpg "Positive lead installed in connector"
[wir6]: ./assets/speaker/InsertNeg.jpg "Both leads installed in connector"


### Speaker Enclosure

Next we will assemble the speaker enclosure. The optional step of sealing around the edge is to secure the top ring better, and will prevent any rattle, as well as it should increase the performance of the enclosure slightly.

1. First place the speaker  into the cup, using the bumps and slots for alignment. The wires on the speaker should be facing the small slot at the bottom, and pressed down into the slot.<br>![alt text][cup1]
2. Place the Face Ring over the speaker. ***Note:*** *The tabs on the speaker are slightly off-centre so it will only fit one way.*
3. Install the two M3x8 BHCS screws to attach the face and secure the speaker.<br>![alt text][cup2]
4. *(Optional)* Flip the assembly over and apply a bead of sealant (epoxy/silicone/hot glue) around the perimeter where the cup and face ring meet.<br>![alt text][cup3]

[cup1]: ./assets/speaker/CupFilled.jpg "Speaker placed in the enclosure cup"
[cup2]: ./assets/speaker/CupScrewed.jpg "Front face installed and secured with screws"
[cup3]: ./assets/speaker/CupGlued.jpg "Detail of seal around perimeter"

### Final Assembly
Now we're ready to bring all the parts together.
1. Install the PCB onto the mount base using the 4 BT2 SHCS (or BHCS) screws in the corners. *(One of the corners will be inaccessible once the speaker is mounted)*<br>![alt text][mnt1]
2. Connect the potentiometer to the PCB as the connector will be inaccessible once the speaker is mounted. *Note: You may wish to install the LED at this point as well, as access to that connector will be tight after the speaker is mounted*![alt text][mnt2]
3. Mount the speaker assembly onto the base using the two M3x10 SHCS screws from the base into the speaker assembly. Note there is a bit of a keying emboss on the top of the base "tower" and the bottom of the speaker mounting tab to help align things. ![alt text][mnt3]
4. Plug the speaker into either of the speaker outputs of the PCB![alt text][mnt4]

[mnt1]: ./assets/speaker/MountPCB.jpg "Radio PCB installed on base"
[mnt2]: ./assets/speaker/MountPot.jpg "PCB with potentiometer installed"
[mnt3]: ./assets/speaker/MountSpk.jpg "Assembly with speaker mounted"
[mnt4]: ./assets/speaker/FinalAssembly.jpg "assembled speaker mount"

And that's it, at this point the assembly can be installed into the radio using the two remaining M3x6 SHCS screws. 

Enjoy the fuller and louder sound!

![alt text][fin]

[fin]: ./assets/speaker/Installed.jpg "Assembly installed inside radio"
