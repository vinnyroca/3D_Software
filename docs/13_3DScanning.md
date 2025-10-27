<style>
 img{
    width:600px;
}


</style>

# 3D Scanning

![](../assets/images/13/13_01.png)


## Introduction

3D Scanning is the process of capturing the form and appearance of a real-world object or larger environment to create a 3D model. There are many methods and approaches for creating 3d scans. For example, many of us interact with a 3D scanner everyday when we unlock our digital devices with our face. On an iphone, for example, the TrueDepth camera on the front of a phone, projects many tiny light dots onto your face and scans those dots using an infrared camera. This allows the camera to capture a 3D form of your face that it can use to compare to whenever you try to unlock your phone.


<img src = " ../assets/images/13/13_01a.png" width = "400px"></img>

<small>From the video Using An Infrared Camera To Show How Face ID Works by Insider Tech</small>

Infrared cameras are only one way of many to create 3D scans. Another common method is called Photogrammetry. In photogrammetry, a collection of photos from an object are gathered from all sides. In the simplest terms, those photos are then compared to each other to find key features, from that comparison, approximate camera positions are found - a photogrammetry program can then calculate millions of points in space, defining the shape of the object.

![](../assets/images/13/12_1b.jpg)

<small>Example of photogrammetry courtesy of bitfab.io</small>

In this class, we will be using a type of 3D Scanner similar to the iphone TrueDepth camera. Our 3D Scanner, the MIRACO by Revopoint, uses a combination of infrared cameras to capture the form of an object and a color camera to capture the texture of an object.

![](../assets/images/13/13_00.png)

## Choosing an Object to Scan

3D scanners, and our MIRACO scanner in particular, have the ability to scan a wide variety of objects. The MIRACO can scan objects of all sizes: using the scanner's two modes of near and far, we can scan any object from a small figurine to a car. However, since 3D scanners use camera technologies that are looking for key features some objects are difficult to impossible to scan:

Objects that are difficult to scan and must be treated:

- **Shiny** or **Reflective** objects: these objects bounce light back that camera distorting their shape. Reflective objects need to be painted with a matte paint or treated with a 3D scanning spray to be detected. Reflective objects include hair.
- **Transparent** object: For the same reason that reflective objects are difficult to scan, transparent and translucent objects are not able to be accurately captured by the cameras on a 3D scanner and must be treated with a matter coating.
- **Dark** objects, such as dark rubber. These objects absorb light and cannot be detected by the scanner.
- **Patterned** Objects: objects with many patterns on them such as patterned clothing are difficult to scan as the key features can be lost in the patterning.
- **Thin** objects such as wires: Very thin objects cannot be detected by most 3D scanners.

In his tutorial, we will be using this small statue of Guanyin which is approximately 7 inches tall:


![](../assets/images/13/13_02.jpg)

## Lighting Conditions

It is best to 3D scan your object in a well and evenly lit environment. This will vary depending on how much control you have on your environment. If using a turntable, you can light your object from one direction as shown below as the scanner will typically only be capturing from a single direction. A turn table allows us to slowly rotate our model and hold our scanner still while the object itself rotates.

![](../assets/images/13/13_03.jpg)

## MIRACO Scanner - Making a Project

When starting a new project with the MIRACO scanner it is best to make a new project to store your scans.

To make a new project:

1. Navigate to Model <br><br>![](../assets/images/13/13_04.png)
2. Press the plus button to add a new project<br><br> ![](../assets/images/13/13_05.png)
3. Name your project and press okay. <br><br>![](../assets/images/13/13_06.png)


## Scanning UI and Settings

After making a new project, this will bring you into the scanning UI. The Scanning UI shows the infrared camera on the top left, the color camera on the bottom left and a live view of your scan in the center.


It is best to check your setting before beginning:

1. Press the settings button <br><br>![](../assets/images/13/13_06a.png)
2. Check that: Accuracy = high, Alignment = feature, and, if you want to capture a texture, color is toggled on.<br><br> ![](../assets/images/13/13_07.png)


## Near or Far

There are two size settings with the MIRACO, near or far.

- **Near**: for objects larger than a coin and ideally less than a can of soda. However, it can go up to the size of a human head, a medium size object, if you want to capture more fine details.
- **Far**: for objects larger than the size of a human head and up to around a large car. Captures will have less detail than near mode.

