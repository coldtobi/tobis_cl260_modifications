# Axisholder for the CL-260 #

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
The first section are the "raw" designs, suitable for modifications, the assembly
sectoin shows the complete assembled parts and the printables show the parts that you
need to print (the numbers at the end say  how often you gonna need it)

## BOM ##

Quantity | Part                                                       | Comment
---------|------------------------------------------------------------|-------
         | *Printed Parts*  (names from the CAD model)                |
       2 | printable/X-Axis                                           |
       2 | printable/Y-Axis                                           |
       4 | printable/Belt_Tightener                                   |
       4 | printable/Clamps                                           |
         | *Nuts and Bolts*                                           |
      18 | M3 metal inserts (M3, OD=4.2 mm, lenght 3mm)               | e.g https://tinyurl.com/y9mz845h
      16 | M3x15 hex screws                                           |
       2 | M3 screws for endstop activation                           |
       4 | M3 nut                                                     |
       4 | M3x~25mm screw (for the belt tightener system)             |

## Assembly ##

The metal inserts are ment to be "melt" into the main parts of the axisholder.
Put on a screw, heat up the screw and push into the plasic part. Put them on the opposite
site of the clamp and they will not be pulled out by the forces of the screw.

The remaining 2 inserts are for the one of the two holes on the "backside" of the main
part. It can then hold a screw suitable to activate the endstop.
