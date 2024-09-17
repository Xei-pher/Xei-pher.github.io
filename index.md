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
</div>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const text = [
      "I'm <strong>Seifer Rija Boado</strong>, a BS in Information Technology graduate from De La Salle University, specializing in <strong>Cybersecurity</strong>.",
      "With <strong>three internships in the field</strong>, I'm passionate about securing systems and exploring emerging threats in cybersecurity.",
      "I'm looking to enter the field full-time and contribute to a secure digital future.",
      "You can explore my <strong>projects, education, work experience, and certifications</strong> below:",
      'Feel free to reach out to me via <a href="https://www.linkedin.com/in/seifer-rija-boado-0a196a238/" target="_blank">LinkedIn</a> or <a href="mailto:seiferboado101@gmail.com">email</a>.'
    ];

    let currentTextIndex = 0;
    let currentCharIndex = 0;
    const typingSpeed = 20; // Faster typing speed
    const typedTextElement = document.getElementById("typed-text");
    const cursorElement = document.getElementById("cursor");

    function type() {
      if (currentCharIndex < text[currentTextIndex].length) {
        typedTextElement.innerHTML += text[currentTextIndex].charAt(currentCharIndex);
        currentCharIndex++;
        setTimeout(type, typingSpeed);
      } else if (currentTextIndex < text.length - 1) {
        currentTextIndex++;
        currentCharIndex = 0;
        typedTextElement.innerHTML += "<br><br>";
        setTimeout(type, typingSpeed);
      } else {
        cursorElement.style.display = "none"; // Hide cursor when done typing
      }
    }

    type();
  });
</script>

<style>
  /* Text styling */
  #typed-text {
    font-family: 'Courier', monospace;
    font-size: 1.2rem;
    white-space: pre-wrap;
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
</style>

<!-- Include Font Awesome for Icons -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
