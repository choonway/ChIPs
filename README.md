# ChIPs - Polycube/Voxel Construction Set

## [GPGT] No more SNOT. You will only need 4 types of bricks

| polycube/voxel | ChIPs |
| --- | --- |
| ![](img/magicavoxel_cat.png) | ![](img/ChIPs_cat.png) |

## tl;dr
Have you wanted to use a construction set to build a model, but don't want to deal with complicated techniques to remove studs / build sideways? Not Square? Too many different types of bricks? Something you can freely 3D print cheaply? etc. Look no further, this is the construction set for you!

## Introduction
ChIPs (Choonway's Interlocking Panels) is an open source (CC-BY 4.0) construction set system that uses interlocking finger joints between panels orientated at 0 degrees or 90 degrees with respect to each other. The resulting object has smooth surfaces on all faces, sharp edges and results in a close physical manifestation of polycube puzzles / voxel art.

![](img/ChIPs-37.5mm-vs-25mm-3DPrinted.png)

On the left is the 37.5mm cube variant with panels colored by type. On the right is the featured cat model using 25mm cube variant with sharp corners. The dimension of the cube variant refers to the length of the side of the unit cube.

![](img/ChIPs-3Dprinted.png)

Only 4 unique panels (Blue, White, Yellow and Orange) are required for building any model. The 5th panel is optional for sharp corners. Note the sharpness of the ears between the 2 models.

## Guided Build Tutorial

At first glance it might seem confusing which panels to join together to make the object, but not to worry, there is an easy way to figure it with the use of [Ephtracy's MagicaVoxel](https://ephtracy.github.io/).

I call this the 'bubblebath' technique. vox files available [here](vox/cat_tut.vox)

![](img/tut-1.png)

Here we start off with a cat voxel shape, with one voxel per unit cube.
Click on 'Fit Model Size' and take note of the bounding box size X = (5, 9, 8) of the original model

![](img/tut-2.png)

Create the unit bubble (3D checkerboard on a 2x2x2 volume)

![](img/tut-3.png)

Double the size of the bubble and cat

![](img/tut-4.png)

Expand the bubble using the formula below

floor(X/2)+1 = (3, 5, 5)

![](img/tut-5.png)

Grid lines shown for clarity.
Move the cat into the bubble, align with right face,

![](img/tut-6.png)

and take one step into the bubble.

![](img/tut-7.png)

Repeat for front and top faces
In effect we are intermeshing the bubbles a half cube step with the cat model.

![](img/tut-8.png)

In the World View,
Click on the bubbles, then the boolean 'operand', the bubbles should disappear.
Click on the cat model, then click on the boolean 'replace', a pattern should appear on the cat.

Examine the patterns on the frazzled cat. They should match one of the 12 fragments. vox files available [here](vox/cat_frag.vox)

| fragment | ChIPs build youtube video | example locations on cat |
| --- | --- | --- |
| 1 | [0:04](https://www.youtube.com/watch?v=te_LA7-NAmI&t=4s) | ![](img/cat-frag-1.png) |
| 2 | [0:22](https://www.youtube.com/watch?v=te_LA7-NAmI&t=22s) | ![](img/cat-frag-2.png) |
| 3 | [0:44](https://www.youtube.com/watch?v=te_LA7-NAmI&t=44s) | ![](img/cat-frag-3.png) |
| 4 | [1:14](https://www.youtube.com/watch?v=te_LA7-NAmI&t=74s) | ![](img/cat-frag-4.png) |
| 5 | [1:54](https://www.youtube.com/watch?v=te_LA7-NAmI&t=114s) | ![](img/cat-frag-5.png) |
| 6 | [2:25](https://www.youtube.com/watch?v=te_LA7-NAmI&t=145s) | ![](img/cat-frag-6.png) |
| 7 | [2:56](https://www.youtube.com/watch?v=te_LA7-NAmI&t=176s) | ![](img/cat-frag-7.png) |
| 8 | [3:31](https://www.youtube.com/watch?v=te_LA7-NAmI&t=211s) | ![](img/cat-frag-8.png) |
| 9 | [4:29](https://www.youtube.com/watch?v=te_LA7-NAmI&t=269s) | ![](img/cat-frag-9.png) |
| 10 | [5:14](https://www.youtube.com/watch?v=te_LA7-NAmI&t=314s) | ![](img/cat-frag-10.png) |
| 11 | [6:00](https://www.youtube.com/watch?v=te_LA7-NAmI&t=360s) | ![](img/cat-frag-11.png) |
| 12 | [6:53](https://www.youtube.com/watch?v=te_LA7-NAmI&t=413s) | ![](img/cat-frag-12.png) |

Fragments 11 and 12 are not used by the cat model. They can be tricky to identify especially if visibility on the opposite diagonal end is limited and be mistaken for Fragments 2 or 4.

Join all the fragments together and you have your cat.

It is possible, with enough practice, to build some intuition about the fragment/panels required that you can do all of this without external aids.

## Tiny Table build video

A full build of a tiny table on youtube. Click on the image below to follow the link onto youtube.

[![](img/table-example.png)](https://www.youtube.com/watch?v=VmErPDY7BgU)

vox files available [here](vox/table.vox)

## Other Examples

![](img/ChIPs-25mm-3DPrinted.png)

An assortment of shapes using 25mm cube variant.

![](img/ChIPs-37.5mm-3DPrinted.png)

An assortment of shapes using 37.5mm basic cube variant.

## Manufacturing

STL files are available for both 37.5mm and 25mm basic cube variants. If you want to build your own variant, parametric FreeCAD files are available. Look through the spreadsheet to adjust parameters.

The panels were designed to be printed in Vase mode, and printed in an array where each panel is printed completely before moving on to the next. The .3mf file to do this was done using PrusaSlicer.

The generated .gcode files are meant for PrusaMini+ printing using PLA. If you want to change materials you will have to go back to edit the .3mf file

Click on this [link](https://www.youtube.com/watch?v=LtgmES9rL5E) to see the print process of the 37.5mm variant panel 4. Note that this printing was done extremely conservatively - you can speed things up by editing the .3mf file

On the other hand the precompiled .gcode for the 25mm variant is done at full speed. If you have problems you can dial back the speed, or look at different brands/colors of filaments.

[Harvesting](https://www.youtube.com/watch?v=6bc6--hOfok) the panels.

## Resources

https://www.youtube.com/channel/UC7Iy1mVaFCpzOD8v4n6sJXQ

Copyright 2022 by Liao Choon Way

License: CC BY 4.0
