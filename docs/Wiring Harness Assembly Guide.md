# Wiring Harness Assembly Guide

![alt text][intro]



In this guide we'll assemble the wiring harnesses for front panel/controls of the vintage radio. For the intermediate/advanced users here is the summary wiring diagram depicting the three front-panel harnesses.

![alt text][diag]

[intro]: ./assets/wiring-photos/parts.jpg "photo of all the wiring parts"
[diag]: ./assets/assembly-renderings/all-harnesses.png "diagram depicting all the wiring harnesses"

## Materials

### Components
- 10K Potentiometer with switch
- Pushbutton
- LED (3mm or 5mm)
- 2x JST XHP-2 2 pin housings
- 1x JST XHP-3 3 pin housing
- 1x JST XHP-5 5 pin housing
- 2x JST-XH 6in (152mm) 22AWG pre-crimped wire lead (ASXHSXH22K152)
- 4x JST-XH 12in (305mm) 22AWG pre-crimped wire lead (ASXHSXH22K305) *

**Note:** The 12in wire leads are intended to be cut in half to each produce two single-ended 6in wire leads. In total we need seven 6in single-ended leads for all the harnesses here. The one left-over can be saved for another unit if building more than one.

### Required Materials
- Solder

### Optional Materials
- 2 pcs 0.062in (1.6mm) pre-cut heatshrink tubing approx 0.5in (6mm) long 
- 5 pcs 0.125in (3mm) pre-cut heatshrink tubing approx 0.5in (6mm) long

## Tools

### Required Tools
- Soldering iron
- Wire cutters
- Wire strippers

### Optional Tools
- Tweezers
- Digital volt meter
- Heat gun
- Permanent marker
- Ruler

---

## Assembly

### Wire Lead Prep

![alt text][wire]

Before we begin with the individual harness, we want to prepare our 6inch single-ended wire leads, that will be used in the individual harnesses.

#### Parts

- 4x JST XH 12in 22AWG pre-crimped wire lead 

#### Steps

For each of the 12 inch wire leads perform the following to produce two 6 inch single-ended leads each (8 in total)

1. Fold the 12in wire lead tightly in half to find the middle <br>![alt text][wire01]
2. Cut the wire lead at the fold to form 2 6in wire leads with a crimp on one end <br>![alt text][wire02]
3. Strip the cut ends removing about 10mm of insulation <br>![alt text][wire03]
4. Twist strands together tightly <br>![alt text][wire04]

When done you should have 8 total single-ended leads. Set one aside and save for another build, only 7 are needed for the harnesses below. 
![alt text][wire05]


[wire]: ./assets/wiring-photos/00-leads.jpg "photo of all the button wiring parts"
[wire01]: ./assets/wiring-photos/00-fold.jpg "folded wire lead"
[wire02]: ./assets/wiring-photos/00-cut.jpg "cut wire lead"
[wire03]: ./assets/wiring-photos/00-strip.jpg "stripped wire lead"
[wire04]: ./assets/wiring-photos/00-twist.jpg "wire lead with twisted strands"
[wire05]: ./assets/wiring-photos/00-done.jpg "completed single ended wire leads"

---

### Button Cable
![alt text][button]

Polarity is not important for the button so we don't need to worry about which pin connects to which terminal of the pushbutton.

![alt text][button-harness]

#### Parts

- 1x Pushbutton
- 1x JST XHP-2 2 pin housing
- 2x JST XH 12in 22AWG pre-crimped single-ended wire lead (prepared above)

#### Optional Materials
- 2x 0.062in pre-cut heatshrink tubing (smaller diameter)

**Note:** Check that the heatshrink tubing will slide over the crimped end of the wire leads. If not please ensure that the tubing used in step 6 below is slipped onto the wires before step 1

#### Steps

1. Bend the stripped ends in the middle into a L shape <br>![alt text][btn01]
2. carefully fish the end of one of the wires, be sure to get all strands through the hole on the tab of the button <br>![alt text][btn02]
3. Fold the bend all the way over back to parallel with the rest of the wire to hold the lead in position <br>![alt text][btn03]
4. Solder the lead to the tab keeping the wire coming as straight off the tab as possible 
5. Repeat steps 2-4 for the other lead <br>![alt text][btn05]
6. If adding heatshrink, follow the optional steps now before continuing
7. insert the crimped ends of the wire leads into the XHP-2 housing <br>![alt text][btn07]

