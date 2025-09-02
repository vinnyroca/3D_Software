# Advanced Modeling

**Recap:**

- What is subdivision modeling and how do we use it to make more complex models?
- How to use Edge Loops to change the shape of subdivided models
- Using subdivision to make a die.
- History of the Utah Teapot
- Using subdivision to model the Utah Teapot

**Plan:**

- The 3D Process Large Scale, Indie and Individual
- Boolean Modeling
- Topology Reduction
- Flow of Topology
- Importing Images
- Modeling complex models from Images

## The 3D Process - Disney/Pixar (Luca)

### Concept and Story Artist

![luca story board](/assets/images/4/04_luca_00.gif)

![Luca sketch](/assets/images/4/04_luca_01.jpg)

---

### Modeling Artist

![Luca rotating model](/assets/images/4/04_luca_02.gif)

---

### Technical Artist - Rigging
![Luca rigging](/assets/images/4/04_luca_03.gif)

---

### Technical Artist - Surfaces
![Luca surfaces](/assets/images/4/04_luca_04.png)
![Luca textures](/assets/images/4/04_luca_05.png)

---

### Camera Artist

![Luca camera placement](/assets/images/4/04_luca_06.gif)

---

### Animator
![Luca animation](/assets/images/4/04_luca_07.gif)

---

### Lighting Artist

![Luca lighting](/assets/images/4/04_luca_08.gif)

---

### Technical Artist - Rendering

![Luca lighting](/assets/images/4/04_luca_09.gif)

---

- **Pro**: Larger productions
- **Con**: Little individual say, long-working conditions

---

### Further Reading/Watching

