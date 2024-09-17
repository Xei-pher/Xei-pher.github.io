---
layout: default
---

# About Me

<div id="typed-text"></div>

<p id="cursor" class="blink">|</p>

<script>
  document.addEventListener("DOMContentLoaded", function() {
    const text = [
      "I'm **Seifer Rija Boado**, a BS in Information Technology graduate from De La Salle University, specializing in **Cybersecurity**.",
      "With **three internships in the field**, I'm passionate about securing systems and exploring emerging threats in cybersecurity.",
      "I'm looking to enter the field full-time and contribute to a secure digital future.",
      "You can explore my **projects, education, work experience, and certifications** below:",
      "Feel free to reach out to me via [LinkedIn](https://www.linkedin.com/in/seifer-rija-boado-0a196a238/) or [email](mailto:seiferboado101@gmail.com)."
    ];

    let currentTextIndex = 0;
    let currentCharIndex = 0;
    const typingSpeed = 50;
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
      }
    }

    type();
  });
</script>

<style>
  #typed-text {
    font-family: 'Courier', monospace;
    font-size: 1.2rem;
    white-space: pre-wrap;
  }

  .blink {
    font-family: 'Courier', monospace;
    font-size: 1.2rem;
    display: inline;
    animation: blink 0.7s step-start infinite;
  }

  @keyframes blink {
    50% { opacity: 0; }
  }
</style>
