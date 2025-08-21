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

<link rel="stylesheet" type="text/css" href="extra.css">
 
# Syllabus

## Course Information
---
**LOCATION:** Scripps College, Steele 229  
**TIME:** Tuesday and Thursday 10:00-12:30, 8/25-12/3

**INSTRUCTOR**  
Vinny Roca, Scripps College  
Email: vroca@scrippscollege.edu  
Office Hours: Lang 227. By appointment; Tuesday & Thursday 1:30-2:30 [Schedule office hours](https://outlook.office.com/bookwithme/user/14e2aa0a493c4a659e608aab96b46635@scrippscollege.edu/meetingtype/ex7sQIfLLkiMdKnIgITX3w2?anonymous&ismsaljsauthenabled&ep=mlink)
---
## Course Description

This interdisciplinary introductory course examines the history, theory, and techniques of 3D software. Through weekly assignments, critical readings, and projects, students will engage with 3D software as a technical tool, artistic medium, and cultural object. This course introduces foundational skills in modeling, rendering, and animation using various software. Weekly discussions, readings, and presentations will critically engage with 3D software’s cultural, social, economic, and political dimensions. The ideas and skills taught in this course will set a foundation for future coursework in game design, animation, video art, digital fabrication, and media studies.

---

## Learning Outcomes

The objective of this course is to introduce foundational technical skills in 3D software and contextualize this knowledge within the cultural,  social, economic, and political impact of modeling, rendering, and animation technologies. Through projects, assignments, discussions, reading responses, technical tutorials, and lectures, students will achieve the following learning outcomes:

- Technical proficiency in modeling, rendering, and animating using 3D software.
- Ability to analyze the role of 3D software in media art.
- Ability to analyze software as cultural, historical, and technical objects.
- Gain critical knowledge of history, theory, and cultural impact of 3D software.
- Ability to craft expansive media art projects using 3D software.

---
## Grading, Assignments, Course Policy
---
#### **Course Breakdown**

|%||
|:---:|---|
|35|Memory Chambre|
|35|Dream Object|
|10|Participation|
|10|Reading Responses|
|10|Exercises|

#### **Evaluation Criteria**
#### Projects & Exercises

Projects are separated into a variety of project pieces.

Project pieces and exercises will be graded on their level of completion in regard to the particular project piece or exercise.

Completed projects will be graded using the following criteria:

|||
|:---:|---|
|Technique| Is the assignment well-crafted? Is the conceptual idea behind the assignment supported by the technical and artistic decisions made by the student?|
|Concept|Does the student comprehend the scope of the assignment? Is the student able to communicate their ideas clearly? Does the student demonstrate comprehension of the concepts covered in class? Is the student able to articulate the concepts behind their work?|
|Generosity|Does the student exhibit insight, criticality, and risk-taking in their work? How much sensitivity and critical insight does the student display towards personal assignments and in critiquing their peers’ work?|

#### Participation & Attendance

All students are expected to participate actively during the discussion periods and critiques.

Students more than ten minutes late for class will be marked as late. Three late marks will result in an unexcused absence. More than two unexcused absences may, at the instructor’s discretion, affect the final participation grade.

All classes are mandatory. If you anticipate missing a class or expect to have more than two absences during the course, inform the instructor as soon as possible.

#### Reading Responses

Reading responses are due by 5 p.m. the day before discussions. Reading responses should be posted in proper Discord channel.

Reading responses will be graded on the level of engagement the student has with the text. Is the student connecting the text to other readings or experiences? Is the student engaging with the text through questions, disagreements, or new lines of thought?

Discussion questions to guide reading responses will be provided for each reading.

Reading responses should be either a 500 word written response or uploaded as 3 minute video of your response to the reading.

As reading responses are essential to the discussion section of the course, late reading responses will not be accepted.

### Late Work and Extensions

For all exercises, late work will not be accepted. Completing exercises on time is essential to the progression of the course. Not completing exercises will result in a student falling behind. In the situation that extra time is needed to complete exercises and project pieces, students must reach out to the instructor as soon as possible.

Late projects not ready by their assigned crit day will automatically lose one letter grade. Each day the project is late, it will lose one more letter grade. After three days, the project will not be accepted.

### Discord and Email

For this class, we will be sharing our exercises, reading responses and project pieces through Discord. Students will be invited to join the class Discord server on the first day of class.

I will respond to Discord messages and email within 24 hrs of receipt. I will respond to messages sent over the weekend on the following Monday.

### Box Submissions

Submissions for the class will be made through Box links. Links to Box submissions will be on the class website.

### Readings

All readings are provided by the Instructor using this [link](https://scrippscollege.box.com/s/yjzmo42f7mg85bpzs9tpyvmzxprs9zlv).

## Course Materials

Although ample time will be provided to work in class and the lab will be open during non-class hours when other classes are not in session, you might still find you want to work on your projects outside the lab.

For working outside the lab on your personal computer, the following hardware is recommended:

1. Entry Level Wacom Drawing Tablet ~ $60
2. A 500Gb+ SSD ~ $50-100
3. A three button mouse ~ $20-50
4. Maxon One Student Subscription (This will be needed to run ZBrush) ~ $60
5. Autodesk Maya ~ Free with student login

## Scripps College Land Acknowledgement

We would like to respectfully acknowledge that Scripps College sits within the historic homeland of the Tongva people. We acknowledge the painful history of genocide and colonization in our area. We acknowledge the strength and resilience of the Tongva people of the past, present, and future as the original caretakers of the land, water, and air, and we recognize our responsibility to be respectful stewards of the Scripps College campus. Today, this area and this campus are home to many Indigenous people from across the globe and we are proud that they are part of our community and institution.

## Statement on Inclusion

We understand the classroom as a space for practicing freedom; where one may challenge
psychic, social, and cultural borders and create meaningful artistic expressions. To do so we must
acknowledge and embrace the different identities and backgrounds we inhabit. This means that
we will use pronouns, respect self-identifications, and be mindful of special needs.
Disagreement is encouraged and supported, however, our differences affect our
conceptualization and experience of reality, and it is extremely important to remember that
certain gender, race, sex, and class identities are more privileged while others are undermined
and marginalized. Consequently, this makes some people feel more protected or vulnerable
during debates and discussions. A collaborative effort between the students and Instructor is
needed to create a supportive learning environment. While everyone should feel free to
experiment creatively and conceptually, if a class member points out that something you have
said or shared with the group is offensive, avoid being defensive; instead approach the discussion
as a valuable opportunity for us to grow and learn from one another. Alternatively, if you feel
that something said in discussion or included in a piece of work is harmful, you are encouraged
to speak with the Instructor.

Statement adopted from voidLab at https://github.com/voidlab/diversity-statement.

## Accommodations

The instructor will work individually with each student on reasonable accommodations.

If you have questions about accommodations for the course, please do not hesitate to contact me.

Campus Disability Coordinators

- [Pomona](http://www.pomona.edu/administration/dean-of-students/disability-accommodations/)
- [Claremont Graduate University](http://www.cgu.edu/disabilityservices)
- [Scripps College](http://www.scrippscollege.edu/academics/students-with-disabilities)
- [Claremont McKenna College](http://www.claremontmckenna.edu/dos/DSS/)
- [Harvey Mudd College](https://www.hmc.edu/student-life/health-wellness/disability-services/)
- [Pitzer College](http://pitweb.pitzer.edu/student-life/academic-support-services/)
- [Keck Graduate Institute](http://www.kgi.edu/current-students/student-services/disabilities-accommodations.html)


## Resources

### Class Resources

- [Maya Hotkeys](https://www.autodesk.com/shortcuts/maya)

### 7C Student Resources

- [Campus Safety](https://services.claremont.edu/campus-safety/)
- [Chaplains](https://services.claremont.edu/chaplains/)
- [Chicano Latino Student Affairs (CLSA)](https://services.claremont.edu/clsa/)
- [Claremont Colleges Library](https://library.claremont.edu/)
- [The Claremont Colleges Services (TCCS)](https://services.claremont.edu/)
- [EmPOWER Center](https://inside.scrippscollege.edu/studentaffairs/empower-center)
- [Health Education Outreach (HEO)](https://services.claremont.edu/heo/)
- [Huntley Bookstore](https://www.bkstr.com/claremontstore/home)
- [LiveSafe App](http://colleges.claremont.edu/livesafe/)
- [Monsour Counseling and Psychological Services (MCAPS)](https://services.claremont.edu/mcaps/)
- [Office of Black Student Affairs (OBSA)](https://services.claremont.edu/obsa/)
- [Student Disability Resource Center](https://services.claremont.edu/sdrc/)
- [Student Health Insurance Plan](https://www.scrippscollege.edu/offices/officesservices/treasurer/student-accounts/student-health-insurance)
- [Student Health Services](https://services.claremont.edu/student-health-services/)
- [Queer Resource Center (QRC)](https://colleges.claremont.edu/qrc/)

