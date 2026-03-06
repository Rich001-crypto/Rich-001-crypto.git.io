<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=yes">
    <title>CEMCC ASBL - Accompagnement recherche</title>
    <!-- Police Roboto -->
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap" rel="stylesheet">
    <!-- Font Awesome pour les icônes -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <!-- Manifest PWA -->
    <link rel="manifest" href="data:application/manifest+json,%7B%22name%22%3A%22CEMCC%20ASBL%22%2C%22short_name%22%3A%22CEMCC%22%2C%22start_url%22%3A%22.%2F%22%2C%22display%22%3A%22standalone%22%2C%22background_color%22%3A%22%230A2472%22%2C%22theme_color%22%3A%22%230A2472%22%2C%22icons%22%3A%5B%7B%22src%22%3A%22data:image%2Fpng%3Bbase64%2CiVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAAAARzQklUCAgICHwIZIgAAAItSURBVFiF7Zc9aBNhHMZ%2Fz71c70pTa7FWJRAIhaB10A4WioMu6iQ6KXaqm4OLdBOcBO0o%2BgE6CIJzFx18%2BwEURKUIkSq0WKmkH3CN5nK53r1cBmlKmt7lLmlS8Vl%2BeN7nf%2B%2F7vM%2FzD%2F%2F%2Fv0IYqJ63mK6iHGGKOsI0LYiC5s%2BjjDDCiB2q6y3T%2Fv0QJk0LUv3E8a1dajdPM30jRZxZxV7aYfB8jqXXL9hYzzHb%2B4DJ2Z9I8QrK0hZh4uTfLqD7Hk3rLcaLLeaaFabmLcKLB%2FHOvcY5e4lwY4vBqxf4e38RjgBptUjaLiAk%2Fp2Az0e23r6gdGmUY%2B0LonNtCikCQkCEAEJARASEEAiIhxKQVitM35xh4nwLI%2BeayHMHkWcPIk41IKbriGINUWkiHrURD9uI%2Bw7iQQv%2BrQV%2BvYqcbSY8%2FwR57hBytoF4upF4qoF4VId4WIM4X0Mcr8I%2FVmD9xgRjBwqE524R3jYRL%2BuR79eR9y3k7yrkz2XkrzLyZwl5U0LeLCF%2FvIu8WkR%2BKyLvimQ%2Bnue2meZq9jT5yT%2FsBwFdE2fFQrQtiLpY8yLhGm%2B8B1z3T2I%2F%2FMb%2BrOj2bPvyG4h0rA%2FBpvh5GnHgUwS%2BTDv%2FKt2u1lE5FQK6Je64FyHl9wR8%2FqBdWgN%2BQ5Xp%2F5BwDXi%2FlVp38H5tkT5XI%2FvOBZnuH%2BzgI71OqI83dP0dxnfjPmN3%2F2gHmwVEF%2B0i3fU7wHcHf3mN5Gqacq7CWP5Xx26N%2FrZxH66RHyuRHyqQ7yqQb8qQr0qQNyVyv4g8L5CfCpAf85Af8uTv5hk9VkTK2iJz%2Fllk5iiZ1WlSpaPkH2cpHq7h%2Bt5tPnh5vCeKeNco4m2jiPd1It7WIr7UIL5UyH0vIu8L5E0B%2BbKAvM%2BDvM2Tt%2FKMzB4j%2B79d2f%2FbYv9vU8r%2FAk7LM56fJJk%2Fc2yBAAAAAElFTkSuQmCC%22%2C%22sizes%22%3A%22192x192%22%2C%22type%22%3A%22image%2Fpng%22%7D%5D%7D">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Roboto', sans-serif;
        }

        body {
            background-color: #f5f5f5;
            color: #333;
            display: flex;
            flex-direction: column;
            min-height: 100vh;
        }

        /* Couleurs de la charte */
        :root {
            --primary: #0A2472;
            --secondary: #2E8B57;
            --white: #FFFFFF;
            --light-bg: #f9f9f9;
            --gray: #e0e0e0;
        }

        /* En-tête */
        header {
            background-color: var(--primary);
            color: var(--white);
            padding: 15px 20px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }

        .logo-container {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo-container i {
            font-size: 2.5rem;
            color: var(--secondary);
        }

        .logo-container h1 {
            font-size: 1.5rem;
            font-weight: 500;
        }

        .logo-container span {
            font-size: 0.9rem;
            opacity: 0.9;
            display: block;
        }

        /* Navigation */
        nav {
            background-color: var(--white);
            padding: 10px 20px;
            box-shadow: 0 2px 5px rgba(0,0,0,0.05);
            position: sticky;
            top: 0;
            z-index: 10;
        }

        nav ul {
            display: flex;
            list-style: none;
            justify-content: space-around;
            gap: 15px;
        }

        nav ul li a {
            text-decoration: none;
            color: var(--primary);
            font-weight: 500;
            padding: 8px 12px;
            border-radius: 20px;
            transition: background 0.3s;
            display: flex;
            flex-direction: column;
            align-items: center;
            font-size: 0.9rem;
        }

        nav ul li a i {
            font-size: 1.3rem;
            margin-bottom: 4px;
        }

        nav ul li a.active, nav ul li a:hover {
            background-color: var(--secondary);
            color: var(--white);
        }

        /* Contenu principal */
        main {
            flex: 1;
            padding: 20px;
            max-width: 1200px;
            margin: 0 auto;
            width: 100%;
        }

        section {
            display: none;
        }

        section.active-section {
            display: block;
        }

        /* Cartes et éléments */
        .card {
            background: var(--white);
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 20px;
            box-shadow: 0 2px 8px rgba(0,0,0,0.05);
            border-left: 4px solid var(--secondary);
        }

        .card h3 {
            color: var(--primary);
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 8px;
        }

        .badge {
            background: var(--secondary);
            color: white;
            padding: 4px 8px;
            border-radius: 20px;
            font-size: 0.75rem;
            font-weight: 500;
            display: inline-block;
        }

        /* Grille pour services */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .service-item {
            background: var(--white);
            border-radius: 12px;
            padding: 20px;
            box-shadow: 0 4px 12px rgba(10,36,114,0.1);
            transition: transform 0.2s;
            cursor: pointer;
            border: 1px solid var(--gray);
        }

        .service-item:hover {
            transform: translateY(-5px);
            border-color: var(--secondary);
        }

        .service-icon {
            font-size: 2.5rem;
            color: var(--secondary);
            margin-bottom: 10px;
        }

        .service-title {
            font-size: 1.2rem;
            font-weight: 600;
            color: var(--primary);
        }

        .service-price {
            color: var(--secondary);
            font-weight: 500;
            margin: 10px 0;
        }

        .service-desc {
            color: #555;
            font-size: 0.95rem;
            line-height: 1.5;
        }

        /* Fil d'actualités */
        .actualite-item {
            background: var(--white);
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 20px;
            border-left: 4px solid var(--primary);
        }

        .actualite-date {
            color: var(--secondary);
            font-size: 0.85rem;
            font-weight: 500;
            display: flex;
            align-items: center;
            gap: 5px;
            margin-bottom: 8px;
        }

        .actualite-content {
            margin: 15px 0;
        }

        .actualite-actions {
            display: flex;
            gap: 15px;
            margin-top: 10px;
        }

        .actualite-actions button {
            background: none;
            border: none;
            color: var(--primary);
            cursor: pointer;
            font-size: 0.9rem;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .actualite-actions button:hover {
            color: var(--secondary);
        }

        /* Formulaire de contact */
        .contact-form {
            background: var(--white);
            padding: 25px;
            border-radius: 12px;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            font-weight: 500;
            color: var(--primary);
        }

        .form-group input, .form-group textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            font-size: 1rem;
        }

        .form-group textarea {
            min-height: 120px;
            resize: vertical;
        }

        .btn {
            background: var(--primary);
            color: white;
            border: none;
            padding: 14px 25px;
            border-radius: 30px;
            font-size: 1rem;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.3s;
            width: 100%;
        }

        .btn:hover {
            background: var(--secondary);
        }

        /* Bouton WhatsApp flottant */
        .whatsapp-float {
            position: fixed;
            bottom: 30px;
            right: 20px;
            background-color: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 2rem;
            box-shadow: 0 4px 12px rgba(0,0,0,0.2);
            z-index: 100;
            transition: transform 0.3s;
            text-decoration: none;
        }

        .whatsapp-float:hover {
            transform: scale(1.1);
        }

        /* Pied de page */
        footer {
            background: var(--primary);
            color: white;
            text-align: center;
            padding: 20px;
            margin-top: 30px;
            font-size: 0.9rem;
        }

        footer a {
            color: var(--secondary);
            text-decoration: none;
            font-weight: 500;
        }

        /* Media queries pour mobile */
        @media (max-width: 600px) {
            header {
                flex-direction: column;
                text-align: center;
            }
            .logo-container {
                justify-content: center;
            }
            nav ul {
                flex-wrap: wrap;
            }
            nav ul li a {
                font-size: 0.8rem;
                padding: 6px 8px;
            }
            nav ul li a i {
                font-size: 1.2rem;
            }
        }

        /* Cache pour offline */
        .offline-note {
            background: #ffecb3;
            padding: 8px;
            text-align: center;
            font-size: 0.85rem;
            display: none;
        }
    </style>
</head>
<body>
    <div class="offline-note" id="offlineNote">
        <i class="fas fa-wifi-slash"></i> Mode hors ligne - certaines données peuvent ne pas être à jour.
    </div>

    <header>
        <div class="logo-container">
            <i class="fas fa-leaf"></i>
            <div>
                <h1>CEMCC ASBL</h1>
                <span>Collège d'Étudiants et Médecins Chrétiens Chercheurs</span>
            </div>
        </div>
        <div class="header-mission">
            <p><i class="fas fa-bullseye" style="color: var(--secondary);"></i> Accompagnement des finalistes en RDC</p>
        </div>
    </header>

    <nav>
        <ul>
            <li><a href="#" data-section="accueil" class="active"><i class="fas fa-home"></i>Accueil</a></li>
            <li><a href="#" data-section="services"><i class="fas fa-cogs"></i>Services</a></li>
            <li><a href="#" data-section="actualites"><i class="fas fa-newspaper"></i>Actualités</a></li>
            <li><a href="#" data-section="contact"><i class="fas fa-envelope"></i>Contact</a></li>
        </ul>
    </nav>

    <main>
        <!-- Section Accueil -->
        <section id="accueil" class="active-section">
            <div class="card">
                <h3><i class="fas fa-info-circle"></i> Qui sommes-nous ?</h3>
                <p>Le <strong>CEMCC ASBL</strong> (Collège d'Étudiants et Médecins Chrétiens Chercheurs) est une organisation basée à Goma (Nord-Kivu, RDC) spécialisée dans l'accompagnement des étudiants finalistes pour leurs travaux de recherche.</p>
                <p style="margin-top: 15px;">Nous offrons une gamme complète de services : rédaction de mémoires/TFC, analyse de données, conception de questionnaires, formations, collecte terrain, et soutenance.</p>
            </div>

            <div class="services-grid" style="grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));">
                <div class="service-item" onclick="window.location='#services'">
                    <i class="fas fa-pen-fancy service-icon"></i>
                    <div class="service-title">Rédaction</div>
                    <p class="service-desc">Mémoires, TFC, articles scientifiques</p>
                </div>
                <div class="service-item" onclick="window.location='#services'">
                    <i class="fas fa-chart-bar service-icon"></i>
                    <div class="service-title">Analyse données</div>
                    <p class="service-desc">SPSS, Excel/XLStat, Power BI</p>
                </div>
                <div class="service-item" onclick="window.location='#services'">
                    <i class="fas fa-clipboard-list service-icon"></i>
                    <div class="service-title">Questionnaires</div>
                    <p class="service-desc">Conception sur Kobocollect</p>
                </div>
            </div>

            <div class="card" style="margin-top: 20px;">
                <h3><i class="fas fa-calendar-alt"></i> Prochain événement</h3>
                <p><strong>Atelier sur les méthodes de recherche</strong> - 15 avril 2025 à Goma. Inscriptions ouvertes !</p>
                <a href="#actualites" style="color: var(--secondary); font-weight: 500;">Voir toutes les actualités →</a>
            </div>
        </section>

        <!-- Section Services -->
        <section id="services">
            <h2 style="color: var(--primary); margin-bottom: 20px;">Nos Services</h2>
            <div class="services-grid" id="servicesContainer"></div>
        </section>

        <!-- Section Actualités -->
        <section id="actualites">
            <h2 style="color: var(--primary); margin-bottom: 20px;">Actualités et Événements</h2>
            <div id="actualitesContainer"></div>
        </section>

        <!-- Section Contact -->
        <section id="contact">
            <h2 style="color: var(--primary); margin-bottom: 20px;">Contactez-nous</h2>
            <div class="contact-form">
                <form id="contactForm">
                    <div class="form-group">
                        <label><i class="fas fa-user"></i> Nom complet</label>
                        <input type="text" id="name" required placeholder="Votre nom">
                    </div>
                    <div class="form-group">
                        <label><i class="fas fa-envelope"></i> Email</label>
                        <input type="email" id="email" required placeholder="votre@email.com">
                    </div>
                    <div class="form-group">
                        <label><i class="fas fa-comment"></i> Message</label>
                        <textarea id="message" required placeholder="Votre message..."></textarea>
                    </div>
                    <button type="submit" class="btn">Envoyer <i class="fas fa-paper-plane"></i></button>
                </form>
                <p style="text-align: center; margin-top: 15px; color: #777; font-size: 0.9rem;">Ou contactez-nous directement sur WhatsApp</p>
            </div>

            <div class="card" style="margin-top: 20px;">
                <h3><i class="fas fa-map-marker-alt"></i> Adresse</h3>
                <p>Goma, Nord-Kivu, RDC</p>
                <p><i class="fas fa-phone-alt"></i> +243 975 121 886</p>
                <p><i class="fas fa-envelope"></i> contact@cemcc-asbl.org</p>
                <div style="display: flex; gap: 15px; margin-top: 15px;">
                    <a href="#" style="color: var(--primary); font-size: 1.5rem;"><i class="fab fa-facebook"></i></a>
                    <a href="#" style="color: var(--primary); font-size: 1.5rem;"><i class="fab fa-twitter"></i></a>
                    <a href="#" style="color: var(--primary); font-size: 1.5rem;"><i class="fab fa-linkedin"></i></a>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 CEMCC ASBL - Tous droits réservés</p>
        <p><a href="#">Mentions légales</a> | <a href="#">Confidentialité</a></p>
    </footer>

    <a href="https://wa.me/243975121886" class="whatsapp-float" target="_blank">
        <i class="fab fa-whatsapp"></i>
    </a>

    <script>
        // Données statiques (simulation d'une base de données)
        const servicesData = [
            {
                id: 1,
                titre: "Rédaction complète de mémoires/TFC",
                description: "Rédaction de qualité, respect des normes académiques, assistance jusqu'à la soutenance.",
                prix: "À partir de 150$",
                icone: "fa-pen-fancy"
            },
            {
                id: 2,
                titre: "Analyse de données",
                description: "SPSS, Excel/XLStat, Power BI. Traitement statistique, interprétation des résultats.",
                prix: "À partir de 100$",
                icone: "fa-chart-bar"
            },
            {
                id: 3,
                titre: "Conception de questionnaires",
                description: "Création sur Kobocollect, optimisation pour la collecte terrain.",
                prix: "À partir de 50$",
                icone: "fa-clipboard-list"
            },
            {
                id: 4,
                titre: "Formations",
                description: "Formation aux outils de collecte (Kobocollect, ODK) et à la méthodologie de recherche.",
                prix: "Sur devis",
                icone: "fa-chalkboard-teacher"
            },
            {
                id: 5,
                titre: "Accompagnement méthodologique",
                description: "Suivi personnalisé, correction, conseils pour la rédaction.",
                prix: "À partir de 80$",
                icone: "fa-user-graduate"
            },
            {
                id: 6,
                titre: "Collecte terrain",
                description: "Déploiement d'enquêteurs, supervision, saisie des données.",
                prix: "Sur devis",
                icone: "fa-people-arrows"
            },
            {
                id: 7,
                titre: "Présentations PowerPoint",
                description: "Réalisation de slides professionnelles pour la soutenance.",
                prix: "À partir de 40$",
                icone: "fa-file-powerpoint"
            }
        ];

        const actualitesData = [
            {
                id: 1,
                titre: "Atelier sur les méthodes de recherche",
                date: "2025-04-15",
                contenu: "Le CEMCC organise un atelier pratique sur les méthodes de recherche à Goma. Inscrivez-vous dès maintenant !",
                image: null,
                lien: "#"
            },
            {
                id: 2,
                titre: "Nouveau service : Analyse Power BI",
                date: "2025-03-28",
                contenu: "Nous proposons désormais des tableaux de bord interactifs avec Power BI pour vos mémoires.",
                image: null,
                lien: "#"
            },
            {
                id: 3,
                titre: "Offre spéciale pour les finalistes",
                date: "2025-03-15",
                contenu: "Bénéficiez de 10% de réduction sur tout service de rédaction jusqu'au 30 avril.",
                image: null,
                lien: "#"
            }
        ];

        // Remplir les services
        function renderServices() {
            const container = document.getElementById('servicesContainer');
            container.innerHTML = '';
            servicesData.forEach(service => {
                const div = document.createElement('div');
                div.className = 'service-item';
                div.innerHTML = `
                    <i class="fas ${service.icone} service-icon"></i>
                    <div class="service-title">${service.titre}</div>
                    <div class="service-price">${service.prix}</div>
                    <p class="service-desc">${service.description}</p>
                `;
                container.appendChild(div);
            });
        }

        // Remplir les actualités
        function renderActualites() {
            const container = document.getElementById('actualitesContainer');
            container.innerHTML = '';
            actualitesData.sort((a,b) => new Date(b.date) - new Date(a.date)).forEach(actu => {
                const div = document.createElement('div');
                div.className = 'actualite-item';
                const dateFormatee = new Date(actu.date).toLocaleDateString('fr-FR', { year: 'numeric', month: 'long', day: 'numeric' });
                div.innerHTML = `
                    <div class="actualite-date"><i class="far fa-calendar-alt"></i> ${dateFormatee}</div>
                    <h3 style="color: var(--primary);">${actu.titre}</h3>
                    <div class="actualite-content">${actu.contenu}</div>
                    <div class="actualite-actions">
                        <button onclick="partagerActu('${actu.titre}', '${actu.contenu}')"><i class="fas fa-share-alt"></i> Partager</button>
                        ${actu.lien ? `<a href="${actu.lien}" style="color: var(--primary);"><i class="fas fa-link"></i> Lire plus</a>` : ''}
                    </div>
                `;
                container.appendChild(div);
            });
        }

        // Fonction de partage (via WhatsApp si possible)
        function partagerActu(titre, contenu) {
            const texte = `*${titre}*\n${contenu}\n\nVia CEMCC ASBL`;
            const url = `https://wa.me/?text=${encodeURIComponent(texte)}`;
            window.open(url, '_blank');
        }

        // Navigation
        const sections = document.querySelectorAll('section');
        const navLinks = document.querySelectorAll('nav ul li a');

        function showSection(sectionId) {
            sections.forEach(s => s.classList.remove('active-section'));
            document.getElementById(sectionId).classList.add('active-section');
            navLinks.forEach(link => {
                link.classList.remove('active');
                if (link.dataset.section === sectionId) {
                    link.classList.add('active');
                }
            });
            // Sauvegarder dans localStorage
            localStorage.setItem('lastSection', sectionId);
        }

        navLinks.forEach(link => {
            link.addEventListener('click', (e) => {
                e.preventDefault();
                const sectionId = link.dataset.section;
                showSection(sectionId);
            });
        });

        // Restaurer la dernière section visitée
        const lastSection = localStorage.getItem('lastSection') || 'accueil';
        showSection(lastSection);

        // Gestion du formulaire de contact (simulation)
        document.getElementById('contactForm').addEventListener('submit', (e) => {
            e.preventDefault();
            alert('Merci pour votre message. Nous vous répondrons dans les plus brefs délais (simulation).');
            e.target.reset();
        });

        // Rendu initial
        renderServices();
        renderActualites();

        // Détection hors ligne (pour notifier)
        window.addEventListener('load', () => {
            if (!navigator.onLine) {
                document.getElementById('offlineNote').style.display = 'block';
            }
        });
        window.addEventListener('online', () => {
            document.getElementById('offlineNote').style.display = 'none';
        });
        window.addEventListener('offline', () => {
            document.getElementById('offlineNote').style.display = 'block';
        });

        // Service Worker pour PWA (offline)
        if ('serviceWorker' in navigator) {
            navigator.serviceWorker.register('service-worker.js')
                .then(reg => console.log('Service Worker enregistré', reg))
                .catch(err => console.error('Erreur SW', err));
        }
    </script>

    <!-- Service Worker (intégré en base64 pour rester dans un seul fichier, mais normalement fichier à part) -->
    <script id="serviceWorker">
        // Ceci serait le contenu du fichier service-worker.js
        // Pour l'utiliser, il faut créer un fichier séparé.
        // Voici le code à copier dans service-worker.js :
        /*
        const CACHE_NAME = 'cemcc-cache-v1';
        const urlsToCache = [
            '/',
            '/index.html',
            'https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap',
            'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css'
        ];

        self.addEventListener('install', event => {
            event.waitUntil(
                caches.open(CACHE_NAME)
                    .then(cache => cache.addAll(urlsToCache))
            );
        });

        self.addEventListener('fetch', event => {
            event.respondWith(
                caches.match(event.request)
                    .then(response => response || fetch(event.request))
            );
        });
        */
    </script>
    <script>
        // Pour simplifier, on peut créer le service worker dynamiquement (si en ligne)
        if ('serviceWorker' in navigator) {
            // Créer un blob avec le code du service worker
            const swCode = `
                const CACHE_NAME = 'cemcc-cache-v1';
                const urlsToCache = [
                    './',
                    './index.html',
                    'https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap',
                    'https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css'
                ];

                self.addEventListener('install', event => {
                    event.waitUntil(
                        caches.open(CACHE_NAME)
                            .then(cache => cache.addAll(urlsToCache))
                    );
                });

                self.addEventListener('fetch', event => {
                    event.respondWith(
                        caches.match(event.request)
                            .then(response => response || fetch(event.request))
                    );
                });
            `;
            const blob = new Blob([swCode], { type: 'application/javascript' });
            const swUrl = URL.createObjectURL(blob);
            navigator.serviceWorker.register(swUrl)
                .then(reg => console.log('Service Worker enregistré via blob'))
                .catch(err => console.error('Erreur SW blob', err));
        }
    </script>
</body>
</html>
