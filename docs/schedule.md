# Schedule
<!--removes sidebar outline-->
<style>
  table {
    border: none !important;
    border-collapse: collapse !important;
    
    
 
  }

  tbody td{
  border: .15em solid !important;
    }
    td:nth-child(1){
        border: none !important;
    }
  tbody{
    
    
  }
  td{
    padding: 1em !important;
  }
  th{
    border: none !important;
  }

  
  tbody tr:nth-child(4n+1),
    tbody tr:nth-child(4n+2) {
  background-color: 
#dee0e3

;
    }
tbody td:first-child {
  border-right: none;
}

#no-class{
    background-color: pink;
}




body{
   
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
|1|TUES<br>8/26| - [Introduction(s)](./0_Introduction.md)| |
||THUR<br>8/28| **- Tutorial:** [Maya interface and object construction](./1_MayaInterface.md)|**Due:**<br>- Sign Up for Maya Student Account<br>- Join the [Class Discord]() and introduce yourself!<br>**Optional:**<br>- If working outside of lab, purchase hard drive for class|
|2|TUES<br>9/2|**- Tutorial:** [Maya Modeling Essentials](./2_ModellingEssentials.md)|**Due:**<br>- Creature Exercise|
||THUR<br>9/4|**- Tutorial:** [Subdivision Modeling](./3_SubdivisionModeling.md)<br>**- Assign:** [Dream Object](./dreamobject.md)|**Due:**<br>- Tree Exercise|
|3|TUES<br>9/9|**- Tutorial:** [Advanced Modeling]|**Due:**<br>- Teapot Handle|
||THUR<br>9/11|- **Studio Time:** Dream Object|**Due:**<br>- [Initial Dream Object Drawings](./dreamobject.md)|
|4|TUES<br>9/16|<span style = "background-color: lightskyblue;">**- Discussion**</span><br> - **Studio Time:** Dream Object|**Due Monday by 5pm:**<br>- Reading Response: [Software Studies]()|
||THUR<br>9/18|**- Tutorial:** [UV Unwrapping]|**Due:**<br>- [Completed Dream Object Model](./dreamobject.md)|
|5|TUES<br>9/23|**- Tutorial:** [Substance Painter]|**Due:**<br>- [Unwrapped Dream Object Model](./dreamobject.md)|
||THUR<br>9/25|**- Tutorial:** [Texturing, Lighting, Rendering, Cameras]|**Due:**<br>- [Textured Dream Object Model](./dreamobject.md)|
|6|TUES<br>9/30|<span style = "background-color: lightskyblue;">**- Discussion**</span><br>**- Studio Time:** Dream Object|**Due Monday by 5pm:**<br> - Reading Response: [Media Archaeology 1]()|
||THUR<br>10/2|<p style="background-color: lightgreen;">CRIT: Dream Object</p>|**Due:**<br>- [Dream Object Project](./dreamobject.md)|
|7|TUES<br>10/7|**- Tutorial:** [ZBrush Essentials]|**Due:**<br> - Watch ZBrush Tutorial|
||THUR<br>10/9|**- Tutorial:** [ZBrush Continued] **- Assign:** Memory Chambre|**Due:**<br> - Exercise|
|8|TUES<br>10/14|<p style="background-color: pink;">No Class: Break </p>|<p style="background-color: pink;">Break </p>|
||THUR<br>10/16|<span style = "background-color: lightskyblue;">**- Discussion**</span><br>**- Studio Time:** Memory Chambre|**Due Monday by 5pm:**<br> - Reading Response: [Media Archaeology 2]()|
|9|TUES<br>10/21|**- Tutorial:** [Retopology]|**Due:**<br> - Familiar Model with Secondary Details|
||THUR<br>10/23|**- Tutorial:** [Projection and Details]|**Due:**<br> - Retopologized Familiar Model|
|10|TUES<br>10/28|**- Tutorial:** [ZBrush and Painter]<br>**- Studio Time:** Memory Chambre|**Due:**<br> - Finalized Familiar Model in ZBrush|
||THUR<br>10/30|**- Tutorial:** [3D Scanning]|**Due:**<br> - Textured and Rendered Familiar Model|
|11|TUES<br>11/4|<span style = "background-color: lightskyblue;">**- Discussion**</span><br>**- Tutorial:** [3D Scanning]|**Due:**<br> - 3D Scanning Exercise <br> **Due Monday by 5pm:**<br>- Reading Response: [Media Archaeology 3]()|
||THUR<br>11/6|**- Tutorial:** [3D Scanning]|**Due:**<br> - 3D Scanning Exercise|
|12|TUES<br>11/11|**- Tutorial:** [Camera Animation]|**Due:**<br> - Block out of Memory Chambre|
||THUR<br>11/13|**- Tutorial:** [Basic Animation]**<br>- Studio Time:** Memory Chambre|**Due:**<br> - Memory Chambre Objects|
|13|TUES<br>11/18|<span style = "background-color: lightskyblue;">**- Discussion**</span><br>**- Studio Time:** Memory Chambre|**Due Monday by 5pm:**<br>- Reading Response: [Cultural Studies]()|
||THUR<br>11/20|**- Studio Time:** Memory Chambre|**Due:**<br> - Continue Progress on Memory Chambre|
|14|TUES<br>11/25|**- Studio Time:** Memory Chambre|**Due:**<br>- Continue Progress on Memory Chambre|
||THUR<br>11/27|<p style="background-color: pink;">No Class: Break</p>|<p style="background-color: pink;">Break </p>|
|15|TUES<br>12/2|<p style="background-color: lightgreen;">CRIT: Memory Chambre</p>|**Due:**<br>- Memory Chambre|