- [The Science Behind Pixar, Museum of Science, Boston](https://sciencebehindpixar.org/)
- [The Making of Toy Story Documentary](https://www.youtube.com/watch?v=6W_HL3nULMM)
- [Into the Unknown: Making Frozen 2](https://www.youtube.com/watch?v=2vQPPEka0ls) 

## The 3D Process - Super Giant Games (Hades)

<iframe width="560" height="315" src="https://www.youtube.com/embed/Bz8l935Bv0Y?si=vLmoMGfEsQfoPJ_y" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

---

### Concept Artist

![Nyx Concept](/assets/images/4/04_Nyx_01.png)

---

### 3D Generalist

Sculpting

![Nyx ](/assets/images/4/04_Nyx_02.png)

Modeling - Retopology
![Nyx ](/assets/images/4/04_Nyx_03.png)

Texturing
![Nyx ](/assets/images/4/04_Nyx_04.png)

Rigging
![Nyx ](/assets/images/4/04_Nyx_05.png)

---
### Animator

![Nyx ](/assets/images/4/04_Nyx_06.gif)

---

**Pro**: Ability to specialize, exciting projects, individual say
**Con**: Jobs can be unstable, freelance

---

### Further Reading/Watching

- [Inside Hades - 3D Modeling and Rigging](https://www.youtube.com/watch?v=cYJ6d1ifSqA)
- [Double Fine PsychOdyssey: The Making of Psychonauts 2](https://www.doublefine.com/dftv/psychodyssey)

## The 3D Process - Individual (Real Things, Everywhere)

1. Concept ![Lie ](/assets/images/4/04_lie_01.png)
2. Initial Sculpting ![Lie ](/assets/images/4/04_lie_02.png)
3. Refined Sculpting ![Lie ](/assets/images/4/04_lie_03.png)
4. Retopology (Not Pictured)
5. Textures ![Lie ](/assets/images/4/04_lie_04.png)
6. Rigging ![Lie ](/assets/images/4/04_lie_05.png)
7. Animations ![Lie ](/assets/images/4/04_lie_06.gif)
8. [Final Game](https://lie.vinnyroca.info/)


## Polysphere

Oftentimes, working with the default sphere model within Maya can present many challenges. Since the sphere model does not have even and quadded topology, it can present many issues when creating more complex models.

Most artists when working with spherical shapes use a poly sphere.
A polysphere is a sphere made up of quadded geometry that has evenly spaced vertices.

---

To make a poly sphere:

1. Create a sphere primitive ![pShpere](/assets/images/4/04_polysphere_01.gif)
2. Create a cube > Smooth 2 Levels > Scale to be size of sphere ![pShpere](/assets/images/4/04_polysphere_02.gif)
3. Click on sphere > Press Make Live (Magnet Button)![pShpere](/assets/images/4/04_polysphere_03.gif)
4. Click on Smooth Cube > Mesh > Conform![pShpere](/assets/images/4/04_polysphere_04.gif)
5. Click Make Live > Delete original sphere![pShpere](/assets/images/4/04_polysphere_05.gif)


## Booleans

We can combine meshes together using boolean operations. When using boolean operations, the same rules of quadded topology still apply. We can combine objects together using booleans, however, we must clean up our geometry after the operation is completed.

To make sure your boolean operations can produce clean topology, you should make sure that meshes you are combining together can have their edge loops connected. This often means combining geometry that has the same number of edge loops.

---

### Boolean Subtract

Steps to make cut in using Booleans:

1. Place one model inside the other model. Ensure that their edges can be connected after the boolean operation is complete. ![pShpere](/assets/images/4/04_bSubtract_01.gif)
2. Select the base model > Shift Select the model you want to subtract ![pShpere](/assets/images/4/04_bSubtract_02.gif)
3. Mesh > Boolean > Difference (A-B)  ![pShpere](/assets/images/4/04_bSubtract_03.gif)
4. To complete the operation navigate to Edit > Delete By Type > History  ![pShpere](/assets/images/4/04_bSubtract_04.gif)
5. Clean up disconnected and loose vertices using the Target Weld tool.  ![pShpere](/assets/images/4/04_bSubtract_05.gif)
6. Clean up nGons using the Multi-cut tool  ![pShpere](/assets/images/4/04_bSubtract_06.gif)

`UI TIP:` Press Right-Click after a cut to stop the cutting operation

---

Steps to combine objects together using Booleans:

1. Place one model inside the other model. Ensure that their edges can be connected after the boolean operation is complete. ![pShpere](/assets/images/4/04_bUnion_01.gif)
2. Select both models > Mesh > Boolean > Union ![pShpere](/assets/images/4/04_bUnion_02.gif)
3. To complete the operation navigate to Edit > Delete By Type > History ![pShpere](/assets/images/4/04_bUnion_03.gif)
4. Clean up disconnected and loose vertices using the Target Weld tool. ![pShpere](/assets/images/4/04_bUnion_04.gif)
4. Clean up nGons using the Multi-cut tool. ![pShpere](/assets/images/4/04_bUnion_05.gif)


## Topology Reduction

When modeling, there are many cases in which we want to reduce the areas of high density topology to low density. Oftentimes, we might have one area of our model that has a lot of detail, while we have other areas that have low detail. We can use topology reduction techniques to go from areas of high poly count to low poly count.

### Examples:

---

### **3 to 1 Reduction:**
![pShpere](/assets/images/4/04_reduction_01.gif)

---

### **5 to 3 to 1 Reduction:**
![pShpere](/assets/images/4/04_reduction_02.gif)

---


### **2 to 1 Reduction:**
![pShpere](/assets/images/4/04_reduction_03.gif)

---

### **Machine Example:**
![pShpere](/assets/images/4/04_reduction_04.gif)


## Topology Flow

When modeling, we often need to adjust the flow of our topology. For example, in the below model, if I want to add in edge loops to give the top part of my object a hard edge, I change the topology of the attached cylinders. After smoothing, this causes the cylinders to have a deformed shape.

Looking at this model, I realize I need to change the flow of my topology to go around the extruded cube. Currently, the topology follows down the sides of the model.

Simplified Example:

![pShpere](/assets/images/4/04_flow_00.png)

The first object is the topology I want, the second model is the topology I have currently.

---

### Steps to changing the flow of topology in the example:

1. Select and Delete the faces where the two sections meet ![pShpere](/assets/images/4/04_flow_01.gif)
2. Add in extra edge loops to match the edge count for both sections  ![pShpere](/assets/images/4/04_flow_02.gif)
3. Bridge the sections together  ![pShpere](/assets/images/4/04_flow_03.gif)
4. Add the extra edge loops to harden the bottom edges  ![pShpere](/assets/images/4/04_flow_04.gif)


## Free Image Plane

We can use Free Image Planes to bring reference images into our Maya scene. As a note, it is important to store all of your reference images in the Source Images folder within your Maya project.

---

To bring in an image on a Free Image Plane:

1. Create > Free Image Plane ![pShpere](/assets/images/4/04_image_01.gif)
2. Select Image Plane > Attribute Editor > Image Plane Shape > File Icon > Choose Image ![pShpere](/assets/images/4/04_image_02.gif)

---

To lock an Image Plane to a particular view:

1. Move the Image Plane back on the Axis you want to view it in. For example, if I want to view my image through my Front Camera, i’ll move it back on my Z Axis.![pShpere](/assets/images/4/04_image_03.gif)

2. Select Image Plane > Attribute Editor > Display - looking through camera > Select Camera. Note: You might need to be in that view for the camera to show up on the list.
Making Image Planes Reference Objects ![pShpere](/assets/images/4/04_image_04.gif)

---

It is very easy to accidentally click on reference images. To prevent this, it is best to put your reference images on a separate layer, and make it a reference layer.

Steps:

1. Select all of your reference images
2. Click the create and add to layer button > Rename Layer![pShpere](/assets/images/4/04_image_06.gif)
3. Set the Layer to Reference ![pShpere](/assets/images/4/04_image_07.gif)
