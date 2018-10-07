# Z-Axis Mod #

License: GPL-2.0+ -- GPL Version 2.0 or later.

    Copyright 2017 Tobias Frost <tobi at coldtobi.de>

    This program is free software; you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation; either version 2 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License along
    with this program; if not, write to the Free Software Foundation, Inc.,
    51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.

The complete GPL License text should be part of this repository.

For the avoidance of doubt, "program" can be replaced with "work" in
the license grant above.

## CAD Model ##

The CAD Model can be opened using FreeCAD. It was developed using version 0.17
on Debian. It should give you an idea about the assembly and function.

## BOM ##

(Please make sure to check the CAD, the table might have errors.)

| Quantity | Part                                                    | Comment                                                                 |
|----------|---------------------------------------------------------|-------------------------------------------------------------------------|
|          | * Metal parts *                                         |                                                                         |
| 1        | Main Aluminium plate (270x385x8 mm)                     |                                                                         |
| 2        | Mounting Plates (270x50x6 mm)                           |                                                                         |
| 4        | Connecting Braces (320x30x5 mm)                         |                                                                         |
| 3        | Distance Blocks for glass mounting (50x30x6mm)          |                                                                         |
| 3        | Clamps for Glass (U-Profile) 15x15x2 mm len=40 mm       | See Bugs                                                                |
|          | * Bolts and Nuts *                                      |                                                                         |
| 8        | Cylindrical Head, M3x16 (hex key)                       | to mount threadnut                                                      |
| 3        | Cylindrical Head, M4x6 (hex key)                        | glass-clamps                                                            |
| 16       | Cylindrical Head, M4x20 (hex key)                       | to mount LMK10UU                                                        |
| 4        | Cylindrical Head, M3x40 -- to mount the NEMA17 to plate | not in CAD                                                              |
| 19       | Countersunk Head, M5x16                                 | M5x18 might work too                                                    |
| 3        | Countersunk Head, M5x50                                 | bed-leveling                                                            |
| 8        | Nuts M3                                                 |                                                                         |
| 16       | Nuts M4                                                 |                                                                         |
| 19       | Nuts M5                                                 |                                                                         |
| 3        | Knurled Nut M5 (DIN 466)                                | internet search for DIN 466                                             |
|          | * Rods, Threads, Linear Bearings, ...                   |                                                                         |
| 2        | LMK10UU                                                 | 4 needed, 2 recycled                                                    |
| 1        | Threaded Rods with matching nut                         |                                                                         |
| 2        | Linear Shaft (10mm)                                     | 2 needed, 1 recycled                                                    |
|          | * Printed Parts (not in the CAD)                        |                                                                         |
| 2        | Holder for Stepper Motors                               | File: Motorhalter.fcstd                                                 |
|          | * Others * (some not in the CAD )                       |                                                                         |
| 1        | Glassplate 255x255x5 mm                                 | Borosilicate glass recommended to avoid cracking due to thermal stress. |
| 1        | Heatbed MK3 Aluminium 3.2 mm thick                      | http://reprap.org/wiki/PCB_Heatbed#MK3_ALU-Heatbed_Dual_Power           |
| 1        | NEMA 17 Stepper Motor + Cable.                          | 17HS4401 <== I ordered one of those                                     |
| 1        | A4988 Polulu Stepper Driver Module                      | (optional)                                                              |
|          | * Recycled Parts * (from the CL-260 kit)                |                                                                         |
| 3        | Springs                                                 |                                                                         |
| 2        | LMK10UU                                                 |                                                                         |
| 1        | Threaded Rod + Nut                                      | make sure to order exact the one from the kit or get two!               |

### Recycled parts and other notes ###

For the recyled parts, please make sure to order matching parts. In doubt,
spend a few extra bucks and disregard the recycled ones. It is important to
have identical ones.

As the Heatbed is not really great, I've replaced it with a metalcore PCB one.
While the regular one should also work with the design, I recommend to get one
too.

I'm using 2 stepper driver modules. The RAMP can drive on Z two steppers with
the same driver, but only at half power. Not tried if that is enough juice, so
I recommend to get an extra A4988, just in case.

Regarding the stepper motor: It is ok just to order one and to make them
matching just put the new motor into the X or Y axis and you'll have two
identicals for the Z...

As a general note, check everything as it might contain errors..:
The BOM might be inaccurate, the drawing too...)

## Assembly instructions ##

nothing written here yet..

With the CAD model it should be obvious how to assemble. Note that there are a few threads
to be cut: 3x M5 for the bed-leveling screws and 3x M4 for the glass-clamps.

Precission is key when drilling. I recommend a drill stand for all the drilling
and using proper marking out equipment.

## CL-260 MAX ##

I was told that the CL-260 MAX has different dimensions (400 mm x 400 mm), so this mod might not be 
applicable for this model without tweaks.

## Bugs ##

Nothing without flaws:
- The U-Profiles are not optimal as they take away build space. Better would be an alu flat profile
  in the required dimension.
