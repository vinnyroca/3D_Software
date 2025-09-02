
## Description

When learning to model more complex objects, its a good practice to try to recreate models made by other 3D artists. For this exercise, we'll be modeling the back part of this polaroid camera:

<div class="sketchfab-embed-wrapper"> <iframe title="Polaroid Spirit 600" frameborder="0" allowfullscreen mozallowfullscreen="true" webkitallowfullscreen="true" allow="autoplay; fullscreen; xr-spatial-tracking" xr-spatial-tracking execution-while-out-of-viewport execution-while-not-rendered web-share width="400" height="400" src="https://sketchfab.com/models/6557b2d4da1e4ad082528035adf24db2/embed"> </iframe> <p style="font-size: 13px; font-weight: normal; margin: 5px; color: #4A4A4A;"> <a href="https://sketchfab.com/3d-models/polaroid-spirit-600-6557b2d4da1e4ad082528035adf24db2?utm_medium=embed&utm_campaign=share-popup&utm_content=6557b2d4da1e4ad082528035adf24db2" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;"> Polaroid Spirit 600 </a> by <a href="https://sketchfab.com/ZachWilkins1997?utm_medium=embed&utm_campaign=share-popup&utm_content=6557b2d4da1e4ad082528035adf24db2" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;"> ZachWilkins1997 </a> on <a href="https://sketchfab.com?utm_medium=embed&utm_campaign=share-popup&utm_content=6557b2d4da1e4ad082528035adf24db2" target="_blank" rel="nofollow" style="font-weight: bold; color: #1CAAD9;">Sketchfab</a></p></div>

<a title="Malopez 21, CC BY-SA 4.0 &lt;https://creativecommons.org/licenses/by-sa/4.0&gt;, via Wikimedia Commons" href="https://commons.wikimedia.org/wiki/File:Polaroid,_Spirit_600.jpg"><img width="512" alt="Polaroid, Spirit 600" src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ea/Polaroid%2C_Spirit_600.jpg/512px-Polaroid%2C_Spirit_600.jpg?20160612223034"></a>

Original Polaroid, Spirit 600 (wikimedia.org)

---

## Tutorial


1. Create a plane > Subdivisions Width = 1 > Subdivisions Height = 1 ![Polaroid Gif](/assets/images/4/04_pBool_01.gif)<br><br><br>
2. Scale plane to be width of back pack of Polaroid ![Polaroid Gif](/assets/images/4/04_pBool_02.gif)<br><br><br>
3. Move vertices of plane to be aligned with back part of Polaroid ![Polaroid Gif](/assets/images/4/04_pBool_03.gif)<br><br><br>
4. Rename plane to “Polaroid Back” > Duplicate plane with Ctrl + D > Rename new plane “Polaroid View Finder” > use Ctrl+H to hide the view finder ![Polaroid Gif](/assets/images/4/04_pBool_04.gif)<br><br><br>
5. Extrude the plane > snap and scale to match the reference ![Polaroid Gif](/assets/images/4/04_pBool_05.gif)<br><br><br>
6. Use Shift+H with View Finder selected to un-hide it ![Polaroid Gif](/assets/images/4/04_pBool_06.gif)<br><br><br>
7. Use the Multi-cut tool to cut bottom edge of view finder > Snap the right edge of view finder to the top of the polaroid back ![Polaroid Gif](/assets/images/4/04_pBool_07.gif)<br><br><br>
8. Delete all faces except for top left corner ![Polaroid Gif](/assets/images/4/04_pBool_08.gif)<br><br><br>
9. Extrude View Finder to match reference ![Polaroid Gif](/assets/images/4/04_pBool_09.gif)<br><br><br>
10. Boolean Union the Polaroid Back and the View Finder ![Polaroid Gif](/assets/images/4/04_pBool_10.gif)<br><br><br>
11. Delete History ![Polaroid Gif](/assets/images/4/04_pBool_11.gif)<br><br><br>
12. Use the Target Weld tool to clean up Topology ![Polaroid Gif](/assets/images/4/04_pBool_12.gif)<br><br><br>
13. Merge all vertices together to prevent any duplicated vertices ![Polaroid Gif](/assets/images/4/04_pBool_13.gif)<br><br><br>
14. Since we won’t see the back or bottom, delete those faces to make the clean up easier ![Polaroid Gif](/assets/images/4/04_pBool_14.gif)<br><br><br>
15. Using the Multi-cut tool to create quadded topology ![Polaroid Gif](/assets/images/4/04_pBool_15.gif)<br><br><br>
16. Extrude out the Viewfinder ![Polaroid Gif](/assets/images/4/04_pBool_16.gif)<br><br><br>