For this example of the statute, we will be using near mode:


![](../assets/images/13/13_08.png)

## Scanning Process

To begin scanning, press the red button with continuous mode set. As seen in the video below, the green parts of the scan indicate parts of the model that MIRACO is accurately scanning. If the MIRACO cannot find recorded features of the model the scan will turn red-orange and it will lose tracking, being unable to capture the object. If the scanner loses tracking, move the scanner until the major features of the model are found again and the 3D scan turns green. It best to keep the scanner at the same distance from your model making sure that the scanner detects the distance as Excellent as indicated at the top of the UI:

![](../assets/images/13/13_10.png)

![](../assets/images/13/13_09.png)

To scan, either slowly rotate your model using the turntable, or slowly move the scanner around your model, making sure that it never loses tracking. If you need to pause scanning, you can press the pause button and resume the scan at anytime after the scanner finds the features of your object.

When scanning your object, it is important to capture the model from all angles to ensure that you are scanning every part of your model.

<iframe width="560" height="315" src="https://www.youtube.com/embed/q88912ngsA4?si=aonrgZ8kIUIWetwy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>


## Turing object

Since the MIRACO tracks key features, after large parts of your model are scanned, you can rotate your object to another angle and continue scanning after the key features are found. In the video example below, the object is rotated on its back to capture the bottom and underside of the model. 

![](../assets/images/13/13_12.jpg)

<iframe width="560" height="315" src="https://www.youtube.com/embed/LwrY8h9t_Gw?si=r6QHL5xKi9QAqyCy" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## Deleting a Scan

If you accidentally create errors within your scan such as misaligning the tracking of your model, you can pause your model and press the x button to delete your scan.

![](../assets/images/13/13_11.png)


## Checking your scan

After you complete your scan, you can quickly check your scan by either rotating around the point cloud to see if there are any large missing areas, or you can create a **One-tap edit**. The one-tap edit will quickly mesh your model allowing you to see if there are any major errors. Errors such as small holes or extra geometry can be removed later. This one-tap edit is mostly to see if you missed parts of your model or if you misaligned your model.

To one-tap edit:

1. Press One-tap edit <br><br>![](../assets/images/13/13_13.png)
2. Make sure Fast is selected and Press apply <br><br>![](../assets/images/13/13_14.png)  
3. Rotate around the completed model using your fingers to see if there are any errors 

### Resume Scan

If there are any errors within your scan, you can use the Resume Scan button to continue scanning to fill in any major gaps:

![](../assets/images/13/13_15.png)  


## Processing Scan

While the MIRACO is an all-in-one 3D scanning, meaning it can both scan and process models, it is often best to process models on your computer using the software **Revo Scan 5**

### Connecting Miraco to PC

1. Open Revo Scan 5
2. Plug the MIRACO into your computer using the white USBC cable
3. On your MIRACO, select Data Transfer and press OK <br><br>![](../assets/images/13/13_15a.png)  

### In Revo Scan 5

1. Make sure the scanner is being detected and your project is present <br><br>![](../assets/images/13/13_16.png)
2. Press the check on your project and press import<br><br> ![](../assets/images/13/13_17.png)
3. Press the three dots on your project and press Open a Project <br><br>![](../assets/images/13/13_18.png)


Processing Model


In Revo Scan 5, we can process our model using the step by step process as listed at the top of the UI. This begins with **Fusion** and ends at **Export**.

![](../assets/images/13/13_19.png)

### Fusion

Fusion with fuse point cloud points together. To fuse a point cloud:

1. Press Fusion
2. Set point distance between .1mm and .2 and press Apply <br><br>![](../assets/images/13/13_20.png)
3. This will create a fused point cloud model <br><br>![](../assets/images/13/13_21.png)


### Isolation

Isolation will detect any hanging objects around our main model. This is used to clean up any excess information that might have been captured while scanning. To isolate an object:

1. Press Isolation and Detect <br><br>![](../assets/images/13/13_22.png)
2. After isolated objects are selected, press Apply <br><br>![](../assets/images/13/13_23.png)

### Overlap Detection, Smooth and Simplify

All three of these options are optional:

