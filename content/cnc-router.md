# The CNC Router - [X-Carve](https://shop.inventables.com/products/x-carve-1)

The X-Carve CNC router works on an XY plane with limited Z-depth, capable of handling dimensions of 1000mm x 1000mm x 50mm. It is specifically designed to cut wood, and in part due to our dust collection system, should not be used for other materials.  
Contrary to a typical CNC machine, our CNC router is designed to move relatively slowly. It relies on tool paths for rounded edges or complex shapes.

## ⚠️ Safety

1. Always keep the router's door closed when power is supplied to it.
2. Secure your workpiece; if it isn't secure, it could go flying. Use a fixture or at least two clamps on each side of your piece.
3. The router collet holding the bit must be properly tightened.
4. **Never** leave the CNC router unattended while it's running. Do not walk away, even for a bathroom break.
5. Running a CAM program on the router is a complex process involving fixturing, homing, and execution. If you haven’t done this before, have somebody walk you through your first run.

## Computer Setup

1. Go to <http://cnc.local.> This should load the cncjs interface.
2. Connect to the router via the UI on the left side of the screen.

## Pre-Cut Steps

Follow these steps before starting a cut:

1. Clean the machine bed.
2. Setup the dust collector:
   1. Connect the hose to the router dust collector.
   2. Open the gate to the dust collector.
   3. Close all other gates for optimum dust extraction.
3. Insert an appropriate cutter into the router and tighten the collet.
4. Close the router's cage.
5. Turn on the machine and home it. Note that 0,0 is to the back right when looking at the front of the machine, and the machine homes to the front left (into the negative direction) and then travels to 0,0.
6. Secure your part and check the collet tightness.
7. Load your CAM code onto the machine, take a pathing pass, and then take the cut pass. Remember, do not leave the machine attended while cutting.

## CAM Information

- The maximum cutting rate of the machine is 2500mm/min.
- Always remember, we operate in metric measurements.

## Fixturing Tips

Here are some options for securing your part:

- Adhere the part to the bed; use a single layer of blue tape to completely cover the matching surfaces of your part and the machine bed, then apply super glue to the tape. Use a super glue activator to help it bind, and stick the part down to the bed. Let it dry for 5-10 minutes before machining.
- Fixturing clamps can secure the edges of your part to the table:
  - Use at least 3 clamps, distributed around the workpiece. Use 4 whenever possible.
  - If any part or scrap will become separated, it also needs fixturing. Consider including bridges in your CAM design.
- Wood screws can be a quick method, but have some limitations:
  - There will be holes in your parts.
  - Any part that will be separated from the rest of the piece during the operation must have at least two screws through it to prevent spin. Consider including bridges in your CAM design.
- For duplicate parts or two sided jobs, build a locating fixture with cutouts or indexing pins. You still need to provide some kind of down-force, such as screws or fixture clamps.
