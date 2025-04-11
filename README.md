<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Rumilly Nettoyage - Professionnels du nettoyage en Haute-Savoie</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;500;600;700&display=swap');
        
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #f5f0e6;
            color: #333;
            scroll-behavior: smooth;
        }
        
        .bg-primary {
            background-color: #6b4f3a;
        }
        
        .text-accent {
            color: #4a7c59;
        }
        
        .border-accent {
            border-color: #4a7c59;
        }
        
        .btn-primary {
            background-color: #4a7c59;
            color: white;
            transition: all 0.3s ease;
        }
        
        .btn-primary:hover {
            background-color: #3a6548;
            transform: translateY(-2px);
        }
        
        .service-card {
            transition: all 0.3s ease;
            border-bottom: 3px solid transparent;
        }
        
        .service-card:hover {
            transform: translateY(-5px);
            border-bottom: 3px solid #4a7c59;
        }
        
        .hero-section {
            background-color: #6b4f3a;
            min-height: 100vh;
        }
        
        .fade-in {
            animation: fadeIn 1s ease-in;
        }
        
        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }
        
        .local-badge {
            background-color: rgba(255,255,255,0.2);
            border: 1px solid white;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header class="bg-primary text-white shadow-md sticky top-0 z-50">
        <div class="container mx-auto px-4 py-4 flex justify-between items-center">
            <div class="flex items-center">
                <i class="fas fa-broom text-accent text-2xl mr-2"></i>
                <h1 class="text-xl font-bold">Rumilly <span class="text-accent">Nettoyage</span></h1>
            </div>
            <nav class="hidden md:block">
                <ul class="flex space-x-8">
                    <li><a href="#accueil" class="hover:text-accent transition">Accueil</a></li>
                    <li><a href="#services" class="hover:text-accent transition">Services</a></li>
                    <li><a href="#local" class="hover:text-accent transition">Notre territoire</a></li>
                    <li><a href="#contact" class="hover:text-accent transition">Devis</a></li>
                </ul>
            </nav>
            <button class="md:hidden text-xl" id="menu-toggle">
                <i class="fas fa-bars"></i>
            </button>
        </div>
        
        <!-- Mobile menu -->
        <div id="mobile-menu" class="hidden bg-primary px-4 pb-4 md:hidden">
            <ul class="flex flex-col space-y-3">
                <li><a href="#accueil" class="hover:text-accent transition block py-2">Accueil</a></li>
                <li><a href="#services" class="hover:text-accent transition block py-2">Services</a></li>
                <li><a href="#local" class="hover:text-accent transition block py-2">Notre territoire</a></li>
                <li><a href="#contact" class="hover:text-accent transition block py-2">Devis</a></li>
            </ul>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="accueil" class="hero-section flex items-center justify-center text-white fade-in">
        <div class="container mx-auto px-4 text-center">
            <div class="local-badge inline-flex items-center px-4 py-2 rounded-full mb-6">
                <i class="fas fa-map-marker-alt mr-2"></i>
                <span>Vallière-sur-Fier, Haute-Savoie</span>
            </div>
            <h1 class="text-4xl md:text-6xl font-bold mb-6">Nettoyage professionnel <span class="text-accent">en Haute-Savoie</span></h1>
            <p class="text-xl md:text-2xl mb-8 max-w-2xl mx-auto">Entreprise locale spécialisée dans le nettoyage pour professionnels et particuliers sur le secteur de Rumilly et Vallières-sur-Fier.</p>
            <div class="flex flex-col sm:flex-row justify-center gap-4">
                <a href="#contact" class="btn-primary px-8 py-3 rounded-lg font-medium">Demander un devis</a>
                <a href="tel:+33450000000" class="bg-white text-primary px-8 py-3 rounded-lg font-medium border border-accent hover:bg-gray-100 transition">
                    <i class="fas fa-phone mr-2"></i>04 50 00 00 00
                </a>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Nos <span class="text-accent">Services</span></h2>
                <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Des solutions de nettoyage adaptées aux besoins des professionnels et particuliers de Haute-Savoie.</p>
            </div>
            
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Service 1 -->
                <div class="service-card bg-gray-50 p-8 rounded-lg shadow-sm">
                    <div class="text-accent text-4xl mb-4">
                        <i class="fas fa-building"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Nettoyage d'Entreprises</h3>
                    <p class="text-gray-600 mb-4">Services de nettoyage réguliers pour vos bureaux et locaux professionnels.</p>
                    <a href="#contact" class="text-accent font-medium inline-flex items-center">
                        Demander un devis <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
                
                <!-- Service 2 -->
                <div class="service-card bg-gray-50 p-8 rounded-lg shadow-sm">
                    <div class="text-accent text-4xl mb-4">
                        <i class="fas fa-home"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Nettoyage Résidentiel</h3>
                    <p class="text-gray-600 mb-4">Services de nettoyage complet pour votre domicile avec des produits écologiques.</p>
                    <a href="#contact" class="text-accent font-medium inline-flex items-center">
                        Demander un devis <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
                
                <!-- Service 3 -->
                <div class="service-card bg-gray-50 p-8 rounded-lg shadow-sm">
                    <div class="text-accent text-4xl mb-4">
                        <i class="fas fa-broom"></i>
                    </div>
                    <h3 class="text-xl font-bold mb-3">Nettoyage après Travaux</h3>
                    <p class="text-gray-600 mb-4">Élimination complète des résidus de construction après rénovation.</p>
                    <a href="#contact" class="text-accent font-medium inline-flex items-center">
                        Demander un devis <i class="fas fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Local Section -->
    <section id="local" class="py-20 bg-gray-50">
        <div class="container mx-auto px-4">
            <div class="flex flex-col lg:flex-row items-center">
                <div class="lg:w-1/2 mb-12 lg:mb-0 lg:pr-12">
                    <h2 class="text-3xl md:text-4xl font-bold mb-6">Une entreprise <span class="text-accent">locale</span></h2>
                    <div class="w-20 h-1 bg-accent mb-6"></div>
                    <p class="text-gray-600 mb-6">Implantée à Vallières-sur-Fier depuis 2010, Rumilly Nettoyage est une entreprise familiale au service des professionnels et particuliers de Haute-Savoie.</p>
                    <p class="text-gray-600 mb-6">Nous intervenons principalement sur les secteurs de :</p>
                    <ul class="grid grid-cols-1 md:grid-cols-2 gap-4 mb-8">
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Rumilly
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Vallières-sur-Fier
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Albens
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Alby-sur-Chéran
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Étercy
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-check text-accent mr-2"></i> Marigny-Saint-Marcel
                        </li>
                    </ul>
                    <a href="#contact" class="btn-primary px-8 py-3 rounded-lg font-medium inline-block">Obtenir un devis local</a>
                </div>
                <div class="lg:w-1/2 bg-white p-8 rounded-lg shadow-sm">
                    <h3 class="text-2xl font-bold mb-6 text-accent">Nos engagements</h3>
                    <div class="space-y-6">
                        <div class="flex items-start">
                            <div class="text-accent mr-4 mt-1">
                                <i class="fas fa-leaf text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold mb-1">Produits écologiques</h4>
                                <p class="text-gray-600">Utilisation de produits respectueux de l'environnement et de la santé.</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-accent mr-4 mt-1">
                                <i class="fas fa-user-tie text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold mb-1">Personnel qualifié</h4>
                                <p class="text-gray-600">Des employés formés et équipés pour répondre à tous vos besoins.</p>
                            </div>
                        </div>
                        <div class="flex items-start">
                            <div class="text-accent mr-4 mt-1">
                                <i class="fas fa-hand-holding-usd text-xl"></i>
                            </div>
                            <div>
                                <h4 class="font-bold mb-1">Tarifs transparents</h4>
                                <p class="text-gray-600">Devis gratuit et sans engagement adapté à votre situation.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-white">
        <div class="container mx-auto px-4">
            <div class="text-center mb-16">
                <h2 class="text-3xl md:text-4xl font-bold mb-4">Demandez votre <span class="text-accent">devis gratuit</span></h2>
                <div class="w-20 h-1 bg-accent mx-auto mb-6"></div>
                <p class="text-gray-600 max-w-2xl mx-auto">Remplissez ce formulaire pour recevoir un devis personnalisé sous 24h.</p>
            </div>
            
            <div class="max-w-3xl mx-auto bg-gray-50 p-8 rounded-lg shadow-sm">
                <form class="space-y-6">
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label for="name" class="block mb-2 font-medium">Nom complet*</label>
                            <input type="text" id="name" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                        </div>
                        <div>
                            <label for="email" class="block mb-2 font-medium">Email*</label>
                            <input type="email" id="email" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                        </div>
                    </div>
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label for="phone" class="block mb-2 font-medium">Téléphone*</label>
                            <input type="tel" id="phone" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                        </div>
                        <div>
                            <label for="ville" class="block mb-2 font-medium">Ville*</label>
                            <input type="text" id="ville" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                        </div>
                    </div>
                    <div>
                        <label for="service" class="block mb-2 font-medium">Service intéressé*</label>
                        <select id="service" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent">
                            <option value="">Sélectionnez un service</option>
                            <option value="entreprise">Nettoyage d'Entreprises</option>
                            <option value="residentiel">Nettoyage Résidentiel</option>
                            <option value="travaux">Nettoyage après Travaux</option>
                            <option value="tapis">Nettoyage de Tapis</option>
                            <option value="vitres">Nettoyage de Vitres</option>
                            <option value="ponctuel">Services Ponctuels</option>
                        </select>
                    </div>
                    <div>
                        <label for="message" class="block mb-2 font-medium">Décrivez vos besoins*</label>
                        <textarea id="message" rows="5" required class="w-full px-4 py-3 border border-gray-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-accent focus:border-transparent"></textarea>
                    </div>
                    <button type="submit" class="btn-primary px-8 py-3 rounded-lg font-medium w-full">Envoyer la demande de devis</button>
                </form>
                
                <div class="mt-8 pt-8 border-t border-gray-200">
                    <div class="flex flex-col md:flex-row items-center justify-between">
                        <div class="flex items-center mb-4 md:mb-0">
                            <i class="fas fa-phone-alt text-accent text-xl mr-4"></i>
                            <div>
                                <h4 class="font-bold">Contact téléphonique</h4>
                                <p class="text-gray-600">04 50 00 00 00</p>
                            </div>
                        </div>
                        <div class="flex items-center">
                            <i class="fas fa-envelope text-accent text-xl mr-4"></i>
                            <div>
                                <h4 class="font-bold">Contact email</h4>
                                <p class="text-gray-600">contact@rumilly-nettoyage.fr</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-primary text-white py-12">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div>
                    <h3 class="text-xl font-bold mb-4 flex items-center">
                        <i class="fas fa-broom text-accent mr-2"></i>
                        Rumilly <span class="text-accent">Nettoyage</span>
                    </h3>
                    <p class="mb-4">Entreprise locale de nettoyage professionnel implantée à Vallières-sur-Fier, Haute-Savoie.</p>
                    <div class="flex items-center">
                        <i class="fas fa-map-marker-alt text-accent mr-2"></i>
                        <span>123 Rue du Propre, 74150 Vallières-sur-Fier</span>
                    </div>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4">Zone d'intervention</h4>
                    <ul class="grid grid-cols-2 gap-2">
                        <li>Rumilly</li>
                        <li>Vallières-sur-Fier</li>
                        <li>Albens</li>
                        <li>Alby-sur-Chéran</li>
                        <li>Étercy</li>
                        <li>Marigny-Saint-Marcel</li>
                    </ul>
                </div>
                
                <div>
                    <h4 class="text-lg font-bold mb-4">Contact rapide</h4>
                    <ul class="space-y-2">
                        <li class="flex items-center">
                            <i class="fas fa-phone-alt text-accent mr-2"></i>
                            <span>04 50 00 00 00</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-envelope text-accent mr-2"></i>
                            <span>contact@rumilly-nettoyage.fr</span>
                        </li>
                        <li class="flex items-center">
                            <i class="fas fa-clock text-accent mr-2"></i>
                            <span>Lun-Ven: 8h-18h</span>
                        </li>
                    </ul>
                    <a href="#contact" class="btn-primary px-6 py-2 rounded-lg font-medium inline-block mt-4">
                        <i class="fas fa-file-alt mr-2"></i> Demander un devis
                    </a>
                </div>
            </div>
            
            <div class="border-t border-gray-700 mt-12 pt-8 text-center">
                <p>&copy; 2023 Rumilly Nettoyage - Tous droits réservés.</p>
            </div>
        </div>
    </footer>

    <!-- Back to top button -->
    <button id="back-to-top" class="fixed bottom-8 right-8 bg-accent text-white w-12 h-12 rounded-full shadow-lg flex items-center justify-center opacity-0 invisible transition-all duration-300">
        <i class="fas fa-arrow-up"></i>
    </button>

    <script>
        // Mobile menu toggle
        document.getElementById('menu-toggle').addEventListener('click', function() {
            const menu = document.getElementById('mobile-menu');
            menu.classList.toggle('hidden');
        });
        
        // Back to top button
        const backToTopButton = document.getElementById('back-to-top');
        
        window.addEventListener('scroll', function() {
            if (window.pageYOffset > 300) {
                backToTopButton.classList.remove('opacity-0', 'invisible');
                backToTopButton.classList.add('opacity-100', 'visible');
            } else {
                backToTopButton.classList.remove('opacity-100', 'visible');
                backToTopButton.classList.add('opacity-0', 'invisible');
            }
        });
        
        backToTopButton.addEventListener('click', function() {
            window.scrollTo({
                top: 0,
                behavior: 'smooth'
            });
        });
        
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                if (targetId === '#') return;
                
                const targetElement = document.querySelector(targetId);
                if (targetElement) {
                    window.scrollTo({
                        top: targetElement.offsetTop - 80,
                        behavior: 'smooth'
                    });
                    
                    // Close mobile menu if open
                    const mobileMenu = document.getElementById('mobile-menu');
                    if (!mobileMenu.classList.contains('hidden')) {
                        mobileMenu.classList.add('hidden');
                    }
                }
            });
        });
    </script>
</body>
</html>
