<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Mouhcine MAHBOUBI - Portfolio</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
:root {
    --rose: #ff4f9a;
    --blue: #1e90ff;
    --black: #0d0d0d;
    --card-bg: #151515;
    --text: #fff;
}
* {margin:0; padding:0; box-sizing:border-box;}
body {font-family:'Segoe UI', sans-serif; background: var(--black); color: var(--text); line-height:1.6;}
header {position:fixed; top:0; left:0; width:100%; background:rgba(13,13,13,0.9); display:flex; justify-content:space-between; align-items:center; padding:1rem 2rem; z-index:1000;}
.logo {font-weight:bold; font-size:1.3rem; background: linear-gradient(45deg,var(--rose),var(--blue)); -webkit-background-clip:text; -webkit-text-fill-color:transparent;}
nav ul {display:flex; list-style:none; gap:1.5rem;}
nav a {color:var(--text); text-decoration:none; position:relative;}
nav a::after {content:""; position:absolute; bottom:-4px; left:0; width:0; height:2px; background:var(--rose); transition:0.3s;}
nav a:hover::after {width:100%;}
.hero {min-height:100vh; display:flex; flex-direction:column; justify-content:center; align-items:center; text-align:center; background: radial-gradient(circle at top left, rgba(255,79,154,0.15), transparent), radial-gradient(circle at bottom right, rgba(30,144,255,0.15), transparent);}
.hero h1 {font-size:2.8rem; background: linear-gradient(45deg,var(--rose),var(--blue)); -webkit-background-clip:text; -webkit-text-fill-color:transparent;}
.hero p {margin-top:0.5rem; color:#ccc;}
section {padding:4rem 2rem; max-width:1200px; margin:auto;}
section h2 {text-align:center; margin-bottom:2rem; font-size:2rem; position:relative;}
section h2::after {content:""; position:absolute; bottom:-8px; left:50%; transform:translateX(-50%); width:60px; height:3px; background:linear-gradient(45deg,var(--rose),var(--blue));}
.timeline {display:flex; flex-direction:column; gap:2rem;}
.timeline-item {background:var(--card-bg); padding:1.5rem; border-radius:10px; border:1px solid #333; position:relative;}
.timeline-item::before {content:""; position:absolute; top:20px; left:-30px; width:15px; height:15px; background:var(--rose); border-radius:50%; box-shadow:0 0 10px var(--rose);}
.skills-grid {display:grid; grid-template-columns:repeat(auto-fit,minmax(250px,1fr)); gap:1.5rem;}
.skill-category {background:var(--card-bg); padding:1.5rem; border-radius:10px; border:1px solid #333;}
.skill-item {margin-bottom:0.5rem;}
.skill-level {width:100%; height:6px; background:#333; border-radius:3px; overflow:hidden;}
.skill-progress {height:100%; background:linear-gradient(90deg,var(--rose),var(--blue));}
.languages-grid, .contact-grid {display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:1rem;}
.card {background:var(--card-bg); padding:1.5rem; border-radius:8px; text-align:center;}
.contact-btn {display:inline-block; padding:0.5rem 1rem; background:var(--rose); color:#fff; border-radius:5px; text-decoration:none;}
.contact-btn:hover {background:var(--blue);}
footer {text-align:center; padding:1rem; color:#999; background:#111; margin-top:2rem;}
@media(max-width:768px) {nav ul {display:none;} nav.active ul {display:flex; flex-direction:column;}}
</style>
</head>
<body>
<header>
    <div class="logo">Mouhcine MAHBOUBI</div>
    <nav>
        <ul>
            <li><a href="#home">Accueil</a></li>
            <li><a href="#formation">Formation</a></li>
            <li><a href="#competences">Compétences</a></li>
            <li><a href="#langues">Langues</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
</header>
<section class="hero" id="home">
    <h1>Futur Ingénieur en Génie Électrique</h1>
    <p>ENSEM Casablanca | 📍 Settat, Maroc</p>
</section>
<section id="formation">
    <h2>Formation</h2>
    <div class="timeline">
        <div class="timeline-item"><h3>Bac STE - Mention Bien</h3><p>2020 - 2023</p></div>
        <div class="timeline-item"><h3>CPGE TSI - Centre Settat</h3><p>2023 - 2025</p></div>
        <div class="timeline-item"><h3>ENSEM - Génie Électrique</h3><p>2025 - Présent</p></div>
    </div>
</section>
<section id="competences">
    <h2>Compétences</h2>
    <div class="skills-grid">
        <div class="skill-category"><h3>Techniques</h3>
            <div class="skill-item">Conception circuits<div class="skill-level"><div class="skill-progress" style="width:80%"></div></div></div>
            <div class="skill-item">Analyse circuits<div class="skill-level"><div class="skill-progress" style="width:85%"></div></div></div>
            <div class="skill-item">Programmation embarquée<div class="skill-level"><div class="skill-progress" style="width:75%"></div></div></div>
            <div class="skill-item">Automatisation industrielle<div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
        </div>
        <div class="skill-category"><h3>Outils</h3>
            <div class="skill-item">Python<div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item">MATLAB<div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
            <div class="skill-item">PSIM<div class="skill-level"><div class="skill-progress" style="width:85%"></div></div></div>
            <div class="skill-item">Arduino<div class="skill-level"><div class="skill-progress" style="width:80%"></div></div></div>
        </div>
        <div class="skill-category"><h3>Personnelles</h3>
            <div class="skill-item">Adaptabilité<div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item">Travail d'équipe<div class="skill-level"><div class="skill-progress" style="width:80%"></div></div></div>
            <div class="skill-item">Gestion du temps<div class="skill-level"><div class="skill-progress" style="width:85%"></div></div></div>
            <div class="skill-item">Créativité<div class="skill-level"><div class="skill-progress" style="width:88%"></div></div></div>
        </div>
    </div>
</section>
<section id="langues">
    <h2>Langues</h2>
    <div class="languages-grid">
        <div class="card">Arabe - Langue Maternelle</div>
        <div class="card">Français - Niveau 4/6</div>
        <div class="card">Anglais - Niveau 4/6</div>
    </div>
</section>
<section id="contact">
    <h2>Contact</h2>
    <div class="contact-grid">
        <div class="card"><a class="contact-btn" href="mailto:mahboubi.mhc.etd@gmail.com">📧 Email</a></div>
        <div class="card"><a class="contact-btn" href="https://wa.me/212650361793" target="_blank">💬 WhatsApp</a></div>
        <div class="card"><a class="contact-btn" href="https://www.linkedin.com/in/mouhcine-mahboubi-ba6210235" target="_blank">LinkedIn</a></div>
        <div class="card"><a class="contact-btn" href="https://www.instagram.com/mhb_b0/" target="_blank">Instagram</a></div>
    </div>
</section>
<footer>© 2025 Mouhcine MAHBOUBI</footer>
</body>
</html>
