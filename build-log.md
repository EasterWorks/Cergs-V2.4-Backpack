# 0: Designing the thing

As mentioned in the landing readme for this repo, I had a series of constraints and requirements to follow.

Of primary concern to me was ensuring that the umbilical cable pathing wouldn't be messy, as I'm running a Stealthchanger toolchanger build, currently with two toolheads. These umbilicals need to not get crushed when the backpack is closed primarily. Another concern was ensuring that there is adequate space behind the flying gantry for the umbililcal cable and a few retainers to run.

To facilitate this, I modified the exhaust plate I designed for my Stealthchanger build so it would protrude out from the back of the printer, then planned to inset the interior panel by around 12mm:

![image](https://github.com/user-attachments/assets/5f5387c8-c1e2-49ca-a1bc-f430e72db9a7)
_Highlighted components: Printer's rear frame loop, modified exhaust plate/umbilical retainer._

The backpack would need two fairly robust hinges at the bottom in order to facilitate opening/closing. I initially tried to design some low-profile hinges using 5mm pins and bushings, but this ended up being weak enough that I wasn't comfortable with the entire weight of the backpack resting on them. I ended up using the commercial hinges that I had based my hinge design's measurements off of:

![image](https://github.com/user-attachments/assets/547ede15-5c14-41ac-a647-98cde1bc1765)

These will leave around a 2mm gap between the front loop of the backpack and the rear loop of the printer - which was perfect, as I intended on using 3mm foam strips to help lock down additional airflow.


# 1: Making the frame

I started by measuring the rear loop of my Voron 2.4 printer's frame. This ended up being 459mm wide, 480mm tall, to confirm my design. The height was reduced by 22mm to faciliate other aspects of the design, such as the commercial hinges. I then cut the frame extrusions to the needed length and connected them using internal 90 degree joints in order to leave needed real estate for the internal panel standoffs. The width extrusions were 120mm, so there is 80mm of accessible height within the enclosure.

![image](https://github.com/user-attachments/assets/cb04b324-309f-4d1a-bc5c-6662921f997b)

I also installed the "skirt" pieces - aesthetically based on the Voron design language and includes Voron logos. I used my Stealthchanger's extra toolhead to embed the red fan grills into the skirt on that span, which would be on the "left" side of the printer when looking at it from the front. The very bottom center skirt panel has a large cutout to allow nylon-sheathed cable looms to pass from the old under-skirt electronics bay to the backpack.


# 2: Panels and Magnets

I then installed the internal panel standoffs, glued in 10mm magnets, and epoxied matching magnets on to the clear acrylic panel after scuffing up the spots underneath (note: I would later end up dremelling in holes for screws to rigidly mount the magnets to the acrylic, as the epoxy didn't hold up well over time):

![image](https://github.com/user-attachments/assets/e4172e2e-670c-4fac-aa60-c7db253dd850)

Once the umbilical clips were printed, 6x2mm magnets would also be glued to the front of the clear acrylic panel to help control any undesirable movement of the umbilicals while the backpack is "closed". These magnets are fairly weak, so when the backpack is opened, they pop off pretty easily - but will likely need manual assist to put back in their correct spot.

The original rear panel of the Voron would work for the rear panel of the backpack after trimming 22mm of material from the bottom. Well, that was the thought anyway, until the original back panel exploded in my hands and I had to buy a new one! This was attached using a total of 8 typical Voron panel clips to give good rigidity around the entire perimeter. 

![image](https://github.com/user-attachments/assets/ae6d57fc-a14b-4ba5-b588-de25638a3365)

I also started moving over the cabling at this point.


# 3: Electronics Migration

For migrating the electronics, I needed to get the Birds' Nest moved off of the back panel and into the enclosure. I designed a mounting plate that could screw on to the standard Voron DIN rail clips and put that in place.

Then I took many, MANY pictures of my existing electronics bay as it stood in case any cables weren't labelled to prevent confusion on cabling. This came in handy a few times, though most of the wire loom was already labelled (LDO kit is amazing).

![image](https://github.com/user-attachments/assets/597ca5f1-e66c-4638-b262-3b49772c134b)

I then removed all of the electronics, installed the DIN rails in the new backpack space, and verified cable lengths were good. All said and done, all I really needed to do was just to run a line from the 24v PSU to the Wago terminals I had planned to use for power distribution, and then I needed to add about 4" to the X/Y endstop daughterboard cable.

![image](https://github.com/user-attachments/assets/633384a7-1cc9-4c33-95cf-68ec3103d442)

As you can see here, I have two rows of WAGO 5x lever nuts for power distribution. On the "bottom" of the backpack, I have two rows of 10 for the 24v power lane, and then on the "top" is the 5v power lane. Since I can always just jump out the last terminal in each lever nut to another lever nut, these are as expandable as space allows for.

As you may understand from the above, I left the 24v PSU and the DIN clip assortment in the original skirt. Moving all of that to the backpack would have been a massive pain and isn't really necessary when I have power distribution options in the backpack.


# 4: Hinges and Locking Mechanism

I used some commercial 2020 hinges with M4x6mm FHCS that fit my design needs. Critically, both "tops" of the hinge plates needed to rest flat against each other so the entire electronics bay could open up at a 90 degree angle. 

I designed the locking mechanisms so each has a spring-loaded shuttle which presses into a hook. My design ended up working fine, but feels a bit flimsy in practice - once the project is "done", I'll be redesigning these.

![image](https://github.com/user-attachments/assets/62c3fb7c-7122-4f6b-82f3-81afdaaecd27)

The spring-loaded shuttle has some decent pretension in order to prevent the shuttles from walking out due to vibrations during normal operation of the printer. The exact closing position can be adjusted by changing how far the hook rests along the backpack's upper frame. When both sides are latched closed, even with the first iteration of the design, it feels VERY secure. 



# 5: Finishing Touches

(this part is TBD - WIP outline)

- paint black perimeter around clear acrylic panel
- line backpack with LED strips?
- CABLE MANAGEMENT 
- install 3mm foam strip tape to frame of backpack and printer.
- install SLS nylon PA-12 backplates and shuttle to Stealthchanger.
- install unified shaft BMG extruder gears to Stealthburner extruders.


# 6: Lessons and improvements

(this is TBD - WIP outline)

- should have made the backpack like 30mm more narrow so the bay doesn't have to entirely hang off the edge of the printer's platform to be accessible



# 7: Replicating this project

(this part is TBD - WIP outline)

I have included all needed STL's in this repo, but be warned - this requires a lot of understanding of the electrical side of your 3D printer, and I am not running a typical Voron 2.4 build. To fully replicate this on a Voron 2.4 without a Stealthchanger or other toolchanging system, you will need a modified exhaust plate.
