# my-portfolio..
<--this is my first project-->

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Jaydip Portfolio</title>

<style>

/* RESET */
*{
margin:0;
padding:0;
box-sizing:border-box;

}

body{
font-family:Arial, Helvetica, sans-serif;
line-height:1.6;
color:#060606;

}

/* SCROLL INDICATOR */

.scroll-indicator{
position:fixed;
top:0;
left:0;
height:4px;
width:0%;
background:linear-gradient(to right,purple,blue);
z-index:1000;
}

/* NAVBAR */

nav{
background:linear-gradient(45deg,purple,blue);
padding:15px;
position:sticky;
top:0;
z-index:100;
box-shadow: 0 4px 10px rgba(0, 0, 0, 0.822);;
}

nav ul{
list-style:none;
display:flex;
justify-content:center;
gap:30px;
}

nav a{
color:white;
text-decoration:none;
font-weight:bold;
transition:0.3s;
}

nav a:hover{
transform:translateY(-3px);
}

/* HERO */

.hero{
background:linear-gradient(45deg,purple,blue);
color:white;
text-align:center;
padding:120px 20px;
display: flex;
justify-content: center;
align-items: center;
height: 300px;
}

.hero h1{
font-size:3rem;
margin-bottom:15px;
animation: fadein 1s forwards;
}

.hero p{
font-size:1.2rem;
margin-bottom:25px;
animation:fadeIn 2s forwards;
animation-delay: 1s;
}

.btn{
background:white;
color:blue;
padding: 5px 7px;
border-radius:10px;
text-decoration:none;
transition:0.3s;
}

.btn:hover{
animation: fadeIn 0.5s forwards;
transform:scale(1.1);
}

/* SECTIONS */

section{
padding:60px 20px;
max-width:1100px;
margin:auto;
}

section h2{
text-align:center;
margin-bottom:40px;
color:black;
font-size: large;
}

/* ABOUT */

.about-content{
display:flex;
gap: 100px;
flex-wrap:wrap;
;

}
.about-image{
    flex: 0.5s;
    text-align: center;
}

