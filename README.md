# Ex01 Portfolio
## Date:

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
HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title><p class="jayapriya"></p> | Portfolio</title>
    <link rel="stylesheet" href="pf.css">
</head>

<body>

<!-- Header -->
<header>
    <nav>
        <h1 class="logo">P.Jayapriya</h1>

        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#projects">Projects</a></li>
            <li><a href="#skills">Skills</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>

    <div class="home-image">
        <img src="prof.png"alt="P.Jayapriya">
    </div>

</section>

<!-- About -->
<section id="about" class="about-section">

    <h2>About Me</h2>

    <p>
        I am an CSE student with knowledge of Python, Java,
        HTML, CSS and JavaScript. I enjoy building web applications
        and learning new AI technologies.
    </p>

</section>

<!-- Projects -->
<section id="projects" class="projects-section">

    <h2>Projects</h2>

    <div class="projects-grid">

        <div class="project-card">
            <h3>Portfolio Website</h3>
            <p>Developed a responsive portfolio using HTML and CSS.</p>
        </div>

        <div class="project-card">
            <h3>AI Face Swap Detection</h3>
            <p>Studied deepfake attacks and AI-based face swap detection methods.</p>
        </div>

        <div class="project-card">
            <h3>Expense Tracker</h3>
            <p>Created an application to manage daily expenses and budgets.</p>
        </div>

    </div>

</section>

<!-- Skills -->
<section id="skills" class="skills-section">

    <h2>Skills</h2>

    <div class="skill">
        <p>Python</p>
        <div class="bar"><div class="fill python"></div></div>
    </div>

    <div class="skill">
        <p>Java</p>
        <div class="bar"><div class="fill java"></div></div>
    </div>

    <div class="skill">
        <p>HTML</p>
        <div class="bar"><div class="fill html"></div></div>
    </div>

    <div class="skill">
        <p>CSS</p>
        <div class="bar"><div class="fill css"></div></div>
    </div>

    <div class="skill">
        <p>JavaScript</p>
        <div class="bar"><div class="fill javascript"></div></div>
    </div>

</section>

<!-- Contact -->
<section id="contact" class="contact-section">

    <h2>Contact</h2>

    <p><strong>Name:</strong> P.Jayapriya</p>

    <p><strong>Department:</strong> Computer Science Engineering </p>

    <p><strong>College:</strong> Saveetha Engineering College</p>

    <p><strong>Email:</strong> jayapriya@gmail.com</p>

</section>

<!-- Footer -->
<footer>

    <p>© 2026 P.Jayapriya|CSE Student</p>

</footer>

</body>
</html>
```
CSS
```
*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    font-family:'Segoe UI',sans-serif;
}

html{
    scroll-behavior:smooth;
}

body{
    background:linear-gradient(135deg,#0f172a,#1e3a8a,#2563eb);
    color:#ffffff;
    line-height:1.6;
}


header{
    width:100%;
    background:rgba(0,0,0,0.35);
    backdrop-filter:blur(10px);
    position:fixed;
    top:0;
    left:0;
    z-index:1000;
    padding:18px 8%;
}

nav{
    display:flex;
    justify-content:space-between;
    align-items:center;
}

.logo{
    font-size:30px;
    color:#00f7ff;
    font-weight:bold;
}

nav ul{
    list-style:none;
    display:flex;
    gap:30px;
}

nav ul li a{
    color:white;
    text-decoration:none;
    font-size:18px;
    transition:.3s;
}

nav ul li a:hover{
    color:#00f7ff;
}



.home-section{
    min-height:100vh;
    display:flex;
    justify-content:space-between;
    align-items:center;
    padding:130px 10% 80px;
    gap:60px;
}

.home-text{
    flex:1;
}

.home-text h2{
    font-size:48px;
    margin-bottom:15px;
}

.home-text span{
    color:#00f7ff;
}

.home-text h3{
    font-size:28px;
    color:#ffd43b;
    margin-bottom:20px;
}

.home-text p{
    font-size:18px;
    text-align:justify;
    margin-bottom:30px;
}

.btn{
    display:inline-block;
    background:#00f7ff;
    color:#000;
    text-decoration:none;
    padding:14px 35px;
    border-radius:30px;
    font-weight:bold;
    transition:.4s;
}

.btn:hover{
    background:#ffd43b;
    transform:scale(1.05);
}

.home-image{
    flex:1;
    display:flex;
    justify-content:center;
}

.home-image img{
    width:320px;
    height:320px;
    object-fit:cover;
    border-radius:50%;
    border:6px solid #00f7ff;
    box-shadow:0 0 25px cyan;
}


section{
    padding:80px 10%;
}

section h2{
    text-align:center;
    font-size:38px;
    margin-bottom:40px;
    color:#00f7ff;
}



.about-section p{
    max-width:900px;
    margin:auto;
    text-align:justify;
    font-size:18px;
    background:rgba(255,255,255,.08);
    padding:30px;
    border-radius:15px;
}



.education-card{
    background:rgba(255,255,255,.08);
    padding:25px;
    margin:25px auto;
    border-radius:15px;
    max-width:700px;
    text-align:center;
    transition:.3s;
}

.education-card:hover{
    transform:translateY(-8px);
}

.education-card h3{
    color:#ffd43b;
    margin-bottom:15px;
}


.projects-grid{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(260px,1fr));
    gap:30px;
}

