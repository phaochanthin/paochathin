<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
<title>Chanthin Pao — Data Scientist</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600;800&family=Inter:wght@300;400;500;600&display=swap" rel="stylesheet"/>

<style>
:root{
  --bg-dark:#0f172a;
  --bg-light:#1e293b;
  --accent:#38bdf8;
  --accent2:#6366f1;
  --white:#ffffff;
  --soft:#94a3b8;
}

*{margin:0;padding:0;box-sizing:border-box}

body{
  font-family:'Inter',sans-serif;
  background:linear-gradient(135deg,var(--bg-dark),var(--bg-light));
  color:var(--white);
  overflow-x:hidden;
}

/* Floating Glow */
body::before{
  content:'';
  position:fixed;
  top:-200px;
  right:-200px;
  width:500px;
  height:500px;
  background:radial-gradient(circle,var(--accent2),transparent 70%);
  opacity:.2;
  filter:blur(120px);
}

/* NAV */
nav{
  position:fixed;
  top:0;left:0;right:0;
  padding:1.3rem 3rem;
  display:flex;
  justify-content:space-between;
  align-items:center;
  backdrop-filter:blur(12px);
  background:rgba(15,23,42,0.6);
  border-bottom:1px solid rgba(255,255,255,0.05);
}

.logo{
  font-family:'Playfair Display',serif;
  font-size:1.5rem;
  font-weight:800;
  letter-spacing:1px;
}
.logo span{color:var(--accent)}

nav a{
  color:var(--soft);
  text-decoration:none;
  margin-left:2rem;
  font-size:.9rem;
  transition:.3s;
}
nav a:hover{color:var(--accent)}

/* HERO */
.hero{
  min-height:100vh;
  display:flex;
  flex-direction:column;
  justify-content:center;
  align-items:center;
  text-align:center;
  padding:6rem 1.5rem 3rem;
}

.tag{
  text-transform:uppercase;
  letter-spacing:3px;
  font-size:.75rem;
  color:var(--accent);
  margin-bottom:1rem;
}

.hero h1{
  font-family:'Playfair Display',serif;
  font-size:clamp(2.5rem,5vw,4rem);
  margin-bottom:1rem;
}
.hero h1 span{color:var(--accent)}

.subtitle{
  max-width:650px;
  color:var(--soft);
  font-size:1rem;
  line-height:1.7;
  margin-bottom:2rem;
}

.btn{
  display:inline-block;
  padding:.8rem 2rem;
  margin:.5rem;
  border-radius:30px;
  font-size:.9rem;
  text-decoration:none;
  transition:.3s;
}

.btn-primary{
  background:linear-gradient(90deg,var(--accent),var(--accent2));
  color:white;
}
.btn-primary:hover{transform:translateY(-3px);box-shadow:0 10px 30px rgba(56,189,248,.4)}

.btn-outline{
  border:1px solid rgba(255,255,255,0.2);
  color:var(--white);
}
.btn-outline:hover{background:rgba(255,255,255,0.05);transform:translateY(-3px)}

/* STATS */
.stats{
  display:flex;
  justify-content:center;
  gap:2rem;
  margin-top:4rem;
  flex-wrap:wrap;
}

.stat{
  background:rgba(255,255,255,0.05);
  padding:1.5rem 2rem;
  border-radius:15px;
  backdrop-filter:blur(12px);
  text-align:center;
  transition:.3s;
}
.stat:hover{
  transform:translateY(-6px);
  background:rgba(255,255,255,0.08);
}
.stat h2{
  font-size:2rem;
  font-family:'Playfair Display',serif;
}
.stat p{
  font-size:.8rem;
  color:var(--soft);
}

/* SKILLS */
.skills{
  max-width:700px;
  margin:5rem auto;
  padding:0 1.5rem;
}

.skills h2{
  text-align:center;
  font-family:'Playfair Display',serif;
  margin-bottom:2rem;
}

.skill{
  margin-bottom:1.2rem;
}

.skill span{
  font-size:.85rem;
  color:var(--soft);
}

.bar{
  height:8px;
  background:rgba(255,255,255,0.1);
  border-radius:50px;
  margin-top:.4rem;
  overflow:hidden;
}

.fill{
  height:100%;
  background:linear-gradient(90deg,var(--accent),var(--accent2));
  width:0;
  animation:grow 1.5s ease forwards;
}

.fill.python{width:92%}
.fill.ml{width:88%}
.fill.sql{width:80%}
.fill.viz{width:85%}

@keyframes grow{
  from{width:0}
}

/* FOOTER */
footer{
  text-align:center;
  padding:2rem;
  font-size:.8rem;
  color:var(--soft);
  border-top:1px solid rgba(255,255,255,0.05);
}

@media(max-width:768px){
  nav{padding:1rem 1.5rem}
}
</style>
</head>

<body>

<nav>
  <div class="logo">Chanthin<span>.</span></div>
  <div>
    <a href="#">Home</a>
    <a href="#">Skills</a>
    <a href="mailto:phaochanthin@gmail.com">Contact</a>
  </div>
</nav>

<section class="hero">
  <div class="tag">Data Scientist, Data Analyst, Machine Learning</div>
  <h1>Hi, I'm <span>Chanthin Pao</span></h1>
  <p class="subtitle">
    I transform raw data into powerful insights that drive smarter decisions.
    Specialized in Machine Learning, Statistical Modeling, and Data Visualization.
  </p>

  <div>
    <a href="#" class="btn btn-primary">View Projects</a>
    <a href="mailto:alex.morgan@email.com" class="btn btn-outline">Contact Me</a>
  </div>

  <div class="stats">
    <div class="stat">
      <h2>1+</h2>
      <p>Years Experience</p>
    </div>
    <div class="stat">
      <h2>10+</h2>
      <p>Projects Completed</p>
    </div>
    <div class="stat">
      <h2>Good</h2>
      <p>Model Accuracy</p>
    </div>
  </div>
</section>

<section class="skills">
  <h2>Core Skills</h2>

  <div class="skill">
    <span>Python</span>
    <div class="bar"><div class="fill python"></div></div>
  </div>

  <div class="skill">
    <span>Machine Learning / AI</span>
    <div class="bar"><div class="fill ml"></div></div>
  </div>

  <div class="skill">
    <span>SQL & Databases</span>
    <div class="bar"><div class="fill sql"></div></div>
  </div>

  <div class="skill">
    <span>Data Visualization</span>
    <div class="bar"><div class="fill viz"></div></div>
  </div>

</section>

<footer>
  Designed & Built by <strong>Chanthin Pao</strong> · Hosted on GitHub
</footer>

</body>
</html>
