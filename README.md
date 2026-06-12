<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Investigación CETis 20 | Rendimiento Escolar y Prevención</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
        /* --- ESTILOS GLOBALES Y PALETA (Rosa, Lila, Blanco) --- */
        :root {--rosa-principal:#ff6b8b;
            --rosa-claro: #ffeef2;
            --lila-principal: #8a70d6;
            --lila-oscuro: #5b45a0;
            --lila-suave: #f3f0ff;
            --blanco: #ffffff;
            --gris-oscuro: #2d2d2d;
            --gris-texto: #555555;
        --sombra: rgba(138, 112, 214,0.15);
            -transition: all 0.3s ease;}*{margin: 0;
  padding: 0;box-sizing: border-box;
            scroll-behavior:smooth;}body{font-family: 'Poppins', sans-serif; background-color:#faf9ff;
            color: var(--gris-oscuro);
            line-height: 1.6;
        }/* --- ENCABEZADO Y MENÚ FIJO --- */header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background: rgba(255, 255, 255, 0.95);
            box-shadow: 0 4px 20px var(--sombra);
            z-index: 1000;
            backdrop-filter: blur(10px);
        }
.nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 15px 20px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }.logo-area {
            display: flex;
            flex-direction: column;
        }.logo-area h1 {
            font-size: 1.1rem;
            color: var(--lila-oscuro);
            font-weight: 700;
        }
