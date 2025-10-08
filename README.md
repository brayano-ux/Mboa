<html lang="fr" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="Brayano - Développeur Full-Stack et Expert IA. Solutions digitales sur mesure pour votre entreprise.">
    <meta name="keywords" content="développeur full-stack, expert IA, développement web, applications mobiles, Cameroun, Douala">
    <meta name="author" content="Brayano">
    <meta property="og:title" content="Brayano - Développeur Full-Stack & Expert IA">
    <meta property="og:description" content="Solutions digitales sur mesure pour votre entreprise.">
    <meta property="og:type" content="website">
    <meta property="og:url" content="https://brayano.dev">
    <meta property="og:image" content="https://brayano.dev/og-image.jpg">
    <title>Brayano - Développeur Full-Stack & Expert IA</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css"/>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <script>
      tailwind.config = {
        darkMode: 'class',
        theme: {
          extend: {
            fontFamily: {
              sans: ['Inter', 'sans-serif'],
            },
            colors: {
              'primary': {
                50: '#eff6ff',
                500: '#3b82f6',
                600: '#2563eb',
                700: '#1d4ed8',
                900: '#1e3a8a'
              },
              'gray': {
                50: '#f9fafb',
                100: '#f3f4f6',
                200: '#e5e7eb',
                800: '#1f2937',
                900: '#111827',
                950: '#0c0e16'
              }
            },
            animation: {
              'fade-in-up': 'fadeInUp 0.8s ease-out',
              'fade-in': 'fadeIn 0.6s ease-out',
              'pulse-slow': 'pulse 3s infinite',
              'float': 'float 6s ease-in-out infinite',
            },
            keyframes: {
              fadeInUp: {
                '0%': { opacity: '0', transform: 'translateY(30px)' },
                '100%': { opacity: '1', transform: 'translateY(0)' }
              },
              fadeIn: {
                '0%': { opacity: '0' },
                '100%': { opacity: '1' }
              },
              float: {
                '0%, 100%': { transform: 'translateY(0px)' },
                '50%': { transform: 'translateY(-10px)' }
              }
            }
          }
        }
      }
    </script>
    <style>
      :root {
        --bg-primary: #ffffff;
        --bg-secondary: #f9fafb;
        --text-primary: #111827;
        --text-secondary: #6b7280;
        --border-color: #e5e7eb;
      }

      .dark {
        --bg-primary: #111827;
        --bg-secondary: #1f2937;
        --text-primary: #f9fafb;
        --text-secondary: #d1d5db;
        --border-color: #374151;
      }

      body {
        background-color: var(--bg-primary);
        color: var(--text-primary);
        transition: background-color 0.3s ease, color 0.3s ease;
      }

      .reveal {
        opacity: 0;
        transform: translateY(50px);
        transition: all 0.8s cubic-bezier(0.25, 0.46, 0.45, 0.94);
      }
      .reveal.active {
        opacity: 1;
        transform: translateY(0);
      }
      .gradient-text {
        background: linear-gradient(135deg, #3b82f6, #8b5cf6);
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
        background-clip: text;
      }
      .card-glow {
        box-shadow: 0 0 20px rgba(59, 130, 246, 0.1);
        transition: all 0.3s ease;
        background-color: var(--bg-secondary);
        border: 1px solid var(--border-color);
      }
      .card-glow:hover {
        box-shadow: 0 0 30px rgba(59, 130, 246, 0.2);
        transform: translateY(-5px);
      }
      .glass-effect {
        background: rgba(255, 255, 255, 0.05);
        backdrop-filter: blur(10px);
        border: 1px solid rgba(255, 255, 255, 0.1);
      }
      
      /* Améliorations pour le responsive et la gestion des z-index */
      body {
        overflow-x: hidden;
        position: relative;
      }
      
      /* Correction des problèmes de z-index */
      header {
        z-index: 100;
      }
      
      .hero-bg {
        z-index: 1;
      }
      
      .hero-content {
        z-index: 2;
        position: relative;
      }
      
      #back-to-top {
        z-index: 90;
      }
      
      /* Améliorations pour le responsive */
      @media (max-width: 768px) {
        .hero-title {
          font-size: 2.5rem;
        }
        
        .hero-subtitle {
          font-size: 1.25rem;
        }
        
        .section-padding {
          padding-top: 4rem;
          padding-bottom: 4rem;
        }
        
        .mobile-menu-open {
          max-height: 500px;
          transition: max-height 0.3s ease-in-out;
        }
      }
      
      /* Animation améliorée pour le menu mobile */
      .mobile-menu {
        max-height: 0;
        overflow: hidden;
        transition: max-height 0.3s ease-in-out;
      }
      
      .mobile-menu.open {
        max-height: 500px;
      }
      
      /* Amélioration de la lisibilité */
      .text-shadow {
        text-shadow: 0 2px 4px rgba(0, 0, 0, 0.5);
      }
      
      /* Amélioration des cartes de projet */
      .project-card {
        transition: all 0.3s ease;
      }
      
      .project-card:hover .project-image {
        transform: scale(1.05);
      }
      
      .project-image {
        transition: transform 0.5s ease;
      }

      /* Bouton dark mode */
      .theme-toggle {
        position: relative;
        width: 60px;
        height: 30px;
        background: var(--border-color);
        border-radius: 15px;
        cursor: pointer;
        transition: background 0.3s ease;
      }

      .theme-toggle::after {
        content: '';
        position: absolute;
        top: 3px;
        left: 3px;
        width: 24px;
        height: 24px;
        background: white;
        border-radius: 50%;
        transition: transform 0.3s ease;
      }

      .dark .theme-toggle::after {
        transform: translateX(30px);
        background: #1f2937;
      }

      .dark .theme-toggle {
        background: #4b5563;
      }

      .theme-icon {
        position: absolute;
        top: 6px;
        font-size: 0.9rem;
        transition: opacity 0.3s ease;
      }

      .sun-icon {
        left: 8px;
        color: #f59e0b;
      }

      .dark .sun-icon {
        opacity: 0;
      }

      .moon-icon {
        right: 8px;
        color: #d1d5db;
        opacity: 0;
      }

      .dark .moon-icon {
        opacity: 1;
      }
    </style>