##### Optional steps:

1. slip one of the strips of heatshrink tubing over the crimped end of a lead and slide up and over the soldered connection at the button. Do this for each of the wire leads/connections.<br>![alt text][btn-opt1]

2. using a heat gun or other heat source heat the tubing to shrink it for a secure fit over the connections.<br>![alt text][btn-opt2]

The finished cable should look something like this
![alt text][btn-done]


[button]: ./assets/wiring-photos/01-button-parts.jpg "photo of all the button wiring parts"
[button-harness]: ./assets/assembly-renderings/button-harness.png "diagram depicting the button wiring harnesses"
[btn01]: ./assets/wiring-photos/00-bend.jpg "bent wire lead end"
[btn02]: ./assets/wiring-photos/01-02.jpg "inserted wire lead"
[btn03]: ./assets/wiring-photos/01-03.jpg "wire lead folded over"
[btn05]: ./assets/wiring-photos/01-05.jpg "soldered wire leads"
[btn07]: ./assets/wiring-photos/01-06.jpg "leads inserted into XHP-2 housing"
[btn-opt1]: ./assets/wiring-photos/01-07.jpg "heatshrink over tabs"
[btn-opt2]: ./assets/wiring-photos/01-08.jpg "heatshrink-shrunk"
[btn-done]: ./assets/wiring-photos/01-done.jpg "completed button harness"

---

### LED Cable
![alt text][led]

Note that for the LED pin 2 of the XHP-3 connector remains unused for a standard LED. 

![alt text][led-harness]

#### Parts

- 1x LED
- 1x JST XHP-3 3 pin housing
- 1x JST XHP-2 2 pin housing
- 2x JST XH 6in 22AWG pre-crimped wire leads (double-ended)

#### Steps

1. Mark Pin 1 on both XHP housings with a permanent marker to make identification easier. <br>![alt text][led01a]![alt text][led01b]
2. Install one end of one of the leads into the pin 1 location of the XHP-3 housing <br>![alt text][led02]
3. Install the other end of the lead into the pin 1 position of the XHP-2 housing <br>![alt text][led03] 
4. Install one end of the remaining lead into the pin 3 position of the XHP-3 housing <br>![alt text][led04]
5. Install the other end of the lead into the pin 2 position of the XHP-2 housing <br>![alt text][led05]
6. Insert the legs of the LED into the XHP-2 housing, with the long leg going into the pin 1 mating position, and the short leg into the pin 2 mating position. Gently push the LED as far as it will go. When fully inserted, only the tip of the longer LED leg should protrude out the other side of the housing. <br>![alt text][led06a]![alt text][led06b]![alt text][led06c]

The finished cable should look something like this
![alt text][led-done]

[led]: ./assets/wiring-photos/02-LED-parts.jpg "photo of all the LED wiring parts"
[led-harness]: ./assets/assembly-renderings/LED-harness.png "diagram depicting the LED wiring harnesses"
[led01a]: ./assets/wiring-photos/02-01a.jpg "XHP connectors, unmarked"
[led01b]: ./assets/wiring-photos/02-01b.jpg "XHP connectors marked"
[led02]: ./assets/wiring-photos/02-02.jpg "XHP-03 pin1 installed"
[led03]: ./assets/wiring-photos/02-03.jpg "XHP-02 pin1 installed"
[led04]: ./assets/wiring-photos/02-04.jpg "XHP-03 pin3 installed"
[led05]: ./assets/wiring-photos/02-05.jpg "XHP-02 pin2 installed"
[led06a]: ./assets/wiring-photos/02-06a.jpg "bent wire lead end"
[led06b]: ./assets/wiring-photos/02-06b.jpg "bent wire lead end"
[led06c]: ./assets/wiring-photos/02-06c.jpg "bent wire lead end"
[led-done]: ./assets/wiring-photos/02-done.jpg "completed LED wiring harness"

---

### Potentiometer Cable 

![alt text][pot]

The final wiring harness is the potentiometer, and is the most complex. While the orientation does not matter for the switch portion, we do need to pay close attention to the orientation for the actual potentiometer (analog) portion.

![alt text][pot-harness]
<br>(colours for clarity only)

#### Parts

- 1x 10K Potentiometer with switch
- 1x JST XHP-5 5 pin housing
- 5x JST XH 12in 22AWG pre-crimped single-ended wire lead (prepared above)

