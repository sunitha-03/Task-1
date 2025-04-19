<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>My Portfolio</title>
  <link rel="stylesheet" href="styles.css" />
</head>
<body>
  <header class="home-section" id="home">
    <h1>Hello, I'm [Your Name]</h1>
    <p>Welcome to my portfolio website!</p>
    <img src="your-image.jpg" alt="Professional Image" />
  </header>

  <section class="skills-section" id="skills">
    <h2>Skills</h2>
    <ul>
      <li>HTML <progress value="90" max="100"></progress></li>
      <li>CSS <progress value="85" max="100"></progress></li>
      <li>JavaScript <progress value="75" max="100"></progress></li>
    </ul>
  </section>

  <section class="projects-section" id="projects">
    <h2>Projects</h2>
    <div class="project">
      <h3>Project 1</h3>
      <p>A short description of the project.</p>
      <a href="https://github.com/your-repo/project1" target="_blank">View on GitHub</a>
    </div>
  </section>

  <section class="contact-section" id="contact">
    <h2>Contact Me</h2>
    <form>
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
    <div class="socials">
      <a href="https://linkedin.com/in/yourprofile">LinkedIn</a>
      <a href="https://github.com/yourprofile">GitHub</a>
    </div>
  </section>

  <footer>
    <p>&copy; 2025 [Your Name]. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
body {
  font-family: 'Segoe UI', sans-serif;
  margin: 0;
  padding: 0;
  line-height: 1.6;
  color: #333;
}

header, section {
  padding: 40px;
  text-align: center;
}

header {
  background-color: #f0f4ff;
}

.skills-section ul {
  list-style-type: none;
  padding: 0;
}

.skills-section li {
  margin-bottom: 10px;
}

.project {
  border: 1px solid #ddd;
  padding: 20px;
  margin: 20px auto;
  max-width: 500px;
  background-color: #fff;
}

form input, form textarea {
  width: 80%;
  padding: 10px;
  margin: 10px 0;
}

button {
  padding: 10px 20px;
  background-color: #6a5acd;
  color: #fff;
  border: none;
  cursor: pointer;
}

footer {
  background-color: #222;
  color: #fff;
  padding: 20px;
  text-align: center;
}

@media (max-width: 600px) {
  header, section {
    padding: 20px;
  }

  form input, form textarea {
    width: 100%;
  }
}
// Optional: Add smooth scrolling for anchor links
document.querySelectorAll('a[href^="#"]').forEach(anchor => {
  anchor.addEventListener('click', function(e) {
    e.preventDefault();
    document.querySelector(this.getAttribute('href')).scrollIntoView({
      behavior: 'smooth'
    });
  });
});
