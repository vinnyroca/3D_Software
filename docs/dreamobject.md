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

# Dream Object

## Project Description

For our Dream Object assignment, you will be creating a digital collection of text and images that tells the story of/describes/complicates a dream object. A dream object can be anything. It could quite literally be an object from your dreams, a normal object turned strange and disturbing, or it might be an object of your own lucid invention. Perhaps, it is a device that only you can operate. Perhaps, it is a familiar object distorted through memories. Perhaps, it is an object you are trying to remember. Perhaps, it lives in a mountain far away, as large as a redwood tree, silently recording the patterns of constellations.

If a dream object is anything, however, it is not a normal object. It is not a basketball, or a cup, or a shoe, or a house, or a boat, or a gun. If it were a real thing, it has changed. It has become something else; or, it was never recognizable at all.

To decide on your dream object, think of its context. We will be taking inspiration from Victor Burgin's [*Afterlife*](https://afterlife.victorburgin.eu/). What do we notice about *Afterlife*? It consists of "pages." It consists of text. It consists of images. Some rendered, some not rendered. But, what is most important is that the text *contextualizes* the images, and the images *contextualize* the text. Separate, they point to two different directions. Together, they create a context. It should be noted, Victor Burgin is a serious guy, very serious. We look to him for form and structure, but his tone is not a requirement. 

Your final assignment will have text and it will have images. Some of those images will be rendered. Others, if you would like others, might be photographs, scans, or any other set of pixels. Using whatever text and image editing software you like, be it Photoshop, InDesign, PowerPoint, or others, you will create a PDF of any dimensions. In this PDF, some pages will be empty. In this PDF, some pages will have images. Some pages will have text. No page will have both. At least 5 of these pages will have renders of your dream object. In other words, you will need to produce 5 renders of your dream object for this assignment. Each of these renders will be different, and describe something different about your dream object. If you wish to create additional renders of places or other objects, do not stop yourself. At least 4 of these pages should have text. As for the text, it might describe a story, tell a lie, give us commands, state a prayer, describe a dance, or anything in between. But, importantly, the text and images together will form a context. At least two of the pages should be blank. Use these blank pages thoughtfully. Some housekeeping: there should be a title page. (You may refuse this last requirement if you like.)

Some options on how to begin:

- Dream, see and record what emerges.
- Don't dream, see and record what emerges.
- Daydream, see and record what emerges.
- Write some words, see what images emerge.
- Think of some images, see what words emerge.
- Think of yourself standing there, holding this thing in your hand, or, perhaps it is a thing in front you, larger than the horizon, or, perhaps it is as small as a pea, right under your foot. Oh no, it's attacking someone. Oh wait, it's not moving at all. Oh look, it is trying to tell you something. Oh wait, it cannot speak. This thing is your dream object.

Another context: This class. We have just learned the fundamentals of hard surface modeling. Creatively, this gives us limitations. There are many things we do not know how to do, yet there are many things we already know how to make. Start there, start with what we have learned and what we know. What can you make? How can you make that more complex, interesting, inspiring, disturbing, compelling? With this in mind, like all things, this assignment will be made one step at a time, piece by piece.

Periodically, we will share these pieces (more information on that below).

**However, there is one rule. And, under no circumstances should this rule be broken:**

**Up until our critique day, in which we will all gather and share what we have been working on, your text, and thus your context, will be a secret. We might see your dream object, examine its textures, but we will not know its world, its story, its ambitions, or its dreams. Up until our crit, it is a dream of your own to ponder, build, and imagine.**

## Pieces

This project will be broken up into a series of project pieces that all have their own due date.
Each project piece is worth a certain percentage of you final grade.

Points:

|Points|Piece|
|---|---|
|5|Initial Drawings|
|5|Object Model|
|5|Unwrapped Object|
|5|Textured Object|
|80|Final Project|

Late project pieces will no be accepted as completing them is fundamental to completing the entire project.

## Initial Drawings (9/11)

5 points

An initial drawings of the assignment in due on September 4th at the start of class. These initial drawings should be shared in the class discord before the start of class.

**These drawings are not quick sketches, or quick jottings of ideas. These drawings should be the final result of many rounds of thinking and sketching.**

These drawings should depict you device from many different angles. They should, at minimum, show your object from a perspective, side and front view. We are sketching in preparation for modeling. You should be as precise as possible even though our ideas will develop. In your drawings, sketch the topology of your model: follow the edge loops, think of which part of your object will be separate meshes, consider the primitive geometry you will begin with. 

Additionally, the drawings should describe the materials you imagine for your object.

Lastly, the should begin to think of the environment, although minimal, the object will be rendered in. Our renders will be be mostly of our object, however, the space around our object should provide additional context.


## Completed Object Model (9/18)

5 Points

You will have two in-class studio sessions to get help with modeling your object.

This completed model will have clean topology including even edge loops and quad topology.

A screenshot of your completed model should be posted to Discord before the class it is due.

## Unwrapped Object (9/23)

5 points

You will have one in-class short studio session to work with the instructor to UV Unwrap your model.

A screenshot of your UV Editor should be posted to Discord before the class it is due.

## Textured Object (9/25)

5 points

A screenshot of your painted model in Substance Painter should be posted to Discord before the class it is due.

## Final Project (10/2)

80 points

Following a brief Discussion, you will have one in-class of studio time to work on your final project.

The following are to be uploaded before class:
[Upload Link]()

Within a zipped folder include:

1. Your final PDF
2. Separate images of each of your renders
3. Images of any additional renders you created for the project

How to Zip a file:

[Windows](https://support.microsoft.com/en-us/windows/zip-and-unzip-files-8d28fa72-f2f9-712f-67df-f80cf89fd4e5)

[MacOS](https://support.apple.com/guide/mac-help/zip-and-unzip-files-and-folders-on-mac-mchlp2528/mac)

## Some Dreams of Others

- [Laurie Anderson *Heart of a Dog*](https://www.youtube.com/watch?v=8PLWVXICQyM)
- [Jim Shaw *Dream Drawings*](https://www.moma.org/collection/works/82235)
- [Apichatpong Weerasethakul *BLUE*](https://www.youtube.com/watch?v=8Hk4zepxyoE)
- [Leonora Carrington's Paintings and Drawings](https://www.moma.org/collection/works/32006?artist_id=993&page=1&sov_referrer=artist)
- [Louise Bourgeois *Tits*](https://www.tate.org.uk/art/artworks/bourgeois-tits-al00227)
- [Lu Yang](http://luyang.asia/)
- [Sharif Farrag](https://shariffarrag.com/)
