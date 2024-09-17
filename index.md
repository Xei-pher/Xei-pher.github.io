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
      "I'm Seifer Rija Boado, a BS in Information Technology graduate from De La Salle University, specializing in Cybersecurity.",
      "With three internships in the field, I'm passionate about securing systems and exploring emerging threats in cybersecurity.",
      "I'm looking to enter the field full-time and contribute to a secure digital future.",
      "You can explore my projects, education, work experience, and certifications below:",
      'Feel free to reach out to me via <a href="https://www.linkedin.com/in/seifer-rija-boado-0a196a238/" target="_blank">LinkedIn</a> or <a href="mailto:seiferboado101@gmail.com">email</a>.'
    ];

    const boldGreenParts = [
      [4, 23], // "Seifer Rija Boado"
      [69, 83], // "Cybersecurity"
      [5, 30], // "three internships in the field"
      [49, 83], // "projects, education, work experience, and certifications"
    ];

    let currentTextIndex = 0;
    let currentCharIndex = 0;
    const typingSpeed = 20; // Adjust typing speed
    const typedTextElement = document.getElementById("typed-text");
    const cursorElement = document.getElementById("cursor");

    function type() {
      if (currentCharIndex < text[currentTextIndex].length) {
        let charToAdd = text[currentTextIndex].charAt(currentCharIndex);

        // Check if the current character is within a range to be bold and green
        let inBoldRange = false;
        boldGreenParts.forEach(([start, end]) => {
          if (currentTextIndex === boldGreenParts.indexOf([start, end])) {
            if (currentCharIndex >= start && currentCharIndex <= end) {
              charToAdd = "<span class='bold-green'>" + charToAdd;
              // Closing 'bold-green'