.profile-pic{
width:200px;
height:200px;
border-radius:50%;
background:linear-gradient(45deg,#6a11cb,#2575fc);
display:flex;
align-items:center;
justify-content:center;
font-size:80px;
color:rgb(250, 248, 248);
}

.about-text{
flex:1;
margin: 20px;
padding: 20px;
font-size: 17px;
}

/* SKILLS */

.skills-container{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
}

.skill-card{
background:#f4f4f4;
padding:20px;
border-radius:10px;
text-align:center;
cursor:pointer;
transition:0.3s;
}

.skill-card:hover{
transform:translateY(-8px);
box-shadow:0 5px 15px rgba(0,0,0,0.2);
}
.skill-card h3{
color: #6a11cb,blue;
margin:0px,0px,10px,0px;
}

.skill-bar{
background:gray;
height:10px;
border-radius:20px;
overflow:hidden;
margin-top:15px;
}

.skill-progress{
height:100%;
width:0%;
background:linear-gradient(45deg,#6a11cb,#2575fc);
transition:width 1s;
}

/* PROJECTS */

.projects-grid{
background: white;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:25px;
border-radius: 1%;
}

.project-card{
background:white;
border-radius:10px;
box-shadow:0 3px 10px rgba(0,0,0,0.1);
overflow:hidden;
transition:0.3s;
}

.project-card:hover{
transform:translateY(-8px);
}

.project-image{
height:120px;
background:linear-gradient(45deg,#6a11cb,#2575fc);
display:flex;
align-items:center;
justify-content:center;
font-size:large;
color:white;
}
.project-info{
padding:20px;
color: #6a11cb;

}






/* CONTACT */

.contact-form{
max-width:500px;
margin:auto;

}

.form-group{
margin-bottom:20px;
}

.form-group label{
display:block;
margin-bottom:5px;
font-weight:bold;
color: #6a11cb;
}

input, textarea{
width:100%;
padding:10px;
border:1px solid #ccc;
border-radius:5px;
}

.submit-btn{
background:linear-gradient(45deg,#6a11cb,#2575fc);
color:white;
border:none;
padding:12px 20px;
border-radius:30px;
cursor:pointer;
transition:0.3s;
font-style: italic;
}

.submit-btn:hover{
transform:scale(1.1);
}

/* FOOTER */

footer{
background:#111;
color:white;
text-align:center;
padding:20px;
}
.scroll-indicator{
position: fixed;
top: 0;
left: 0;
height: 4px;
width: 0%;
background: linear-gradient(90deg, #6a11cb, #2575fc);
z-index: 9999;
transition: width 0.2s ease;
}
/* RESPONSIVE */

@media(max-width:768px){

.hero h1{
font-size:2rem;
}

.about-content{
flex-direction:column;
align-items:center;
}

nav ul{
flex-wrap:wrap;
}

}

</style>
</head>

<body>

<div class="scroll-indicator" id="scrollIndicator"></div>

<!-- NAVBAR -->

<nav>
<ul>
<li><a href="#home" class="nav-link">Home</a></li>
<li><a href="#about" class="nav-link">About</a></li>
<li><a href="#skills" class="nav-link">Skills</a></li>
<li><a href="#projects" class="nav-link">Projects</a></li>
<li><a href="#contact" class="nav-link">Contact</a></li>
</ul>
</nav>

<!-- HERO -->

<section id="home" class="hero">

<h1>Welcome to My Portfolio</h1>
<p>Hello, I'm Jaydip am learning web development.</p>
<a href="#contact" class="btn">Contact Me</a>
</section>

<!-- ABOUT -->

<section id="about">
<h2>About Me</h2>

<div class="about-content">

<div class="profile-pic">👨‍💻</div>

<div class="about-text">
<p>I am learning web development and building modern websites.</p>
<p>I enjoy working with HTML, CSS and JavaScript.</p>
<p>My goal is to become a professional full stack developer.</p>
</div>

</div>
</section>

<!-- SKILLS -->

<section id="skills">

<h2>My Skills</h2>

<div class="skills-container">

<div class="skill-card" data-skill="90">
<h3>HTML5</h3>
<p>i use html5 to create semantic and accessible web pages.</p>
<div class="skill-bar">
<div class="skill-progress"></div>
</div>
</div>

<div class="skill-card" data-skill="80">
<h3>CSS3</h3>
<p>i use css3 for styling and creating responsive layouts.</p>
<div class="skill-bar">
<div class="skill-progress"></div>
</div>
</div>

<div class="skill-card" data-skill="70">
<h3>JavaScript</h3>
<p>i use javascript to add interactivity to websites.</p>
<div class="skill-bar">
<div class="skill-progress"></div>
</div>
</div>

</div>

</section>

<!-- PROJECTS -->

<section id="projects">

<h2>My Projects</h2>

<div class="projects-grid">

<div class="project-card">
<div class="project-image">🌐</div>
<div class="project-info">
<h3>My Portfolio</h3>
<p>this is my personal portfolio website to showcase my work.</p>
</div>
</div>

<div class="project-card">
<div class="project-image">📱</div>
<div class="project-info">
<h3>Landing Page</h3>
<p>A responsive landing page.</p>
</div>
</div>

<div class="project-card">
<div class="project-image">🎨</div>
<div class="project-info">
<h3>UI Design</h3>
<p>Interactive UI components.</p>
</div>
</div>

</div>

</section>

<!-- CONTACT -->

<section id="contact">

<h2>Get In Touch</h2>

<form class="contact-form" id="contactForm">

<div class="form-group">
<label for="name">Name</label>
<input type="text" id="name" required>
</div>

<div class="form-group">
<label for="email">Email</label>
<input type="email" id="email" required>
</div>

<div class="form-group">
<label for="message">Message</label>
<textarea id="message" required></textarea>
</div>

<button class="submit-btn">submit</button>

</form>

</section>

<footer>
<p>@jaydip2002|portfolio</p>
</footer>

<script>

/* SMOOTH SCROLL */

document.querySelectorAll(".nav-link").forEach(link=>{
link.addEventListener("click",function(e){
e.preventDefault()

const target=document.querySelector(this.getAttribute("href"))

target.scrollIntoView({
behavior:"smooth"
})

})
})

/* SCROLL INDICATOR */

window.addEventListener("scroll",()=>{

const indicator=document.getElementById("scrollIndicator")

const height=document.documentElement.scrollHeight-window.innerHeight

const scrolled=(window.scrollY/height)*100

indicator.style.width=scrolled+"%"

})

/* SKILL ANIMATION */

function animateSkills(){

document.querySelectorAll(".skill-card").forEach(card=>{

const rect=card.getBoundingClientRect()

if(rect.top<window.innerHeight){

const level=card.dataset.skill

card.querySelector(".skill-progress").style.width=level+"%"

}

})

}

window.addEventListener("scroll",animateSkills)
window.addEventListener("load",animateSkills)

/* FORM */

document.getElementById("contactForm").addEventListener("submit",function(e){

e.preventDefault()

alert("Thank you! Your message has been sent.")

this.reset()

})

</script>

</body>
</html>