.project-card{
    background:white;
    color:#333;
    padding:25px;
    border-radius:15px;
    transition:.4s;
    box-shadow:0 10px 25px rgba(0,0,0,.3);
}

.project-card:hover{
    transform:translateY(-10px);
}

.project-card h3{
    color:#2563eb;
    margin-bottom:15px;
}

.project-card p{
    text-align:justify;
}



.skill{
    margin-bottom:25px;
}

.skill p{
    margin-bottom:8px;
    font-size:18px;
}

.bar{
    width:100%;
    height:16px;
    background:#d1d5db;
    border-radius:20px;
    overflow:hidden;
}

.fill{
    height:100%;
    border-radius:20px;
}

/* Skill Percentages */

.python{
    width:90%;
    background:#00d4ff;
}

.java{
    width:85%;
    background:#ff9800;
}

.html{
    width:95%;
    background:#ff3b5f;
}

.css{
    width:92%;
    background:#3f8cff;
}

.javascript{
    width:80%;
    background:#ffd43b;
}

.ml{
    width:88%;
    background:#00c853;
}

.cloud{
    width:82%;
    background:#7c4dff;
}

.cyber{
    width:78%;
    background:#ff1744;
}



.achievement-section ul{
    max-width:850px;
    margin:auto;
    background:rgba(255,255,255,.08);
    padding:30px;
    border-radius:15px;
}

.achievement-section li{
    margin:15px 0;
    font-size:18px;
}


.contact-section{
    text-align:center;
}

.contact-section p{
    font-size:18px;
    margin:12px 0;
}



footer{
    background:#08101f;
    text-align:center;
    padding:25px;
    font-size:17px;
    margin-top:40px;
}


@media(max-width:992px){

.home-section{
    flex-direction:column-reverse;
    text-align:center;
}

.home-text p{
    text-align:center;
}

.home-image img{
    width:260px;
    height:260px;
}

nav{
    flex-direction:column;
    gap:15px;
}

nav ul{
    flex-wrap:wrap;
    justify-content:center;
}

}

@media(max-width:600px){

.home-text h2{
    font-size:34px;
}

.home-text h3{
    font-size:22px;
}

section h2{
    font-size:30px;
}

.logo{
    font-size:24px;
}

nav ul{
    gap:15px;
}

nav ul li a{
    font-size:16px;
}

}
```

## OUTPUT

<img width="1525" height="702" alt="Screenshot 2026-09-16 105327" src="https://github.com/user-attachments/assets/33701a49-6949-48ae-8eaf-a44de2d7ebb1" />
<img width="1510" height="692" alt="Screenshot 2026-09-16 105348" src="https://github.com/user-attachments/assets/5819f579-e978-4739-82ba-c5c6ca3ddb17" />
<img width="1493" height="673" alt="Screenshot 2026-09-16 105404" src="https://github.com/user-attachments/assets/1ec48761-b8f0-4365-8620-492534be6ad5" />
<img width="1511" height="611" alt="Screenshot 2026-09-16 105422" src="https://github.com/user-attachments/assets/1e6d69c0-c806-4ab8-af44-fae1dae469b4" />


## RESULT
The program for creating Portfolio using HTML and CSS is executed successfully.
