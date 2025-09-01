[index.html](https://github.com/user-attachments/files/22084970/index.html)
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Inteligencia Artificial Generativa - El Futuro Digital</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css" rel="stylesheet">
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700;900&family=Exo+2:wght@300;400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-cyan: #00d4ff;
            --secondary-cyan: #00a8cc;
            --dark-blue: #0a1628;
            --darker-blue: #051018;
            --accent-purple: #6c5ce7;
            --text-light: #e8f4f8;
            --text-muted: #a0b4b7;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Exo 2', sans-serif;
            background: linear-gradient(135deg, var(--darker-blue) 0%, var(--dark-blue) 100%);
            color: var(--text-light);
            overflow-x: hidden;
        }

        /* Efectos de partículas animadas */
        .particles {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            pointer-events: none;
            z-index: 1;
        }

        .particle {
            position: absolute;
            width: 2px;
            height: 2px;
            background: var(--primary-cyan);
            border-radius: 50%;
            animation: float 6s infinite linear;
            opacity: 0.6;
        }

        @keyframes float {
            0% { transform: translateY(100vh) translateX(0px); opacity: 0; }
            10% { opacity: 0.6; }
            90% { opacity: 0.6; }
            100% { transform: translateY(-100px) translateX(100px); opacity: 0; }
        }

        /* Navegación futurista */
        .navbar-custom {
            background: rgba(10, 22, 40, 0.95);
            backdrop-filter: blur(10px);
            border-bottom: 1px solid var(--primary-cyan);
            padding: 1rem 0;
        }

        .navbar-brand {
            font-family: 'Orbitron', monospace;
            font-weight: 900;
            font-size: 1.5rem;
            color: var(--primary-cyan) !important;
            text-shadow: 0 0 10px var(--primary-cyan);
        }

        .nav-link {
            color: var(--text-light) !important;
            font-weight: 600;
            position: relative;
            transition: all 0.3s ease;
        }

        .nav-link:hover {
            color: var(--primary-cyan) !important;
            text-shadow: 0 0 5px var(--primary-cyan);
        }

        .nav-link::after {
            content: '';
            position: absolute;
            bottom: -5px;
            left: 0;
            width: 0;
            height: 2px;
            background: var(--primary-cyan);
            transition: width 0.3s ease;
        }

        .nav-link:hover::after {
            width: 100%;
        }

        /* Hero Section con imagen de fondo */
        .hero-section {
            min-height: 100vh;
            background: linear-gradient(rgba(10, 22, 40, 0.7), rgba(5, 16, 24, 0.8)), url('https://hebbkx1anhila5yf.public.blob.vercel-storage.com/ChatGPT%20Image%201%20sept%202025%2C%2006_39_43%20p.m.-QNbrU0wIriJlIQVZxMDEJoHPFtdwi9.png');
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            display: flex;
            align-items: center;
            position: relative;
            z-index: 2;
        }

        .hero-content {
            text-align: center;
            z-index: 3;
        }

        .hero-title {
            font-family: 'Orbitron', monospace;
            font-size: 4rem;
            font-weight: 900;
            background: linear-gradient(45deg, var(--primary-cyan), var(--accent-purple));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            background-clip: text;
            margin-bottom: 2rem;
            text-shadow: 0 0 30px rgba(0, 212, 255, 0.5);
            animation: glow 2s ease-in-out infinite alternate;
        }

        @keyframes glow {
            from { filter: drop-shadow(0 0 20px var(--primary-cyan)); }
            to { filter: drop-shadow(0 0 30px var(--accent-purple)); }
        }

        .hero-subtitle {
            font-size: 1.5rem;
            color: var(--text-muted);
            margin-bottom: 3rem;
            font-weight: 300;
        }

        /* Botones futuristas */
        .btn-futuristic {
            background: linear-gradient(45deg, var(--primary-cyan), var(--secondary-cyan));
            border: none;
            color: var(--darker-blue);
            font-weight: 700;
            padding: 15px 40px;
            border-radius: 50px;
            text-transform: uppercase;
            letter-spacing: 1px;
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
            box-shadow: 0 0 20px rgba(0, 212, 255, 0.3);
        }

        .btn-futuristic:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(0, 212, 255, 0.5);
            color: var(--darker-blue);
        }

        .btn-futuristic::before {
            content: '';
            position: absolute;
            top: 0;
            left: -100%;
            width: 100%;
            height: 100%;
            background: linear-gradient(90deg, transparent, rgba(255,255,255,0.3), transparent);
            transition: left 0.5s;
        }

        .btn-futuristic:hover::before {
            left: 100%;
        }

        /* Secciones con diseño único */
        .section-custom {
            padding: 100px 0;
            position: relative;
            z-index: 2;
        }

        .section-title {
            font-family: 'Orbitron', monospace;
            font-size: 3rem;
            font-weight: 700;
            text-align: center;
            margin-bottom: 4rem;
            color: var(--primary-cyan);
            position: relative;
        }

        .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(45deg, var(--primary-cyan), var(--accent-purple));
            border-radius: 2px;
        }

        /* Cards futuristas */
        .card-futuristic {
            background: rgba(10, 22, 40, 0.8);
            border: 1px solid var(--primary-cyan);
            border-radius: 20px;
            padding: 2rem;
            margin-bottom: 2rem;
            position: relative;
            overflow: hidden;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
        }

        .card-futuristic:hover {
            transform: translateY(-10px);
            box-shadow: 0 20px 40px rgba(0, 212, 255, 0.2);
            border-color: var(--accent-purple);
        }

        .card-futuristic::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 2px;
            background: linear-gradient(90deg, var(--primary-cyan), var(--accent-purple));
        }

        .card-icon {
            font-size: 3rem;
            color: var(--primary-cyan);
            margin-bottom: 1rem;
            text-shadow: 0 0 10px var(--primary-cyan);
        }

        .card-title {
            font-family: 'Orbitron', monospace;
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-cyan);
            margin-bottom: 1rem;
        }

        .card-text {
            color: var(--text-muted);
            line-height: 1.6;
        }

        /* Timeline futurista */
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
            background: linear-gradient(to bottom, var(--primary-cyan), var(--accent-purple));
            transform: translateX(-50%);
        }

        .timeline-item {
            position: relative;
            margin: 3rem 0;
            width: 45%;
        }

        .timeline-item:nth-child(odd) {
            left: 0;
            text-align: right;
        }

        .timeline-item:nth-child(even) {
            left: 55%;
            text-align: left;
        }

        .timeline-content {
            background: rgba(10, 22, 40, 0.9);
            border: 1px solid var(--primary-cyan);
            border-radius: 15px;
            padding: 2rem;
            position: relative;
        }

        .timeline-year {
            font-family: 'Orbitron', monospace;
            font-size: 2rem;
            font-weight: 900;
            color: var(--primary-cyan);
            margin-bottom: 1rem;
        }

        .timeline-dot {
            position: absolute;
            top: 50%;
            width: 20px;
            height: 20px;
            background: var(--primary-cyan);
            border-radius: 50%;
            transform: translateY(-50%);
            box-shadow: 0 0 20px var(--primary-cyan);
        }

        .timeline-item:nth-child(odd) .timeline-dot {
            right: -60px;
        }

        .timeline-item:nth-child(even) .timeline-dot {
            left: -60px;
        }

        /* Footer futurista */
        .footer-custom {
            background: var(--darker-blue);
            border-top: 1px solid var(--primary-cyan);
            padding: 3rem 0;
            text-align: center;
        }

        .footer-text {
            color: var(--text-muted);
            font-size: 0.9rem;
        }

        /* Efectos de scroll */
        .fade-in {
            opacity: 0;
            transform: translateY(30px);
            transition: all 0.6s ease;
        }

        .fade-in.visible {
            opacity: 1;
            transform: translateY(0);
        }

        /* Responsive */
        @media (max-width: 768px) {
            .hero-title {
                font-size: 2.5rem;
            }
            
            .section-title {
                font-size: 2rem;
            }
            
            .timeline::before {
                left: 20px;
            }
            
            .timeline-item {
                width: calc(100% - 40px);
                left: 40px !important;
                text-align: left !important;
            }
            
            .timeline-dot {
                left: -30px !important;
            }
        }
    </style>
