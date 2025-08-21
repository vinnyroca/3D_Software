

<style>
/* Button styling */
#focusToggle {
  position: fixed;
  bottom: 20px;
  right: 20px;
  z-index: 1000;
  padding: 0.5em 1em;
  background: #333;
  color: #fff;
  border: none;
  border-radius: 6px;
  cursor: pointer;
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

<button id="focusToggle">F</button>

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
    button.textContent = focusEnabled ? "X" : "F";
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

## Schedule and Class Website

[Schedule](./schedule.md)

Class Website: 3DSoftware.vinnyroca.info

## Class Discord

[Join the Class Discord](https://discord.gg/D7wfJDQ3QJ)







## Course Goals

To learn the practice, theory, and history of 3D Software

## Practice

Autodesk Maya - Hardsurface 3D models, Animation, and Simulation

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

**We live in a society of software.**

How we interface with these computational devices is often through software with a graphical user interface. Think of the interface of your iPhone, consider the levels of computation that this elaborately designed interface hides away.

In the early history of computing, people didn’t interact with software. Engineers, programmers, and artists interacted with computers through physical punch cards or other physical inputs and outputs.

<p><a href="https://commons.wikimedia.org/wiki/File:Two_women_operating_ENIAC_(full_resolution).jpg#/media/File:Two_women_operating_ENIAC_(full_resolution).jpg"><img src="https://upload.wikimedia.org/wikipedia/commons/8/8c/Two_women_operating_ENIAC_%28full_resolution%29.jpg" alt="Two women programming ENIAC."  width="800"></a><br>By Unidentified U.S. Army photographer - Image from <a rel="nofollow" class="external text" href="https://ftp.arl.army.mil/ftp/historic-computers/">Historic Computer Images</a>, Public Domain, <a href="https://commons.wikimedia.org/w/index.php?curid=26253297">Link</a></p>

## Software

Software and computer graphics mediate our experience with the computer. In other words, they provide an interface that translates the work being done by the computer and the work being done by the artist, designer, engineer, or even the consumer.

The field of software studies looks to understand the impact of software on culture.

In this class, we’ll be studying 3D computer graphics software, looking to understand its cultural, political, and economic effects.

Where we’ll start:

- Software Takes Command - Lev Manovich (2013)

- Getting to Know Software: A Study of Autodesk Maya - Aylish Wood (2015)

From this starting point, we’ll continue to Image Objects: An Archaeology of Computer Graphics - Jacob Gaboury (2021)

Image Objects will guide us through the history of computer graphics that leads to the software we will be using in class: Maya and ZBrush. Focusing particularly on the early research in computer graphics at the University of Utah, Image Objects will demonstrate how many of the objects we use today, from our phones to our books, can trace their origins back to the beginnings of computer graphics.

From there, we’ll consider further readings on the continued impact of 3D models and computer graphics.

**All readings will have a reading response assignment. These reading response assignments can either be done in writing (min 500 words) or submitted as a video response (min 3 minutes). Prompt questions will be provided.**

**All readings besides our first reading assignment on Software Takes Command will be accompanied by a 30-minute - 1-hour class discussion.**

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







