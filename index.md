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
  <a href="https://medium.com/@seiferboado101" target="_blank" class="contact-icon">
    <i class="fab fa-medium"></i>
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
      "I'm Seifer Rija Boado, an Information Security Engineer currently working at Continent 8 Technologies. I specialize in Security Operations and Digital Forensics & Incident Response (DFIR).",
      "I hold certifications such as CySA+, CDSA, eCIR, eCTHP, BTL1, eJPT, PJPT, PSAA, and more—validating my practical expertise across both blue and offensive security disciplines.",
      "In my role, I actively monitor, investigate, and respond to threats in real-time, optimize SIEM and detection rules, conduct threat hunting, and perform root cause analysis on security incidents.",
      "I have hands-on experience with Microsoft Defender, Intune, Purview, XDR, DLP, MDM, IDS/IPS, firewalls, NAC, and a range of SIEM solutions. I’ve helped boost ISO 27001/27002 compliance and improve incident response efficiency across diverse industries.",
      "I earned my Bachelor's Degree in Information Technology from De La Salle University, where I consistently made the Dean’s List and graduated with Honorable Mention.",
      "Feel free to explore my projects, certifications, and career journey below—or reach out via LinkedIn, Medium, or email. Always open to opportunities, collaboration, or just a good conversation about cybersecurity."
    ];


    let currentTextIndex = 0;
    let currentCharIndex = 0;
    const typingSpeed = 1;
    const typedTextElement = document.getElementById("typed-text");
    const cursorElement = document.getElementById("cursor");

    function type() {
      if (currentCharIndex < text[currentTextIndex].length) {
        typedTextElement.innerHTML += text[currentTextIndex].charAt(currentCharIndex);
        currentCharIndex++;
        setTimeout(type, typingSpeed);
      } else if (currentTextIndex < text.length - 1) {
        styleText(currentTextIndex);
        currentTextIndex++;
        currentCharIndex = 0;
        typedTextElement.innerHTML += "<br><br>";
        setTimeout(type, typingSpeed);
      } else {
        styleText(currentTextIndex);
        cursorElement.style.display = "none";
      }
    }

    function styleText(index) {
      const typedTextHTML = typedTextElement.innerHTML;

      if (index === 0) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "Seifer Rija Boado",
          "<span class='bold-green'>Seifer Rija Boado</span>"
        ).replace(
          "Threat and Vulnerability Management",
          "<span class='bold-green'>Threat and Vulnerability Management</span>"
        );
      } else if (index === 1) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "CySA+, Security+, CCNA, eJPT, AZ-900, CNSP, and BTL1",
          "<span class='bold-green'>CySA+, Security+, CCNA, eJPT, AZ-900, CNSP, and BTL1</span>"
        );
      } else if (index === 3) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "ISO 27001/27002",
          "<span class='bold-green'>ISO 27001/27002</span>"
        );
      } else if (index === 4) {
        typedTextElement.innerHTML = typedTextHTML.replace(
          "LinkedIn",
          "<span class='bold-green'>LinkedIn</span>"
        ).replace(
          "Medium",
          "<span class='bold-green'>Medium</span>"
        ).replace(
          "email",
          "<span class='bold-green'>email</span>"
        );
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
    color: green;
    font-size: 2rem;
  }

  .contact-icon:hover {
    color: darkgreen;
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