#### Optional Materials
- 5x 0.125in pre-cut heatshrink tubing (larger diameter)

**Note:** Check that the heatshrink tubing will slide over the crimped end of the wire leads. If not please ensure that the tubing used in step 7 below is slipped onto the wires before step 1

#### Steps

1. Mark Pin 1 on the XHP-5 housing with a permanent marker to make identification easier. <br>![alt text][pot01a]![alt text][pot01b]
2. Bend the stripped ends in the middle into a L shape <br>![alt text][pot02]
3. carefully fish the end of one of the wires, be sure to get all strands through the <br>![alt text][pot03] hole on the tab of the button
4. Fold the bend all the way over back to parallel with the rest of the wire to hold the lead in position <br>![alt text][pot04]
5. solder the lead to the tab keeping the wire coming as straight off the tab as possible 
6. repeat steps 3-5 for each of the 4 remaining terminals on the pot <br>![alt text][pot06]   
7. If adding heatshrink, follow the optional steps now before continuing
8. Locate the two leads coming from the switch terminals on the back of the potentiometer. Insert the crimps into the pin1 and pin 2 positions of the XHP-5 housing. Order does not matter here. <br>![alt text][pot08]
9. with the shaft of the potentiometer facing away from you, and the 3 terminals facing down to the floor, locate the lead connected to the right-most terminal, insert the crimped end of lead into the pin 3 position of the XHP-5 housing. <br>![alt text][pot09a]![alt text][pot09b] 
10. with the shaft of the potentiometer facing away from you, and the 3 terminals facing down to the floor, locate the lead connected to the centre terminal, insert the crimped end of lead into the pin 4 position of the XHP-5 housing.  <br>![alt text][pot10]
11. insert the crimped end of the remaining lead into the pin 5 position of the XHP-5 housing <br>![alt text][pot11]

##### Optional steps:

1. slip one of the strips of heatshrink tubing over the crimped end of a lead and slide up and over the soldered connection at the button. Do this for each of the wire leads/connections.<br>![alt text][pot-opt1]

2. using a heat gun or other heat source heat the tubing to shrink it for a secure fit over the connections.<br>![alt text][pot-opt2]

The finished cable should look something like this
![alt text][pot-done]

[pot]: ./assets/wiring-photos/03-potentiometer-parts.jpg "photo of all the potentiometer wiring parts"
[pot-harness]: ./assets/assembly-renderings/pot-harness.png "diagram depicting the potentiometer wiring harnesses"
[pot01a]: ./assets/wiring-photos/03-01a.jpg "XHP connector, unmarked"
[pot01b]: ./assets/wiring-photos/03-01b.jpg "XHP connector, marked"
[pot02]: ./assets/wiring-photos/00-bend.jpg "bent wire lead end"
[pot03]: ./assets/wiring-photos/03-03.jpg "potentiometer with lead through a tab"
[pot04]: ./assets/wiring-photos/03-04.jpg "potentiometer with lead folded back"
[pot06]: ./assets/wiring-photos/03-06.jpg "potentiometer with leads soldered"
[pot08]: ./assets/wiring-photos/03-08.jpg "harness with pins 1 & 2 installed in XHP connector"
[pot09a]: ./assets/wiring-photos/03-09a.jpg "rightmost lead singled out"
[pot09b]: ./assets/wiring-photos/03-09b.jpg "harness with pin 3 installed in XHP connector"
[pot10]: ./assets/wiring-photos/03-10.jpg "harness with pin 4 installed in XHP connector"
[pot11]: ./assets/wiring-photos/03-11.jpg "harness with pin 5 installed in XHP connector"
[pot-opt1]: ./assets/wiring-photos/03-opt1.jpg "heatshrink slipped over connections"
[pot-opt2]: ./assets/wiring-photos/03-opt2.jpg "heatshrink after being shrunk"
[pot-done]: ./assets/wiring-photos/03-done.jpg "completed potentiometer harness"

---

## Fin

Congratulations on making it to the end. You now have all the wiring harnesses you need to complete your vintage radio. Assuming you have soldered up your PCB, and printed your enclosure. Now is the time to put it all together and enjoy the fruits of your labour.

![alt text][fin]

[fin]: ./assets/wiring-photos/all-harnesses.jpg "photo of all the completed wiring harnesses"
