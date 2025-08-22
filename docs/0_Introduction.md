

<style>
/* Button styling */
#focusToggle {
  position: fixed;
  bottom: 20px;
  right: 20px;
  z-index: 1000;
  padding: 0.2em .5em;
  background: #333;
  color: #fff;
  border: none;
  border-radius: 6px;
  cursor: pointer;
  opacity: .5;
}

/* Hide button on small screens */
@media (max-width: 767.9px) {
  #focusToggle {
    display: none;
  }
}

/* Focus mode styles */
.focus-mode .section-content,
.focus-mode h2 {
  display: none; /* hide all by default in focus mode */
}

.focus-mode .section-content.active,
.focus-mode h2.active {
  display: block; /* show only active section */
}
</style>

<button id="focusToggle">Focus</button>

<script>
document.addEventListener("DOMContentLoaded", () => {
  const button = document.getElementById("focusToggle");
  let focusEnabled = false;

  // Wrap content after each h2
  const headings = document.querySelectorAll("h2");
  headings.forEach(h2 => {
    const wrapper = document.createElement("div");
    wrapper.classList.add("section-content");

    let sibling = h2.nextElementSibling;
    while (sibling && sibling.tagName !== "H2") {
      const next = sibling.nextElementSibling;
      wrapper.appendChild(sibling);
      sibling = next;
    }
    h2.insertAdjacentElement("afterend", wrapper);
  });

  const sections = document.querySelectorAll(".section-content");

  function showSectionById(id) {
    sections.forEach(wrapper => {
      const h2 = wrapper.previousElementSibling;
      if (h2.id === id) {
        wrapper.classList.add("active");
        h2.classList.add("active");
      } else {
        wrapper.classList.remove("active");
        h2.classList.remove("active");
      }
    });
  }

  // Default section
  if (location.hash) {
    showSectionById(location.hash.substring(1));
  } else if (headings.length) {
    showSectionById(headings[0].id);
  }

  window.addEventListener("hashchange", () => {
    showSectionById(location.hash.substring(1));
  });

  // Toggle focus mode
  function toggleFocusMode(enable) {
    focusEnabled = enable;
    document.body.classList.toggle("focus-mode", focusEnabled);
    button.textContent = focusEnabled ? "Exit Focus" : "Focus";
  }

  button.addEventListener("click", () => {
    toggleFocusMode(!focusEnabled);
  });

  // Disable focus mode on small screens
  function checkScreenWidth() {
    if (window.innerWidth <= 767.9) {
      toggleFocusMode(false); // automatically turn off
      button.style.display = "none"; // hide button
    } else {
      button.style.display = "block"; // show button
    }
  }

  window.addEventListener("resize", checkScreenWidth);
  checkScreenWidth(); // initial check
});
</script>


# HELLO!

## Plan For Today

2 Hours 30 min


- Introductions - 30 min
- About Me - 5 min
- Syllabus Review - 20 min
- Schedule and Class Website - 10 min
- Class Discord - 5 min
- Break - 10 min
- Course Goals - 20 min
- 3D Exercise - 50 min



## Introductions

- Name
- Pronouns
- Home college/Major/Year
- Any experience you have had with 3D software
- Why were you interested in signing up for this course and what is one thing you are looking to take away from this class?
- Favorite 3D Object: animation, video game, visual effects, render, infographic, etc.

## About Me


- Vincent Roca, Assistant Professor of Media Studies (you can call me Vinny)
- He/Him
- Media Art/Games/Animation/Sculpture

## Syllabus

[Class Syllabus](./index.md)

## Class Website and Schedule

Class Website: 3DSoftware.vinnyroca.info

If you see an error or typo, please send me an email or Discord message.

[Schedule](./schedule.md)


## Class Discord

