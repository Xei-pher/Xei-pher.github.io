---
layout: default
---

# About Me

<div id="typed-text"></div>

<p id="cursor" class="blink">|</p>

<div id="contact-links">
  <a href="https://www.linkedin.com/in/seifer-rija-boado-0a196a238/" target="_blank" class="contact-icon">
    <i class="fab fa-linkedin"></i>
  </a>
  <a href="mailto:seiferboado101@gmail.com" class="contact-icon">
    <i class="fas fa-envelope"></i>
  </a>
  <!-- Download CV Button -->
  <a href="./Boado_CV_Security.pdf" download class="cv-button">
    <i class="fas fa-file-download"></i> Download CV
  </a>
</div>

<!-- New section for additional links -->
# Quick Links
  - [Projects](./projects.md)
  - [Education & Work Experience](./education-work.md)
  - [Certifications & Skills](./certifications-skills.md)

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const text = [
      "I'm Seifer Rija Boado, a BS in Information Technology graduate from De La Salle University, specializing in Cybersecurity.",
      "With three internships in the field, I'm passionate about securing systems and exploring emerging threats in cybersecurity.",
      "I'm looking to enter the field full-time and contribute to a secure digital future.",
      "You can explore my projects, education, work experience, and certifications below:",
      'Feel free to reach out to me via LinkedIn or email.'
    ];

    let currentTextIndex = 0;
    let currentCharIndex = 0;
    const typingSpeed = 7; // Fast typing speed
    const typedTextElement = document.getElementById("typed-text");
    const cursorElement = document.getElementById("cursor");

    function type() {
      if (currentCharIndex < text[currentTextIndex].length) {
        typedTextElement.innerHTML += text[currentTextIndex].charAt(currentCharIndex);
        currentCharIndex++;
        setTimeout(type, typingSpeed);
      } else if (currentTextIndex < text.length - 1) {
        // Apply bold and green styles after typing the current line
        styleText(currentTextIndex);
        
        currentTextIndex++;
        currentCharIndex = 0;
        typedTextElement.innerHTML += "<br><br>";
        setTimeout(type, typingSpeed);
      } else {
        styleText(currentTextIndex); // Style the last line
        cursorElement.style.display = "none"; // Hide cursor when done typing
      }
    }

    function styleText(index) {
      const typedTextHTML = typedTextElement.innerHTML;

      if (index === 0) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "Seifer Rija Boado",
          "<span class='bold-green'>Seifer Rija Boado</span>"
        ).replace(
          "Cybersecurity",
          "<span class='bold-green'>Cybersecurity</span>"
        );
      } else if (index === 1) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "three internships in the field",
          "<span class='bold-green'>three internships in the field</span>"
        );
      } else if (index === 3) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "projects, education, work experience, and certifications",
          "<span class='bold-green'>projects, education, work experience, and certifications</span>"
        );
      } else if (index === 4) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "LinkedIn",
          "<span class='bold-green'>LinkedIn</span>"
        ).replace(
          "email",
          "<span class='bold-green'>email</span>"
        );
      }
    }

    type(); // Start typing
  });
</script>

<style>
  /* Text styling */
  #typed-text {
    font-family: 'Courier', monospace;
    font-size: 1.2rem;
    white-space: pre-wrap;
  }

  /* Green and bold class */
  .bold-green {
    font-weight: bold;
    color: green;
  }

  /* Blinking cursor */
  .blink {
    font-family: 'Courier', monospace;
    font-size: 1.2rem;
    display: inline;
    animation: blink 0.7s step-start infinite;
  }

  @keyframes blink {
    50% { opacity: 0; }
  }

  /* Contact icon styling */
  #contact-links {
    margin-top: 20px;
  }

  .contact-icon {
    margin-right: 15px;
    text-decoration: none;
    color: green; /* Green color for icons */
    font-size: 2rem; /* Size of the icons */
  }

  .contact-icon:hover {
    color: darkgreen; /* Darken the icon color on hover */
  }

  /* CV button styling */
  .cv-button {
    margin-left: 15px;
    text-decoration: none;
    color: green;
    font-size: 1.5rem;
    border: 2px solid green;
    padding: 5px 10px;
    border-radius: 5px;
    font-weight: bold;
    display: inline-block;
    transition: all 0.3s ease;
  }

  .cv-button:hover {
    background-color: green;
    color: white;
    border-color: darkgreen;
  }

  /* Quick Links styling */
  #quick-links {
    margin-top: 20px;
  }

  #quick-links h2 {
    font-size: 1.5rem;
    color: green;
    margin-bottom: 10px;
  }

  #quick-links ul {
    list-style-type: none;
    padding: 0;
  }

  #quick-links li {
    margin-bottom: 10px;
  }

  .link-item {
    text-decoration: none;
    color: green;
    font-weight: bold;
  }

  .link-item:hover {
    text-decoration: underline;
    color: darkgreen;
  }
</style>

<!-- Include Font Awesome for Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
