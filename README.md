<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Mouhcine MAHBOUBI - Futur Ingénieur Électrique</title>
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
<style>
:root {
    --primary: #e91e63;
    --secondary: #9c27b0;
    --accent: #ff4081;
    --bg-dark: #0a0a0a;
    --bg-card: #1a1a1a;
    --text: #fff;
    --text-muted: #b0b0b0;
}
* {margin:0;padding:0;box-sizing:border-box;}
body {font-family: 'Segoe UI', sans-serif; background: var(--bg-dark); color: var(--text); line-height: 1.6; overflow-x:hidden;}
header {position:fixed; top:0; width:100%; background: rgba(26,26,26,0.95); display:flex; justify-content:space-between; align-items:center; padding:1rem 2rem; z-index:1000;}
.logo {font-weight:bold; background: linear-gradient(45deg,var(--primary),var(--secondary)); -webkit-background-clip:text; -webkit-text-fill-color:transparent;}
nav ul {display:flex; list-style:none; gap:1.5rem;}
nav a {color:var(--text-muted); text-decoration:none; transition:0.3s; position:relative;}
nav a::after {content:""; position:absolute; bottom:-4px; left:0; width:0; height:2px; background:var(--accent); transition:0.3s;}
nav a:hover {color:var(--accent);} nav a:hover::after {width:100%;}
.burger {display:none; flex-direction:column; gap:5px; cursor:pointer;}
.burger div {width:25px; height:3px; background:var(--text);}
.hero {min-height:100vh; display:flex; align-items:center; justify-content:center; text-align:center; padding:2rem; background: radial-gradient(circle at top left, rgba(233,30,99,0.15), transparent), radial-gradient(circle at bottom right, rgba(156,39,176,0.15), transparent);}
.hero h1 {font-size:2.8rem; background: linear-gradient(45deg, var(--primary), var(--secondary)); -webkit-background-clip:text; -webkit-text-fill-color:transparent; animation: glow 2s infinite alternate;}
@keyframes glow {from {text-shadow:0 0 10px rgba(233,30,99,0.3);} to {text-shadow:0 0 20px rgba(156,39,176,0.5);}}
.section {padding:4rem 2rem; max-width:1200px; margin:auto;}
.section h2 {text-align:center; margin-bottom:2rem; font-size:2rem; position:relative;}
.section h2::after {content:""; position:absolute; bottom:-8px; left:50%; transform:translateX(-50%); width:60px; height:3px; background:linear-gradient(45deg,var(--primary),var(--secondary));}
.timeline {position:relative; padding:2rem 0;}
.timeline::before {content:""; position:absolute; left:50%; transform:translateX(-50%); top:0; bottom:0; width:2px; background:linear-gradient(180deg,var(--primary),var(--secondary));}
.timeline-item {position:relative; width:45%; background:var(--bg-card); padding:1.5rem; border-radius:10px; border:1px solid #333; animation: fadeInUp 1s ease forwards; opacity:0;}
.timeline-item:nth-child(odd){left:0;} .timeline-item:nth-child(even){left:55%;}
.timeline-item::before {content:""; position:absolute; top:20px; width:20px; height:20px; background:var(--accent); border-radius:50%; border:3px solid var(--bg-dark);}
.timeline-item:nth-child(odd)::before {right:-60px;} .timeline-item:nth-child(even)::before {left:-60px;}
.timeline-date {color:var(--accent); font-weight:bold; margin-bottom:0.5rem;}
@keyframes fadeInUp {to {opacity:1; transform:translateY(0);} from {transform:translateY(30px);} }
.skills-grid {display:grid; grid-template-columns:repeat(auto-fit,minmax(300px,1fr)); gap:2rem;}
.skill-category {background:var(--bg-card); padding:2rem; border-radius:10px; border:1px solid #333; transition:0.3s;}
.skill-category:hover {transform:translateY(-5px); box-shadow:0 0 20px rgba(233,30,99,0.2);}
.skill-item {display:flex; justify-content:space-between; align-items:center; margin-bottom:0.5rem;}
.skill-level {width:100px; height:6px; background:#333; border-radius:3px; overflow:hidden;}
.skill-progress {height:100%; background:linear-gradient(90deg,var(--primary),var(--accent)); animation: progressFill 2s ease-out;}
@keyframes progressFill {from{width:0;}}
.languages-grid, .contact-grid {display:grid; grid-template-columns:repeat(auto-fit,minmax(200px,1fr)); gap:1rem;}
.card {background:var(--bg-card); padding:1.5rem; border-radius:8px; text-align:center; transition:0.3s;}
.card:hover {transform:translateY(-5px);}
.contact-btn {display:inline-block; padding:0.5rem 1rem; background:var(--primary); color:#fff; border-radius:5px; text-decoration:none; transition:0.3s;}
.contact-btn:hover {background:var(--accent);}
footer {text-align:center; padding:1rem; font-size:0.9rem; color:var(--text-muted); background:#111;}
@media(max-width:768px){nav ul {position:absolute; top:60px; right:0; background:rgba(26,26,26,0.95); flex-direction:column; width:200px; transform:translateX(100%); transition:transform 0.3s; padding:1rem;} nav ul.active{transform:translateX(0);} .burger{display:flex;} .timeline::before{left:20px;} .timeline-item{width:calc(100% - 40px) !important; left:40px !important;} .timeline-item::before{left:-45px !important;}}
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
    <div class="burger" onclick="document.querySelector('nav ul').classList.toggle('active')">
        <div></div><div></div><div></div>
    </div>
</header>
<section class="hero" id="home">
    <div>
        <h1>Futur Ingénieur en Génie Électrique</h1>
        <p>ENSEM Casablanca | 📍 Settat, Maroc</p>
    </div>
</section>
<section class="section" id="formation">
    <h2>Formation</h2>
    <div class="timeline">
        <div class="timeline-item"><div class="timeline-date">2020 - 2023</div><h3>Bac STE - Mention Bien</h3><p>Sciences et Technologies Électriques...</p></div>
        <div class="timeline-item"><div class="timeline-date">2023 - 2025</div><h3>CPGE TSI - Centre Settat</h3><p>Formation intensive en sciences de l'ingénieur...</p></div>
        <div class="timeline-item"><div class="timeline-date">2025 - Présent</div><h3>ENSEM - Génie Électrique</h3><p>Formation d'ingénieur spécialisée...</p></div>
    </div>
</section>
<section class="section" id="competences">
    <h2>Compétences</h2>
    <div class="skills-grid">
        <div class="skill-category"><h3>⚡ Compétences Techniques</h3>
            <div class="skill-item"><span>Conception de circuits électriques</span><div class="skill-level"><div class="skill-progress" style="width:80%"></div></div></div>
            <div class="skill-item"><span>Analyse des circuits électriques</span><div class="skill-level"><div class="skill-progress" style="width:85%"></div></div></div>
            <div class="skill-item"><span>Systèmes électroniques</span><div class="skill-level"><div class="skill-progress" style="width:75%"></div></div></div>
        </div>
        <div class="skill-category"><h3>💻 Outils & Langages</h3>
            <div class="skill-item"><span>Python</span><div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item"><span>PSIM</span><div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item"><span>MATLAB</span><div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
            <div class="skill-item"><span>LaTeX</span><div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
            <div class="skill-item"><span>Proteus</span><div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
            <div class="skill-item"><span>Langage C</span><div class="skill-level"><div class="skill-progress" style="width:50%"></div></div></div>
            <div class="skill-item"><span>Suite Office</span><div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
        </div>
        <div class="skill-category"><h3>🤝 Compétences Personnelles</h3>
            <div class="skill-item"><span>Adaptabilité</span><div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item"><span>Patience</span><div class="skill-level"><div class="skill-progress" style="width:90%"></div></div></div>
            <div class="skill-item"><span>Travail d'équipe</span><div class="skill-level"><div class="skill-progress" style="width:80%"></div></div></div>
            <div class="skill-item"><span>Gestion du temps</span><div class="skill-level"><div class="skill-progress" style="width:70%"></div></div></div>
        </div>
    </div>
</section>
<section class="section" id="langues">
    <h2>Langues</h2>
    <div class="languages-grid">
        <div class="card">🇲🇦 Arabe - Langue Maternelle</div>
        <div class="card">🇫🇷 Français - Niveau 4/6</div>
        <div class="card">🇬🇧 Anglais - Niveau 4/6</div>
    </div>
</section>
<section class="section" id="contact">
    <h2>Contact</h2>
    <div class="contact-grid">
        <div class="card"><a class="contact-btn" href="mailto:mahboubi.mhc.etd@gmail.com">📧 Envoyer un email</a></div>
        <div class="card"><a class="contact-btn" href="https://wa.me/212650361793" target="_blank">💬 Contacter sur WhatsApp</a></div>
        <div class="card"><a class="contact-btn" href="https://www.linkedin.com/in/mouhcine-mahboubi-ba6210235" target="_blank">LinkedIn</a></div>
        <div class="card"><a class="contact-btn" href="https://www.instagram.com/mhb_b0/" target="_blank">Instagram</a></div>
    </div>
</section>
<footer>&copy; 2025 Mouhcine MAHBOUBI</footer>
<script>
const observer=new IntersectionObserver(entries=>{entries.forEach(e=>{if(e.isIntersecting){e.target.classList.add('visible');}})},{threshold:0.1});
document.querySelectorAll('.timeline-item, .skill-category').forEach(el=>{observer.observe(el);});
</script>
</body>
</html>