</head>
<body>
    <!-- Partículas animadas -->
    <div class="particles" id="particles"></div>

    <!-- Navegación -->
    <nav class="navbar navbar-expand-lg navbar-custom fixed-top">
        <div class="container">
            <a class="navbar-brand" href="#home">
                <i class="fas fa-brain me-2"></i>IA GENERATIVA
            </a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#home">Inicio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#definicion">Definición</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#usos">Usos Cotidianos</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#futuro">Futuro</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- Hero Section -->
    <section id="home" class="hero-section">
        <div class="container">
            <div class="row justify-content-center">
                <div class="col-lg-10">
                    <div class="hero-content">
                        <h1 class="hero-title">INTELIGENCIA ARTIFICIAL GENERATIVA</h1>
                        <p class="hero-subtitle">Explorando el futuro de la creatividad digital y la innovación tecnológica</p>
                        <a href="#definicion" class="btn btn-futuristic me-3">
                            <i class="fas fa-rocket me-2"></i>Explorar
                        </a>
                        <a href="#futuro" class="btn btn-outline-light">
                            <i class="fas fa-eye me-2"></i>Ver Futuro
                        </a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Definición -->
    <section id="definicion" class="section-custom">
        <div class="container">
            <h2 class="section-title fade-in">¿Qué es la IA Generativa?</h2>
            <div class="row">
                <div class="col-lg-8 mx-auto">
                    <div class="card-futuristic fade-in">
                        <div class="text-center">
                            <i class="fas fa-brain card-icon"></i>
                            <h3 class="card-title">Definición Fundamental</h3>
                            <p class="card-text">
                                La Inteligencia Artificial Generativa es una rama revolucionaria de la IA que utiliza algoritmos avanzados 
                                para crear contenido nuevo y original. A diferencia de los sistemas tradicionales que solo analizan datos, 
                                la IA generativa puede producir texto, imágenes, música, código y otros tipos de contenido que antes 
                                requerían creatividad humana.
                            </p>
                        </div>
                    </div>
                </div>
            </div>
            <div class="row mt-5">
                <div class="col-md-4">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-cogs card-icon"></i>
                        <h4 class="card-title">Tecnología Base</h4>
                        <p class="card-text">
                            Utiliza redes neuronales profundas, transformers y modelos de difusión para aprender patrones 
                            complejos de grandes conjuntos de datos.
                        </p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-lightbulb card-icon"></i>
                        <h4 class="card-title">Capacidades</h4>
                        <p class="card-text">
                            Genera contenido original, traduce idiomas, crea arte digital, compone música y desarrolla código 
                            de programación de forma autónoma.
                        </p>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-infinity card-icon"></i>
                        <h4 class="card-title">Potencial</h4>
                        <p class="card-text">
                            Revoluciona industrias enteras al democratizar la creación de contenido y acelerar procesos 
                            creativos e innovadores.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Usos Cotidianos -->
    <section id="usos" class="section-custom" style="background: rgba(5, 16, 24, 0.5);">
        <div class="container">
            <h2 class="section-title fade-in">Usos en la Vida Cotidiana</h2>
            <div class="row">
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-pen-fancy card-icon"></i>
                        <h4 class="card-title">Creación de Contenido</h4>
                        <p class="card-text">
                            Generación automática de artículos, blogs, guiones publicitarios y contenido para redes sociales. 
                            Herramientas como ChatGPT y Jasper AI ayudan a escritores y marketers a crear contenido de calidad 
                            en minutos.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-palette card-icon"></i>
                        <h4 class="card-title">Arte y Diseño</h4>
                        <p class="card-text">
                            Creación de imágenes, ilustraciones y diseños únicos mediante DALL-E, Midjourney y Stable Diffusion. 
                            Democratiza el arte digital permitiendo a cualquier persona crear obras visuales impresionantes.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-code card-icon"></i>
                        <h4 class="card-title">Programación</h4>
                        <p class="card-text">
                            GitHub Copilot y CodeT5 asisten a desarrolladores generando código, depurando errores y 
                            sugiriendo optimizaciones. Acelera el desarrollo de software y reduce errores comunes.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-graduation-cap card-icon"></i>
                        <h4 class="card-title">Educación</h4>
                        <p class="card-text">
                            Tutores virtuales personalizados, generación de material educativo adaptado y explicaciones 
                            simplificadas de conceptos complejos. Revoluciona el aprendizaje personalizado.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-music card-icon"></i>
                        <h4 class="card-title">Música y Audio</h4>
                        <p class="card-text">
                            Composición automática de melodías, generación de efectos sonoros y creación de podcasts 
                            sintéticos. AIVA y Amper Music permiten crear bandas sonoras profesionales.
                        </p>
                    </div>
                </div>
                <div class="col-lg-6">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-comments card-icon"></i>
                        <h4 class="card-title">Comunicación</h4>
                        <p class="card-text">
                            Chatbots inteligentes, traducción instantánea y asistentes virtuales que comprenden contexto 
                            y emociones. Mejora la comunicación global y la atención al cliente.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Sección Futuro -->
    <section id="futuro" class="section-custom">
        <div class="container">
            <h2 class="section-title fade-in">El Futuro de la IA Generativa</h2>
            <div class="timeline">
                <div class="timeline-item fade-in">
                    <div class="timeline-content">
                        <div class="timeline-year">2024-2025</div>
                        <h4 class="card-title">Integración Masiva</h4>
                        <p class="card-text">
                            Adopción generalizada en empresas, integración en herramientas cotidianas y mejora 
                            significativa en la calidad de contenido generado.
                        </p>
                    </div>
                    <div class="timeline-dot"></div>
                </div>
                
                <div class="timeline-item fade-in">
                    <div class="timeline-content">
                        <div class="timeline-year">2026-2028</div>
                        <h4 class="card-title">IA Multimodal Avanzada</h4>
                        <p class="card-text">
                            Sistemas que combinan texto, imagen, audio y video de forma seamless. Creación de 
                            experiencias inmersivas y contenido multimedia complejo.
                        </p>
                    </div>
                    <div class="timeline-dot"></div>
                </div>
                
                <div class="timeline-item fade-in">
                    <div class="timeline-content">
                        <div class="timeline-year">2029-2032</div>
                        <h4 class="card-title">Creatividad Colaborativa</h4>
                        <p class="card-text">
                            IA como co-creadora en proyectos artísticos, científicos y tecnológicos. Desarrollo 
                            de nuevas formas de arte y expresión humano-máquina.
                        </p>
                    </div>
                    <div class="timeline-dot"></div>
                </div>
                
                <div class="timeline-item fade-in">
                    <div class="timeline-content">
                        <div class="timeline-year">2033+</div>
                        <h4 class="card-title">Inteligencia Artificial General</h4>
                        <p class="card-text">
                            Sistemas de IA con capacidades cognitivas equiparables a las humanas, capaces de 
                            innovar, crear y resolver problemas complejos de forma autónoma.
                        </p>
                    </div>
                    <div class="timeline-dot"></div>
                </div>
            </div>
            
            <div class="row mt-5">
                <div class="col-lg-8 mx-auto text-center">
                    <div class="card-futuristic fade-in">
                        <i class="fas fa-rocket card-icon"></i>
                        <h3 class="card-title">Impacto Transformador</h3>
                        <p class="card-text">
                            La IA Generativa no solo cambiará cómo trabajamos y creamos, sino que redefinirá 
                            conceptos fundamentales sobre creatividad, originalidad y colaboración humano-máquina. 
                            Estamos al borde de una nueva era donde la imaginación será el único límite para la 
                            innovación tecnológica.
                        </p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="footer-custom">
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <p class="footer-text">
                        © 2024 IA Generativa - Explorando el Futuro Digital | 
                        <i class="fas fa-brain text-primary"></i> Powered by Innovation
                    </p>
                </div>
            </div>
        </div>
    </footer>

    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
    <script>
        // Crear partículas animadas
        function createParticles() {
            const particlesContainer = document.getElementById('particles');
            const particleCount = 50;
            
            for (let i = 0; i < particleCount; i++) {
                const particle = document.createElement('div');
                particle.className = 'particle';
                particle.style.left = Math.random() * 100 + '%';
                particle.style.animationDelay = Math.random() * 6 + 's';
                particle.style.animationDuration = (Math.random() * 3 + 3) + 's';
                particlesContainer.appendChild(particle);
            }
        }

        // Animaciones de scroll
        function handleScrollAnimations() {
            const elements = document.querySelectorAll('.fade-in');
            
            elements.forEach(element => {
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 150;
                
                if (elementTop < window.innerHeight - elementVisible) {
                    element.classList.add('visible');
                }
            });
        }

        // Smooth scrolling para navegación
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

        // Inicializar efectos
        document.addEventListener('DOMContentLoaded', function() {
            createParticles();
            handleScrollAnimations();
        });

        // Escuchar scroll para animaciones
        window.addEventListener('scroll', handleScrollAnimations);

        // Efecto parallax para hero section
        window.addEventListener('scroll', function() {
            const scrolled = window.pageYOffset;
            const hero = document.querySelector('.hero-section');
            if (hero) {
                hero.style.transform = `translateY(${scrolled * 0.5}px)`;
            }
        });
    </script>
</body>
</html>
