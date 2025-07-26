# Schedule
<!--removes sidebar outline-->
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

> This scedule contains links to all in-class lectures and tutorials as well as links to class assignments.

#### Typical weekly plan

| Tuesday | Thursday |
| --- | --- |
| Discussion - 50 min <br> Software Tutorial - 1 H 30 M| Lecture - 20 M<br>Software Tutorial - 2 H

## Course Plan

|Session/Module |In-Class | Reading/Watching/Assignment Due |
|---|---|---|
|1|<mark>Introduction</mark>||
|**Tuesday** 8/26|[Introduction(s)](./0_Introduction.md)<br><br>**Tutorial:** [Maya interface and object construction](./1_MayaInterface.md)||
|2|<mark>Modeling Software</mark>||
|**Thursday** 8/28|Review of Assignment<br><br>**Tutorial:** Object modeling with Maya|**Assignment Due:**<br>- Assignment One<br>- Hardrive for class|
|**Tuesday** 9/2|||






