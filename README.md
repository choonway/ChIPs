# ChIPs - Polycube/Voxel Construction Set

## GPGT

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

I call this the 'bubblebath' technique.

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
click on the bubbles, then the boolean 'operand', the bubbles should disappear
click on the cat model, then click on the boolean 'replace', a pattern should appear on the cat.

Examine the patterns on the frazzled cat. They should match one of the 12 fragments.

Join all the fragments together.

You have your cat.

Some patterns may be be a bit tricky.

It is possible, with enough practice, to build some intuition about the fragment/panels required that you can do all of this without external aids.

## Manufacturing

WIP

## Resources

See the following websites for more information:

https://www.thingiverse.com/thing:5376746

https://www.printables.com/model/192718-chips-polycube-construction-set

https://www.youtube.com/channel/UC7Iy1mVaFCpzOD8v4n6sJXQ

Copyright 2022 by Liao Choon Way

License: CC BY 4.0
