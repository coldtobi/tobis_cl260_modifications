# Z-Axis guide for the CL-260 #

This parts "holds" the Z-Axis in place from the top position, avoiding the axis
to wobble to much due to the play of my rod-driving nuts.
(Make sure to align the rod, though, the guid only adresses wobble due to the
play of the nut)

## License ##

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

The CAD model can be opened using FreeCAD. It was developed using version 0.17
on Debian. 

The CAD model ist structured in 3 parts: Design files, Assembly and Printables.
The first section are the "raw" designs, suitable for modifications, the
assembly
section shows the complete assembled parts and the printables show the parts
that you
need to print, in the orientation that I've used to print mine.

## BOM ##

Quantity | Part                                                       | Comment
---------|------------------------------------------------------------|-------
         | *Printed Parts*  (names from the CAD model)                |
       2 | printable/Z-Axis_Guide                                     |
         | *Nuts and Bolts*                                           |
       4 | M3 metal inserts (M3, OD=4.2 mm, lenght 3mm)               | e.g https://tinyurl.com/y9mz845h
       4 | M3x10 hex screws                                           |
         | *For assembly to the printer frame*                        | not in the drawing
       4 | M4x10 hex screws                                           |
       4 | M4 T-Nuts for your frame                                   |

## Assembly ##

The metal inserts are ment to be "melt" into the main parts of the main part.
Put on a screw, heat up the screw and push into the plasic part. The assembly
drawing should give you the idea…

## Print Setting ##

I've printed with 3 perimeters and a layer height of 0.25 mm using ABS.
Honeycomb infill was set to 25%.