</head>

<body class="font-sans overflow-x-hidden">
    <!-- Navigation -->
    <header class="fixed top-0 left-0 right-0 z-100 glass-effect dark:bg-gray-900/95">
        <nav class="max-w-7xl mx-auto px-4 sm:px-6 py-4">
            <div class="flex justify-between items-center">
                <a href="#" class="text-2xl font-bold text-gray-900 dark:text-white">
                    Brayano<span class="text-primary-500">.</span>
                </a>
                
                <div class="flex items-center space-x-6">
                    <!-- Dark mode toggle -->
                    <div class="flex items-center space-x-4">
                        <div class="theme-toggle" id="theme-toggle">
                            <i class="fas fa-sun theme-icon sun-icon"></i>
                            <i class="fas fa-moon theme-icon moon-icon"></i>
                        </div>
                    </div>
                    
                    <div class="hidden md:flex items-center space-x-8">
                        <a href="#about" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 font-medium">À propos</a>
                        <a href="#services" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 font-medium">Services</a>
                        <a href="#portfolio" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 font-medium">Portfolio</a>
                        <a href="#contact" class="bg-primary-600 hover:bg-primary-700 text-white px-6 py-2.5 rounded-full font-medium transition-all duration-300 transform hover:scale-105">
                            Contact
                        </a>
                    </div>
                    
                    <button id="mobile-menu-btn" class="md:hidden text-gray-700 dark:text-gray-300 text-xl">
                        <i class="fas fa-bars"></i>
                    </button>
                </div>
            </div>
            
            <!-- Mobile Menu -->
            <div id="mobile-menu" class="mobile-menu md:hidden mt-4 pt-4 border-t border-gray-300 dark:border-gray-700">
                <div class="flex flex-col space-y-3 pb-4">
                    <a href="#about" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 py-2">À propos</a>
                    <a href="#services" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 py-2">Services</a>
                    <a href="#portfolio" class="text-gray-700 dark:text-gray-300 hover:text-primary-500 dark:hover:text-primary-500 transition-colors duration-300 py-2">Portfolio</a>
                    <a href="#contact" class="bg-primary-600 hover:bg-primary-700 text-white px-4 py-2 rounded-lg font-medium transition-colors duration-300 text-center">
                        Contact
                    </a>
                </div>
            </div>
        </nav>
    </header>

    <main>
        <!-- Hero Section -->
        <section class="min-h-screen flex items-center justify-center relative overflow-hidden pt-20 bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-950">
            <!-- Animated Background -->
            <div class="hero-bg absolute inset-0">
                <div class="absolute top-1/4 left-1/4 w-64 h-64 bg-primary-500/20 rounded-full blur-3xl animate-pulse-slow"></div>
                <div class="absolute bottom-1/4 right-1/4 w-64 h-64 bg-purple-500/20 rounded-full blur-3xl animate-pulse-slow" style="animation-delay: 1s;"></div>
            </div>
            
            <div class="hero-content max-w-6xl mx-auto px-4 sm:px-6 text-center">
                <div class="animate-fade-in-up">
                    <h1 class="hero-title text-4xl sm:text-5xl md:text-7xl font-bold text-gray-900 dark:text-white mb-6 text-shadow">
                        Salut, je suis <span class="gradient-text">Brayano</span>
                    </h1>
                    <h2 class="hero-subtitle text-lg sm:text-xl md:text-2xl text-gray-600 dark:text-gray-400 mb-8 font-light">
                        Développeur Full-Stack & Spécialiste Intelligence Artificielle
                    </h2>
                    <p class="max-w-3xl mx-auto text-base sm:text-lg md:text-xl text-gray-700 dark:text-gray-300 mb-12 leading-relaxed">
                        Je transforme vos idées en solutions digitales innovantes. 
                        Spécialisé dans le développement d'applications web et mobiles performantes, 
                        avec une expertise pointue en intelligence artificielle.
                    </p>
                    <div class="flex flex-col sm:flex-row gap-6 justify-center items-center">
                        <a href="#portfolio" class="group bg-primary-600 hover:bg-primary-700 text-white px-8 py-4 rounded-full font-semibold text-lg transition-all duration-300 transform hover:scale-105 flex items-center gap-2">
                            Voir mes projets
                            <i class="fas fa-arrow-down group-hover:translate-y-1 transition-transform"></i>
                        </a>
                        <a href="#contact" class="border-2 border-primary-500 text-primary-500 hover:bg-primary-500 hover:text-white px-8 py-4 rounded-full font-semibold text-lg transition-all duration-300 transform hover:scale-105">
                            Discutons ensemble
                        </a>
                    </div>
                </div>
                
                <!-- Stats -->
                <div class="mt-20 grid grid-cols-1 sm:grid-cols-3 gap-8 max-w-2xl mx-auto">
                    <div class="text-center animate-fade-in" style="animation-delay: 0.2s;">
                        <div class="text-3xl font-bold text-gray-900 dark:text-white mb-2">2+</div>
                        <div class="text-gray-600 dark:text-gray-400">Années d'expérience</div>
                    </div>
                    <div class="text-center animate-fade-in" style="animation-delay: 0.4s;">
                        <div class="text-3xl font-bold text-gray-900 dark:text-white mb-2">40+</div>
                        <div class="text-gray-600 dark:text-gray-400">Projets réalisés</div>
                    </div>
                    <div class="text-center animate-fade-in" style="animation-delay: 0.6s;">
                        <div class="text-3xl font-bold text-gray-900 dark:text-white mb-2">90%</div>
                        <div class="text-gray-600 dark:text-gray-400">Clients satisfaits</div>
                    </div>
                </div>
            </div>
        </section>

        <!-- About Section -->
        <section id="about" class="section-padding py-24 bg-white dark:bg-gray-900">
            <div class="max-w-6xl mx-auto px-4 sm:px-6">
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-center">
                    <div class="reveal">
                        <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 dark:text-white mb-8">
                            Passionné par <span class="gradient-text">l'innovation</span>
                        </h2>
                        <div class="space-y-6 text-gray-700 dark:text-gray-300 leading-relaxed">
                            <p class="text-base sm:text-lg">
                                Développeur full-stack basé à Douala, je me spécialise dans la création de solutions digitales sur mesure qui répondent aux défis réels des entreprises.
                            </p>
                            <p>
                                Mon expertise couvre l'ensemble de la chaîne de développement : des interfaces utilisateur intuitives aux architectures backend robustes, en passant par l'intégration d'intelligence artificielle pour automatiser et optimiser vos processus.
                            </p>
                            <p>
                                Chaque projet est une opportunité d'innover et de créer des solutions qui ont un impact tangible sur votre activité.
                            </p>
                        </div>
                        
                        <!-- Skills Progress -->
                        <div class="mt-12 space-y-6">
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="text-gray-900 dark:text-white font-medium">Développement Frontend</span>
                                    <span class="text-primary-500">95%</span>
                                </div>
                                <div class="w-full bg-gray-200 dark:bg-gray-800 rounded-full h-2">
                                    <div class="bg-gradient-to-r from-primary-500 to-purple-500 h-2 rounded-full" style="width: 95%;"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="text-gray-900 dark:text-white font-medium">Développement Backend</span>
                                    <span class="text-primary-500">90%</span>
                                </div>
                                <div class="w-full bg-gray-200 dark:bg-gray-800 rounded-full h-2">
                                    <div class="bg-gradient-to-r from-primary-500 to-purple-500 h-2 rounded-full" style="width: 90%;"></div>
                                </div>
                            </div>
                            <div>
                                <div class="flex justify-between mb-2">
                                    <span class="text-gray-900 dark:text-white font-medium">Intelligence Artificielle</span>
                                    <span class="text-primary-500">85%</span>
                                </div>
                                <div class="w-full bg-gray-200 dark:bg-gray-800 rounded-full h-2">
                                    <div class="bg-gradient-to-r from-primary-500 to-purple-500 h-2 rounded-full" style="width: 85%;"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                    
                    <div class="reveal relative">
                        <div class="relative">
                            <div class="absolute -inset-4 bg-gradient-to-r from-primary-500 to-purple-500 rounded-2xl blur-lg opacity-20 animate-pulse-slow"></div>
                            <div class="relative bg-white dark:bg-gray-800 p-8 rounded-2xl border border-gray-200 dark:border-gray-700">
                                <div class="space-y-6">
