# Monster Kossel: v3.0

A Kossel-inspired Delta printer with:
* large build volume
* an incredibly stiff frame
* an easily fully enclosed build volume
* piezo-based bed probing (Andromeda layout from precisionpiezo.co.uk)
* easy to tune / upgrade setups
* M3 and M5 screws only

![Monster Kossel](preview.png)

## Design history:

V1 started with my taking a Kossel XL idea but noticing the OpenBeam frames just weren't rigid enough. 
I tweaked the STL files with Blender to use 2040 towers instead. It was better... But still a bit wobbly.

V2 was still done with Blender but introduced the T-based towers using 2060 and 2040 extrusions for the maximum possible rigidity.
It also introduced the concept of the fully enclosed build volume. 

It became the test bed for a series of remote drive extruder designs by Dan Cook, which are proving to be incredibly reliable.
The latest iteration of which is a mix of extruder and effector design for Kossel sized rod widths. 
It's proven to handle flexibles as good as a Prusa MK3's stock extruder, if not better.

V3, shared here, is an ongoing effort to properly draw and design a revision of V2 in a proper CAD format.
The aim is to further enhance the experience by incorporating many lessons learned with regards to cable management.
It is currently being drawn and assembled in FreeCAD 0.19_pre release, using the Assembly4 plugin.

## Assembly file(s)

The main assembly file is `assembly2.FCStd`, made for the `A4Plus` plugin installed in `FreeCAD 0.19_pre+`, it will open all the other parts as needed from the folder.

## Current development status

The main frame of V3 has not been tested, and only exists as CAD files at present.

The V3 frame will be built after the telescopic shaft design is fully validated. 
A replacement for the Flex'Y effector may be forthcoming, but will not impact V3 development in any way.
The current and upcoming effector/remote drive extruder are designed by Dan Cook (OCD3D on Thingiverse), and are his designs to distribute.

The V3 repository currently contains a mock step file for validation of the delta and telescopic shaft dimensions.

The telescopic shaft has been built, and is printing successfully on the Flex'Y v17 (not shared as not my design) with regular and flexible filament prints on the V2 frame.
A new revision of the Flex'Y that removes the worm drive is currently being developped to use printed bevel gears instead of a worm drive.

Carriages have been redrawn as the original Kossel carriages designed for the MGN19H carriage pattern don't have enough rigidity when using the adapter plate. They will be mounted and validated on the v2 frame first, then v2 will be used to print the remaining v3 frame parts. All parts will be printed in PETG rather than PLA for heat resistance.

