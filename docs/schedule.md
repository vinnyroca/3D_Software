# Schedule
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

> Please note that is this is a live schedule and is ever evolving as the course (/world) changes. Please check back frequently for due dates of assignments and course proceedings.

> This schedule contains links to all in-class lectures and tutorials as well as links to class assignments.

## Course Plan

|W|Day|Class| Due |
|---|---|---|---|
|1|TUES<br>8/26| **- Introduction(s)**<br>**- Tutorial:** [Maya interface and object construction](./1_MayaInterface.md)|
||THUR<br>8/28|**- Tutorial:** [Maya Modeling Essentials](./2_ModellingEssentials.md)|**Due:**<br>- Creature Exercise<br>- Hard drive for class|
|2|TUES<br>9/2|**- Tutorial:** [Subdivision Modeling](./3_SubivisionModeling)|**Due:**<br>- Tree Exercise|
||THUR<br>9/4|- **Discussion**<br>**- Tutorial:** [Advanced Modeling]|**Due:**<br>|
|3|TUES<br>9/9|- **Studio Time:** Dream Object|**Due:**<br>|
||THUR<br>9/11|**- Discussion** <br> - **Studio Time:** Dream Object|**Due:**<br>|
|4|TUES<br>9/16|**- Tutorial:** [UV Unwrapping]|**Due:**<br>|
||THUR<br>9/18|**- Tutorial:** [Substance Painter]|**Due:**<br>Clock|
|5|TUES<br>9/23|**- Tutorial:** [Texturing, Lighting, Rendering, Cameras]|**Due:**<br>|
||THUR<br>9/25|**- Studio Time:** Dream Object|**Due:**<br>|
|6|TUES<br>9/30|<p style="color: green;">`CRIT: Dream Object`</p>|**Due:**<br>|
||THUR<br>10/2|**- Tutorial:** [ZBrush Essentials]|**Due:**<br>|
|7|TUES<br>10/7|**- Tutorial:** [ZBrush Continued]|**Due:**<br>|
||THUR<br>10/9|**- Discussion** <br>**- Studio Time:** Memory Chambre|**Due:**<br>|
|8|TUES<br>10/14|<p style="color: red;">`No Class: Break` </p>|**Due:**<br>|
||THUR<br>10/16|**- Tutorial:** [Retopology]|**Due:**<br>Interactive Image|
|9|TUES<br>10/21|**- Tutorial:** [Projection and Details]|**Due:**<br>|
||THUR<br>10/23|**- Discussion**<br>**- Tutorial:** [ZBrush and Painter]<br>**- Studio Time:** Memory Chambre|**Due:**|
|10|TUES<br>10/28|**- Tutorial:** [3D Scanning]|**Due:**<br>|
||THUR<br>10/30|**- Tutorial:** [3D Scanning]|**Due:**<br>|
|11|TUES<br>11/4|**- Tutorial:** [3D Scanning]|**Due:**<br>Performance|
||THUR<br>11/6|**- Tutorial:** [Camera Animation]|**Due:**<br>|
|12|TUES<br>11/11|**- Studio Time:** Memory Chambre|**Due:**<br>|
||THUR<br>11/13|**- Discussion**<br>**- Studio Time:** Memory Chambre|**Due:**<br>|
|13|TUES<br>11/18|**- Studio Time:** Memory Chambre|**Due:**<br>|
||THUR<br>11/20|**- Studio Time:** Memory Chambre|**Due:**<br>|
|14|TUES<br>11/25|**- Studio Time:** Memory Chambre|**Due:**<br>|
||THUR<br>11/27|<p style="color: red;">`No Class: Break`</p>|**Due:**<br>|
|15|TUES<br>12/2|**- Studio Time:** Memory Chambre|**Due:**<br>|
||THUR<br>12/4|<p style="color: green;">`CRIT: Memory Chambre`|**Due:**<br>|






