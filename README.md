<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mouhcine MAHBOUBI - Ingénieur Électrique</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        :root {
            --primary-color: #e91e63;
            --secondary-color: #9c27b0;
            --accent-color: #ff4081;
            --bg-dark: #0a0a0a;
            --bg-darker: #050505;
            --bg-card: #1a1a1a;
            --text-primary: #ffffff;
            --text-secondary: #b0b0b0;
            --border-color: #333;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: var(--bg-dark);
            color: var(--text-primary);
            line-height: 1.6;
            overflow-x: hidden;
        }

        /* Circuit background pattern */
        body::before {
            content: '';
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: 
                radial-gradient(circle at 20% 20%, rgba(233, 30, 99, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 80%, rgba(156, 39, 176, 0.1) 0%, transparent 50%),
                linear-gradient(45deg, transparent 48%, rgba(233, 30, 99, 0.03) 50%, transparent 52%),
                linear-gradient(-45deg, transparent 48%, rgba(156, 39, 176, 0.03) 50%, transparent 52%);
            background-size: 100% 100%, 100% 100%, 20px 20px, 20px 20px;
            z-index: -2;
            animation: circuitFlow 20s linear infinite;
        }

        @keyframes circuitFlow {
            0% { background-position: 0% 0%, 100% 100%, 0 0, 0 0; }
            100% { background-position: 100% 100%, 0% 0%, 20px 20px, -20px -20px; }
        }

        /* Navigation - Supprimée */
        nav {
            display: none;
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            gap: 2rem;
        }

        nav a {
            color: var(--text-secondary);
            text-decoration: none;
            padding: 0.5rem 1rem;
            border-radius: 25px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
        }

        nav a::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(233, 30, 99, 0.2), transparent);
            transition: left 0.5s;
        }

        nav a:hover::before {
            left: 100%;
        }

        nav a:hover {
            color: var(--accent-color);
            background: rgba(233, 30, 99, 0.1);
        }

        /* Hero Section */
        .hero {
            height: 100vh;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            position: relative;
            background: transparent;
        }

        .hero-content h1 {
            font-size: 3.5rem;
            background: linear-gradient(45deg, var(--primary-color), var(--secondary-color));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 1rem;
            animation: glow 2s ease-in-out infinite alternate;
        }

        .hero-content {
            background: transparent;
            padding: 0;
            border: none;
            border-radius: 0;
        }

        @keyframes glow {
            from { filter: drop-shadow(0 0 10px rgba(233, 30, 99, 0.3)); }
            to { filter: drop-shadow(0 0 20px rgba(156, 39, 176, 0.5)); }
        }

        .hero-content p {
            font-size: 1.3rem;
            color: var(--text-secondary);
            margin-bottom: 2rem;
        }

        .tech-icons {
            display: flex;
            justify-content: center;
            gap: 1rem;
            margin: 2rem 0;
        }

        .tech-icon {
            font-size: 2rem;
            padding: 1rem;
            background: var(--bg-card);
            border-radius: 50%;
            border: 2px solid transparent;
            transition: all 0.3s ease;
            animation: float 3s ease-in-out infinite;
        }

        .tech-icon:nth-child(even) {
            animation-delay: -1.5s;
        }

        .tech-icon:hover {
            border-color: var(--accent-color);
            transform: scale(1.1);
            box-shadow: 0 0 20px rgba(233, 30, 99, 0.3);
        }

        @keyframes float {
            0%, 100% { transform: translateY(0px); }
            50% { transform: translateY(-10px); }
        }

        /* Section Styles */
        section {
            padding: 5rem 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .section-title {
            font-size: 2.5rem;
            text-align: center;
            margin-bottom: 3rem;
            position: relative;
        }

        .section-title::after {
            display: none;
        }

        /* Formation Timeline */
        .timeline {
            position: relative;
            padding: 2rem 0;
        }

        .timeline::before {
            content: '';
            position: absolute;
            left: 50%;
            top: 0;
            bottom: 0;
            width: 2px;
            background: linear-gradient(180deg, var(--primary-color), var(--secondary-color));
            transform: translateX(-50%);
        }

        .timeline-item {
            position: relative;
            margin: 2rem 0;
            padding: 2rem;
            background: var(--bg-card);
            border-radius: 15px;
            border: 1px solid var(--border-color);
            width: 45%;
            transition: all 0.3s ease;
        }

        .timeline-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 30px rgba(233, 30, 99, 0.2);
        }

        .timeline-item:nth-child(odd) {
            left: 55%;
        }

        .timeline-item:nth-child(even) {
            left: 0%;
        }

        .timeline-item::before {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            background: var(--accent-color);
            border-radius: 50%;
            top: 50%;
            border: 3px solid var(--bg-dark);
        }

        .timeline-item:nth-child(odd)::before {
            left: -60px;
        }

        .timeline-item:nth-child(even)::before {
            right: -60px;
        }

        .timeline-date {
            color: var(--accent-color);
            font-weight: bold;
            margin-bottom: 0.5rem;
        }

        /* Skills Grid */
        .skills-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .skill-category {
            background: var(--bg-card);
            padding: 2rem;
            border-radius: 15px;
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
        }

        .skill-category:hover {
            transform: translateY(-5px);
            border-color: var(--accent-color);
            box-shadow: 0 10px 30px rgba(233, 30, 99, 0.15);
        }

        .skill-category h3 {
            color: var(--accent-color);
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 0.5rem;
        }

        .skill-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 0.5rem 0;
            border-bottom: 1px solid var(--border-color);
        }

        .skill-item:last-child {
            border-bottom: none;
        }

        .skill-level {
            height: 6px;
            background: var(--border-color);
            border-radius: 3px;
            overflow: hidden;
            width: 100px;
        }

        .skill-progress {
            height: 100%;
            background: linear-gradient(90deg, var(--primary-color), var(--accent-color));
            border-radius: 3px;
            animation: progressFill 2s ease-out;
        }

        @keyframes progressFill {
            from { width: 0%; }
        }

        /* Languages Section */
        .languages-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .language-item {
            background: var(--bg-card);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
        }

        .language-item:hover {
            transform: scale(1.05);
            border-color: var(--accent-color);
        }

        .flag {
            font-size: 3rem;
            margin-bottom: 1rem;
            display: block;
        }

        /* Contact Section */
        .contact-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .contact-item {
            background: var(--bg-card);
            padding: 1.5rem;
            border-radius: 15px;
            text-align: center;
            border: 1px solid var(--border-color);
            transition: all 0.3s ease;
            text-decoration: none;
            color: inherit;
        }

        .contact-item:hover {
            transform: translateY(-5px);
            border-color: var(--accent-color);
            box-shadow: 0 10px 30px rgba(233, 30, 99, 0.2);
        }

        .contact-icon {
            font-size: 2rem;
            margin-bottom: 1rem;
            display: block;
            color: var(--accent-color);
        }

        /* Responsive Design */
        @media (max-width: 768px) {
            .hero-content h1 {
                font-size: 2.5rem;
            }

            nav ul {
                flex-wrap: wrap;
                gap: 1rem;
            }

            .timeline::before {
                left: 30px;
            }

            .timeline-item {
                width: calc(100% - 60px);
                left: 60px !important;
            }

            .timeline-item::before {
                left: -45px !important;
            }

            .tech-icons {
                flex-wrap: wrap;
            }
        }

        /* Scroll animations */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }
    </style>