- **Overlap**: This is used if you have parts of your model that are overlapping and you want to fuse them together. <br><br>![](../assets/images/13/13_24.png)
- **Smooth**: This is used if you have any unusually sharp areas on your model that you want to remove by smoothing. <br><br>![](../assets/images/13/13_25.png)
- **Simplify**: This is used if your mesh has too much detail causing visual errors. This will simplify the shape of your point cloud and cause you to lose detail. <br><br>![](../assets/images/13/13_26.png)

## Meshing Point Cloud

Meshing our point cloud converts our collection of points into a 3D mesh that can be used into other pieces of software. To mesh your scan:


### Creating Mesh

1. Press Mesh
2. Set Quality to between 6 and 8 > Press Apply <br><br>![](../assets/images/13/13_27.png)
3. Check the meshed result by checking on No Color in the top right corner of the viewport <br><br>![](../assets/images/13/13_28.png)

###  Mesh Isolation

If there are small objects that still exist after the mesh step, you can use mesh isolation to remove them. 

![](../assets/images/13/13_29.png)


### Deleting objects with Selection tools

On the right side of the UI there are a variety of selection tools that we can use to edit our model. For example, if I wanted to delete the large piece of floor that was captured when I turned my model on its side:

1. Select the lasso tool <br><br><img src = " ../assets/images/13/13_30.png" width = "50" ></img>
2. Select the part to delete <br><br>![](../assets/images/13/13_31.png)
3. Press the delete key <br><br>![](../assets/images/13/13_32.png)


### Filling Holes

Often when making a mesh for our point cloud there will be holes in our model. We can fill-in these holes using the fill hole tool. To fill holes:

1. Select Fill Holes and press Detect<br><br> ![](../assets/images/13/13_33.png)
2. This will display holes within the model<br><br> ![](../assets/images/13/13_34.png)
3. Select each hole individually or select all holes. <br><br>![](../assets/images/13/13_35.png)
4. Decide if the hole should be filled in with a curved mesh or a flat mesh
5. Press apply.<br><br> ![](../assets/images/13/13_36.png)

### Cleaning up Geometry

If you notice small irregularities in your geometry, you can use the selection tools and the delete keys to remove parts of your model. If you create new holes within your model, you will need to repeat the Fill Hole operation.

![](../assets/images/13/13_37.png)

### Smooth

Smooth will smooth out jagged parts of your mesh. To smooth your model:

1. Select Smooth and Apply <br><br>![](../assets/images/13/13_38.png)

### Simplify

Simplify will reduce the topology of your model. It is good practice to reduce the topology of your model by around 20 percent depending on the density of your mesh. 

To view the density of your mesh:

1. Navigate to Display > Mesh Model Display > Wireframe Overlay <br><br>![](../assets/images/13/13_40.png)

To simplify mesh:

1. Select Simplify
2. Set ratio to between 20 and 40 percent and press Apply <br><br> ![](../assets/images/13/13_39.png)

## Texture

We can create a texture from our image data by using the texture tool. To create a texture:

1. Press the texture tool
2. Select Color Image and press Apply


![](../assets/images/13/13_41.png)

## Export

To Export your model:

1. Press Export > Texture Mesh <br><br>![](../assets/images/13/13_42.png)
2. Save your model as a .obj file <br><br>![](../assets/images/13/13_43.png)


## Importing your 3D Scan into ZBrush

1. Press Import in the Tool menu and select your .obj file <br><br> ![](../assets/images/13/13_44.png)
2. Click and drag in your viewpoint to import your model
3. Press Edit

![](../assets/images/13/13_z_01.gif)

### Add Texture to Model

1. Set material to SkinShade4
2. Navigate to Texture > Import in the Top Shelf
3. Select your Texture

![](../assets/images/13/13_z_02.gif)

### Applying Texture to Model

1. In your tool menu, Select Texture Map
2. Select NewTexr > Select your texture in the Image Section

![](../assets/images/13/13_z_03.gif)

### Fix Texture

ZBrush, by default, flips UV vertically. To fix this error we need to flip our texture.

1. Navigate to Texture
2. Select your texture and press FlipY
3. Reselect your texture in the Tool panel

![](../assets/images/13/13_z_04.gif)
























