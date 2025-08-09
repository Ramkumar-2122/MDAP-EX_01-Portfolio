# MDAP-EX_01-Portfolio
## Date: 09-08-2025

## AIM
To create a Portfolio using HTML and CSS.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for introduction, about, projects, and contact details.

### STEP 5
Define global styles for fonts, colors, and layout.

### STEP 6
Style the header, navigation bar, and sections.

### STEP 7
Use Flexbox or CSS Grid for layout design.

### STEP 8
Add hover effects and transitions for interactivity.

### STEP 9
Add Images and Media.

### STEP 10
Use optimized images for a professional look.

### STEP 11
Open the HTML file in a browser to check layout and functionality.

### STEP 12
Fix styling issues and refine content placement.

### STEP 13
Deploy the Portfolio.

### STEP 14
Upload to GitHub Pages for free hosting.

## PROGRAM
## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header -->
    <header>
        <nav>
            <h1 class="logo">MyPortfolio</h1>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <h2>Hello, I'm <span>Kamal raj A</span></h2>
        <p>Aspiring Machine Learning & Web Developer</p>
        <a href="#projects" class="btn">View My Work</a>
    </section>

    <!-- About Section -->
    <section id="about" class="about">
        <h2>About Me</h2>
        <p>
            I'm a passionate developer who loves building interactive web apps and AI-powered projects.
            Skilled in HTML, CSS, JavaScript, Python, and Machine Learning frameworks.
        </p>
    </section>

    <!-- Projects Section -->
    <section id="projects" class="projects">
    <h2>Projects</h2>
    <div class="project-grid">

        <!-- Project 1 -->
        <a href="https://github.com/username/healthcare-prediction-app" target="_blank" class="project-link">
            <div class="project-card">
                <h3>Healthcare Prediction App</h3>
                <p>ML-powered app to predict diseases and suggest precautions.</p>
            </div>
        </a>

        <!-- Project 2 -->
        <a href="https://github.com/username/stock-price-predictor" target="_blank" class="project-link">
            <div class="project-card">
                <h3>Stock Price Predictor</h3>
                <p>Flask-based app predicting stock prices using Keras models.</p>
            </div>
        </a>

        <!-- Project 3 -->
        <a href="https://github.com/username/number-plate-recognition" target="_blank" class="project-link">
            <div class="project-card">
                <h3>Number Plate Recognition</h3>
                <p>YOLOv5 and OCR-based vehicle number plate detection.</p>
            </div>
        </a>
    </div>
    </section>


    <!-- Contact Section -->
    <section id="contact" class="contact">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:kamalraj3106@gmail.com">kamalraj3106@gmail.com</a></p>
        <p>
            <a href="https://github.com/Kamal-Raj-A" target="_blank">GitHub</a> |
            <a href="https://www.linkedin.com/in/kamal-raj-a-2a5054290?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app" target="_blank">LinkedIn</a>
        </p>
    </section>

    <footer>
        <p>&copy; 2025 Kamal Raj. All Rights Reserved.</p>
    </footer>
</body>
</html>

```
## style.css
```
/* General Styles */
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background-color: #f4f4f4;
    color: #333;
}

/* Navbar */
header {
    background: #222;
    padding: 15px 0;
}
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    max-width: 1100px;
    margin: auto;
    padding: 0 20px;
}
.logo {
    color: #fff;
    font-size: 1.5em;
}
.nav-links {
    list-style: none;
    display: flex;
}
.nav-links li {
    margin-left: 20px;
}
.nav-links a {
    color: #fff;
    text-decoration: none;
    font-weight: bold;
}
.nav-links a:hover {
    color: #00bcd4;
}

/* Hero Section */
.hero {
    background: linear-gradient(to right, #00bcd4, #009688);
    color: #fff;
    text-align: center;
    padding: 100px 20px;
}
.hero h2 {
    font-size: 2.5em;
}
.hero span {
    color: #ffeb3b;
}
.hero .btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 20px;
    background: #ffeb3b;
    color: #333;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
}
.hero .btn:hover {
    background: #ffc107;
}

/* About Section */
.about {
    padding: 50px 20px;
    max-width: 800px;
    margin: auto;
    text-align: center;
}

/* Projects Section */
.projects {
    background: #fff;
    padding: 50px 20px;
}
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}
.project-card {
    background: #fafafa;
    padding: 20px;
    border-radius: 10px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    text-align: center;
}
.project-card:hover {
    transform: scale(1.05);
    transition: 0.3s ease;
}

/* Contact Section */
.contact {
    background: #02b4cb;
    color: #fff;
    padding: 50px 20px;
    text-align: center;
}
.contact a {
    color: #ffeb3b;
    text-decoration: none;
}
.contact a:hover {
    text-decoration: underline;
}

/* Footer */
footer {
    background: #222;
    color: #fff;
    padding: 15px;
    text-align: center;
}

/* Responsive */
@media (max-width: 600px) {
    .hero h2 {
        font-size: 1.8em;
    }
}

```

## OUTPUT
![WhatsApp Image 2025-08-08 at 09 30 01_9a4bcd7b](https://github.com/user-attachments/assets/abdce4c0-1823-4d5d-a777-33e1f16aebe3)


![Uploading WhatsApp Image 2025-08-08 at 09.30.01_d1dddfc2.jpg…]()



## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