.logo-area span {
            font-size: 0.75rem;
            color: var(--rosa-principal);
            font-weight: 600;
            letter-spacing: 1px;
        }

     .nav-menu {
            display: flex;
            list-style: none;
            gap: 20px;
        }

    .nav-menu a {
            text-decoration: none;
            color: var(--gris-texto);
            font-weight: 600;
            font-size: 0.9rem;
            transition: var(--transition);
            padding: 8px 12px;
            border-radius: 20px;
        }

    .nav-menu a:hover, .nav-menu a.active {
            color: var(--rosa-principal);
            background: var(--rosa-claro);
        }

     .menu-toggle {
            display: none;
            font-size: 1.5rem;
            color: var(--lila-principal);
            cursor: pointer;
        }
        /* --- PORTADA PRINCIPAL --- */
        .hero {
            margin-top: 70px;
            min-height: calc(85vh - 70px);
            background: linear-gradient(135deg, var(--rosa-claro) 0%, var(--lila-suave) 100%);
            display: flex;
            align-items: center;
            padding: 40px 20px;
            position: relative;
            overflow: hidden;
        }

    .hero::before {
            content: '';
            position: absolute;
            width: 300px;
            height: 300px;
            background: rgba(255, 107, 139, 0.1);
            border-radius: 50%;
            top: -50px;
            right: -50px;
        }

    .hero-container {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

   .hero-text h2 {
            font-size: 2.3rem;
            color: var(--lila-oscuro);
            line-height: 1.3;
            margin-bottom: 20px;
        }

   .hero-text p {
            font-size: 1.1rem;
            color: var(--gris-texto);
            margin-bottom: 30px;
            border-left: 4px solid var(--rosa-principal);
            padding-left: 15px;
            font-style: italic;
        }

    .cta-btn {
            display: inline-block;
            padding: 12px 30px;
            background: linear-gradient(45deg, var(--rosa-principal), var(--lila-principal));
            color: var(--blanco);
            text-decoration: none;
            font-weight: 600;
            border-radius: 30px;
            box-shadow: 0 4px 15px rgba(255, 107, 139, 0.4);
            transition: var(--transition);
        }

    .cta-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 6px 20px rgba(138, 70, 214, 0.4);
        }

    .hero-img {
            display: flex;
            justify-content: center;
        }

    .hero-img svg {
            width: 100%;
            max-width: 450px;
            filter: drop-shadow(0 10px 15px var(--sombra));
            animation: float 4s ease-in-out infinite;
        } @keyframes float {
            0%, 100% { transform: translateY(0); }
            50% { transform: translateY(-15px); }
        }  /* --- SECCIONES COMUNES --- */
        section {
            padding: 80px 20px;
            max-width: 1200px;
            margin: 0 auto;
        }

    .section-title {
            text-align: center;
            font-size: 2rem;
            color: var(--lila-oscuro);
            margin-bottom: 50px;
            position: relative;
        }

    .section-title::after {
            content: '';
            position: absolute;
            bottom: -10px;
            left: 50%;
            transform: translateX(-50%);
            width: 60px;
            height: 4px;
            background: var(--rosa-principal);
            border-radius: 2px;
        }

     /* --- INTRODUCCIÓN Y PROBLEMA --- */
        .intro-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            background: var(--blanco);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 30px var(--sombra);
        }

    .intro-box h3, .problem-box h3 {
            color: var(--rosa-principal);
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        /* --- OBJETIVOS --- */
        .objectives-container {
            background: linear-gradient(135deg, var(--lila-principal), var(--lila-oscuro));
            color: var(--blanco);
            padding: 50px 40px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(91, 69, 160, 0.3);
        }

        .general-obj {
            text-align: center;
            margin-bottom: 40px;
            padding-bottom: 30px;
            border-bottom: 1px solid rgba(255,255,255,0.2);
        }

        .general-obj h3 {
            font-size: 1.5rem;
            margin-bottom: 15px;
        }

        .specific-objs h3 {
            text-align: center;
            margin-bottom: 25px;
        }

        .specific-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 20px;
        }

        .spec-card {
            background: rgba(255, 255, 255, 0.1);
            padding: 25px;
            border-radius: 15px;
            backdrop-filter: blur(5px);
            border: 1px solid rgba(255,255,255,0.1);
            transition: var(--transition);
        }

        .spec-card:hover {
            transform: translateY(-5px);
            background: rgba(255, 255, 255, 0.18);
        }

        .spec-card i {
            font-size: 1.5rem;
            color: var(--rosa-principal);
            margin-bottom: 15px;
        }

        /* --- MARCO TEÓRICO Y TARJETAS --- */
        .cards-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }

        .card {
            background: var(--blanco);
            border-radius: 20px;
            padding: 35px 25px;
            box-shadow: 0 10px 25px var(--sombra);
            transition: var(--transition);
            border: 1px solid transparent;
            text-align: center;
        }

        .card:hover {
            transform: translateY(-10px);
            border-color: var(--rosa-principal);
            box-shadow: 0 15px 35px rgba(255, 107, 139, 0.15);
        }

        .card-icon {
            width: 70px;
            height: 70px;
            background: var(--lila-suave);
            color: var(--lila-principal);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.8rem;
            margin: 0 auto 20px;
            transition: var(--transition);
        }

        .card:hover .card-icon {
            background: var(--rosa-principal);
            color: var(--blanco);
        }

        .card h3 {
            color: var(--lila-oscuro);
            margin-bottom: 15px;
        }

        /* --- INDICADORES VISUALES / RESULTADOS ESPERADOS --- */
        .results-section {
            background: var(--blanco);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 10px 30px var(--sombra);
        }

        .results-dashboard {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
            align-items: center;
        }

        .metrics-grid {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 20px;
        }

        .metric-box {
            background: var(--lila-suave);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            border-top: 4px solid var(--lila-principal);
        }

        .metric-box .number {
            font-size: 2.2rem;
            font-weight: 700;
            color: var(--lila-oscuro);
            margin-bottom: 5px;
        }

        .chart-box {
            background: #fff;
            border: 1px solid #eee;
            padding: 25px;
            border-radius: 15px;
            box-shadow: inset 0 2px 10px rgba(0,0,0,0.02);
        }

        .chart-title {
            font-weight: 600;
            font-size: 0.95rem;
            margin-bottom: 20px;
            color: var(--gris-texto);
            text-align: center;
        }

        .bar-container {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .bar-row {
            display: flex;
            align-items: center;
            gap: 15px;
        }

        .bar-label {
            width: 100px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .bar-track {
            flex-grow: 1;
            height: 15px;
            background: #f0f0f0;
            border-radius: 10px;
            overflow: hidden;
        }

        .bar-fill {
            height: 100%;
            background: linear-gradient(90deg, var(--lila-principal), var(--rosa-principal));
            border-radius: 10px;
            width: 0%; 
            transition: width 1.5s cubic-bezier(0.1, 1, 0.1, 1);
        }

        .bar-pct {
            font-size: 0.8rem;
            font-weight: 700;
            width: 35px;
            color: var(--rosa-principal);
        }

        /* --- CONSECUENCIAS Y CONCLUSIONES --- */
        .consequences-layout {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 40px;
        }

        .consequences-list {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .consequence-item {
            background: var(--blanco);
            padding: 20px;
            border-radius: 15px;
            box-shadow: 0 4px 15px var(--sombra);
            display: flex;
            gap: 15px;
            align-items: flex-start;
            border-left: 5px solid var(--rosa-principal);
            transition: var(--transition);
        }

        .consequence-item:hover {
            transform: scale(1.02);
        }

        .consequence-item i {
            font-size: 1.3rem;
            color: var(--rosa-principal);
            background: var(--rosa-claro);
            padding: 10px;
            border-radius: 10px;
        }

        .conclusion-box {
            background: linear-gradient(135deg, var(--rosa-claro) 0%, var(--lila-suave) 100%);
            padding: 40px;
            border-radius: 20px;
            border: 2px dashed var(--lila-principal);
        }

        .conclusion-box h3 {
            color: var(--lila-oscuro);
            margin-bottom: 15px;
        }

        /* --- BIBLIOGRAFÍA --- */
        .biblio-box {
            background: var(--blanco);
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 5px 20px var(--sombra);
        }

        .biblio-list {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 15px;
        }

        .biblio-list li {
            padding-left: 30px;
            position: relative;
            font-size: 0.95rem;
            color: var(--gris-texto);
        }

        .biblio-list li::before {
            content: "\f02d";
            font-family: "Font Awesome 6 Free";
            font-weight: 900;
            position: absolute;
            left: 0;
            top: 2px;
            color: var(--lila-principal);
        }

        /* --- PIE DE PÁGINA --- */
        footer {
            background: var(--lila-oscuro);
            color: var(--blanco);
            padding: 40px 20px 20px;
            margin-top: 60px;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            display: grid;
            grid-template-columns: 2fr 1fr;
            gap: 40px;
            padding-bottom: 30px;
            border-bottom: 1px solid rgba(255,255,255,0.1);
        }

        .footer-about h4 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: var(--rosa-principal);
        }

        .footer-links h4 {
            margin-bottom: 15px;
        }

        .footer-links ul {
            list-style: none;
            display: flex;
            flex-direction: column;
            gap: 10px;
        }

        .footer-links a {
            color: rgba(255,255,255,0.7);
            text-decoration: none;
            transition: var(--transition);
        }

        .footer-links a:hover {
            color: var(--rosa-principal);
            padding-left: 5px;
        }

        .footer-bottom {
            text-align: center;
            padding-top: 20px;
            font-size: 0.85rem;
            color: rgba(255,255,255,0.5);
        }

        /* --- RESPONSIVE / ADAPTABILIDAD --- */
        @media (max-width: 992px) {
            .hero-container, .intro-grid, .results-dashboard, .consequences-layout {
                grid-template-columns: 1fr;
            }
            
            .hero-img {
                order: -1;
            }

            .hero-text {
                text-align: center;
            }

            .hero-text p {
                border-left: none;
                border-bottom: 3px solid var(--rosa-principal);
                padding-left: 0;
                padding-bottom: 15px;
            }
        }

        @media (max-width: 768px) {
            .nav-menu {
                display: none;
                position: absolute;
                top: 100%;
                left: 0;
                width: 100%;
                background: var(--blanco);
                flex-direction: column;
                padding: 20px;
                box-shadow: 0 10px 20px var(--sombra);
                gap: 15px;
                text-align: center;
            }

            .nav-menu.active {
                display: flex;
            }

            .menu-toggle {
                display: block;
            }

            .section-title {
                font-size: 1.6rem;
            }

            .footer-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="nav-container">
            <div class="logo-area">
                <h1>CETis No. 20</h1>
                <span>PROYECTO DE INVESTIGACIÓN</span>
            </div>
            <div class="menu-toggle" id="mobile-menu">
                <i class="fas fa-bars"></i>
            </div>
            <ul class="nav-menu" id="nav-list">
                <li><a href="#inicio" class="active">Inicio</a></li>
                <li><a href="#planteamiento">Problema</a></li>
                <li><a href="#objetivos">Objetivos</a></li>
                <li><a href="#marco-teorico">Marco Teórico</a></li>
                <li><a href="#resultados">Resultados</a></li>
                <li><a href="#consecuencias">Consecuencias</a></li>
            </ul>
        </div>
    </header>

    <section class="hero" id="inicio">
        <div class="hero-container">
            <div class="hero-text">
                <h2>¿Cómo influye el uso de las drogas en el rendimiento escolar?</h2>
                <p>"La educación y la prevención son las herramientas más poderosas para construir un futuro académico brillante y libre de adicciones."</p>
                <p style="font-size:0.9rem; font-style:normal; border:none; color:var(--lila-oscuro); font-weight:600;">
                    Estudio enfocado en alumnos de segundo semestre de preparatoria del CETis 20 <br>Ciclo Escolar 2025-2026
                </p>
                <a href="#planteamiento" class="cta-btn">Explorar Investigación</a>
            </div>
            <div class="hero-img">
                <svg viewBox="0 0 500 400" xmlns="http://www.w3.org/2000/svg">
                    <circle cx="250" cy="200" r="180" fill="#f3f0ff"/>
                    <rect x="120" y="280" width="260" height="40" rx="10" fill="#8a70d6"/>
                    <path d="M180,280 L180,160 L320,160 L320,280 Z" fill="#ff6b8b" opacity="0.8"/>
                    <polygon points="250,80 150,140 350,140" fill="#5b45a0"/>
                    <rect x="235" y="140" width="30" height="140" fill="#ffffff" opacity="0.3"/>
                    <circle cx="250" cy="210" r="40" fill="#ffffff"/>
                    <path d="M235,210 L250,225 L270,195" stroke="#8a70d6" stroke-width="6" stroke-linecap="round" stroke-linejoin="round" fill="none"/>
                </svg>
            </div>
        </div>
    </section<section id="planteamiento"> <h2 class="section-title">Planteamiento del Proyecto</h2>
        <div class="intro-grid">
  <div class="intro-box"><h3><i class="fas fa-book-open"></i> Introducción</h3><p>El presente proyecto de investigación analiza la correlación directa entre el consumo de sustancias psicoactivas y el desempeño escolar. Centrado en una etapa crítica del desarrollo humano, este estudio busca visibilizar los desafíos internos y externos que afrontan los jóvenes del nivel medio superior.</p></div>
 <div class="problem-box">
  <h3><i class="fas fa-exclamation-triangle"></i> Problema de Investigación</h3><p>Durante el ciclo escolar 2025-2026, se ha observado una inquietante fluctuación en las calificaciones y permanencia de los alumnos de <strong>segundo semestre del CETis 20</strong>. El problema radica en identificar el impacto real del consumo temprano de estupefacientes en la deserción escolar, la pérdida de motivación cognitiva y el qu
