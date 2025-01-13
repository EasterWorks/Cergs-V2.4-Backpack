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

I then installed the internal panel standoffs, glued in 10mm magnets, and epoxied matching magnets on to the clear acrylic panel after scuffing up the spots underneath:

![image](https://github.com/user-attachments/assets/e4172e2e-670c-4fac-aa60-c7db253dd850)

Once the umbilical clips were printed, 6x2mm magnets would also be glued to the front of the clear acrylic panel to help control any undesirable movement of the umbilicals while the backpack is "closed" (more TBD)

The original rear panel of the Voron would work for the rear panel of the backpack after trimming 22mm of material from the bottom (more TBD). This was attached using a total of 8 typical Voron panel clips to give good rigidity around the entire perimeter. (TBD)

(Pic of back panel installed - TBD)


# 3: Electronics Migration

(this part is TBD - WIP outline)

- Print a DIN rail mounting solution for the Isiks Tech Birds' Nest.
- Photograph electronics bay for future reference.
- Where the source is not obvious, label any connectors.
- Remove BTT Octopus Pro, Raspberry Pi 3B+, and all other non-PSU electronics from the bay.
- Install DIN rails in the backpack and transfer above electronics over to it.
- Measure needed extension length and put them together. Thread through nylon sheathing from underskirt bay to backpack.
- Create endpoints for 5V and 24V power lines using Wago lever nuts and label.
- Install cable raceways and route all cabling.
- Remove display unit from original skirt.
- Install skirt macro panel and keys to original skirt.
- Power-on test and ensuring all fans, heaters, lights, and endstops are functional


# 4: Hinges and Locking Mechanism

(this part is TBD - WIP outline)

- demonstration of locking mechanism (design is proven, just need to manufacture)
- connecting hinges
- optional: adding nylon strapping to prevent overextension of backpack when open (shouldn't need this though)
- demonstration of "open" and "closed" positions


# 5: Finishing Touches

(this part is TBD - WIP outline)

- paint black perimeter around clear acrylic panel
- install 3mm foam strip tape to frame of backpack and printer.
- install SLS nylon PA-12 backplates and shuttle to Stealthchanger.
- install unified shaft BMG extruder gears to Stealthburner extruders.


# 6: Replicating this project

(this part is TBD - WIP outline)

I have included all needed STL's in this repo, but be warned - this requires a lot of understanding of the electrical side of your 3D printer, and I am not running a typical Voron 2.4 build. To fully replicate this on a Voron 2.4 without a Stealthchanger or other toolchanging system, you will need a modified exhaust plate.
