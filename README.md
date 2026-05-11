<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Arshman Abbas | Cybersecurity Portfolio</title>

<link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;900&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet">

<style>

*{
margin:0;
padding:0;
box-sizing:border-box;
scroll-behavior:smooth;
}

body{
background:#020617;
font-family:'Inter',sans-serif;
color:white;
overflow-x:hidden;
}

body::before{
content:"";
position:fixed;
width:100%;
height:100%;
background:
radial-gradient(circle at top left,#00ffe015,transparent 25%),
radial-gradient(circle at bottom right,#0066ff20,transparent 30%);
z-index:-3;
}

.grid{
position:fixed;
width:100%;
height:100%;
background-image:
linear-gradient(rgba(255,255,255,0.03) 1px, transparent 1px),
linear-gradient(90deg, rgba(255,255,255,0.03) 1px, transparent 1px);
background-size:50px 50px;
z-index:-2;
}

.blur{
position:fixed;
width:500px;
height:500px;
background:#00ffe030;
filter:blur(180px);
border-radius:50%;
top:-100px;
right:-100px;
z-index:-1;
animation:move 10s infinite alternate ease-in-out;
}

@keyframes move{
100%{
transform:translate(-100px,100px);
}
}

.container{
width:90%;
max-width:1300px;
margin:auto;
}

nav{
display:flex;
justify-content:space-between;
align-items:center;
padding:30px 0;
}

.logo{
font-size:1.8rem;
font-family:'Orbitron',sans-serif;
font-weight:900;
color:#00ffe0;
text-shadow:0 0 15px #00ffe0;
letter-spacing:2px;
}

nav a{
text-decoration:none;
color:#d7e3ff;
margin-left:30px;
transition:0.3s;
font-size:15px;
}

nav a:hover{
color:#00ffe0;
}

.hero{
min-height:90vh;
display:flex;
justify-content:space-between;
align-items:center;
gap:50px;
flex-wrap:wrap;
}

.left{
flex:1;
}

.tag{
display:inline-block;
padding:10px 18px;
background:#00ffe010;
border:1px solid #00ffe040;
border-radius:40px;
color:#00ffe0;
font-size:14px;
margin-bottom:25px;
backdrop-filter:blur(10px);
}

.hero h1{
font-size:5rem;
font-family:'Orbitron',sans-serif;
line-height:1.1;
margin-bottom:25px;
background:linear-gradient(to right,#00ffe0,#4facfe);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
}

.hero p{
max-width:700px;
font-size:18px;
line-height:1.9;
color:#b9c6e3;
}

.buttons{
margin-top:40px;
display:flex;
gap:20px;
flex-wrap:wrap;
}

.btn{
padding:16px 32px;
border-radius:14px;
text-decoration:none;
font-weight:600;
transition:0.4s;
}

.primary{
background:linear-gradient(90deg,#00ffe0,#4facfe);
color:black;
box-shadow:0 0 25px #00ffe055;
}

.primary:hover{
transform:translateY(-5px);
box-shadow:0 0 40px #00ffe099;
}

.secondary{
border:1px solid #ffffff20;
color:white;
backdrop-filter:blur(10px);
}

.secondary:hover{
border-color:#00ffe0;
color:#00ffe0;
}

.right{
flex:1;
display:flex;
justify-content:center;
align-items:center;
position:relative;
}

.cyber-box{
width:420px;
height:420px;
border-radius:30px;
background:rgba(255,255,255,0.04);
border:1px solid rgba(255,255,255,0.08);
backdrop-filter:blur(15px);
display:flex;
justify-content:center;
align-items:center;
position:relative;
overflow:hidden;
box-shadow:0 0 50px rgba(0,255,224,0.1);
}

.cyber-box::before{
content:"";
position:absolute;
width:150%;
height:150%;
background:conic-gradient(
from 0deg,
transparent,
#00ffe080,
transparent,
#4facfe90,
transparent
);
animation:spin 5s linear infinite;
}

.cyber-box::after{
content:"";
position:absolute;
inset:4px;
background:#020617;
border-radius:26px;
}

.shield{
position:relative;
z-index:5;
font-size:120px;
text-shadow:0 0 30px #00ffe0;
animation:float 3s ease-in-out infinite;
}

@keyframes spin{
100%{
transform:rotate(360deg);
}
}

@keyframes float{
50%{
transform:translateY(-15px);
}
}

section{
padding:120px 0;
}

.title{
font-size:3rem;
font-family:'Orbitron',sans-serif;
margin-bottom:20px;
background:linear-gradient(to right,#00ffe0,#4facfe);
-webkit-background-clip:text;
-webkit-text-fill-color:transparent;
}

.desc{
max-width:800px;
line-height:1.9;
color:#a8b6d3;
margin-bottom:60px;
}

.projects{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(300px,1fr));
gap:30px;
}

.card{
background:rgba(255,255,255,0.04);
border:1px solid rgba(255,255,255,0.06);
padding:35px;
border-radius:24px;
transition:0.5s;
position:relative;
overflow:hidden;
backdrop-filter:blur(12px);
}

.card:hover{
transform:translateY(-10px);
border-color:#00ffe080;
box-shadow:0 0 35px rgba(0,255,224,0.12);
}

.card h3{
font-size:1.6rem;
margin-bottom:18px;
color:#00ffe0;
}

.card p{
line-height:1.8;
color:#c1cee8;
}

.skills{
display:flex;
flex-wrap:wrap;
gap:18px;
margin-top:50px;
}

.skill{
padding:15px 24px;
background:rgba(255,255,255,0.04);
border:1px solid rgba(255,255,255,0.08);
border-radius:14px;
transition:0.3s;
color:#dbe8ff;
}

.skill:hover{
background:#00ffe0;
color:black;
transform:translateY(-4px);
}

footer{
padding:60px 0;
text-align:center;
border-top:1px solid rgba(255,255,255,0.08);
color:#91a3c7;
margin-top:60px;
}

footer a{
color:#00ffe0;
text-decoration:none;
}

@media(max-width:900px){

.hero{
flex-direction:column;
padding-top:80px;
}

.hero h1{
font-size:3.5rem;
}

.cyber-box{
width:320px;
height:320px;
}

}

</style>
</head>

<body>

<div class="grid"></div>
<div class="blur"></div>

<div class="container">

<nav>
<div class="logo">ARSHII.exe</div>

<div>
<a href="#">Home</a>
<a href="#">Projects</a>
<a href="#">Skills</a>
<a href="#">Contact</a>
</div>
</nav>

<section class="hero">

<div class="left">

<div class="tag">
🛡️ SOC • Cloud Security • GRC
</div>

<h1>
DEFENDING<br>
DIGITAL<br>
SYSTEMS
</h1>

<p>
I build modern cybersecurity solutions focused on threat detection,
Shadow IT monitoring, cloud security, governance, and real-time security visibility.
Passionate about creating offensive and defensive security projects that combine
automation, intelligence, and modern cyber defense practices.
</p>

<div class="buttons">

<a href="#" class="btn primary">
View Projects
</a>

<a href="https://linkedin.com/in/arshman-abbas-89a95732a" class="btn secondary">
LinkedIn
</a>

</div>

</div>

<div class="right">

<div class="cyber-box">
<div class="shield">🛡️</div>
</div>

</div>

</section>

<section>

<h2 class="title">Featured Projects</h2>

<p class="desc">
Building cybersecurity-focused platforms and tools centered around monitoring,
threat intelligence, cloud exposure analysis, compliance, and security automation.
</p>

<div class="projects">

<div class="card">
<h3>ShadowScan</h3>

<p>
AI-powered Shadow IT monitoring platform capable of detecting unauthorized SaaS usage,
performing risk analysis, integrating threat intelligence, and visualizing exposure
through a real-time SOC-style dashboard.
</p>
</div>

<div class="card">
<h3>ThreatLens</h3>

<p>
Advanced security monitoring and log analysis system designed to centralize event
correlation, improve visibility, and accelerate suspicious activity detection workflows.
</p>
</div>

<div class="card">
<h3>CloudGuard Audit</h3>

<p>
Cloud security auditing environment focused on identifying risky configurations,
security gaps, compliance issues, and exposure risks across modern infrastructures.
</p>
</div>

</div>

<div class="skills">

<div class="skill">Splunk</div>
<div class="skill">Wazuh</div>
<div class="skill">ELK Stack</div>
<div class="skill">Python</div>
<div class="skill">Linux</div>
<div class="skill">Threat Intelligence</div>
<div class="skill">Cloud Security</div>
<div class="skill">Risk Assessment</div>
<div class="skill">SOC Monitoring</div>

</div>

</section>

<footer>

<p>
© 2026 Arshman Abbas — Cybersecurity Portfolio
</p>

<br>

<p>
Connect:
<a href="https://linkedin.com/in/arshman-abbas-89a95732a">
linkedin.com/in/arshman-abbas-89a95732a
</a>
</p>

</footer>

</div>

</body>
</html>
