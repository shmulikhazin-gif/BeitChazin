<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>מלון בוטיק בית חזין | אומן | Beit Chazin Boutique Hotel Uman</title>
    <!-- Font Awesome Icons (Facebook, WhatsApp, Sauna, etc.) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Assistant:wght@300;400;600;700;800&family=Cinzel:wght@500;700;800&display=swap" rel="stylesheet">
    
    <style>
        :root {
            --royal-blue: #0A1931;
            --deep-blue: #152B52;
            --accent-blue: #185ADB;
            --neon-blue: #00d2ff;
            --gold-primary: #D4AF37;
            --gold-light: #F3E5AB;
            --dark-bg: #090C10;
            --card-bg: #111622;
            --text-light: #F5F7FA;
            --text-muted: #A0AEC0;
            --border-color: rgba(212, 175, 55, 0.25);
            --font-he: 'Assistant', sans-serif;
            --font-en: 'Cinzel', serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: var(--font-he);
            background-color: var(--dark-bg);
            color: var(--text-light);
            line-height: 1.6;
            overflow-x: hidden;
        }

        .damask-bg {
            background-color: #0b1329;
            background-image: radial-gradient(rgba(212, 175, 55, 0.08) 1px, transparent 0), radial-gradient(rgba(24, 90, 219, 0.15) 1px, #0b1329 1px);
            background-size: 40px 40px;
        }

        /* Header Navigation */
        header {
            position: fixed;
            top: 0;
            left: 0;
            right: 0;
            z-index: 1000;
            background: rgba(9, 12, 16, 0.95);
            backdrop-filter: blur(12px);
            border-bottom: 1px solid var(--border-color);
            padding: 12px 24px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo-container {
            text-decoration: none;
        }

        .glowing-logo {
            font-family: var(--font-en);
            font-weight: 800;
            font-size: 1.5rem;
            color: #ffffff;
            text-shadow: 0 0 5px #00d2ff, 0 0 10px #00d2ff, 0 0 20px #185ADB;
            letter-spacing: 1px;
            line-height: 1.1;
        }

        .glowing-logo span {
            display: block;
            font-size: 0.6rem;
            color: var(--gold-light);
            text-shadow: 0 0 5px var(--gold-primary);
            letter-spacing: 2px;
        }

        .nav-actions {
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .btn-lang {
            background: rgba(212, 175, 55, 0.15);
            border: 1px solid var(--gold-primary);
            color: var(--gold-light);
            padding: 6px 12px;
            border-radius: 20px;
            cursor: pointer;
            font-weight: 600;
            display: flex;
            align-items: center;
            gap: 5px;
        }

        .fb-nav-btn {
            background: #1877F2;
            color: #ffffff;
            padding: 8px 14px;
            border-radius: 20px;
            text-decoration: none;
            font-weight: 600;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        .wa-nav-btn {
            background: #25D366;
            color: #ffffff;
            padding: 8px 14px;
            border-radius: 20px;
            text-decoration: none;
            font-weight: 700;
            font-size: 0.85rem;
            display: flex;
            align-items: center;
            gap: 6px;
        }

        /* Hero Banner */
        .hero {
            min-height: 90vh;
            padding-top: 100px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: linear-gradient(180deg, rgba(9, 12, 16, 0.75) 0%, rgba(13, 25, 49, 0.9) 100%),
                        url('https://images.unsplash.com/photo-1566073771259-6a8506099945?auto=format&fit=crop&w=1920&q=80') center/cover no-repeat;
            text-align: center;
        }

        .renaissance-frame {
            border: 2px solid var(--gold-primary);
            padding: 35px 25px;
            background: rgba(10, 25, 49, 0.85);
            backdrop-filter: blur(10px);
            border-radius: 8px;
            max-width: 800px;
            margin: 20px;
        }

        .hero-title-glowing {
            font-family: var(--font-en);
            font-size: 2.5rem;
            color: #ffffff;
            text-shadow: 0 0 10px #00d2ff, 0 0 20px #00d2ff, 0 0 30px #185ADB;
        }

        .hero-subtitle {
            font-size: 1.3rem;
            color: var(--gold-light);
            margin-bottom: 20px;
        }

        .location-badge {
            display: inline-flex;
            align-items: center;
            gap: 8px;
            background: rgba(212, 175, 55, 0.2);
            border: 1px solid var(--gold-primary);
            padding: 8px 16px;
            border-radius: 25px;
            font-size: 1rem;
            font-weight: 700;
            margin-bottom: 15px;
        }

        .hill-notice {
            background: rgba(24, 90, 219, 0.25);
            border-right: 4px solid var(--neon-blue);
            padding: 10px 15px;
            border-radius: 4px;
            font-size: 0.9rem;
            color: #d1e8ff;
            margin-bottom: 20px;
            text-align: right;
        }

        html[dir="ltr"] .hill-notice {
            border-right: none;
            border-left: 4px solid var(--neon-blue);
            text-align: left;
        }

        .btn-primary-wa {
            background: linear-gradient(135deg, #25D366, #128C7E);
            color: white;
            padding: 12px 28px;
            border-radius: 30px;
            text-decoration: none;
            font-size: 1rem;
            font-weight: 700;
            display: inline-flex;
            align-items: center;
            gap: 8px;
        }

        /* Sections */
        section {
            padding: 60px 20px;
            max-width: 1100px;
            margin: 0 auto;
        }

        .section-title {
            text-align: center;
            margin-bottom: 40px;
        }

        .section-title h2 {
            font-size: 2rem;
            color: var(--gold-light);
        }

        /* Mikveh Section */
        .mikveh-card {
            background: var(--card-bg);
            border: 1px solid var(--gold-primary);
            border-radius: 12px;
            padding: 30px;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            align-items: center;
        }

        .mikveh-img {
            width: 100%;
            height: 280px;
            object-fit: cover;
            border-radius: 8px;
            border: 1px solid var(--border-color);
        }

        .mikveh-list {
            list-style: none;
            margin: 15px 0;
        }

        .mikveh-list li {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
            color: var(--text-light);
        }

        .mikveh-list i {
            color: var(--gold-primary);
        }

        /* Facebook Section */
        .fb-card {
            background: linear-gradient(135deg, #0d2347, #0a1931);
            border: 1px solid #1877F2;
            padding: 30px;
            border-radius: 12px;
            text-align: center;
        }

        /* Footer */
        footer {
            background: #05070a;
            border-top: 1px solid var(--border-color);
            padding: 30px 20px;
            text-align: center;
        }

        .footer-socials {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 15px 0;
        }

        .footer-socials a {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: white;
            text-decoration: none;
        }

        .floating-wa {
            position: fixed;
            bottom: 20px;
            left: 20px;
            background: #25D366;
            color: white;
            width: 55px;
            height: 55px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.5);
            text-decoration: none;
            z-index: 999;
        }

        html[dir="ltr"] .floating-wa { left: auto; right: 20px; }

        @media (max-width: 768px) {
            .mikveh-card { grid-template-columns: 1fr; }
            .fb-nav-btn span, .wa-nav-btn span { display: none; }
        }
    </style>
</head>
<body class="damask-bg">

    <!-- Header -->
    <header>
        <a href="#" class="logo-container">
            <div class="glowing-logo">
                BEIT CHAZIN
                <span>BOUTIQUE HOTEL</span>
            </div>
        </a>

        <div class="nav-actions">
            <button class="btn-lang" onclick="toggleLanguage()">
                <i class="fa-solid fa-globe"></i>
                <span id="langLabel">English</span>
            </button>

            <a href="https://www.facebook.com/smw.l.ywsp.hzyn" target="_blank" class="fb-nav-btn">
                <i class="fab fa-facebook-f"></i>
                <span data-i18n="fbNav">פייסבוק</span>
            </a>

            <a href="https://wa.me/972509558399" target="_blank" class="wa-nav-btn">
                <i class="fab fa-whatsapp"></i>
                <span data-i18n="waNav">וואצאפ</span>
            </a>
        </div>
    </header>

    <!-- Hero Banner -->
    <div class="hero">
        <div class="renaissance-frame">
            <div class="hero-title-glowing">BEIT CHAZIN</div>
            <div class="hero-subtitle" data-i18n="hotelSubtitle">מלון בוטיק בית חזין - אומן</div>
            
            <div class="location-badge">
                <i class="fa-solid fa-person-walking"></i>
                <span data-i18n="distText">2 דקות הליכה מהציון הקדוש של רבי נחמן מברסלב</span>
            </div>

            <div class="hill-notice">
                <i class="fa-solid fa-mountain-city"></i>
                <span data-i18n="hillNotice">שימו לב: הדרך לציון כוללת עלייה/גבעה קצרה של כ-2 דקות הליכה בלבד.</span>
            </div>

            <a href="https://wa.me/972509558399?text=%D7%A9%D7%9C%D7%95%D7%9D%20%D7%91%D7%99%D7%AA%20%D7%97%D7%96%D7%99%D7%9F%2C%20%D7%90%D7%A9%D7%9E%D7%97%20%D7%9C%D7%A7%D7%91%D7%9C%20%D7%A4%D7%A8%D7%90%D7%99%D7%9D%20%D7%A2%D7%9C%20%D7%97%D7%93%D7%A8%D7%99%D7%9D" target="_blank" class="btn-primary-wa">
                <i class="fab fa-whatsapp"></i>
                <span data-i18n="heroWaBtn">להזמנה מהירה בוואצאפ</span>
            </a>
        </div>
    </div>

    <!-- Mikveh & Sauna Section -->
    <section>
        <div class="section-title">
            <h2 data-i18n="mikvehTitle">מקווה טהרה וסאונה במלון</h2>
        </div>
        <div class="mikveh-card">
            <img src="https://images.unsplash.com/photo-1584622650111-993a426fbf0a?auto=format&fit=crop&w=800&q=80" alt="מקווה וסאונה" class="mikveh-img">
            <div>
                <h3 style="color: var(--gold-light); margin-bottom: 10px;" data-i18n="mikvehHead">מקווה מחומם ונקי תמיד</h3>
                <p style="color: var(--text-muted); margin-bottom: 15px;" data-i18n="mikvehDesc">לרווחת האורחים במלון בית חזין באומן – מקווה טהרה מהודר, מתוחזק ברמת ניקיון קפדנית ביותר, עם מים חמים ומתחם סאונה מפנק.</p>
                
                <ul class="mikveh-list">
                    <li><i class="fa-solid fa-temperature-arrow-up"></i> <span data-i18n="m1">מים חמים ומפונקים 24/7</span></li>
                    <li><i class="fa-solid fa-sparkles"></i> <span data-i18n="m2">נקי, סטרילי ומתוחזק באופן קבוע</span></li>
                    <li><i class="fa-solid fa-hot-tub-person"></i> <span data-i18n="m3">סאונה מרעננת ומפנקת</span></li>
                </ul>

                <a href="https://wa.me/972509558399?text=%D7%A9%D7%9C%D7%95%D7%9D%20%D7%90%D7%A9%D7%9E%D7%97%20%D7%9C%D7%A7%D7%91%D7%9C%20%D7%A4%D7%A8%D7%90%D7%99%D7%9D%20%D7%A2%D7%9C%20%D7%94%D7%9E%D7%A7%D7%95%D7%95%D7%94" target="_blank" class="btn-primary-wa" style="margin-top: 10px;">
                    <i class="fab fa-whatsapp"></i>
                    <span data-i18n="mikvehWa">לבירור על המקווה בוואצאפ</span>
                </a>
            </div>
        </div>
    </section>

    <!-- Facebook Section -->
    <section>
        <div class="fb-card">
            <i class="fab fa-facebook-f" style="font-size: 3rem; color: #1877F2; margin-bottom: 10px;"></i>
            <h2 style="color: white; margin-bottom: 10px;" data-i18n="fbTitle">עקבו אחרינו בפייסבוק</h2>
            <p style="color: var(--text-muted); margin-bottom: 20px;" data-i18n="fbDesc">עדכונים, תמונות וחדשות ממלון בית חזין באומן</p>
            <a href="https://www.facebook.com/smw.l.ywsp.hzyn" target="_blank" class="fb-nav-btn" style="display: inline-flex; padding: 10px 24px;">
                <i class="fab fa-facebook-f"></i>
                <span data-i18n="fbBtn">מעבר לעמוד הפייסבוק</span>
            </a>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <div class="glowing-logo" style="font-size: 1.2rem;">
            BEIT CHAZIN
            <span>BOUTIQUE HOTEL • UMAN</span>
        </div>
        <div class="footer-socials">
            <a href="https://www.facebook.com/smw.l.ywsp.hzyn" target="_blank" style="background: #1877F2;"><i class="fab fa-facebook-f"></i></a>
            <a href="https://wa.me/972509558399" target="_blank" style="background: #25D366;"><i class="fab fa-whatsapp"></i></a>
        </div>
        <p style="color: var(--text-muted); font-size: 0.85rem;">© מלון בוטיק בית חזין • אומן, אוקראינה</p>
    </footer>

    <!-- Floating WhatsApp Button -->
    <a href="https://wa.me/972509558399" target="_blank" class="floating-wa">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- Language Script -->
    <script>
        const translations = {
            he: {
                fbNav: "פייסבוק",
                waNav: "וואצאפ",
                hotelSubtitle: "מלון בוטיק בית חזין - אומן",
                distText: "2 דקות הליכה מהציון הקדוש של רבי נחמן מברסלב",
                hillNotice: "שימו לב: הדרך לציון כוללת עלייה/גבעה קצרה של כ-2 דקות הליכה בלבד.",
                heroWaBtn: "להזמנה מהירה בוואצאפ",
                mikvehTitle: "מקווה טהרה וסאונה במלון",
                mikvehHead: "מקווה מחומם ונקי תמיד",
                mikvehDesc: "לרווחת האורחים במלון בית חזין באומן – מקווה טהרה מהודר, מתוחזק ברמת ניקיון קפדנית ביותר, עם מים חמים ומתחם סאונה מפנק.",
                m1: "מים חמים ומפונקים 24/7",
                m2: "נקי, סטרילי ומתוחזק באופן קבוע",
                m3: "סאונה מרעננת ומפנקת",
                mikvehWa: "לבירור על המקווה בוואצאפ",
                fbTitle: "עקבו אחרינו בפייסבוק",
                fbDesc: "עדכונים, תמונות וחדשות ממלון בית חזין באומן",
                fbBtn: "מעבר לעמוד הפייסבוק"
            },
            en: {
                fbNav: "Facebook",
                waNav: "WhatsApp",
                hotelSubtitle: "Beit Chazin Boutique Hotel - Uman",
                distText: "2-Minute Walk to Rabbi Nachman's Holy Tziyon",
                hillNotice: "Note: The walk to the Tziyon includes a short 2-minute hill incline.",
                heroWaBtn: "Quick WhatsApp Booking",
                mikvehTitle: "On-Site Mikveh & Sauna",
                mikvehHead: "Heated & Impeccably Clean Mikveh",
                mikvehDesc: "For guests at Beit Chazin Hotel in Uman – fully heated Mikveh, strictly maintained cleanliness, and relaxing sauna facilities.",
                m1: "Heated water 24/7",
                m2: "Pristine, sanitized, and regularly maintained",
                m3: "Relaxing on-site sauna",
                mikvehWa: "Inquire via WhatsApp",
                fbTitle: "Follow Us on Facebook",
                fbDesc: "Photos, news, and updates from Beit Chazin Hotel Uman",
                fbBtn: "Visit Facebook Page"
            }
        };

        let currentLang = 'he';

        function toggleLanguage() {
            currentLang = currentLang === 'he' ? 'en' : 'he';
            document.documentElement.lang = currentLang;
            document.documentElement.dir = currentLang === 'he' ? 'rtl' : 'ltr';

            document.getElementById('langLabel').textContent = currentLang === 'he' ? 'English' : 'עברית';

            document.querySelectorAll('[data-i18n]').forEach(elem => {
                const key = elem.getAttribute('data-i18n');
                if (translations[currentLang][key]) {
                    elem.textContent = translations[currentLang][key];
                }
            });
        }
    </script>
</body>
</html>
