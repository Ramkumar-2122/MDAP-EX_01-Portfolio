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
    <title>Animated Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navbar -->
    <header>
        <nav>
            <h1 class="logo">My Portfolio</h1>
            <ul class="nav-links">
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-text fade-in">
            <h2>Hello, I'm <span>Ram kumar S</span></h2>
            <p>Aspiring Machine Learning & Web Developer</p>
            <a href="#projects" class="btn">See My Work</a>
        </div>
    </section>

    <!-- About -->
    <section id="about" class="about fade-in">
        <h2>About Me</h2>
        <p>
            I create interactive websites and AI-powered applications.
            Skilled in HTML, CSS, JavaScript, Python, Flask, and Machine Learning.
        </p>
    </section>

    <!-- Projects -->
    <section id="projects" class="projects fade-in">
        <h2>Projects</h2>
        <div class="project-grid">
            <a href="https://github.com/username/healthcare" target="_blank" class="project-card">
                <h3>Healthcare Prediction App</h3>
                <p>Predict diseases and suggest precautions using ML.</p>
            </a>
            <a href="https://github.com/username/stock" target="_blank" class="project-card">
                <h3>Stock Price Predictor</h3>
                <p>Predict stock trends with deep learning models.</p>
            </a>
            <a href="https://github.com/username/numberplate" target="_blank" class="project-card">
                <h3>E-commerce website</h3>
                <p>Building an online platform for selling products or services.</p>
            </a>
        </div>
    </section>

    <!-- Contact -->
    <section id="contact" class="contact fade-in">
        <h2>Contact Me</h2>
        <p>Email: <a href="mailto:sramkumar2122@gmail.com">sramkumar2122@gmail.com</a></p>
        <p>
            <a href="https://github.com/username" target="_blank">GitHub</a> |
            <a href="https://linkedin.com/in/username" target="_blank">LinkedIn</a>
        </p>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2025 Ram kumar. All Rights Reserved.</p>
    </footer>

</body>
</html>

```
## style.css
```
/* General */
body {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    background: #0f0f0f;
    color: #fff;
    scroll-behavior: smooth;
}

/* Navbar */
header {
    background: rgba(0,0,0,0.8);
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 100;
}
nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 15px 40px;
}
.logo {
    color: #00f7ff;
    font-size: 1.5em;
    font-weight: bold;
}
.nav-links {
    list-style: none;
    display: flex;
}
.nav-links li {
    margin-left: 20px;
}
.nav-links a {
    text-decoration: none;
    color: #fff;
    transition: color 0.3s;
}
.nav-links a:hover {
    color: #00f7ff;
}

/* Hero Section */
.hero {
    height: 100vh;
    background: linear-gradient(120deg, #ff0080, #7928ca, #00f7ff);
    background-size: 300% 300%;
    animation: gradientShift 10s ease infinite;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
}
.hero h2 {
    font-size: 2.5em;
}
.hero span {
    color: #00f7ff;
}
.btn {
    display: inline-block;
    margin-top: 15px;
    padding: 10px 25px;
    background: #00f7ff;
    color: #000;
    text-decoration: none;
    font-weight: bold;
    border-radius: 30px;
    transition: transform 0.3s, background 0.3s;
}
.btn:hover {
    background: #fff;
    transform: scale(1.1);
}

/* About Section */
.about, .projects, .contact {
    padding: 80px 20px;
    max-width: 900px;
    margin: auto;
    text-align: center;
}

/* Projects */
.project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}
.project-card {
    background: #1e1e1e;
    padding: 20px;
    border-radius: 10px;
    text-decoration: none;
    color: #fff;
    box-shadow: 0 0 10px rgba(0,0,0,0.3);
    transition: transform 0.3s, box-shadow 0.3s;
}
.project-card:hover {
    transform: translateY(-8px);
    box-shadow: 0 0 20px #00f7ff;
}

/* Contact Section */
.contact a {
    color: #00f7ff;
}
.contact a:hover {
    text-decoration: underline;
}

/* Footer */
footer {
    background: #000;
    padding: 15px;
    text-align: center;
}

/* Fade In Animation */
.fade-in {
    animation: fadeIn 1.5s ease forwards;
    opacity: 0;
}
@keyframes fadeIn {
    from { opacity: 0; transform: translateY(30px); }
    to { opacity: 1; transform: translateY(0); }
}

/* Background Gradient Animation */
@keyframes gradientShift {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}

```

## OUTPUT
![WhatsApp Image 2025-08-08 at 09 30 01_9a4bcd7b](https://github.com/user-attachments/assets/abdce4c0-1823-4d5d-a777-33e1f16aebe3)

![WhatsApp Image 2025-08-08 at 09 30 01_99526a5c](https://github.com/user-attachments/assets/11d218f4-da5f-4f4c-ab0a-f9e6c8426ac7)

## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
