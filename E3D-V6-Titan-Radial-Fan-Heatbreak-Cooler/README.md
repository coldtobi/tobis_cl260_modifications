# E3D-V6-Titan-Radial-Fan-Heatbreak-Cooler #

License: GPL-2.0+ -- GPL Version 2.0 or later.

    Copyright 2019 Tobias Frost <tobi at coldtobi.de>

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

You can find the "original" git repository on [github].

## What is this?

This is an adapter to allow to mount a radial fan to the fan shroud of a 
E3D-V6 using a [titan] as extruder.

As radial fans are more powerful to work against resistance (e.g a fanduct)
this adapter improves the cooling of the heat break, working against possible
jams due to that. (and of course the fan is bigger :)

This adapter should work with every printer that supports the Titan, but note that
the thickness is 12 mm while your axial fan might be around 7 mm.

I use it on my CL-260 together with my Titan mod, also available in this repo
and on thingiverse: [titan-carrier]


## CAD Model ##

The CAD model can be opened using FreeCAD. It was developed using version 0.18
on Debian. 

The CAD model ist structured in 4 parts: Design, Printables, Assembly and 3rd-Party parts.
The first section are the "raw" designs, suitable for modifications. it also shows 
the complete assembly.

The printables section show the parts that you need to print in (IMHO) the recommendated
orientation on the print bed.

The Assembly section shows an example assembly with my titan carrier.

(the 3rd part, 3rd party models is described below)

### Parts and Printing ###

#### Fanattachment-Titan ####

This part allows that the radial fan be mounted on the Titan. It uses two screws of
the titan assembly for that. You possibly need to replace the Titan screws with bit 
larger ones. 

The fan is assembled using a M4x20mm screws with hex nuts going into the part. One of the 
holes is slotted to allow for different fan types, you probably want to add some glue
to fix the hex nuts when assembled.

Prints without support. 

#### Fanadapter-30mm-Radial ####

This screws to the original E3D V6 fan shroud.
The radial just fan slides into the top part.

Prints without support. 


## 3rd Party Models ##

The FreeCAD Model may also contain a few external objects, listed below with their license:
Those model are only used for illustration, so they are not "derived" work and not subject
to the GPL license of the remaining work.

The Titan assembly model has been modified to have the mirrored version and the
stepper motor / mounting bracket removed. 

You can find the parts in the "3rd Party Models" Group of the FreeCAD file and as a subfolder
in the git repository as source. 

| Part                 | License      | Author         | Source |
|----------------------|--------------|----------------|--------|
| E3D_v6_To_Spec       | CC BY 3.0    | lXGaimMasterXl | https://www.thingiverse.com/thing:341689 |
| 50mm radial fan      | CC BY 3.0    | Brendon Tower  | https://www.thingiverse.com/thing:2717523 |
| Titan Assembly       | GPL 3.0+     | E3D            | https://files.e3d-online.com/Titan/ASM_EX_THUMB_SCREW.stp |
| E3DV6 Fan Duct       | GPL 2.0      | joshuarowley42 |  https://www.thingiverse.com/thing:340312 |

## References ##

- [github] https://github.com/coldtobi/tobis_cl260_modifications
- [titan-carrier] https://www.thingiverse.com/thing:4065490
- [titan] https://e3d-online.com/titan-extruder