[Join the Class Discord](https://discord.gg/DV4HeM27)

Please change your nickname on the server to match your name in the classroom.

[How to change your server nickname](https://support.discord.com/hc/en-us/articles/219070107-Server-Nicknames)


## Course Goals

To learn the fundamentals of the practice, theory, and history of 3D Software.

## Practice

Autodesk Maya - Hard-surface 3D models, Animation, and Simulation

- Maya Interface
- Basic modeling
- Subdivision modeling
- Texturing with Substance Painter
- Rendering
- Camera Animation

Maxon Zbrush - Organic 3D Models

- Modeling organic objects
- Creating high-detail models

Revpoint MIRACO - 3D Scanning

- Creating and cleaning up 3D Scans of real-world objects

## Projects & Exercises 

- Dream Object - A digital artist book of text and renders

- Memory Chambre - An animation of a memory palace, filled with 3D models and Scans

+ A variety of exercises to get us comfortable navigating the 3D tools

## Theory & History

**We live in a society of computation.**

What does this mean?

It means that all parts of our life, from our cars, homes, classrooms, social life, and leisure are dominated by the culture of computation, AKA computers and computer programming.


How we interface with these computational devices is often through computer graphics with a graphical user interface. Think of the interface of your iPhone, consider the levels of computation that this elaborately designed interface hides away.

In the early history of computing, people didn’t interact with software. Engineers, programmers, and artists interacted with computers through physical punch cards or other physical inputs and outputs.

This course asks, how did the invention of computer graphics and particularly 3D computer graphics, change our relationship to computation as well as how we understand objects and motion in our world.

We'll approach this question through 3 different academic fields:

- Software Studies
- Media Archeology
- Cultural Studies

<p><a href="https://commons.wikimedia.org/wiki/File:Two_women_operating_ENIAC_(full_resolution).jpg#/media/File:Two_women_operating_ENIAC_(full_resolution).jpg"><img src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Two_women_operating_ENIAC_%28full_resolution%29.jpg" alt="Two women programming ENIAC."  width="800"></a><br>By Unidentified U.S. Army photographer - Image from <a rel="nofollow" class="external text" href="https://ftp.arl.army.mil/ftp/historic-computers/">Historic Computer Images</a>, Public Domain, <a href="https://commons.wikimedia.org/w/index.php?curid=26253297">Link</a></p>

## Software Studies

Software and computer graphics mediate our experience with the computer. In other words, they provide an interface that translates the work being done by the computer and the work being done by the artist, designer, engineer, or even the consumer.

The field of software studies looks to understand the impact of software.

In this class, we’ll be studying 3D computer graphics software, looking to understand its cultural, political, and economic effects.

Where we’ll start:

- *Getting to Know Software: A Study of Autodesk Maya* - Aylish Wood (2015)
- *RGBFAQ* - Alan Warburton

## Media Archaeology

Media Archaeology as field explores the history of media and looks to understand the impact of this history on our present. In particular, media archaeology looks to counter the main narrative that technology moves in a linear fashion by some invisible force of *progress*.

- *What is Media Archaeology* - Jussi Parikka (2012)
- *Image Objects: An Archaeology of Computer Graphics* - Jacob Gaboury (2021)

Image Objects will guide us through the history of computer graphics that leads to the software we will be using in class: Maya and ZBrush. Focusing particularly on the early research in computer graphics at the University of Utah, Image Objects will demonstrate how many of the objects we use today, from our phones to our books, can trace their origins back to the beginnings of computer graphics.

## Cultural Studies

Cultural studies work in media studies asks how contemporary and historic media shape culture and are shaped by culture.

- *Where the Model Ends* - Alenda Chang (2024)
- *3D Media In The Transversal Era* - DB Bauer (2024)
- *Open Source Afro Hair Library* - AM Darke (Ongoing)

## A Note on Overlap

Although the readings for this class are separated into these different sections, many of they pull from all these fields and more to draw their conclusions.

Media studies is an overlapping field the pulls not only from the above mentioned fields, but also:

- Science and Technology Studies
- Game Studies
- Critical Code Studies
- Gender and Feminist Studies
- Critical Race Studies
- Environmental Studies
- Post-colonial Studies

## Responses and Discussion

**All readings/watching will have a  response assignment. These reading response assignments can either be done in writing (min 500 words) or submitted as a video response (min 3 minutes). Prompt questions will be provided.**

**All readings will be accompanied by a 30 minute to 1 hour class discussion.**

## 3D Exercise - 3D Shapes

Basic Shape Drawing - 10 min

Using only cubes, rectangular prisms, cylinders and spheres, draw simplified versions of the objects on the table

## 3D Exercise - Device

Basic Shape Device - 15 min

Based on your experience of simplifying objects in the first exercise, use the same basic 3D shapes to make a drawing of a device that only you know how to operate. Think of what the device does? The challenge: it should not look like a conventional device like a computer mouse or blender.



<!-- <script>
document.addEventListener("DOMContentLoaded", () => {
  const headings = document.querySelectorAll("h2");

  headings.forEach(h2 => {
    // Create details + summary
    const details = document.createElement("details");
    const summary = document.createElement("summary");
    summary.textContent = h2.textContent;
    details.appendChild(summary);

    // Move content after h2 until next h2
    let sibling = h2.nextElementSibling;
    while (sibling && sibling.tagName !== "H2") {
      const next = sibling.nextElementSibling;
      details.appendChild(sibling);
      sibling = next;
    }

    // Insert collapsible right after the heading
    h2.insertAdjacentElement("afterend", details);
  });
});
</script> -->







