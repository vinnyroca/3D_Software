<!--removes sidebar outline-->
<style>
  table {
    border: none !important;
    border-collapse: collapse !important;
 
  }
 
  
  tbody tr:nth-child(4n+1),
    tbody tr:nth-child(4n+2) {
  background-color: lightgray;
    }
tbody td:first-child {
  border-right: none;
}
}

</style>
<style>
    @media (min-width: 768px) {
        .col-md-9 {
            width: 100% !important;
        }
        
        .d-md-block {
        display: none !important;
        }
        
        #component-content{
            margin-left:0 !important;
        }
    }
</style>

<!--jump to anchor tag adjusted to header height offset-->
<script>
    // Get the header element
    let header = document.querySelector('header');
    
    // Get the height of the header
    document.querySelectorAll('a[href^="#"]')
    .forEach(function (anchor) {
        anchor.addEventListener('click', 
        function (event) {
            event.preventDefault();
    
            // Get the target element that 
            // the anchor link points to
            let target = document.querySelector(
                this.getAttribute('href')
            );
            
            let headerHeight = header.offsetHeight*2;
            
            let targetPosition = target
                .getBoundingClientRect().top - headerHeight;
    
            window.scrollTo({
                top: targetPosition + window.scrollY,
                behavior: 'smooth'
            });
        });
    });
    </script>

# Modeling the Utah Teapot

Begin by turning on the visibility for the "Teapot_images" layer. We will use these images for reference while modeling.

