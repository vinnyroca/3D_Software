# Modeling a Die with Subdivision

## Dice Model on Sketchfab 

In this exercise, we'll be making a Die, similar to this one on **Sketchfab**.

**Sketchfab** is a great resource for sourcing free 3D models, as well as for examining the topology created by other artists.

Press play to start the model and use **Click+Drag** to rotate the model.

<div class="sketchfab-embed-wrapper"> <iframe title="Dice d6 low-poly PBR" frameborder="0"  height = "400px" width = "400px" src="https://sketchfab.com/models/7c7c839a76c44f36be942b1c87b040d7/embed"> </iframe> <p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4A4A4A;"> <a href="https://sketchfab.com/3d-models/dice-d6-low-poly-pbr-7c7c839a76c44f36be942b1c87b040d7?utm_medium=embed&utm_campaign=share-popup&utm_content=7c7c839a76c44f36be942b1c87b040d7" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;"> Dice d6 low-poly PBR </a> by <a href="https://sketchfab.com/ArmorAndRum?utm_medium=embed&utm_campaign=share-popup&utm_content=7c7c839a76c44f36be942b1c87b040d7" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;"> Armor and Rum </a> on <a href="https://sketchfab.com?utm_medium=embed&utm_campaign=share-popup&utm_content=7c7c839a76c44f36be942b1c87b040d7" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a></p></div>

## Part 1:

First, we'll add edge loops all around our model so it smooths to a cube shape.

An easy way to add edges around all parts of our existing edge loops is to use the **Bevel tool.**

The bevel tool will *bevel* our model, or, in other words, soften the edges of our model.

1. Begin by selecting all the edges of our die. <figure> <img src = "/assets/images/maya_03_dice_01.gif"><figcaption></figcaption></figure>

2. Use **Shift+RMB** to navigate to **Bevel**. Set fraction to .01 and our segments to 2.<figure> <img src = "/assets/images/maya_03_dice_02.gif"><figcaption></figcaption></figure>

3. Let's add in edge loops for the number indicators for our die. Use the insert edge loop tool to add two additional edge loops on all sides of our die. Make sure to click on the setting box to change the number of edge loops we are inserting.<figure> <img src = "/assets/images/maya_03_dice_03.gif"><figcaption></figcaption></figure>

4. Next, let's start by making the 1-Side and 6-Side of our die by selecting the appropriate faces. The 1-Side and 6-Side are opposite each other.<figure> <img src = "/assets/images/maya_03_dice_04.gif"><figcaption></figcaption></figure>

5. We want the indentation for our die to have a hard edge. Let's add one edge loop inside our selected faces by using the offset tool in our extrude settings.Make sure **Keep Faces Together** is set to off.<br><br>`UI TIP:` Hold **Ctrl+Shift** while dragging on a parameter in a dialog box to make it change values slower.<br><figure> <img src = "/assets/images/maya_03_dice_05.gif"><figcaption></figcaption></figure>

6. Next, let's extrude in slightly to fully fence in our inset area. This will give us a hard edge around our inset area.<br><figure> <img src = "/assets/images/maya_03_dice_06.gif"><figcaption></figcaption></figure>

7. Extrude again to make the full inset.<br><figure> <img src = "/assets/images/maya_03_dice_07.gif"><figcaption></figcaption></figure>

8. We'll be using this model in another exercise. Let's duplicate it so we have a clean copy before smoothing.<br><figure> <img src = "/assets/images/maya_03_dice_08.gif"><figcaption></figcaption></figure>

9. Finally, let's give our model 2 levels of subdivision and see how it looks!<br><figure> <img src = "/assets/images/maya_03_dice_09.gif"><figcaption></figcaption></figure>

## Part 2:

Use the die model from **Sketchfab** to see which sides of the die are next to and opposite each other.

Use the steps above to make a complete die with two levels of subdivision.



