# CL-260: Carrier and Fan Assembly for E3D's Titan Extruder #

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

This is an modifcation for the CL260 from bowden extruding to direct extruding
using a E3D Titan extruder assembly [titan] and a pancake nema 23 stepper motor [stepper]

When shopping for the Titan: You will need the Mirrored version!

Note as the Titan Aero is not a perfect fit for the CL-260 this mod employs the
original Titan.

This design works best with my other parts for the CL-260, e.g I recommend to use
the Axis Holder [axisholder] to avoid mechanical interference.

## CAD Model ##

The CAD model can be opened using FreeCAD. It was developed using version 0.18
on Debian. 

The CAD model ist structured in 3 parts: Design, Printables and 3rd-Party parts.
The first section are the "raw" designs, suitable for modifications. it also shows 
the complete assembly. 

The printables section show the parts that you need to print in (IMHO) the recommendated
orientation on the print bed.

(the 3rd part, 3rd party models is described below)

### Parts and Printing ###

#### XY-Carrier ####

This is the main part of the carrier. It is designed to hold two LM8UU bearings per axis.
It might be that you need to fixate the bearings with a grub screw, if they slide out
by themselves or you might need to tune in the tolerances accordingly in the CAD. 

Most of the titan assembly and fan assembly is done with M3 screws, many uses
metal inserts, e.g [metal inserts].

There are a lot of extra holes to have a possiblity to mount extra stuff,
so not every hole is used.

Prints without support. I recommend 3-4 perimeters,  20% infill and a 
layer height of 0.2 mm.

Note that the heater block is rotated by 90°. So if you use the silicon sock
for the E3DV6 (you should!), the E3D logo will be sideways, not facing you.

(Another note: the images shows an alternative cooling for the heatsink.
The files for this will be released soonish.)

##### Bugs / known issues #####

- Grub-Screws for bearing fixations not in the CAD.
- The titan aero holder is only fixated by 2 screws, this
  is leads that the titan can be easily "tilted" by an upward force,
  like a pulling filament. A bit of glue or a manually adding another screw fixes that.
  The original purpose was to support the Piezo Z-probe, but I guess this should
  be implemented otherwise (I have plans for this in the future)

#### (left) Fan Assembly ####

The fan assembly mounts a 50mm radial fan using two parts:
- Clamp1
- Clamp2

##### Clamp1 #####

The flag at the end holds a M4 screw that will fixate the fan.
Together with Clamp2, it is screwed to the XY carrier using M3 screws and nuts.
(For this, the two screws at the edge are sufficient, the one below the fan is not needed.) 

Prints without support. I recommend 2 perimeters,  20% infill and a 
layer height of 0.2 mm.

##### Clamp2 #####

This clamps the fan and adapts to the fanduct.

(There are holes for grub screws for the fan duct, but this should not
be necessary due to the snug fit.) 

Prints without support. I recommend 2-4 perimeters and a layer height of 0.2 mm.

##### Fanduct #####

Straightforward... it slides into Clamp2 and can be screwed to the titan
with a screw. The bottom end then interface to a nozzle.

Prints without support. I recommend 1-2 perimeter, and a layer height of 0.15 - 0.2 mm.

##### Fanduct-Nozzle #####

There are two options for a nozzle, just print yourself one and slide it in.
They should be "friction fit", if not add a dap of glue.



The "small" nozzle has a small bug: when designing the E3D hotend was misplaced
in the CAD by a few mm, so it is not centered on the nozzle. Though it still
works quite well.

I'm still experimenting with the 180° one, so I cant tell which one is better,
but for sure it also depends on what you are going to print. Suggested reading
on [cooling].

Both, The "small" and the "180°" shoud be printed with support, but make
sure to select your slicers "from the build plate only" option.
I recommend 2 perimeters and a layer height of 0.1 - 0.15 mm.

#### (right) Fan Assembly ####

there is currently no right fan assembly, as for me a one-fan solution seems
to be good enough.

However, the clamps from the left one can be mirrored and used for a right fan as well.
If you design a fan duct 


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
| titan_aero_holder_v5 | CC BY 3.0    | Frank Jakobsen | https://www.thingiverse.com/thing:2490018 |
| Titan Assembly       | GPL 3.0+     | E3D            | https://files.e3d-online.com/Titan/ASM_EX_THUMB_SCREW.stp |
| E3DV6 Fan Duct       | GPL 2.0      | joshuarowley42 |  https://www.thingiverse.com/thing:340312 |

## References ##

- [github] https://github.com/coldtobi/tobis_cl260_modifications
- [titan] https://e3d-online.com/titan-extruder
- [axisholder] https://www.thingiverse.com/thing:3141984
- [stepper] I'm using a NEMA 17 25mm pancake stepper with 1.8°/step. Make sure that the axle is long enough! (E3D documentation seems to suggest ~22.2mm) Hint: if it is becoming too hot, you can attach a fan to cool it. 
- [metal inserts] available eg. at AliExpress. Outer Diameter around 4.15 mm, lenght 3mm.
 e.g https://tinyurl.com/y9mz845h
- [cooling] http://www.desiquintans.com/coolingtests and http://www.desiquintans.com/coolingtests2