1. Start by creating a cylinder with **8** sides. <br><figure> <img src = "../assets/images/maya_03_teapot_01.gif"><figcaption></figcaption></figure>
1. Delete the top and bottom faces. <br><figure> <img src = "../assets/images/maya_03_teapot_02.gif"><figcaption></figcaption></figure>
1. Exit the perspective view by tapping Space. However over the front view and tap Space to enter the front view.<br><figure> <img src = "../assets/images/maya_03_teapot_03.gif"><figcaption></figcaption></figure>
1. Scale out cylinder to be the size of the base of our teapot.<br><figure> <img src = "../assets/images/maya_03_teapot_04.gif"><figcaption></figcaption></figure>
1. To see things better, let's turn on X-Ray mode which allows use to see through our model.<br><figure> <img src = "../assets/images/maya_03_teapot_05.gif"><figcaption></figcaption></figure>
1. In Smooth Preview mode, let's scale our cylinder to be the height of our base.<br><figure> <img src = "../assets/images/maya_03_teapot_06.gif"><figcaption></figcaption></figure>
1. Double Click our edge loop to select it, and extrude it up to begin forming the teapot. We know we want a hard edge on the base of our model, so lets add in some edge loops. <br><figure> <img src = "../assets/images/maya_03_teapot_07.gif"><figcaption></figcaption></figure>
1. Continue extruding our model up to key points including the base of our spout, the center of our spout, the top of our spot, the bottom of the top handle and the top of the top handle.<br><figure> <img src = "../assets/images/maya_03_teapot_08.gif"><figcaption></figcaption></figure>
1. Scale these edges in smooth preview mode to match the shape of our teapot.<br><figure> <img src = "../assets/images/maya_03_teapot_09.gif"><figcaption></figcaption></figure>
1. Smooth our Model with 1 level of subdivision<br><figure> <img src = "../assets/images/maya_03_teapot_10.gif"><figcaption></figcaption></figure>
1. Delete the extra edge loops at the bottom of the model using **Ctrl+Backspace**. Its good to keep topology tidy as we subdivide. <br><figure> <img src = "../assets/images/maya_03_teapot_11.gif"><figcaption></figcaption></figure>
1. Offset the bottom edge of our model so we can get a hard edge as we begin to close it off. You can use Shift + Scale Tool<br><figure> <img src = "../assets/images/maya_03_teapot_12.gif"><figcaption></figcaption></figure>
1. Select the bottom edge loop, then deselected the two pairs of edge loops along that are along the Z axis. Use the bridge tool with 1 level of divisions. <br><figure> <img src = "../assets/images/maya_03_teapot_13.gif"><figcaption></figcaption></figure>
1. Use the Target Weld tool to seal up the bottom. We can see how it looks using Smooth Preview (3 Key). <br><figure> <img src = "../assets/images/maya_03_teapot_14.gif"><figcaption></figcaption></figure>
1. We might notice our model is a little off. If it is we can minimally scale and move some edges. <br><figure> <img src = "../assets/images/maya_03_teapot_15.gif"><figcaption></figcaption></figure>
1. Select the 8 faces where we will join the spout to the teapot. And use the Offset tool to offset the edge slightly. <br><figure> <img src = "../assets/images/maya_03_teapot_16.gif"><figcaption></figcaption></figure><figure> <img src = "../assets/images/maya_03_teapot_16_a.gif"><figcaption></figcaption></figure>
1. Make a new cylinder for the spout. <br><figure> <img src = "../assets/images/maya_03_teapot_17.gif"><figcaption></figcaption></figure>
1. The faces we selected to attach our spout had 12 edges along the border. Set our cylinder to have 12 side. <br><figure> <img src = "../assets/images/maya_03_teapot_18.gif"><figcaption></figcaption></figure>
1. Move our cylinder to be in front of the attach area on our teapot and delete the top and bottom faces on the cylinder. <br><figure> <img src = "../assets/images/maya_03_teapot_19.gif"><figcaption></figcaption></figure>
1. Navigate to the front view. <br><figure> <img src = "../assets/images/maya_03_teapot_20.gif"><figcaption></figcaption></figure>
1. We might notice we need a little more space to attach our spout to our teapots. If so, we can slide edges on our model to move them.<br><br>Sliding edges will attempt to keep to same topology, same shape, while allowing us to move our edges.<br><br>To slide an edge loop, select the edge loop and press **Ctrl+Shift** while dragging with the **Middle Mouse Button** pressed.<br><figure> <img src = "../assets/images/maya_03_teapot_21.gif"><figcaption></figcaption></figure>
1. We can also go ahead and delete any extra edge loop on our teapot using **Ctrl+Backspace**<br><figure> <img src = "../assets/images/maya_03_teapot_22.gif"><figcaption></figcaption></figure>
1. Let's also Slide an edge loop down using **Ctrl+Shift** while dragging with the **Middle Mouse Button** pressed to move one edge loop to the center of our lower handle and one edge loop closer to the top of our lower handle.<br><figure> <img src = "../assets/images/maya_03_teapot_23.gif"><figcaption></figcaption></figure>
1. Scale and position your cylinder to be the size of the spout opening. <br><figure> <img src = "../assets/images/maya_03_teapot_24.gif"><figcaption></figcaption></figure>
1. Begin extruding our the edge loop of our spout to form the spout shape. Use move, rotate and scale tools while toggling on smooth preview to get the correct shape. The rotation of the edge loops should follow the flow of the spout.<br><figure> <img src = "../assets/images/maya_03_teapot_25.gif"><figcaption></figcaption></figure>
1. Continue extruding out the spout making sure the edge loops follow the flow of the spout. We can use the scale tool on the y-axis of the last edge loop to make sure it is perfectly straight. <br><figure> <img src = "../assets/images/maya_03_teapot_26.gif"><figcaption></figcaption></figure>
1. Lets enter the top view. Its hard to see our spout with the teapot in the way. Before we hide our teapot, let's rename it so we know where to find it later. <br><figure> <img src = "../assets/images/maya_03_teapot_27.gif"><figcaption></figcaption></figure>
1. Click on your teapot and press **Ctrl+H** to hide your teapot<br><figure> <img src = "../assets/images/maya_03_teapot_28.gif"><figcaption></figcaption></figure>
1. We can toggle on Wireframe mode to get a better view of our model by pressing the **4** key. With wireframe on, scale the edge loops on your spout along the x axis to match them to the image. <br><figure> <img src = "../assets/images/maya_03_teapot_29.gif"><figcaption></figcaption></figure>
1. Check the Left view to make sure everything looks lined up. <br><figure> <img src = "../assets/images/maya_03_teapot_30.gif"><figcaption></figcaption></figure>
1. Un-hide your teapot by selecting it from the Outliner and pressing **Shift+H** <br><figure> <img src = "../assets/images/maya_03_teapot_31.gif"><figcaption></figcaption></figure>
1. Let's make our teapot **Live** by selecting on the teapot and selecting the live button. Making a model live will allow the components of other models to snap to its surface.<br><figure> <img src = "../assets/images/maya_03_teapot_32.gif"><figcaption></figcaption></figure>
1. Turn on Symmetry along the World - Z axis.<br><figure> <img src = "../assets/images/maya_03_teapot_33.gif"><figcaption></figcaption></figure>
1. Using the move tool, drag each vertex slightly on the base of the spout to snap them to the surface of the teapot. Only move them along the Z and Y axis. Try to keep them in somewhat of the same relative position.<br><figure> <img src = "../assets/images/maya_03_teapot_34.gif"><figcaption></figcaption></figure>
1. Turn off **Live** on the teapot. <br><figure> <img src = "../assets/images/maya_03_teapot_35.gif"><figcaption></figcaption></figure>
1. Combine the teapot and the spout together. <br><figure> <img src = "../assets/images/maya_03_teapot_36.gif"><figcaption></figcaption></figure>
1. Delete the faces to make room to attach our spout. <br><figure> <img src = "../assets/images/maya_03_teapot_37.gif"><figcaption></figcaption></figure>
1. Use the Target Weld tool in object mode to weld the spout to the teapot. <br><figure> <img src = "../assets/images/maya_03_teapot_38.gif"><figcaption></figcaption></figure>
1. Let's use Ctrl with the Multi Cut tool to add in some edge loops to give the transition between our teapot and spout a hard edge.<br><figure> <img src = "../assets/images/maya_03_teapot_39.gif"><figcaption></figcaption></figure>
1. We can slide our vertices just like our edges by holding **Ctrl+Shift** while dragging with the **Middle Mouse Button** pressed. Drag in the corners to make the topology flow better. Adjust other vertices as needed. <br><figure> <img src = "../assets/images/maya_03_teapot_40.gif"><figcaption></figcaption></figure>
1. Extrude the full model inward. <br><figure> <img src = "../assets/images/maya_03_teapot_41.gif"><figcaption></figcaption></figure>
1. Reverse the normals. <br><figure> <img src = "../assets/images/maya_03_teapot_42.gif"><figcaption></figcaption></figure>
1. Let's clean of the bottom. First using the Shift + Double Click method to select a ring of faces towards the bottom of our model. Delete those faces. Double click on the *Island* of faces we created to select them. Delete those faces.<br><figure> <img src = "../assets/images/maya_03_teapot_43.gif"><figcaption></figcaption></figure>
1. Use the same method we used to bridge the bottom of our teapot to close up our teapot.<br><figure> <img src = "../assets/images/maya_03_teapot_43.gif"><figcaption></figcaption></figure>
1. Snap the inner top edge loop to the top edge loop of the teapot along the Y Axis. Scale the top inner edge loop of the spout along the Y Axis to make it level. Snap it in place. <br><figure> <img src = "../assets/images/maya_03_teapot_45.gif"><figcaption></figcaption></figure>
