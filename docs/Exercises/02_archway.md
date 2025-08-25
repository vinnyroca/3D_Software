
# Class Exercise: Archway

To combine all the skills we learned today, we are going to be making this archway!

You can preview the final model by turning on the visibility of the "ARCH" layer in the Polygon Modeling practice file.

<figure> <img src = "/assets/images/02_maya_arch_0.png"></figure>

>`NOTE`: There are many correct ways to make the same 3D model! This is just one way of many to make this archway.


1. Make a cylinder and use the channel box to give it 16 sides - enter the value in "Subdivision Axis"<br><br><figure> <img src = "/assets/images/02_maya_arch_1.gif"></figure>
2. Select all the sides of the cylinder by either using **Box Select** or by using selecting one face and the **Shift+Double Clicking** on an adjacent face.<br><br>Then invert the selection using **Ctrl+Shift+I** and delete the top and bottom faces. <br><br><figure> <img src = "/assets/images/02_maya_arch_2.gif"></figure>
3. Rotate the cylinder 90 degrees along the X Axis. Hold the **J key** while rotating to snap to 15 degree increments.<br><br><figure> <img src = "/assets/images/02_maya_arch_3.gif"></figure>
4. Enter face mode, and delete the bottom half of our cylinder.<br><br>Use the scale tool in object mode to make it thinner along the Z Axis.<br><br><figure> <img src = "/assets/images/02_maya_arch_4.gif"></figure>
5. Select the center 8 edges on the outside of our arch and extrude them along the Y Axis. <br><br><figure> <img src = "/assets/images/02_maya_arch_5.gif"></figure>
6. The scale tool can also be used to flatten edges to a common height <br><br>With the top 8 edges selected, scale the edges along the Y Axis to make them level.<br><br><figure> <img src = "/assets/images/02_maya_arch_6.gif"></figure>
7. Our normals are facing the wrong direction! Enter face mode, select all the faces using **Ctrl+Shift+A**, and navigate holding **Shift+RMB** to **Face Normals** -> **Reverse Normals**<br><br><figure> <img src = "/assets/images/02_maya_arch_7.gif"></figure>
8. We want to extrude the sides of our arch. Our model is symmetrical so we can turn on **Symmetry** to carry out the same operations on both sides of our model.<br><br>Select your model and make sure the move tool is active.<br><br> Holding **Shift+Ctrl+RMB** to open up the setting for our move tool.<br><br>Navigate to **Symmetry**<br><br>Make sure the following are checked on. 
>World (the space of our symmetry)
>
>X Axis (the Axis on which we want symmetry to happen)
>
>Symmetry (activates our Symmetry tool)
>
> <figure> <img src = "/assets/images/02_maya_arch_8.gif"></figure>
> `UI TIP`: At the top of your View Panel, you can see if symmetry is active.
><figure> <img src = "/assets/images/02_maya_arch_1.png"></figure>

1. Extrude the side edges of our arch along the X Axis.<br><br><figure> <img src = "/assets/images/02_maya_arch_9.gif"></figure>
2. Scale the sides along the X Axis to make the level <br><br><figure> <img src = "/assets/images/02_maya_arch_10.gif"></figure>
3. Select the top edges on one of our newly extruded sides.<br><br>Extrude along the Y Axis and snap them to the top vertices of our model.<br><br><figure> <img src = "/assets/images/02_maya_arch_11.gif"></figure>
4. Select all the vertices of our model using **Ctrl+Shift+A**<br><br>Use the **Merge Vertices** tool to merge them together.<br><br><figure> <img src = "/assets/images/02_maya_arch_12.gif"></figure>
5. Using the **Bridge** tool, bridge the sides of our arch together.<br><br><figure> <img src = "/assets/images/02_maya_arch_13.gif"></figure>
6. Double click an edge part of the top edge loop.<br><br>Deselect the two edges on the side.<br><br>Using the **Bridge** tool, bridge the top of our arch together.<br><br><figure> <img src = "/assets/images/02_maya_arch_14.gif"></figure>
7. Select the edge loop on the bottom of our arch.<br><br>Extrude along the Y Axis.<br><br><figure> <img src = "/assets/images/02_maya_arch_15.gif"></figure>
8. Bridge the bottom of our arch. <br><br> <figure> <img src = "/assets/images/02_maya_arch_16.gif"></figure>
9. Snap the Pivot point of our model to the bottom-most vertices.<br><br>Place on model on the origin point of our world.<br><br><figure> <img src = "/assets/images/02_maya_arch_17.gif"></figure>
10. Duplicate our arch by dragging the move tool on the Z Axis while holding **Shift**<br><br>Move the pivot point of this new model to be on the front left bottom corner (see gif below)<br><br><figure> <img src = "/assets/images/02_maya_arch_18.gif"></figure>
11. Rotate the new arch by 90 degrees along the Y Axis.<br><br>Snap it to the bottom corner of our original arch.<br><br><figure> <img src = "/assets/images/02_maya_arch_19.gif"></figure>
12. Duplicate the new arch and snap it to our original arch.<br><br><figure> <img src = "/assets/images/02_maya_arch_20.gif"></figure>
13. Using the **Combine** tool, combine our arches together.<br><br><figure> <img src = "/assets/images/02_maya_arch_21.gif"></figure>
14. With Symmetry still on, delete the interior faces of the corner of our archway.<br><br><figure> <img src = "/assets/images/02_maya_arch_22.gif"></figure>
15. Select and Merge all vertices. <br><br><figure> <img src = "/assets/images/02_maya_arch_23.gif"></figure>
16. Extrude the sides of our arch and snap them to the front vertices along the Z Axis.<br><br><figure> <img src = "/assets/images/02_maya_arch_24.gif"></figure>
17. Bridge the front of our model. <br><br> <figure> <img src = "/assets/images/02_maya_arch_25.gif"></figure>
18. Bridge the top and bottom of our model.<br><br><figure> <img src = "/assets/images/02_maya_arch_26.gif"></figure>
19. We are going to use a new tool, the **Mirror** tool, to complete our model.<br><br>start by deleting the unedited half of our archway.<br><br><figure> <img src = "/assets/images/02_maya_arch_27.gif"></figure>
20. Snap our pivot to the back-most vertices of our model.<br><br>Then snap the pivot to the bottom-most vertices.<br><br>Finally, snap the model to the center of our grid.<figure> <img src = "/assets/images/02_maya_arch_28.gif"></figure>
21. Let's prepare our model for the **Mirror** tool by deleting its history.<br><br>Select our model and navigate to **Edit** -> **Delete by Type** -> **History**<br><br><figure> <img src = "/assets/images/02_maya_arch_29.gif"></figure>
22. Select our model in Object mode.<br><br>Holding **Shift+RMB** activate the **Mirror** tool. This tool allows us to reflect and weld our model along a certain axis.<br><br>
Make sure you change the following parameters:
>Axis Position = World (changes the space in which of model reflects).
>
> Axis = Z (changes the Axis over which our model reflects)
>
> Merge Threshold = .01 (minimum distance for our vertices to marge together)
>
><figure> <img src = "/assets/images/02_maya_arch_30.gif"></figure>
1. Finally, let's clean up our model by deleting its history and freezing its transformations.<br><br>
To Delete History - **Edit** -> **Delete by Type** -> **History**.<br><br>To Freeze Transformations - **Modify** -> **Freeze Transformations**<br><br><figure> <img src = "/assets/images/02_maya_arch_31.gif"></figure>