<img src="c:\Users\lenovo\Pictures\1000010184.jpg" alt="">                                   
                                   
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Services Section -->
        <section id="services" class="section-padding py-24 bg-gray-50 dark:bg-gray-800/50">
            <div class="max-w-7xl mx-auto px-4 sm:px-6">
                <div class="text-center mb-16 reveal">
                    <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
                        Mes <span class="gradient-text">Services</span>
                    </h2>
                    <p class="max-w-3xl mx-auto text-lg sm:text-xl text-gray-600 dark:text-gray-400">
                        Des solutions complètes pour digitaliser et faire croître votre entreprise
                    </p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="reveal card-glow p-8 rounded-2xl group">
                        <div class="w-16 h-16 bg-gradient-to-br from-primary-500 to-blue-600 rounded-2xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                            <i class="fas fa-laptop-code text-white text-2xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Développement Web</h3>
                        <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                            Sites web et applications web modernes, rapides et optimisées pour le SEO. 
                            Interface utilisateur intuitive et expérience utilisateur exceptionnelle.
                        </p>
                        <ul class="space-y-2 text-sm text-gray-700 dark:text-gray-300">
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                React, Html, Css,Tailling css,Boostrap
                            </li>
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                Firebase
                            </li>
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                Responsive & Progressive Web Apps
                            </li>
                        </ul>
                    </div>
                    <div class="reveal card-glow p-8 rounded-2xl group" style="animation-delay: 0.4s;">
                        <div class="w-16 h-16 bg-gradient-to-br from-green-500 to-teal-600 rounded-2xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                            <i class="fas fa-brain text-white text-2xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">Intelligence Artificielle</h3>
                        <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                            Intégration d'IA pour automatiser vos processus : chatbots, analyse de données, 
                            reconnaissance d'images et recommandations personnalisées.
                        </p>
                        <ul class="space-y-2 text-sm text-gray-700 dark:text-gray-300">
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                Chatbots intelligents
                            </li>
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                APIs d'IA (OpenAI, Google)
                            </li>
                        </ul>
                    </div>

                    <div class="reveal card-glow p-8 rounded-2xl group" style="animation-delay: 0.6s;">
                        <div class="w-16 h-16 bg-gradient-to-br from-orange-500 to-red-600 rounded-2xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
                            <i class="fas fa-shopping-cart text-white text-2xl"></i>
                        </div>
                        <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-4">E-commerce</h3>
                        <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                            Boutiques en ligne complètes avec gestion des stocks, paiements sécurisés 
                            et tableau de bord administrateur avancé.
                        </p>
                        <ul class="space-y-2 text-sm text-gray-700 dark:text-gray-300">
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                Gestion des stocks
                            </li>
                            <li class="flex items-center gap-2">
                                <i class="fas fa-check text-primary-500"></i>
                                Analytics & reporting
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </section>

        <!-- Portfolio Section -->
        <section id="portfolio" class="section-padding py-24 bg-white dark:bg-gray-900">
            <div class="max-w-7xl mx-auto px-4 sm:px-6">
                <div class="text-center mb-16 reveal">
                    <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
                        Mes <span class="gradient-text">Réalisations</span>
                    </h2>
                    <p class="max-w-3xl mx-auto text-lg sm:text-xl text-gray-600 dark:text-gray-400">
                        Découvrez quelques projets qui illustrent mon expertise et ma passion pour l'innovation
                    </p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <!-- Project 2 -->
                    <div class="reveal project-card card-glow rounded-2xl overflow-hidden group" style="animation-delay: 0.2s;">
                        <div class="relative overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=600&h=400&fit=crop" 
                                 alt="Plateforme mobile Petit Jobs Express" 
                                 loading="lazy"
                                 class="project-image w-full h-48 object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-900 via-transparent to-transparent opacity-60"></div>
                            <div class="absolute top-4 right-4">
                                <span class="bg-primary-600 text-white px-3 py-1 rounded-full text-xs font-medium">
                                  web  Mobile
                                </span>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">Petit Jobs Express</h3>
                            <p class="text-gray-600 dark:text-gray-400 mb-4 leading-relaxed">
                                Plateforme mobile connectant prestataires et clients pour des services de proximité. 
                                Géolocalisation, paiements sécurisés et système de notation.
                            </p>
                            <div class="flex flex-wrap gap-2 mb-4">
                                <span class="bg-blue-600/20 text-blue-400 text-xs px-2 py-1 rounded-full">React Native,Html:5</span>
                                <span class="bg-green-600/20 text-green-400 text-xs px-2 py-1 rounded-full">Firebase</span>
                            </div>
                            <div class="flex justify-between items-center">
                                <a href=" https://brayano-ux.github.io/restauratione/" class="text-primary-500 hover:text-primary-400 font-medium flex items-center gap-2">
                                    Voir le projet <i class="fas fa-external-link-alt text-xs"></i>
                                </a>
                                <div class="flex gap-2">
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fab fa-github text-xs"></i>
                                    </button>
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fas fa-play text-xs"></i>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Project 3 -->
                    <div class="reveal project-card card-glow rounded-2xl overflow-hidden group" style="animation-delay: 0.4s;">
                        <div class="relative overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?w=600&h=400&fit=crop" 
                                 alt="Collection de templates Vitrine Pro" 
                                 loading="lazy"
                                 class="project-image w-full h-48 object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-900 via-transparent to-transparent opacity-60"></div>
                            <div class="absolute top-4 right-4">
                                <span class="bg-orange-600 text-white px-3 py-1 rounded-full text-xs font-medium">
                                    Web Design
                                </span>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">Vitrine Pro</h3>
                            <p class="text-gray-600 dark:text-gray-400 mb-4 leading-relaxed">
                                Collection de templates de sites web optimisés pour les TPE/PME. 
                                Design moderne, responsive et optimisé SEO pour restaurants.
                            </p>
                            <div class="flex flex-wrap gap-2 mb-4">
                                <span class="bg-orange-600/20 text-orange-400 text-xs px-2 py-1 rounded-full">HTML5</span>
                                <span class="bg-blue-600/20 text-blue-400 text-xs px-2 py-1 rounded-full">Tailwind CSS</span>
                                <span class="bg-yellow-600/20 text-yellow-400 text-xs px-2 py-1 rounded-full">JavaScript</span>
                            </div>
                            <div class="flex justify-between items-center">
                                <a href="https://brayano-ux.github.io/MBOA-LIBRAIRIE/" class="text-primary-500 hover:text-primary-400 font-medium flex items-center gap-2">
                                    Voir le projet <i class="fas fa-external-link-alt text-xs"></i>
                                </a>
                                <div class="flex gap-2">
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fab fa-github text-xs"></i>
                                    </button>
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fas fa-play text-xs"></i>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Project 4 -->
                    <div class="reveal project-card card-glow rounded-2xl overflow-hidden group" style="animation-delay: 0.6s;">
                        <div class="relative overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1677442136019-21780ecad995?w=600&h=400&fit=crop" 
                                 alt="Chatbot Assistant IA Business" 
                                 loading="lazy"
                                 class="project-image w-full h-48 object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-900 via-transparent to-transparent opacity-60"></div>
                            <div class="absolute top-4 right-4">
                                <span class="bg-green-600 text-white px-3 py-1 rounded-full text-xs font-medium">
                                    IA & Chatbot
                                </span>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">Assistant IA Scolaire</h3>
                            <p class="text-gray-600 dark:text-gray-400 mb-4 leading-relaxed">
                                Chatbot intelligent pour Vous aider a reviser et a gerer vos cours avec traitement du langage naturel. 
                            </p>
                            <div class="flex flex-wrap gap-2 mb-4">
                                <span class="bg-green-600/20 text-green-400 text-xs px-2 py-1 rounded-full">OpenAI API</span>
                                <span class="bg-blue-600/20 text-blue-400 text-xs px-2 py-1 rounded-full">Python</span>
                                <span class="bg-purple-600/20 text-purple-400 text-xs px-2 py-1 rounded-full">React</span>
                            </div>
                            <div class="flex justify-between items-center">
                                <a href="https://brayano-ux.github.io/p/" class="text-primary-500 hover:text-primary-400 font-medium flex items-center gap-2">
                                    Voir le projet <i class="fas fa-external-link-alt text-xs"></i>
                                </a>
                                <div class="flex gap-2">
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fab fa-github text-xs"></i>
                                    </button>
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fas fa-play text-xs"></i>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Project 5 -->
                    <div class="reveal project-card card-glow rounded-2xl overflow-hidden group" style="animation-delay: 0.8s;">
                        <div class="relative overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1551650975-87deedd944c3?w=600&h=400&fit=crop" 
                                 alt="Tableau de bord Dashboard Analytics Pro" 
                                 loading="lazy"
                                 class="project-image w-full h-48 object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-900 via-transparent to-transparent opacity-60"></div>
                            <div class="absolute top-4 right-4">
                                <span class="bg-indigo-600 text-white px-3 py-1 rounded-full text-xs font-medium">
                                    Dashboard
                                </span>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">Dashboard Analytics Pro</h3>
                            <p class="text-gray-600 dark:text-gray-400 mb-4 leading-relaxed">
                                Tableau de bord avancé pour le suivi des KPIs business. 
                                Visualisations interactives et rapports automatisés en temps réel.
                            </p>
                            <div class="flex flex-wrap gap-2 mb-4">
                                <span class="bg-blue-600/20 text-blue-400 text-xs px-2 py-1 rounded-full">React</span>
                                <span class="bg-green-600/20 text-green-400 text-xs px-2 py-1 rounded-full">D3.js</span>
                                <span class="bg-purple-600/20 text-purple-400 text-xs px-2 py-1 rounded-full">PostgreSQL</span>
                            </div>
                            <div class="flex justify-between items-center">
                                <a href="#" class="text-primary-500 hover:text-primary-400 font-medium flex items-center gap-2">
                                    Voir le projet <i class="fas fa-external-link-alt text-xs"></i>
                                </a>
                                <div class="flex gap-2">
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fab fa-github text-xs"></i>
                                    </button>
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fas fa-play text-xs"></i>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>

                    <!-- Project 6 -->
                    <div class="reveal project-card card-glow rounded-2xl overflow-hidden group" style="animation-delay: 1s;">
                        <div class="relative overflow-hidden">
                            <img src="https://images.unsplash.com/photo-1560472354-b33ff0c44a43?w=600&h=400&fit=crop" 
                                 alt="Application fintech PaySafe Mobile" 
                                 loading="lazy"
                                 class="project-image w-full h-48 object-cover">
                            <div class="absolute inset-0 bg-gradient-to-t from-gray-900 via-transparent to-transparent opacity-60"></div>
                            <div class="absolute top-4 right-4">
                                <span class="bg-emerald-600 text-white px-3 py-1 rounded-full text-xs font-medium">
                                    Fintech
                                </span>
                            </div>
                        </div>
                        <div class="p-6">
                            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">Chat educatif</h3>
                            <p class="text-gray-600 dark:text-gray-400 mb-4 leading-relaxed">
                                Application discution privée entre partenaire pour  echanger sur vos projets
                            </p>
                            <div class="flex flex-wrap gap-2 mb-4">
                                <span class="bg-blue-600/20 text-blue-400 text-xs px-2 py-1 rounded-full">HTML5</span>
                                <span class="bg-green-600/20 text-green-400 text-xs px-2 py-1 rounded-full">Firebase</span>
                                <span class="bg-red-600/20 text-red-400 text-xs px-2 py-1 rounded-full">js</span>
                            </div>
                            <div class="flex justify-between items-center">
                                <a href="#" class="text-primary-500 hover:text-primary-400 font-medium flex items-center gap-2">
                                    Voir le projet <i class="fas fa-external-link-alt text-xs"></i>
                                </a>
                                <div class="flex gap-2">
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fab fa-github text-xs"></i>
                                    </button>
                                    <button class="w-8 h-8 bg-gray-200 dark:bg-gray-800 hover:bg-primary-600 rounded-full flex items-center justify-center transition-colors">
                                        <i class="fas fa-play text-xs"></i>
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Call to Action -->
                <div class="text-center mt-16 reveal">
                    <a href="#contact" class="inline-flex items-center gap-2 bg-primary-600 hover:bg-primary-700 text-white px-8 py-4 rounded-full font-semibold text-lg transition-all duration-300 transform hover:scale-105">
                        Discutons de votre projet
                        <i class="fas fa-arrow-right"></i>
                    </a>
                </div>
            </div>
        </section>

        <!-- Testimonials Section -->
        <section class="section-padding py-24 bg-gray-50 dark:bg-gray-800/50">
            <div class="max-w-6xl mx-auto px-4 sm:px-6">
                <div class="text-center mb-16 reveal">
                    <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
                        Ce que disent mes <span class="gradient-text">clients</span>
                    </h2>
                    <p class="max-w-3xl mx-auto text-lg sm:text-xl text-gray-600 dark:text-gray-400">
                        Leur satisfaction est ma priorité
                    </p>
                </div>

                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                    <div class="reveal card-glow p-8 rounded-2xl">
                        <div class="flex items-center gap-1 mb-4">
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                        </div>
                        <p class="text-gray-700 dark:text-gray-300 mb-6 leading-relaxed">
                            "Brayano a transformé notre vision en une application mobile exceptionnelle. 
                            Son expertise technique et sa compréhension des enjeux business sont remarquables."
                        </p>
                        <div class="flex items-center gap-3">
                            <div class="w-12 h-12 bg-primary-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold">JM</span>
                            </div>
                            <div>
                                <div class="text-gray-900 dark:text-white font-semibold">Jean-Marie K.</div>
                                <div class="text-gray-600 dark:text-gray-400 text-sm">CEO, TechStart Cameroun</div>
                            </div>
                        </div>
                    </div>

                    <div class="reveal card-glow p-8 rounded-2xl" style="animation-delay: 0.2s;">
                        <div class="flex items-center gap-1 mb-4">
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                        </div>
                        <p class="text-gray-700 dark:text-gray-300 mb-6 leading-relaxed">
                            "Un développeur passionné qui livre toujours des solutions de qualité. 
                            Notre site e-commerce dépasse nos attentes en termes de performance et design."
                        </p>
                        <div class="flex items-center gap-3">
                            <div class="w-12 h-12 bg-purple-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold">AN</span>
                            </div>
                            <div>
                                <div class="text-gray-900 dark:text-white font-semibold">Aminata N.</div>
                                <div class="text-gray-600 dark:text-gray-400 text-sm">Fondatrice, MBOA Store</div>
                            </div>
                        </div>
                    </div>

                    <div class="reveal card-glow p-8 rounded-2xl" style="animation-delay: 0.4s;">
                        <div class="flex items-center gap-1 mb-4">
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                            <i class="fas fa-star text-yellow-400"></i>
                        </div>
                        <p class="text-gray-700 dark:text-gray-300 mb-6 leading-relaxed">
                            "L'intégration de l'IA dans notre processus client a révolutionné notre service. 
                            Brayano maîtrise parfaitement les technologies émergentes."
                        </p>
                        <div class="flex items-center gap-3">
                            <div class="w-12 h-12 bg-green-600 rounded-full flex items-center justify-center">
                                <span class="text-white font-bold">PD</span>
                            </div>
                            <div>
                                <div class="text-gray-900 dark:text-white font-semibold">Paul D.</div>
                                <div class="text-gray-600 dark:text-gray-400 text-sm">Directeur IT, Innovation Hub</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Contact Section -->
        <section id="contact" class="section-padding py-24 bg-white dark:bg-gray-900">
            <div class="max-w-6xl mx-auto px-4 sm:px-6">
                <div class="text-center mb-16 reveal">
                    <h2 class="text-3xl sm:text-4xl md:text-5xl font-bold text-gray-900 dark:text-white mb-6">
                        Lançons votre <span class="gradient-text">projet</span>
                    </h2>
                    <p class="max-w-3xl mx-auto text-lg sm:text-xl text-gray-600 dark:text-gray-400">
                        Prêt à transformer vos idées en solutions digitales innovantes ? 
                        Contactez-moi pour un devis gratuit et personnalisé.
                    </p>
                </div>

                <div class="grid grid-cols-1 lg:grid-cols-2 gap-16 items-start">
                    <!-- Contact Info -->
                    <div class="reveal">
                        <div class="space-y-8">
                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-primary-600 rounded-lg flex items-center justify-center flex-shrink-0">
                                    <i class="fas fa-map-marker-alt text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-gray-900 dark:text-white font-semibold mb-2">Localisation</h4>
                                    <p class="text-gray-600 dark:text-gray-400">Douala, Littoral, Cameroun</p>
                                    <p class="text-gray-600 dark:text-gray-400">Disponible pour des projets à distance</p>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-green-600 rounded-lg flex items-center justify-center flex-shrink-0">
                                    <i class="fab fa-whatsapp text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-gray-900 dark:text-white font-semibold mb-2">WhatsApp</h4>
                                    <p class="text-gray-600 dark:text-gray-400">Disponible 7j/7 pour vos urgences</p>
                                    <a href="https://wa.me/237657300644" target="_blank" rel="noopener noreferrer" class="text-primary-500 hover:text-primary-400 font-medium">
                                        Démarrer une conversation
                                    </a>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-blue-600 rounded-lg flex items-center justify-center flex-shrink-0">
                                    <i class="fas fa-envelope text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-gray-900 dark:text-white font-semibold mb-2">Email</h4>
                                    <p class="text-gray-600 dark:text-gray-400">Réponse sous 24h maximum</p>
                                    <a href="mailto:contact@brayano.dev" class="text-primary-500 hover:text-primary-400 font-medium">
