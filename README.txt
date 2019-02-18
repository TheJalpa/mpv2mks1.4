This is my current configuration that i'm using for marlin with the following hardware:

- monoprice v2 select 3d printer in which the meltzi board went up in smoke, along with the power supply.
- Replacement power supply, Mean Well NES-350-12 12V 350 Watt Ul Switching Power Supply 110-240 Volt
- replacement board is a KINGPRINT MKS 1.4 RAMPS
- BIQU Heat Bed Power Module Expansion Hot Bed MOS Tube for 3D Printer
- KINGPRINT 12864 LCD Graphic Smart Display Controller Board with Adapter and Cable for 3D Printer Ramps 1.4 RepRap 3D Printer Mendel Prusa Arduino
- BIQU A4988 Compatible Stepper StepStick Motor Diver Module with Heat Sink for 3D Printer Controller Ramps 1.4(Pack of 5pcs)

Addons:
- BLTouch sensor

Printed stuff used:
- https://www.thingiverse.com/thing:3236858 (didn't quite clear my fan on monoprice v2 select, had to slightly trim edge)
- https://www.thingiverse.com/thing:2010282 to mount meanwell power supply
- https://www.thingiverse.com/thing:1725755 to mount MKS to meltzi mount spot

Current motors used on my printer:
- Extruder - C17HD401202-02N (moons)
- X - C17HD40102-02N (moons)
- Z - C17HD6039-06N (moons)
- Y -  C17HD40102-03N (moons)

I take zero responsibility for anyone attempting to use this config, it's just an example of what i've been trying to load for my particular setup.
I will update this as more info becomes available and I've thoroughly tested the crap out of it.
As it stands of this update the following has been tested:

(First week)
- Increment steps of 5C up to 240C for nozzle, temp tested with thermal gun
- Increment steps of 5C up to 70C for bed, temp tested with thermal gun
- Wires for heat bed and nozzle tested with thermal gun to ensure no draw issues
- all axes are homing properly thus far
- LCD config is working perfectly, reads SD card and will attempt to print from SD card
- Auto home used to make sure it measures properly, and functioned just as I'd expect it to.
- Ramped the temp up to 70C on heatbed, then quickly changed to 40, turned it off while usb was on and the drastic temp change forced it into thermal
runaway mode, so the feature seems to catch the heat differences as expected.  Though I have no way at this time to properly test thermal runaway
in a real scenario, going to research a way to test this in a "real" scenario via artificial means to make sure it protects it as intended.
- Ran some petg through it to make sure the nozzle temp vs extrusion was working, got wonderful petg barf as would expect.

(third week)
- prints going reliably, working fantastic.  still haven't finished buttoning up the case since it's still halfway hanging out of the printer, but it's printing beautifully.  Changed a few things on the stepper calibration to make sure it was accurate.
- bltouch also installed, working beautifully.
Again, use this config at your own risk.  I will be updating and testing as I find more information and get a chance to run through this
and test the everliving crap out of this.
