# UV Mapping

`Recap:`

- The 3D Process Large Scale, Indie and Individual
- Boolean Modeling
- Topology Reduction
- Flow of Topology
- Importing Images
- Modeling complex models from Images

`Plan:`

- What are UVs and what is UV unwrapping
- How to unwrap and clean up UVs in Maya

## What are UVs

For a brief explanation of what UVs are, and why we need to use them when producing 3D models for renders, animations, and games, check out this video:

<iframe width="560" height="315" src="https://www.youtube.com/embed/Yx2JNbv8Kpg?si=4xexsHra9x6HDAsg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

UV mapping, in short, is a way to transfer a 3D model into a 2D space so that we might be able to apply textures to that model.

## UVs and Maya

In Maya, we can create UVs using the UV Editor and a variety of tools associated with it.

There are many complex ways to produce UVs in Maya.

We will be using an extremely simple workflow that allows for easy UV creation.

This workflow uses the following steps:

1. Separate objects by material.
2. Clear all existing UVs
2. Identify seam edges and cut.
3. Unfold UVs using Unfold
4. Use Layout, Straighten, Rotate, Move and Scale as necessary to create UV layout

## Creating Materials

The best first step to unwrapping our model is deciding which material our model will be made out of. This will help in guiding where the seams of our model will go. If our model only has one material, we can just apply a single material to the whole model.

To apply separate materials to different parts of our model:

1. Select the faces where we want our material to be applied. ![gif](../assets/images/5/05_Materials_01.gif)
2. Right Click on the faces > Assign Favorite Material > Lambert ![gif](../assets/images/5/05_Materials_02.gif)
3. In the Attribute Editor, select the tab of the newly created material. ![gif](../assets/images/5/05_Materials_03.gif)
4. Change Type to Ai Standard Surface ![gif](../assets/images/5/05_Materials_04.gif)
5. Name your material. ![gif](../assets/images/5/05_Materials_05.gif)
5. Change the color value to a unique color to distinguish it from other materials ![gif](../assets/images/5/05_Materials_06.gif)

If you need to apply that same material to other parts of your model:

1. Select the faces where we want our material to be applied. ![gif](../assets/images/5/05_SameMaterial_01.gif)
2. Right Click on the faces > Assign Existing Material> Name of your material ![gif](../assets/images/5/05_SameMaterial_03.gif)

Make sure to assign materials to all parts of your model.
![gif](../assets/images/5/05_SameMaterial_04.gif)
![gif](../assets/images/5/05_SameMaterial_05.gif)

The main reason we are assigning materials as our first step, is that we will be using a program called Substance Painter to create our textures and materials. Substance Painter identifies different parts of our model by the different materials they contain. It will also help us see more clearly where we can place seam lines on our model.

## UV Editor Workspace

To enter the UV Editing workspace within Maya:

1. Navigate to the Workspace drop down in the upper right corner of the UI 
2. From the dropdown, select UV Editing

![gif](../assets/images/5/05_Workspace_05.gif)

The UV Editing workspace will bring up the UV Editor and the UV Toolkit.

## Clear Existing UVs

The easiest way to clear existing UVs is to apply a Planar UV to our model. A Planar UV will use a plane to project onto our model, creating a flat set of UVs.

1. Select your object
2. Navigate to UV > Planar

![gif](../assets/images/5/05_Clear_01.gif)

## Identify and Cut Seams

The best place to cut seams is where they might exist naturally on our model. This might be the seam lines of clothes, where two metal panels meet, or along the edge where two bits of plastic are attached together. This will vary greatly depending on the type of model that you are building.

As an example:

Using this Jack as my model, I would first cut seams along the separating edge between the two materials.

To cut a seam:

1. Select all the edges I want to cut.
2. Navigate to UV >  Cut UV Edges (If I need to un-cut an edge, I can use UV > Sew UV edges)

![gif](../assets/images/5/05_UV_01.gif)

Next, I would cut along the bottom of my Jack tip to allow the UV object to unfold.

![gif](../assets/images/5/05_UV_02.gif)

For the body of the Jack, I can begin by cutting all the center edges.

![gif](../assets/images/5/05_UV_03.gif)

Then, along the right and left side, I can cut from the end of one protruding part to the other. This will add in an edge that will allow each segment to open and unfold.

![gif](../assets/images/5/05_UV_04.gif)

## Unfold and and Clean-up

Now that I have cut my UV seams, I need to unfold my UVs.

1. With our object selected, navigate to the Unfold dropdown in the UV Toolkit window
2. Select Unfold

![gif](../assets/images/5/05_Unfold_01.gif)

With our object unfolded, we can then layout all the UV Shells in our UV Editor.

To layout our UVs

1. With our object selected, navigate to the Arrange and Layout dropdown in the UV Toolkit window
2. Select Layout

![gif](../assets/images/5/05_Unfold_02.gif)

If we want to Move, Rotate and Scale our UV Shells:

1. Use Right Click in our UV Editor and navigate to UV Shell
2. Use Move, Rotate and Scale Tool to Change the layout of our UVs.

## Checker Map

When editing our UVs, sometimes it is beneficial to a have a default texture on our model so that we can see the changes that the UV map is making.

To turn on a checker map:


1. In your UV Editor window, navigate to Textures > Checker Map

![gif](../assets/images/5/05_Unfold_03.gif)
