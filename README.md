This BNBSX "Short Ears" extruder for MK3S sensor is the edition needed for upgrading  Prusa MK3S and MMU2S printers. 

For MK3 printers, see instead short ears for MK3 printers. https://www.thingiverse.com/thing:3606189 

Build guide is being written, but not yet complete. Complex and Bunny Science specific portions of BNBSX assembly are already in guide. Remaining, generic steps should be easy for experienced builders.

https://bunnyscience.dozuki.com/Guide/Bunny+and+Bear+(BNBSX)+MKS3+Geared+Extruder+Assembly/2?lang=en

Advantages of this extruder over stock MK3S R4

- Geared 1:3.5 for more consistent extrusion.
- Indirect drive isolates filament from extruder motor heat
- Corrected filament path/Bontech alignment (as in Bear extruder)
- Lower total mass by about 80 gm
- Extreme rearward motor position reduces moment arm
- Continuous PTFE path deep into extruder for MMU2S and Palette 2
- Two, swappable filament sensor systems (armature for single filament, internal lever for MMU2S)
- Internal filament sensor lever eliminates Prusa filament sensor chimney on MMU2S
- Internal filament sensor lever allows full opening of idler door
- Single screw tuning of MMU2S filament sensing
- New MK3S sensor armature design eliminates steel ball rattling
- Provisioned for LED filament sensor indicator mod
- Only one magnet needed for filament sensor
- Easy motor plate and hot end removal for service
- Separately printable hot fins for heat resistance
- Hot fins tightly encircle hot end.
- Replace PTFE, heater cartridge or filament sensor without full tear down.
- Fits E3DV6, Volcano, or Mosquito hot ends
- Air plenum optimum whether E3D or Mosquito installed