ulrichbrayan492@gmail.com                                    </a>
                                </div>
                            </div>

                            <div class="flex items-start gap-4">
                                <div class="w-12 h-12 bg-purple-600 rounded-lg flex items-center justify-center flex-shrink-0">
                                    <i class="fas fa-calendar text-white"></i>
                                </div>
                                <div>
                                    <h4 class="text-gray-900 dark:text-white font-semibold mb-2">Consultation gratuite</h4>
                                    <p class="text-gray-600 dark:text-gray-400">30 minutes pour discuter de votre projet</p>
                                    <a href="#" class="text-primary-500 hover:text-primary-400 font-medium">
                                        Planifier un appel
                                    </a>
                                </div>
                            </div>
                        </div>

                        <!-- Social Links -->
                        <div class="mt-12">
                            <h4 class="text-gray-900 dark:text-white font-semibold mb-4">Suivez-moi</h4>
                            <div class="flex gap-4">
                                <a href="#" class="w-12 h-12 bg-gray-200 dark:bg-gray-800 hover:bg-blue-600 rounded-lg flex items-center justify-center transition-colors">
                                    <i class="fab fa-linkedin text-gray-700 dark:text-gray-300"></i>
                                </a>
                                <a href="#" class="w-12 h-12 bg-gray-200 dark:bg-gray-800 hover:bg-gray-700 rounded-lg flex items-center justify-center transition-colors">
                                    <i class="fab fa-github text-gray-700 dark:text-gray-300"></i>
                                </a>
                                <a href="#" class="w-12 h-12 bg-gray-200 dark:bg-gray-800 hover:bg-blue-400 rounded-lg flex items-center justify-center transition-colors">
                                    <i class="fab fa-twitter text-gray-700 dark:text-gray-300"></i>
                                </a>
                                <a href="#" class="w-12 h-12 bg-gray-200 dark:bg-gray-800 hover:bg-red-600 rounded-lg flex items-center justify-center transition-colors">
                                    <i class="fab fa-youtube text-gray-700 dark:text-gray-300"></i>
                                </a>
                            </div>
                        </div>
                    </div>

                    <!-- Contact Form -->
                    <div class="reveal" style="animation-delay: 0.2s;">
                        <div class="glass-effect p-8 rounded-2xl bg-gray-50 dark:bg-gray-800">
                            <form id="contact-form" class="space-y-6">
                                <div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
                                    <div>
                                        <label class="block text-gray-900 dark:text-white font-medium mb-2">Nom *</label>
                                        <input type="text" name="name" id="nom" required 
                                               class="w-full p-4 bg-white dark:bg-gray-700 border border-gray-300 dark:border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary-500 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400" 
                                               placeholder="Votre nom">
                                    </div>
                                    <div>
                                        <label class="block text-gray-900 dark:text-white font-medium mb-2">Email *</label>
                                        <input type="email" name="email" id="email" required 
                                               class="w-full p-4 bg-white dark:bg-gray-700 border border-gray-300 dark:border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary-500 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400" 
                                               placeholder="votre@email.com">
                                    </div>
                                </div>

                                <div>
                                    <label class="block text-gray-900 dark:text-white font-medium mb-2">Type de projet</label>
                                    <select name="project_type" id="selection"
                                            class="w-full p-4 bg-white dark:bg-gray-700 border border-gray-300 dark:border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary-500 text-gray-900 dark:text-white">
                                        <option value="">Sélectionnez un type de projet</option>
                                        <option value="web">Site web / Application web</option>
                                        <option value="ecommerce">E-commerce</option>
                                        <option value="ia">Intelligence artificielle</option>
                                        <option value="consultation">Consultation / Formation</option>
                                        <option value="autre">Autre</option>
                                    </select>
                                </div>

                                <div>
                                    <label class="block text-gray-900 dark:text-white font-medium mb-2">Budget estimé</label>
                                    <select name="budget"  id="budget"
                                            class="w-full p-4 bg-white dark:bg-gray-700 border border-gray-300 dark:border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary-500 text-gray-900 dark:text-white">
                                        <option value="">Sélectionnez une fourchette</option>
                                        <option value="50k">Moins de 50 000 FCFA</option>
                                        <option value="50k-1M">50 000 - 100 000 FCFA</option>
                                        <option value="1M-2M">100 000 - 200 000 FCFA</option>
                                        <option value=">2M">Plus de 200 000 FCFA</option>
                                        <option value="discuss">À discuter</option>
                                    </select>
                                </div>

                                <div>
                                    <label class="block text-gray-900 dark:text-white font-medium mb-2">Décrivez votre projet *</label>
                                    <textarea name="message" rows="6" required id="description"
                                              class="w-full p-4 bg-white dark:bg-gray-700 border border-gray-300 dark:border-gray-600 rounded-lg focus:outline-none focus:ring-2 focus:ring-primary-500 text-gray-900 dark:text-white placeholder-gray-500 dark:placeholder-gray-400" 
                                              placeholder="Décrivez votre projet, vos objectifs et vos attentes..."></textarea>
                                </div>

                                <button type="submit" id="envoi"
                                        class="w-full bg-gradient-to-r from-primary-600 to-purple-600 hover:from-primary-700 hover:to-purple-700 text-white py-4 px-6 rounded-lg font-semibold text-lg transition-all duration-300 transform hover:scale-[1.02] flex items-center justify-center gap-2">
                                    <span>Envoyer ma demande</span>
                                    <i class="fas fa-paper-plane"></i>
                                </button>

                                <p class="text-gray-600 dark:text-gray-400 text-sm text-center">
                                    Réponse garantie sous 24h • Devis gratuit et sans engagement
                                </p>
                            </form>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-50 dark:bg-gray-800 py-12 border-t border-gray-200 dark:border-gray-700">
        <div class="max-w-7xl mx-auto px-4 sm:px-6">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div class="md:col-span-2">
                    <a href="#" class="text-2xl font-bold text-gray-900 dark:text-white mb-4 block">
                        Brayano<span class="text-primary-500">.</span>
                    </a>
                    <p class="text-gray-600 dark:text-gray-400 mb-6 leading-relaxed">
                        Développeur full-stack passionné par l'innovation et l'intelligence artificielle. 
                        Je transforme vos idées en solutions digitales performantes.
                    </p>
                    <div class="flex gap-4">
                        <a href="#" class="w-10 h-10 bg-gray-200 dark:bg-gray-700 hover:bg-gray-300 dark:hover:bg-gray-600 rounded-lg flex items-center justify-center transition-colors">
                            <i class="fab fa-github text-gray-700 dark:text-gray-300"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-gray-200 dark:bg-gray-700 hover:bg-blue-400 rounded-lg flex items-center justify-center transition-colors">
                            <i class="fab fa-twitter text-gray-700 dark:text-gray-300"></i>
                        </a>
                        <a href="https://wa.me/237657300644" class="w-10 h-10 bg-gray-200 dark:bg-gray-700 hover:bg-green-600 rounded-lg flex items-center justify-center transition-colors">
                            <i class="fab fa-whatsapp text-gray-700 dark:text-gray-300"></i>
                        </a>
                    </div>
                </div>

                <div>
                    <h4 class="text-gray-900 dark:text-white font-semibold mb-4">Services</h4>
                    <ul class="space-y-2 text-gray-600 dark:text-gray-400">
                        <li><a href="#services" class="hover:text-primary-500 transition-colors">Développement Web</a></li>
                        <li><a href="#services" class="hover:text-primary-500 transition-colors">Intelligence Artificielle</a></li>
                        <li><a href="#services" class="hover:text-primary-500 transition-colors">E-commerce</a></li>
                        <li><a href="#services" class="hover:text-primary-500 transition-colors">Consultation</a></li>
                    </ul>
                </div>

                <div>
                    <h4 class="text-gray-900 dark:text-white font-semibold mb-4">Contact</h4>
                    <ul class="space-y-2 text-gray-600 dark:text-gray-400">
                        <li class="flex items-center gap-2">
                            <i class="fas fa-map-marker-alt text-primary-500"></i>
                            Douala, Cameroun
                        </li>
                        <li class="flex items-center gap-2">
                            <i class="fas fa-envelope text-primary-500"></i>
                            <a href="mailto:contact@brayano.dev" class="hover:text-primary-500 transition-colors">ulrichbrayan@gmail.com</a>
                        </li>
                        <li class="flex items-center gap-2">
                            <i class="fab fa-whatsapp text-primary-500"></i>
                            <a href="https://wa.me/237657300644" class="hover:text-primary-500 transition-colors">WhatsApp</a>
                        </li>
                    </ul>
                </div>
            </div>

            <div class="border-t border-gray-200 dark:border-gray-700 mt-12 pt-8">
                <div class="flex flex-col md:flex-row justify-between items-center gap-4">
                    <p class="text-gray-600 dark:text-gray-400 text-center md:text-left">
                        &copy; 2025 Brayano. Tous droits réservés. Conçu avec ❤️ à Douala.
                    </p>
                    <div class="flex gap-6 text-sm text-gray-600 dark:text-gray-400">
                        <a href="#" class="hover:text-primary-500 transition-colors">Mentions légales</a>
                        <a href="#" class="hover:text-primary-500 transition-colors">Politique de confidentialité</a>
                        <a href="#" class="hover:text-primary-500 transition-colors">CGV</a>
                    </div>
                </div>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button id="back-to-top" class="fixed bottom-8 right-8 w-12 h-12 bg-primary-600 hover:bg-primary-700 text-white rounded-full flex items-center justify-center transition-all duration-300 opacity-0 pointer-events-none z-90">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        document.getElementById('envoi').addEventListener('click',function(){
            nom=document.getElementById('nom').value.trim();
            selection=document.getElementById('selection').value;
            budget=document.getElementById('budget').value;
            email =document.getElementById('email').value.trim();
            description=document.getElementById('description').value.trim();
            if(!nom||!email||!selection){
                alert("Veuillez remplir les informations");
            }
            else{
            const mumero = '237657300644';
            const whatsapp=`https://wa.me/${mumero}?text=bonjour monsieur je m'appelle${nom} je voudrais causer par rapport a ${selection} pour un budget de ${budget}. Voici mon email:${email}`;
window.open(whatsapp,'_blank');
  }
        })
        // Dark mode toggle
        const themeToggle = document.getElementById('theme-toggle');
        const prefersDarkScheme = window.matchMedia('(prefers-color-scheme: dark)');
        
        // Check for saved theme or use preferred color scheme
        const currentTheme = localStorage.getItem('theme') || (prefersDarkScheme.matches ? 'dark' : 'light');
        
        if (currentTheme === 'dark') {
            document.documentElement.classList.add('dark');
        } else {
            document.documentElement.classList.remove('dark');
        }
        
        themeToggle.addEventListener('click', () => {
            document.documentElement.classList.toggle('dark');
            const theme = document.documentElement.classList.contains('dark') ? 'dark' : 'light';
            localStorage.setItem('theme', theme);
        });

        // Smooth reveal animations
        function reveal() {
            const reveals = document.querySelectorAll('.reveal');
            
            reveals.forEach(element => {
                const windowHeight = window.innerHeight;
                const elementTop = element.getBoundingClientRect().top;
                const elementVisible = 100;
                
                if (elementTop < windowHeight - elementVisible) {
                    element.classList.add('active');
                }
            });
        }

        // Mobile menu toggle
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        
        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('open');
            const icon = mobileMenuBtn.querySelector('i');
            icon.classList.toggle('fa-bars');
            icon.classList.toggle('fa-times');
        });

        // Close mobile menu when clicking on links
        document.querySelectorAll('#mobile-menu a').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.remove('open');
                const icon = mobileMenuBtn.querySelector('i');
                icon.classList.add('fa-bars');
                icon.classList.remove('fa-times');
            });
        });

        // Back to top button
        const backToTopBtn = document.getElementById('back-to-top');
        
        function toggleBackToTop() {
            if (window.pageYOffset > 300) {
                backToTopBtn.classList.remove('opacity-0', 'pointer-events-none');
                backToTopBtn.classList.add('opacity-100');
            } else {
                backToTopBtn.classList.add('opacity-0', 'pointer-events-none');
                backToTopBtn.classList.remove('opacity-100');
            }
        }

        backToTopBtn.addEventListener('click', () => {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });

        // Contact form handling
        const contactForm = document.getElementById('contact-form');
        contactForm.addEventListener('submit', (e) => {
            e.preventDefault();
            
            // Get form data
            const formData = new FormData(contactForm);
            const data = Object.fromEntries(formData);
            
            // Simulate form submission
            const submitBtn = contactForm.querySelector('button[type="submit"]');
            const originalText = submitBtn.innerHTML;
            
            submitBtn.innerHTML = '<i class="fas fa-spinner fa-spin mr-2"></i>Envoi en cours...';
            submitBtn.disabled = true;
            
            setTimeout(() => {
                alert('Merci pour votre message ! Je vous répondrai dans les 24h.');
                contactForm.reset();
                submitBtn.innerHTML = originalText;
                submitBtn.disabled = false;
            }, 2000);
        });

        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                const target = document.querySelector(this.getAttribute('href'));
                if (target) {
                    const headerOffset = 80;
                    const elementPosition = target.getBoundingClientRect().top;
                    const offsetPosition = elementPosition + window.pageYOffset - headerOffset;

                    window.scrollTo({
                        top: offsetPosition,
                        behavior: 'smooth'
                    });
                }
            });
        });

        // Header background on scroll
        const header = document.querySelector('header');
        function updateHeaderBackground() {
            if (window.pageYOffset > 100) {
                header.classList.add('bg-white/95', 'dark:bg-gray-900/95');
                header.classList.remove('glass-effect');
            } else {
                header.classList.remove('bg-white/95', 'dark:bg-gray-900/95');
                header.classList.add('glass-effect');
            }
        }

        // Initialize on page load
        window.addEventListener('load', () => {
            reveal();
            toggleBackToTop();
            updateHeaderBackground();
        });

        // Event listeners
        window.addEventListener('scroll', () => {
            reveal();
            toggleBackToTop();
            updateHeaderBackground();
        });

        // Add loading animation to project links
        document.querySelectorAll('.card-glow a').forEach(link => {
            link.addEventListener('click', (e) => {
                if (link.getAttribute('href') === '#') {
                    e.preventDefault();
                    // Add a subtle loading effect
                    link.style.opacity = '0.7';
                    setTimeout(() => {
                        link.style.opacity = '1';
                        alert('Ce projet sera bientôt disponible en ligne !');
                    }, 500);
                }
            });
        });

        // Add hover effect to service cards
        document.querySelectorAll('.card-glow').forEach(card => {
            card.addEventListener('mouseenter', () => {
                card.style.transform = 'translateY(-10px) scale(1.02)';
            });
            
            card.addEventListener('mouseleave', () => {
                card.style.transform = 'translateY(0) scale(1)';
            });
        });

        // Typing animation for hero section
        const roles = [
            'Développeur Full-Stack',
            'Spécialiste Intelligence Artificielle',
            'Consultant Digital'
        ];
        
        let currentRole = 0;
        const roleElement = document.querySelector('h2');
        
        function typeRole() {
            if (roleElement) {
                roleElement.style.opacity = '0';
                setTimeout(() => {
                    roleElement.textContent = roles[currentRole];
                    roleElement.style.opacity = '1';
                    currentRole = (currentRole + 1) % roles.length;
                }, 300);
            }
        }

        // Start typing animation after page load
        setTimeout(() => {
            setInterval(typeRole, 3000);
        }, 2000);

        // Add intersection observer for better performance
        const observerOptions = {
            threshold: 0.1,
            rootMargin: '0px 0px -50px 0px'
        };

        const observer = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('active');
                }
            });
        }, observerOptions);

        // Observe all reveal elements
        document.querySelectorAll('.reveal').forEach(el => {
            observer.observe(el);
        });
    </script>
</body>
