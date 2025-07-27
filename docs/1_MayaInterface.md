

# Maya Interface & Object Creation

## Getting Started  

Let's start by opening Autodesk Maya 2025 or 2026 on the lab computers. You can navigate to the search menu on the bottom of your screen and search for "Maya."<br><figure> <img src = "../assets/images/Maya_Loading_Screen.png"><figcaption> Maya Loading Screen </figcaption></figure>  

This will open you to the Maya homepage where we can create a new project by pressing new. <br><figure> <img src = "../assets/images/Maya_New.png"> </figure>

You might notice that we need to keep tabbing back and forth between our tutorial and our Maya interface. Since in the lab we are only using one monitor, lets use Windows default split screen feature to create a divided screen. 

Click on top bar of your Maya interface and hold the **Windows Key** and then tap the **Left Arrow Key.** Release the **Windows Key** and you should then see the option to click our **Browser** to have the two screens side by side.

By click and dragging on the dividing line between the two screens you can change the amount of your screen each window takes up. This class website has flexible scaling so feel free to make the **browser** as small as you like.

We'll be using this technique for the remainder of this class so refer back to this section if you forget the order of operations.

## Maya Interface
<figure> <img src = "../assets/images/Maya_Interface.png"><figcaption> My Maya interface</figcaption> </figure> 

Although the Maya interface seems very confusing at first, as we move through the course you will notice that your navigation of buttons and menus will become more intuitive. Our readings for this introductory module will introduce software studies through an examination of Maya's interface.

To keep things simple, we will cover parts of the interface as needed for different parts of the course. As a continuous reminder, as an experimental arts course we are not looking for technical *mastery*, we are looking to understand Maya/3D software in general artistically and critically.
___

## View Panel