</head>
<body>
    <!-- Hero Section -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Mouhcine MAHBOUBI</h1>
            <p>Étudiant Ingénieur en Génie Électrique | ENSEM Casablanca</p>
            <p>📍 Settat, Maroc</p>
        </div>
    </section>

    <!-- Formation Section -->
    <section id="formation" class="fade-in">
        <h2 class="section-title">Formation</h2>
        <div class="timeline">
            <div class="timeline-item">
                <div class="timeline-date">2025 - Présent</div>
                <h3>ENSEM - Cycle d'Ingénieur</h3>
                <p><strong>Génie Électrique</strong> - École Nationale Supérieure d'Électricité et de Mécanique</p>
                <p>Formation d'ingénieur spécialisée en génie électrique, couvrant l'électronique de puissance, les systèmes électriques, l'automatique et les énergies renouvelables. Développement de projets concrets et stage en entreprise.</p>
            </div>
            <div class="timeline-item">
                <div class="timeline-date">2023 - 2025</div>
                <h3>Classes Préparatoires aux Grandes Écoles</h3>
                <p><strong>Filière TSI</strong> - Centre Settat</p>
                <p>Formation intensive en mathématiques, physique et sciences de l'ingénieur, préparant aux concours d'entrée des grandes écoles d'ingénieurs.</p>
            </div>
            <div class="timeline-item">
                <div class="timeline-date">2020 - 2023</div>
                <h3>Baccalauréat STE</h3>
                <p><strong>Mention Bien</strong> - Lycée Technique Settat</p>
                <p>Sciences et Technologies Électriques avec spécialisation dans les systèmes électroniques, la maintenance et la conception de circuits électriques.</p>
            </div>
        </div>
    </section>

    <!-- Compétences Section -->
    <section id="competences" class="fade-in">
        <h2 class="section-title">Compétences</h2>
        <div class="skills-grid">
            <div class="skill-category">
                <h3>⚡ Compétences Techniques</h3>
                <div class="skill-item">
                    <span>Conception de circuits électriques</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 80%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Analyse des circuits électriques</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 85%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Systèmes électroniques</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 75%"></div>
                    </div>
                </div>
            </div>

            <div class="skill-category">
                <h3>💻 Outils & Langages</h3>
                <div class="skill-item">
                    <span>Python</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 90%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>PSIM</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 90%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>MATLAB</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 70%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>LaTeX</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 70%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Proteus</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 70%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Langage C</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 50%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Suite Office</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 90%"></div>
                    </div>
                </div>
            </div>

            <div class="skill-category">
                <h3>🤝 Compétences Personnelles</h3>
                <div class="skill-item">
                    <span>Adaptabilité</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 90%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Patience</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 90%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Travail d'équipe</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 80%"></div>
                    </div>
                </div>
                <div class="skill-item">
                    <span>Gestion du temps</span>
                    <div class="skill-level">
                        <div class="skill-progress" style="width: 70%"></div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Langues Section -->
    <section id="langues" class="fade-in">
        <h2 class="section-title">Langues</h2>
        <div class="languages-grid">
            <div class="language-item">
                <span class="flag">🇲🇦</span>
                <h3>Arabe</h3>
                <p>Langue Maternelle</p>
            </div>
            <div class="language-item">
                <span class="flag">🇫🇷</span>
                <h3>Français</h3>
                <p>Niveau 4/6</p>
            </div>
            <div class="language-item">
                <span class="flag">🇬🇧</span>
                <h3>Anglais</h3>
                <p>Niveau 4/6</p>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="fade-in">
        <h2 class="section-title">Contactez-moi</h2>
        <div class="contact-grid">
            <a href="mailto:mahboubi.mhc.etd@gmail.com" class="contact-item">
                <span class="contact-icon">📧</span>
                <h3>Email</h3>
                <p>mahboubi.mhc.etd@gmail.com</p>
            </a>
            <a href="tel:+212650361793" class="contact-item">
                <span class="contact-icon">📱</span>
                <h3>Téléphone</h3>
                <p>+212 650-361793</p>
            </a>
            <a href="https://www.linkedin.com/in/mouhcine-mahboubi-ba6210235" target="_blank" class="contact-item">
                <span class="contact-icon">🔗</span>
                <h3>LinkedIn</h3>
                <p>Mouhcine Mahboubi</p>
            </a>
            <a href="https://www.instagram.com/mhb_b0/" target="_blank" class="contact-item">
                <span class="contact-icon">📷</span>
                <h3>Instagram</h3>
                <p>@mhb_b0</p>
            </a>
            <div class="contact-item">
                <span class="contact-icon">📍</span>
                <h3>Localisation</h3>
                <p>Settat, Maroc</p>
            </div>
        </div>
    </section>

    <script>
        // Smooth scrolling for navigation links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    target.scrollIntoView({
                        behavior: 'smooth',
                        block: 'start'
                    });
                }
            });
        });

        // Intersection Observer for fade-in animations
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver(function(entries) {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                }
            });
        }, observerOptions);

        // Observe all fade-in elements
        document.querySelectorAll('.fade-in').forEach(el => {
            observer.observe(el);
        });

        // Active navigation highlighting
        window.addEventListener('scroll', () => {
            const sections = document.querySelectorAll('section[id]');
            const navLinks = document.querySelectorAll('nav a[href^="#"]');
            
            let current = '';
            sections.forEach(section => {
                const sectionTop = section.offsetTop - 100;
                const sectionHeight = section.offsetHeight;
                
                if (window.scrollY >= sectionTop && window.scrollY < sectionTop + sectionHeight) {
                    current = section.getAttribute('id');
                }
            });

            navLinks.forEach(link => {
                link.style.color = '';
                link.style.background = '';
                if (link.getAttribute('href').slice(1) === current) {
                    link.style.color = '#ff4081';
                    link.style.background = 'rgba(233, 30, 99, 0.1)';
                }
            });
        });

        // Animate skill progress bars when in view
        const skillObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    const progressBars = entry.target.querySelectorAll('.skill-progress');
                    progressBars.forEach(bar => {
                        bar.style.animation = 'none';
                        bar.offsetHeight; // Trigger reflow
                        bar.style.animation = 'progressFill 2s ease-out';
                    });
                }
            });
        }, { threshold: 0.5 });

        document.querySelectorAll('.skill-category').forEach(category => {
            skillObserver.observe(category);
        });

        // Add hover effects for tech icons
        document.querySelectorAll('.tech-icon').forEach(icon => {
            icon.addEventListener('mouseenter', function() {
                this.style.transform = 'scale(1.2) rotate(10deg)';
            });
            
            icon.addEventListener('mouseleave', function() {
                this.style.transform = 'scale(1) rotate(0deg)';
            });
        });

        // Parallax effect for hero section
        window.addEventListener('scroll', () => {
            const hero = document.querySelector('.hero');
            const scrolled = window.pageYOffset;
            hero.style.transform = `translateY(${scrolled * 0.5}px)`;
        });
    </script>
</body>
</html>
