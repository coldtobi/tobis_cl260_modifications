# CL-260: Carrier for E3DV6 #

License: GPL-2.0+ -- GPL Version 2.0 or later.

    Copyright 2018 Tobias Frost <tobi at coldtobi.de>

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
on Debian, but parts of the model have been imported from earlier versions of FreeCAD
(the ones without a Body element) 

The CAD model ist structured in 3 parts: Design files, Assembly and Printables.
The first section are the "raw" designs, suitable for modifications, the assembly
section shows the complete assembled parts and the printables show the parts that you
need to print (the numbers at the end say  how often you gonna need it)

(the 4th part, 3rd party models are described below)

The model is still missing the fanducts... the original FreeCAD model broke and I 
still have to reconstruct it... 

### Parts and Printing ###

#### HET 1 ####

This is the main part of the carrier. It can hold one or two LM8UU bearings,
according to your taste.It runs fine with just one, this is the configuration
I'm using.

The metal inserts are ment to be "melt" into this part of the holder).
Put on a screw, heat up the screw and push into the plasic part. 

Printing should be possible without supports; I've used the orientiation as
shown in the "printables" section of the model (and how the stl are exported)

#### HET 2 ####

The second part clamps the E3DV6 to the first part, using 2 screws. The other two holes
take the top screws of the 40x40 fan, which cools the heatsink.

#### FanShroud ####

Well, it goes around the heatsink… It takes the other two screws of the fan to fix everything
together...

#### Clamp ####

The clamp (not shown on the screenshot) was intended to house a piezo for piezo-
based z-homing. I never came around to actually use this…
In other words, you probably won't need it, and it likely needs tweaks to work
for the original purpose. 

#### Fanduct ####

The fanduct in the model is a two piece design: The main body and the outlet.
Unfortunatly the original FreeCAD model broke, so it is only there without the
possiblity to redo. There was also a second fanduct, but its model is damaged
beyond repair in the same FreeCAD file, so it needs to be redesigned later.

However, I'm ousing it only with the (included) Fanduct, so the second one is
optional.

I recommend to use a sleeve for the hotend, to thermally isolate it and prevent
cooling by the airflow.

## 3rd Party Models ##

The FreeCAD Model may also contain a few external objects, listed below with their license:
(Those model are only used for illustration, so they are not "derived" work and not subject
to the GPL license of the remaining work.)
You can find the parts in the "3rd Party Models" Group of the FreeCAD file and as a subfolder
in the git repository as source. 

| Part            | License      | Author         | Source |
|-----------------|--------------|----------------|--------|
| E3D_v6_To_Spec  | CC BY 3.0    | lXGaimMasterXl | https://www.thingiverse.com/thing:341689 |
| LM8UU           | CC BY 3.0    | 3DRap.it       | https://www.thingiverse.com/thing:1811769 |
| 50mm radial fan | CC BY 3.0    | Brendon Tower  | https://www.thingiverse.com/thing:2717523 |



## BOM ##

| Quantity | Part                                           | Comment                          |
|----------|-----------------------------------------------|----------------------------------|
|          | **Printed Parts** (names from the CAD model)  |                                  |
| 1        | printable/HET1                                | main part                        |
| 1        | printable/HET2                                | part for clamping the E3DV6      |
| 1        | printable/FanShroud                           | guiding the air                  |
| (1)      | printable/Clamp                               | optional. The clamp was intended for holding a piezo, but this feature is untested.   |
| 4        | printable/Clamp                               |                                  |
|          | **Nuts and Bolts**                            |                                  |
| 3-7      | M3 metal inserts (M3, OD=4.2 mm, lenght 3mm)  | e.g https://tinyurl.com/y9mz845h |
| 1        | M3x?? hex screws                              | fanshroud 1 mounting             |
| 2        | M3x?? hex screws                              | HET2 -> HET1 mounting            |
| (4)      | M3x?? hex screws                              | clamp mounting                   |
|          | **other parts**                               |                                  |
|          | 40x40 mm Fan with its screws                  |                                  |
| 2-4      | IGUS 15mm Linear bearings                     | There is place for 2 in series, but it also works with just one per axis.  |

## TODO ##

- Illustrate the screws and inserts in the CAD
- Reconstruct the fanducts.
- Make the Piezo thing (and make it working).