In the center of our screen we have our [view panel](https://help.autodesk.com/view/MAYAUL/2025/ENU/?guid=GUID-455539A6-3506-458C-92DA-14F171C14553). This is where we can view 3D objects and manipulate them in real time.

> `Although we are just starting, begin to consider the relationship between the view panel, which shows a live 3D view, and the various data points around this central portion. How is a 3D model both represented as a real-time image and data?`

_You might see four view panels as shown below:_

<figure> <img src = "../assets/images/maya_four_panels.png"><figcaption> Four view panels</figcaption> </figure>

If you do not see four panels, hover over your main panel and tap the *space* key.

Each of these view panels represents a different way of viewing our model.

To make things easier, lets create a basic 3D model (called a [polygon primitive](https://help.autodesk.com/view/MAYAUL/2025/ENU/?guid=GUID-45D2EAD4-5BCF-42DA-A1AB-EC6EE09FE705)) to see how an object appears in each view port.

Click on the icon of the cube within the Poly Modeling [Shelf](https://help.autodesk.com/view/MAYAUL/2025/ENU/?guid=GUID-4A21F741-C9AC-4AE5-897E-B6F8C68ADF90) located in the upper right corner of your screen.

<figure> <img src = "../assets/images/maya_cube_polymodelingshelf.png"></figure>

In the center of our screen, we should now see our cube four, each time from a slightly different perspective. Each of these view ports represents a different way of viewing our model.

<figure> <img src = "../assets/images/maya_cube_four_viewports.png"><figcaption> Four view panels with Cube (I have zoomed in on the cube slightly)</figcaption></figure>

We can infer what each of these view panels are displaying based on the name at the bottom of each quadrant. The image below shows the name of the perspective view port (persp). While the other view panels show the cube from the top, front and side position using orthographic projection. We'll learn a bit more about the technology of *projection* later on in the course but what we need to know for now is that these view panels are showing the two-dimensional representation of a three-dimensional object.



<figure><img src = "../assets/images/maya_cube_persp.png" style = "width: 50%;"></figure>
- Perspective Projection: a method for projecting a 3D object onto a 2D picture plane to approximate how a 3D object might be viewed by a camera IRL.

- Orthographic Projection: a method for projecting an 3D object to make all lines parallel. You might think for now of *isometric* projection used in many video games or architectural drawings.


<figure><img src = "../assets/images/rct2.jpg"><figcaption> Isometric Projection in Roller Coaster Tycoon 2 - Image: <a href="https://www.giantbomb.com/rollercoaster-tycoon-2/3030-11178/">Giant Bomb</a></figcaption></figure>

Now that we have a slight understanding of what we are looking at in our view panel, let's begin to dive into the relationship between our object and our scene.
___

## Cartesian Coordinate Space

You might remember from your math classes learning about unit space, or what is more formally known as Cartesian Coordinate space (named after René Descartes). This is a simple coordinate system where, generally, each whole number is marked in a grid structure. You can see a simple example below with some points marked using the common (x,y) notation with x being the horizontal axis and y being the vertical axis.

<a title="Kbolino, Public domain, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Cartesian-coordinate-system.svg"><img width="512" alt="Cartesian coordinate system" src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Cartesian-coordinate-system.svg/512px-Cartesian-coordinate-system.svg.png?20240520164627"></a>

The important thing to know here is that Maya, and all 3D programs, make use of this coordinate space to visualize the location of models within our scene. The only difference from the image above is that instead of making use of a 2D x,y space, in Maya we use a 3D (x,y,z) space.

In our Maya interface, we should see four view panels. Let's hover over our Perspective view panel and tap the **space key** to maximize this panel.

We should see our cube highlighted with a green outline. If not, we can click on our cube.

Finally, press the **W Key** on your keyboard. We'll talk more shortly about what this hot key does. This should show the Gizmo on our cube.

<figure><img src = "../assets/images/maya_cube_gizmo.png" ></figure>

>**UI TIP**: Press the + or - key to change the size of your gizmo

The **Red Arrow** points in the direction of the positive **X Axis**, the **Blue Arrow**, the positive **Z Axis**, and the **Green Arrow**, the positive **Y Axis**.

> **NOTE:** Different 3D software represent the coordinate space differently. While Maya uses the Y Axis to represent the vertical direction, some software use the Z Axis.

What we can infer is that our cube, being in the center of our grid, is at the (0,0,0) position, also known as the origin point. We can see a numerical representation of our object in the coordinate space by looking at our **Channel Box**.
___

## Channel Box

<figure><img src = "../assets/images/maya_cube_channelbox.png" style = "width: 50%" ><figcaption> The Channel Box with our Cube selected. Our cube is named pCube1 (the first polygon cube in our scene!)</figcaption></figure>

The Channel Box is UI panel that allows us to quickly see information about our model. The Channel Box is most commonly used in animation to edit various aspects about our models quickly, but it is also a great descriptor of basic information about our model.

We can notice that our Channel Box is separated into different values:

- **Translate**: The position of our object.

- **Rotate**: The rotation of our object.

- **Scale**: The size of our object.

- **Visibility**: Whether or not our object is visible in the scene (we'll touch on this later in the course.)

To start, try inputting some values into of of the **Translate** Channels to see how it affects our Cube.

> **UI TIP:** If you click on a channel such as **TranslateX** and see it highlight, you can **click and drag** your **middle mouse key** to smoothly change the values of the channel.

Notice how changing the channel values of **Translate** directly affects the position of our object within our scene.

Now let's try the opposite. Make sure you can still see the translate gizmo on your cube by clicking on your cube and pressing the **W Key**. Then, **click and drag** on one of the arrows to translate your cube in the view panel. Notice how the corresponding channel values change as you translate your cube.

> **UI TIP:** If you **click and drag** on the plane between two axis, this will move your object along two axes simultaneously. Also notice that our last click axis is highlighted yellow. <figure><img src = "../assets/images/maya_cube_gizmo_plane.png" ><figcaption> By clicking on this highlighted plane, we can move our object along the X Axis and Y Axis </figcaption></figure>

Now, that we have moved our object around a bit, we might notice that it is hard to see how our object is exactly moving from our single viewing perspective.

Let's return our Cube to the origin point by entering in **0** for **Translate X,Y, and Z** in our channel box and begin to discuss view panel.
___

## Navigating around our View Panels

One of the most important UI interactions with Maya in navigating around the 3D space of our perspective view panel. Luckily, view port navigation in Maya is quite simple and only uses our **Alt Key** and **Mouse Buttons**.

### ZOOM:
First, let's try zooming into our cube. Hold the **Alt Key** and **Right Mouse Button** and begin dragging in the vertical or horizontal direction. You will notice that dragging on the positive Y and positive X zoom us out, while dragging on the negative Y and negative X zoom us in. <figure><img src = "../assets/images/maya_cube_zoom.gif" ><figcaption> Zooming In and Out</figcaption></figure>

### ROTATE:
Next, let's try rotating around our cube. Hold the **Alt Key** and **Left Mouse Button** and begin dragging in the vertical or horizontal direction. Notice the different behaviors between dragging vertically and horizontally.<figure><img src = "../assets/images/maya_cube_rotate.gif" ><figcaption> Rotating around our Cube </figcaption> </figure>

## PAN:
Lastly, let's try panning around our scene. Hold the **Alt Key** and **Middle Mouse Button** and begin dragging in the vertical or horizontal direction. Panning allows us to focus on different parts of our scene.<figure><img src = "../assets/images/maya_cube_pan.gif" ><figcaption>Panning around our Scene</figcaption> </figure>

> **UI TIP:** If you loose track of your object in your scene or if you want to focus on a particular object, you can click on any give object and press the **F Key** to *focus* on that object. When you focus on an object and then rotate your camera, you will notice that the camera will rotate around the particular focused object.

> **NOTE:** What is actually happening behind the scenes when we pan, rotate and zoom, is that we are moving a camera called "persp" (from which our View Panel gets its name) changing the properties of this camera. You can click on this camera in the left side of your screen in the **Outliner** (which we will cover shortly) and edit properties such as the Focal Length of your pesrp camera in the Channel Box.<figure><img src = "../assets/images/maya_cube_camera.png" ><figcaption>persp camera made visible!</figcaption> </figure>

> **NOTE:** In our orthographic view panels, we are only able to pan and zoom.






















