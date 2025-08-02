# Polygonal Modelling with Maya


> `RECAP:` What we learned last class:

> - How to Navigate Around the UI of Maya
> - How to **Create** basic Polygon objects in Maya (called Polygon Primitives!)
> - How to **Translate**, **Rotate** and **Scale** Objects
> - How to move and object's **pivot**
> - How to **snap** objects together

> `PLAN:`

> - Aspects of Polygonal Modeling with Maya
> - Making an Arch Way Follow Along
> - Modeling a Low Poly Camera Exercise

## Components of a Polygon Object

We've been talking in class about using Polygon primitives, basic shapes such as cubes and spheres, but what exactly is a **Polygon** objects.

In short, polygon objects are made up of three components:

- Vertices
- Edges
- Faces (sometimes called Polygons or Polys)

Before software like Maya, Polygon Models were made by manually entering the location of vertices into a computer. Often modelers and researchers would trace objects and use specialized equipment to find the distance between vertices.

<figure> <img src = "../assets/images/maya_VWBug.png"><figcaption>Image from Image Objects by Jacob Gaboury</figcaption></figure>

Today, **Polygonal Modeling** involves manipulating these three components to create a wide variety of shapes. We are no longer limited to jamming polygon primitives together and now can create objects of our own design.

Let's start by loading the practice file for today's class. Download Here.

After the file is open, you'll notice on the right side of the screen there are a variety of layers.

Layers all us to store different models on different layers of our scene.

<figure> <img src = "../assets/images/maya_layers.png"></figure>

We can begin by turning on the visibility of our "FACES" layer by pressing the left-most button on the layer.

<figure> <img src = "../assets/images/maya_layers_on.png"></figure>

## Faces

To navigate to faces, hover over your model and press the **Right Mouse Button**.

This will bring up our [**Marking Menu**](https://help.autodesk.com/view/MAYAUL/2024/ENU/?guid=GUID-8BA1A3AA-4C44-4779-8B22-0AAE3627E8EB). Marking Menus are context specific and allow us to get easy access to all the functionality of Maya.

You don't click in the marking menu. Instead, however over the tool you want to access and release the right mouse button.

> `UI TIP`: You can use the same marking menu to return to **Object Mode** when you are done selecting on faces.

<figure> <img src = "../assets/images/2_maya_facemode.gif"></figure> 

### Modify

We can modify faces using the translate, rotate and scale tools.

Use the translate, rotate and scale tools to create the object on the right.

<figure> <img src = "../assets/images/2_maya_faces_modify.gif"></figure> 

### Delete

We can also delete faces to allow for interesting shapes.

Use the Translate and Delete tools to make the shape on the right.

<figure> <img src = "../assets/images/2_maya_faces_delete.gif"></figure> 

### Normals

Notice that the inside of our box is black, while the outside is gray.

This is because faces have not thickness to them, they are infinitely thin!
The direction the face is facing is the normal direction. We always want the normal direction to be facing outwards towards our camera.

We'll learn more about the complication of normals as the course progresses, but for now,
let's reverse the normals this model so that the inside of model is correctly facing the camera.

To select all the faces on our model:

1. Click on the model
2. Right click navigate to Face Mode
3. Press **Ctrl+Shift+A** to select all the faces.

<figure> <img src = "../assets/images/2_maya_faces_normal_select.gif"></figure> 

Next, we can press and hold **Shift+RMB** over our model. This will bring up a marking menu of contextual tools related to the component mode that we are in. In our case, it will bring up tools related to faces.

To reverse our normals:

1. Press and hold **Shift+RMB** over our model
2. Navigate to **Face Normals**
3. Navigate to **Reverse Normals**

<figure> <img src = "../assets/images/2_maya_faces_normal_reverse.gif"></figure>

### Extrude

The most important tool associate with faces and for poly-modeling in general, is the **Extrude** tool. The extrude tool allows us to extrude out additional faces from our model to build out geometry.

We can open the extrude tool by using the **Shift+RightClick** marking menu and then navigating to **Extrude Face**.

#### Thickness

In the pop-up box for the tool, we can use the **Thickness** parameter to extrude the selected face. Let's use this parameter to match the model on the right.

<figure> <img src = "../assets/images/2_maya_faces_extrude_thickness.gif"></figure>

#### Offset

The **Offset** parameter allows us to inset our face. Let's use the extrude tool twice to make the model on the right.

<figure> <img src = "../assets/images/2_maya_faces_extrude_offset.gif"></figure>

#### Keep Faces Together

The **Keep Faces Together** parameter will allow us to extrude faces separately.
Extrude all the faces on the cube with **Keep Faces Together** off.

> `UI TIP`: Press **Ctrl+E** with a face selected to bring up the extrude tool.

<figure> <img src = "../assets/images/2_maya_faces_extrude_together.gif"></figure>

#### Hot Keys

Lastly, we can use the **Shift** Hot Key with our Translate, Rotate and Scale tools to quickly extrude.

Hold **Shift** while moving and scaling the top face to make the model on the right.

> `UI TIP:` If you have trouble rotating around face or seeing a face clearly, press the **F Key** on your keyboard to focus on a particular face. The clip below shows what happens when you zoom in on a face.

<figure> <img src = "../assets/images/2_maya_faces_extrude_hotkeys.gif"></figure>

#### Face Selection

Lastly, let's go over a common face selection technique. This allows us to select a large number of faces next to each other at once. Let's follow the below steps to make the model in the "face selection" area.

- Create a new cylinder in your scene and move it over to the "face selection" area. <br><figure> <img src = "../assets/images/2_maya_faces_selection_newcylinder.gif"></figure>
> `UI TIP`:Use the **Shift+RMB** marking menu with nothing selected to quickly create new objects.


- Change the number of sides on your cylinder to 16 to match the object on the right.<figure> <img src = "../assets/images/2_maya_faces_selection_cylindersides.gif"></figure>
>`UI TIP`: We can change the amount of sides our cylinder has in the **Channel Box**.


- Next let's select everything but the top and bottom of our cylinder. We'll do this by selecting on face and then, hold **Shift**, double click on one of the faces next to our selected face. <figure> <img src = "../assets/images/2_maya_faces_selection_cylinderselect.gif"></figure>

- Then, we'll press **Ctrl+Shift+I** to reverse the selection, followed by the **Delete Key** to delete our top and bottom faces.<figure> <img src = "../assets/images/2_maya_faces_selection_cylinderdelete.gif"></figure>








