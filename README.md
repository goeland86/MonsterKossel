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

The main assembly file is `assembly_a2plus.FCStd`, made for the `A2Plus` plugin installed in `FreeCAD 0.19` or later, it will open all the other parts as needed from the folder.
The other workbench that is required is the `Fasteners` workbench, to include all the screws & nuts into the assemblies.

## Current development status

The main frame of V3 has not yet been tested in real life, and only exists as CAD files at present.

The V3 frame will be built soon, as the parts have been printed. Dan Cook has released his all in one effector / direct drive extruder on [Thingiverse](https://www.thingiverse.com/thing:4886240/files), including the telescoping shaft of my conception.

The telescopic shaft has been built, and is printing successfully on the Flex'Y v17 (not shared as not my design) with regular and flexible filament prints on the V2 frame.
A new revision of the Flex'Y that removes the worm drive is currently being developped to use printed bevel gears instead of a worm drive.

Carriages have been redrawn as the original Kossel carriages designed for the MGN19H carriage pattern don't have enough rigidity when using an adapter plate. 
All parts will be printed in PETG rather than PLA for heat resistance.

The top cover will come in two versions: one as a blank template for builders to customize the layout of elements on their own, the other as I intend to build it, using 100mm AC extraction ventilation systems with filters, mounting holes for the extruder motor, wire and filament paths.

### BOM

M3 nuts: 69 (bottom assembly: 42, top frame: 12, motor frames: 9, idler centering: 6)

M3 washers: 18 (motor frames: 18)

socket cap M3x5: 15 (motor frames: 3, carriage assemblies: 12)

socket cap M3x8: 69 (tower assemblies: 45, top frame: 12, motor frames: 12)

socket cap M3x10: 24 (bottom frame: 24) - can also be M3x12

button cap M3x15 : 6 (motor frames: 6) - can also be longer, for bed assembly

socket cap M3x16: 18 (bottom frame assembly: 18) - can also be M3x15

countersunk head M3x20: 6 (bottom frame assembly: 6)

socket cap M3x30: 3

socket cap M5x8: 24 (top frame: 12, bottom frame: 12)

socket cap M5x10: 9 (top frame: 9)

socket cap M5x12: 18 (bottom frame: 18)

socket cap M5 Openbuilds flat nuts: 51

F623ZZ flanged bearings: 6 OR idler pulleys for GT2x6mm : 3

Nema 17: 4

16-teeth pulley for 5mm shaft (with M3x4 set screw): 3

Acrylic sheet (3mm): 3x 900mm x 500mm

Acrylic sheet (5mm): 450mm x 400mm


## Credit

I want to thank [Dan Cook](https://www.thingiverse.com/dancook3d/designs) for his wonderful [bevel geared extruder design](https://www.thingiverse.com/thing:4886240/files). We've exchanged a fair bit before he published it, and I'm happy to see that project being this successful on its own.
Additionally he made a [great delta carriage](https://www.thingiverse.com/thing:3070352) which I'm using in the Monster Kossel design.
Both of those designs you'll find the relevant step files in the `STEP` subfolder.
