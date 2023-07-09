# Midnite Toolhead

Inspired by the [VzBot Printed Printhead](https://github.com/VzBoT3D/Vz-Printhead-Printed) and the [EVA Carriage](https://main.eva-3d.page/), the Midnite Toolhead is designed to provide a back-attached CPAP cooling duct that is more compact and reduces the amount of Y travel lost when using the same cooling set up provided by VzBot and EVA on a Voron-style printer.

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/79416515-5c9b-4537-be2e-43f7e30e97c4)

## Design
Similar to VzBot, the design relies on 4 x 30mm aluminum standoffs and a top and bottom printed piece. There are only 5 necessary parts: the CPAP cooling duct, the duct spacer, the bottom part cooling duct, the top carriage piece, and the bottom carriage piece.

## Compatibility
This was made with these components in mind:
- Sherpa Mini Extruder (mine is CNC but it should work exactly the same for the printed version)
- VzBot Goliath Hotend (mine is watercooled but I think the mounting holes are the same for the air-cooled version)
- CPAP Cooling (I am using the standard CPAP tubing, which comes with a rubber end that I just push onto the end of the CPAP duct)
- SHT36 CAN Board (I'm sure others will work fine but this is the one I have been using and including in my models and test builds)
- Any Voron gantry, as long as you flip your X assembly (extrusion & XY joints) because that allows you to install a top-mounted rail. Flipping your X assembly shouldn't change anything (belt pathing, performance, etc), it just means your Y linear rails are also on top.
- If you have backers, they just go on the opposite side your rails are installed on the extrusions, just make sure your backer screws are flush - there's only 2mm of extra clearance to account for backers.
- You will need to run some tests to test the X and Y endstops. Currently this isn't a step I've gotten to in the development, 

## Bill of Materials
- 4 x 5x30mm Aluminum Standoffs (for carriage assembly)
- 8 x 16mm M3 Flat Head Countersunk Screws (for top & bottom carriage plates)
- 4 x 8mm M3 Flat Head Countersunk Screws (for attaching top carriage plate to MGN12H linear rail carriage)
- 2 x 6mm M3 Button Head Screws (for attaching the endstop piece to the top of the rail)
- 2 x 8mm M3 Button Head Screws (for attaching CPAP fan duct on the back, thru duct spacer, to bottom cooling duct)
- 2 x 10mm M3 Button Head Screws (for attaching Sherpa Mini Extruder to top carriage plate)
- 2 x 18mm M3 Button Head Screws (for attaching the bottom cooling duct, thru carriage spacer, to bottom carriage plate) [This is sort of optional but adds a lot of strength and prevents the CPAP fan duct from snapping off at the 90 degree bend]
- 6 x 5mm M3 Heatset Inserts (2 for the carriage top plate for attaching Sherpa Mini, 2 for bottom fan duct for attaching CPAP fan duct thru duct spacer)

## Printability
The CPAP fan duct is not easy to print. The only orientation I've found is shown in the image below. My settings are stock from Andrew Ellis's print guide. I have a 0.6mm nozzle, printing Sparta ABS+, at 240C, with Supports on build plate and Brim turned on.

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/272fc2e0-3f40-4225-93fa-ea3ea0e1aad8)

## Assembly
Install it whatever way makes sense to you. Note that you should read through the steps and do things differently depending on your setup. For example, you might want 

Here's how I do it:
1. Put the CPAP fan duct and the bottom carriage piece together, then put the back 2 aluminum standoffs thru the CPAP fan duct holes and into the bottom carriage piece.
2. Push the CPAP fan duct all the way down (while it's freely sliding up and down on the aluminum standoffs) to make room, then put the screws into the back 2 aluminum standoffs thru the bottom carriage piece. Try to not snap off the CPAP fan duct's mounting holes.
3. Put the front 2 aluminum standoffs into the bottom carriage piece, then screw them in.
4. At this point, if your X assembly (extrusion + linear rail) is already installed, you can do the next step around your extrusion. Meaning, when you put the top carriage piece down onto the aluminum standoffs that are in the bottom piece, you're doing it directly on your X rail.
5. Put the top carriage piece down onto the aluminum standoffs carefully and as straight as possible so you don't snap the plastic around the standoffs. Screw the aluminum standoffs in.
6. Install the heatset inserts on the top and bottom carriage pieces (this can be done at any step but I do it on this step so if I broke anything, I don't have to salvage heatset inserts from broken parts or leave them in the broken parts and waste them)
7. Install the heatset inserts on the bottom fan duct. Put screws through the holes in the bottom fan duct up thru the carriage spacers, ready for the next step
8. Screw thru the CPAP fan duct mount holes, thru the fan spacer (make sure the flat side of the fan spacer is touching the bottom fan duct), into the bottom fan duct.
9. Screw from the bottom the bottom fan duct thru the carriage spacers, into the bottom carriage.
10. Install the whole assembly onto your X rail if you haven't done so already, assuming your X assembly isn't pre-installed and set up. If your X assembly isn't in the printer, you can easily slide on the entire built assembly onto it, then screw it into the linear rail.
11. Install your Hotend and Extruder. This can technically be done in any order, but note that the motor on the Sherpa Mini extruder will make it difficult/impossible to access the screws for installing the toolhead onto a linear rail. The Hotend screws are also impossible to access with the extruder installed.

These instructions are far from perfect. I recommend just putting the whole thing together outside the printer, so you understand how it goes together, then take the top off and install it onto the printer the way that works for you.

## NOTE
This is a work in progress that may or may not get updates in the future. Use at your own risks. I have put in enough work to get it printable with my machine and my hotend, extruder, and other personal needs/requirements. If you have requests, you're welcome to submit a GitHub issue or make the change yourself using the CAD file and submit a Pull Request.

There are **many** problems with this project. The CPAP fanduct probably needs to be redesigned so it has thicker walls and isn't as easy to break, as well as (somehow) changing the design so that it is easier to reliably print without a tuned printer.


## Gallery
![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/dfc30c1e-5142-4dcc-8c96-0ab1f561f086)

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/a1773a13-d507-42d1-946f-d48ce67ec31b)

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/57b916c6-54e0-49db-82cc-de5a62c62eb5)

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/a27309c6-93f4-45d8-a630-0eaa9729ac3d)

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/821dc777-08e9-4506-beee-cfdf7bcc14a2)

![image](https://github.com/Midnite3DP/midnite-toolhead/assets/84816186/c4abffeb-644d-429e-983e-60f748dad9c5)