(See Mosquito compatibility kit for mounting adapter and special hot fins for Mosquito, https://www.thingiverse.com/thing:3651160)

(See Volcano compatibility hot fin for special hot fin for Volcano, https://www.thingiverse.com/thing:3657574


For comparison, the following are how far various extruders place motor from rear of extruder body.

MK3 R3 30.5 mm
MK3S  R4 28 mm
Bear 27 mm
BNB Retrograde 23 mm
BNB Short Ears Edition 16.5 mm (with Bunny Science Universal x-carriage, 18 mm otherwise)

Because extruder motor is pushed so far back, this must be mounted on Short Ears version of Bear x-axis to clear the motor x-end. Normal Bear x-axis mounts will impinge against motor.

You can also mount on Prusa x-axis using the BNB Universal X-carriage, but the Prusa axis is much more difficult to tension properly.


Videos of BNBSX in operation 
https://youtu.be/z7LmkS7mqpA
https://youtu.be/9z_EihvkaD8

Filament armature detecting above Bondtechs. Optional LED mod indicates when filament is detected by either armature or MMU2S internal lever
https://youtu.be/ReESJ-j2wwU

Internal lever MMU2S sensor (M7 revision) undergoing bench test. I am manually turning shaft to move filament in/out of Bondtechs.
 https://www.youtube.com/watch?v=YfuO-00C6_s

---
Essential to use the BNB Universal X-carriage when doing this upgrade. https://www.thingiverse.com/thing:3610593. BNB Universal X-carriage has cable management features to reduce risk of hot end cable damage during XYZ calibration

That carriage also lets you remove the motor plate WITHOUT taking off the back of the extruder.

**** Double check lead dress of hot end wires with x-carriage max left and print bed max forward BEFORE XYZ calibration. Verify cables do not contact print bed cable cover.
***

Build differences from the regular Bunny and Bear Geared Extruder...

- Short Ears X-Ends must be installed to allow motor to clear
- Compact shaft locks required
- Bunny and Bear Short Ears Shaft is different
	Length	55 mm for 2 bearings
	Pulley Flat	0 to 9 mm
	Bondtech Flat	42 mm to end



If you do not already have a hot-end collet clip, print one from Bear extruder (https://www.thingiverse.com/thing:3226689). That STL is included here for your convenience.

Motor plate / gearbox MUST be printed with supports. 3mf file supplied with suggested plating and support enforcement block. 3mf's are set for 0.15 mm layers for nicer finish.

Removing support material from inside gearbox cavity takes 10 to 15 minutes. Take care to completely clean out mounting holes for bearings. Push shaft rod into gearbox from outside to remove support material within bearing mounts. If you do not clear out bearing mount holes completely, bearings will not spin freely. There will be a small amount of support material near filament path. Clear those out as well.

Some support scarring will remain, but is largely hidden by installed extruder cover.

Build with two shaft bearings. No 3rd bearing is used for this extruder

Materials needed...

5 mm diameter shaft rod	
Length	55 mm
Pulley Flat	0 to 9 mm
Bondtech Flat	42 mm to end
see https://www.thingiverse.com/thing:3595205 for shaft cutting guide and instructions


5 of Bearings - 3x6x2.5 mm Miniature Steel Bearings MR63ZZ 
https://www.amazon.com/gp/product/B00ZHSQX42

M2 x 16 mm socket end cap screw, in black alloy to connect MMU2S internal lever to its optical interruptor arm. THIS SCREW CANNOT BE STAINLESS STEEL. MUST BE STRONGLY ATTRACTED BY MAGNET )
https://www.amazon.com/gp/product/B07MN9X2KN

Remainder of screws are hex head, stainless steel

I suggest these sets of multiple sizes as you will may sizes of M3 from short to long.
Not the strongest hardware, but adequate for plastic to plastic work.
https://www.amazon.com/gp/product/B071KBVZVV
https://www.amazon.com/gp/product/B07C9F2347

MK3S IR filament sensor kit

5 x M2 screws x 12 mm for hot fins and lower x-carriage cover
1 x M2 screw x 6 mm for MK3S IR sensor (Screw supplied with MK3S sensor is too long)
1 x M2 screw x 8 mm for optical path insert
2 x M3 screws x 8 mm for optical armature

2 x 1050ZZ bearings
1 x continuous loop 140-2GT-6 Timing Belt
4 x M3 square nuts
3 x M3 set screws
M3 hex nuts & bolts (various lengths from 12 to 30 mm long. Some must be cut to custom length during assembly)
M3 washers
M3 Nylock nuts

1 x 16T drive pulley (to simplify alignment, use one for a 10 mm wide GT2 belt despite the belt being 6 mm wide)

Motor - 1.8 degree, STEPPERONLINE Nema 17 Bipolar Stepper Motor 0.7A 13Ncm (18.4oz.in) 17HS10-0704S. This is the ONLY short body motor that worked well in my testing.

Wiring harness for motor. Must plug into EINSY upside down to reverse motor direction.

--
You MUST also set e-steps by sending g-codes to printer
M92 E980
M500

--
Pulley gearing originally inspired by Skelestruder

--
Issues:
Check motor x-end top clamp bolt. Depending on build tolerances, your motor may come into slight contact with the head of that bolt. If that is happening, file off a bit of the bolt head or change to button cap bolt (with smaller head profile)

Upper bolt tab of print fan likely to contact drive belt. Use x-acto knife to shave a bit of plastic from fan's bolt tab to clear belt. Takes just a few minutes to perfrom.

--
Recent Change Log

BO3 improves PTFE path into extruder from MMU2S and Palette 2. PTFE path is now continuous all the way to optical sensor cutout. Also, enlarged bore of non-PTFE portions of filament path.

To gain B03 improvements, use new STL's...

BNBSX Extruder Plated b03m1.3mf
BNBSX Motor Plate Gearbox 26mm B03.stl
BNBSX Motor Plate Gearbox 35mm B03.stl
BNBSX Motor Plate Gearbox standard 25mm B03.stl
BNBSX top cover MMU2S B03.stl
BNBSX top cover palette 2 B03.stl
BNBSX top cover PC4-M10 B03.stl
BNBSXM extruder main BO3.stl

Two mounting changes as well
Lower left motor bay screw is now standard length M3 x 16 mm

PINDA clamp changed to Nylock M3 nut instead of M2S. Former, M2S nut left clamp prone to loosening after hundreds of hours printing. 

Motor Plate Gearbox has greater range arc for belt tightening

Added taller, 26 mm version of Motor Plate Gearbox to fit 26 mm body E3d Motor (untested motor)


----
post print

Plated 3mf file includes spares of the small parts like optical armatures, levers and interruptor rod.
---
Motor X-End has "Short Ears" to let motor clear. 

Draw in the M3 nuts for the x-end clamps WITHOUT the bearings in place. This lets the two ends of clamps contact each other during the drawing in process. With the bearings in place, the ends cannot abut each other during the drawing in process. 

CRITICAL ***** X-End Motor plate M3 bolts for bearing clamps must be correctly sized. If they are too long, they will damage Z-axis screw. Grind bolt lengths to be flush with nut and no longer. Should be about 7.0 to 7.5 mm. Double check that z-screw is not impinged during install. ****

Do not over tighten the bolts with bearings in place. The clamps do not travel as far with the bearings inserted. They are not intended to close the gap. You risk breaking the plastic if you over tighten. Just snug the bolts and no tighter.

Embed an M3 nut into hex recess at end of each rod hole before inserting rods. You can later use long M3 bolts to engage the nut and easily push out axis rods.

---
When routing motor cable, leave enough slack to route from front or below motor. 

Do NOT route cable BEHIND the motor. That will pinch the cable between motor and the x-end. 
---

- Remove all support material, paying particular attention to bearing mount recesses and near filament path. Stray support material left inside the recesses prevents free bearing function. 

- Once the majority of support material is removed, tap shaft rod into each bearing hole to pop out support material.

- Pass a small, flat screwdriver through opposite hole to clean out bearing mounts. 

- Flatten mating surfaces and motor mount. Uneven surfaces like the main extruder body and motor mount can be flattened with a file. Rear of motor plate can be lapped flat with wet sanding on a glass plate. Remove just high spots.

- Draw in 4 M3 nuts for motor plate using standard bolt and washer technique.

- Press in two motor plate bearings with a bolt, nut and two washers. Outside washer should be 20 to 30 mm diameter. Inside washer (which presses agains bearing) should be just a bit larger than the bearing. Reach into gear cage with needle nose pliers or small wrench to stabilize nut while tightening bolt. Press just flush. Don't over tighten to point of deforming plastics. Gearbox has uneven surface opposite 2nd bearing. Requires spacer to even out surface for washer to press against while pressing in bearing. PINDA mount piece happens to be perfect size to use as spacer during pressing of 2nd bearing.

- Prep bearings by degreasing shipment oil and re-lubricate with light machine oil

- Check each bearing for free motion. The front bearing of the gearbox is the most prone to debris preventing free motion. Use special care cleaning out that mounting recess. If you need to remove a bearing, they can be gently tapped back out using a 5 mm Allen wrench as knockout pin.

-  IMPORTANT: Most 5 mm shafts arrive slightly too large in diameter. If diameter of shaft is too large to easily slide through bearings, slightly decrease its diameter by chucking in drill and using fine sandpaper while spinning it. Make it just slide fit, not loose. The entire length of the shaft should be tested for easy passage. 

- Shaft flats for pulley and Bondtech drive must be ground to depth of 0.38 to 0.4 mm. Grind lightly with Dremel and measure frequently. Use a shaft cutting guide to make the process easier.
https://www.thingiverse.com/thing:3595205

---
Retrograde Shaft and Pulley

- Prepare motor by grinding a flat on its shaft

- Insert motor (without drive pulley) into gear box 

- Insert rear end of shaft through front of large pulley. Front end of shaft should be flush with pulley front surface. 

- Place one spacer onto shaft behind pulley. Orient spacer so it's narrow diameter side is away from pulley.

- Advance shaft through 1st bearing.

- Add 1st shaft lock. Orient narrow tip end of lock towards front bearing.

- Advance shaft further and add 2nd shaft lock. Second shaft lock should have its narrow tip towards second bearing.

- Advance shaft through 2nd bearing. Keep advancing until large pulley is about length of motor shaft away from gearbox.

- Add 2GT belt and motor drive pulley.

- Advance shaft further while also slipping motor drive pulley onto motor shaft.

- Position shaft to leave just a narrow space between spacer front of gearbox.

- Use shaft locks to to secure position of shaft. Each lock is placed against its corresponding bearing and set screwed in place. Once both locks are engaged, the shaft and bearings will no longer slide in/out.

- Secure pulley set screw against shaft flat.

- Secure motor in position to take up belt slack, but not "stretched" tight.

- Slide Bondtech drive gear onto shaft. Align its filament gripping teeth centered with rear surface of motor plate.

- Cut motor plate M3 bolts to lengths for tips to be flush when fully engaged. Too short and they won't engage with embedded nuts. Too long and they can protrude and interfere with motor.

The below are best estimate for flush fit of custom length screws. Please check actual fit before grinding bolts to length. Lengths are tip of bolt to shoulder, not including head

Motor plate screws as viewed from front
upper right 36 mm
lower right 27 mm
upper left 26 mm
lower left 17 mm

hot end cover top screws 27 mm

extruder body air plenum to x-carriage screws
upper x 2	13.7 mm
lower center 8 mm

- Always with optical armature out of way slightly when attaching motor plate. A length of filament inserted into filament path will move armature out of way sufficiently. Motor plate assembly slides straight in easily. If there is resistance, verify optical armature isn't being crushed and idler tension screw is loose.

. Index pins help with final alignment of motor plate. Installation is easier if all mounting bolts are backed out flush with extruder body front surface.

- Recheck alignment of Bondtech is centered on plane between motor plate and main extruder body. Filament path is centered in that plane.

---
This upgrade requires plugging in motor cable flipped 180 degrees at EINSY to reverse motor direction.

--- 
BNB Universal x-carriage has two filament paths. Upper one is for Bear axis, lower one is for Prusa axis. Put 2 tooth piece of belt into unused path before inserting belt. The universal carriage also needs 8 mm bolt instead of normal 10 mm one middle of belt path.

---
Hot fins at bottoms of extruder body and hot end cover are to be attached via M2 x 12 mm screws. Once hot fins are attached, remainder of assembly is as usual.

Included hot fins and plenum inserts are used for E3DV6 hot end. The plenum inserts go into tabs of extruder and hot end cover before attaching hot fins.

See Mosquito compatability kit for Mosquito specific hot fins. Omit plenum inserts if using Mosquito hot end.

Hints...

Main extruder body has a thin, intrinsic support where internal MMU2S lever will pass. That intrinsic support must be removed. A combination of pliers and knife are needed to fully clear it out.

Thoroughly clean support material from motor plate around filament path. There are lots of tiny support bits that must be fully removed. Be patient and get it all, especially that inside recesses.

Press bearing into optical armature from BOTTOM (the side away opposite fin). It should be barely inset from bottom of armature.

Pre-thread MM3U2S internal lever's optical interrupter bar mount hole beforehand. Trying to attach tiny optical interruptor's M2 screw without pre-threading is difficult. The M2 screw needs a H1.5 driver. Do not use the allen key supplied with the Amazon screw kit. A mini screwdriver kit's H1.5 bit is far easier to use and less likely to strip the head.

When mounting motor plate to extruder, don't crush filament sensor armature. The armature naturally swings beyond filament path when motor plate is off. To avoid crushing the armature,  swing it out of way (towards IR sensor) and insert a piece of filament in filament path to push armature out of way until motor plate is installed.

In case it isn't obvious, you install either the filament armature OR the MMU2S internal sensor lever, not both at the same time

If MMU2S internal lever option is installed, a filament path insert can be installed in motor plate to close hole in filament path. Might run ok without the insert, but having the insert in place reduces risk of filament leaving path. 

PTFE tubing of extruder must be shortened by 5.5 mm, like in MK3S. Remember, this extruder is short bodied like the MK3S R4.

Use 8 mm length PTFE tubing in top cover to guide filament into extruder body.

No nylon washers are used with the idler doors.

Gear shaft should cut a little shorter than in Short Ears. The rear end of shaft should barely extend beyond Bondtech. Otherwise, gear shaft will impinge internal MMU2S sensor lever.

M3 bolt through bottom right of idler door adjusts MMU2S internal sensor lever system. 
Completely clean inside idler door M3S nut recess before inserting nut.

If single filament sensor armature option, place a MR63ZZ bearing to right of idler, on its mounting bolt. Bearing will fill space that the MMU2S internal sensor lever would otherwise occupy.

Nuts for hot end cover bolts press into REAR of extruder body.

Nuts for connecting extruder to x-carriage press into front of extruder body. 
M3 12mm bolts are inserted "backwards" into hex pockets of universal carriage to secure extruder body. Despite there being nut recesses in those positions of the universal carriage, do NOT put nuts into those pockets of universal carriage. Bunnies intentionally use those holes backwards for the BNBSX.

Bolts attaching hot end cover need to be 28 mm to not impinge x-carriage.

Parts cooling fan and drive belt are very close to each other due to 5.5 mm higher E3DV6 position. If yours is too close, shave a bit of plastic off fan's bolt mount with a sharp knife. It only takes just a few strokes.

**** Watch out for motor plate mounting bolts extending into motor recess. Those bolts must be cut to custom length to avoid impinging motor. Test fit the bolts and adjust lengths before inserting motor. ****

Top covers previously did not bridge well around LED observation port. They now print with a trapezoidal shaped, intrinsic support. The support cleans up the print, but it MUST be removed before using any of the covers. 
