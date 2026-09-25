<!DOCTYPE html>
<html lang="fa" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>میلاد یوسفی | مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی</title>
    <meta name="description" content="میلاد یوسفی - مهندس راه‌اندازی بیسیم موتورولا، شبکه‌های رادیویی و سایت‌های تکرارکننده در قائمشهر، مازندران و سراسر ایران. همکاری با شرکت امیدان صنعت.">
    <meta name="keywords" content="مهندس بیسیم, راه اندازی بیسیم, مهندس راه اندازی بیسیم, راه اندازی بیسیم موتورولا, راه اندازی سایت بیسیم, شرکت امیدان صنعت, بیسیم مازندران, بیسیم قائمشهر, 09048818508">
    
    <!-- فونت استاندارد و زیبای وزیرمتن -->
    <link href="https://cdn.jsdelivr.net/gh/rastikerdar/vazirmatn@v33.003/Vazirmatn-font-face.css" rel="stylesheet" type="text/css" />

    <style>
        :root {
            --bg-dark: #070a14;
            --bg-card: rgba(15, 23, 42, 0.75);
            --blue-glow: #3b82f6;
            --gold-primary: #f59e0b;
            --gold-light: #fbbf24;
            --gold-gradient: linear-gradient(135deg, #d97706 0%, #f59e0b 50%, #fef08a 100%);
            --blue-gradient: linear-gradient(135deg, #1e3a8a 0%, #3b82f6 100%);
            --text-main: #f8fafc;
            --text-sub: #94a3b8;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Vazirmatn', sans-serif;
        }

        body {
            background-color: var(--bg-dark);
            color: var(--text-main);
            line-height: 1.8;
            overflow-x: hidden;
            position: relative;
            min-height: 100vh;
        }

        /* --- پس‌زمینه زنده امواج رادیویی --- */
        .radio-waves-bg {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            background: radial-gradient(circle at 50% 15%, #0f1c3f 0%, #070a14 75%);
            overflow: hidden;
        }

        .wave-line {
            position: absolute;
            width: 200%;
            height: 200%;
            top: -50%;
            left: -50%;
            background: repeating-radial-gradient(
                circle at 50% 30%,
                transparent 0,
                transparent 40px,
                rgba(59, 130, 246, 0.05) 41px,
                transparent 42px
            );
            animation: wavePulse 12s infinite linear;
        }

        @keyframes wavePulse {
            0% { transform: scale(0.9); opacity: 0.3; }
            50% { transform: scale(1.1); opacity: 0.7; }
            100% { transform: scale(0.9); opacity: 0.3; }
        }

        /* --- هیرو / بالای سایت --- */
        .hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            justify-content: center;
            padding: 70px 20px 40px;
            text-align: center;
            position: relative;
        }

        /* آیکون فرستنده رادیویی زنده (جایگزین عکس) */
        .antenna-container {
            position: relative;
            width: 130px;
            height: 130px;
            margin-bottom: 25px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: rgba(15, 23, 42, 0.8);
            border-radius: 50%;
            border: 3px solid var(--gold-primary);
            box-shadow: 0 0 30px rgba(245, 158, 11, 0.3), inset 0 0 15px rgba(59, 130, 246, 0.4);
        }

        .pulse-ring {
            position: absolute;
            border: 2px solid var(--gold-primary);
            border-radius: 50%;
            animation: ringExpand 3s infinite cubic-bezier(0.215, 0.61, 0.355, 1);
            opacity: 0;
        }

        .pulse-ring:nth-child(1) { animation-delay: 0s; }
        .pulse-ring:nth-child(2) { animation-delay: 1s; }
        .pulse-ring:nth-child(3) { animation-delay: 2s; }

        @keyframes ringExpand {
            0% { width: 130px; height: 130px; opacity: 0.8; border-color: var(--gold-primary); }
            50% { border-color: var(--blue-glow); }
            100% { width: 280px; height: 280px; opacity: 0; }
        }

        .antenna-icon {
            width: 60px;
            height: 60px;
            fill: url(#goldGradient);
            z-index: 2;
        }

        .hero h1 {
            font-size: 2.4rem;
            font-weight: 900;
            background: var(--gold-gradient);
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
            margin-bottom: 8px;
            letter-spacing: -0.5px;
        }

        .hero h2 {
            font-size: 1.25rem;
            color: #e2e8f0;
            font-weight: 500;
            margin-bottom: 18px;
        }

        .badges {
            display: flex;
            flex-wrap: wrap;
            gap: 12px;
            justify-content: center;
        }

        .badge {
            background: rgba(30, 58, 138, 0.4);
            border: 1px solid rgba(59, 130, 246, 0.4);
            color: #f1f5f9;
            padding: 6px 18px;
            border-radius: 30px;
            font-size: 0.88rem;
            backdrop-filter: blur(8px);
        }

        .badge.gold-badge {
            background: rgba(245, 158, 11, 0.15);
            border-color: var(--gold-primary);
            color: var(--gold-light);
            font-weight: 600;
        }

        /* --- کانتینر محتوا --- */
        .container {
            max-width: 900px;
            margin: 0 auto;
            padding: 0 20px 40px;
        }

        .card {
            background: var(--bg-card);
            border: 1px solid rgba(245, 158, 11, 0.25);
            border-radius: 20px;
            padding: 32px;
            margin-bottom: 25px;
            backdrop-filter: blur(16px);
            box-shadow: 0 15px 35px rgba(0, 0, 0, 0.4);
            transition: all 0.3s ease;
        }

        .card:hover {
            border-color: var(--gold-primary);
            box-shadow: 0 15px 40px rgba(245, 158, 11, 0.15);
            transform: translateY(-2px);
        }

        .card-title {
            font-size: 1.35rem;
            color: var(--gold-light);
            border-right: 4px solid var(--gold-primary);
            padding-right: 14px;
            margin-bottom: 22px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 18px;
        }

        .service-box {
            background: rgba(10, 15, 30, 0.7);
            border: 1px solid rgba(255, 255, 255, 0.08);
            border-radius: 14px;
            padding: 22px;
            border-right: 3px solid var(--blue-glow);
            transition: border-color 0.3s ease;
        }

        .service-box:hover {
            border-right-color: var(--gold-primary);
        }

        .service-box h4 {
            color: #ffffff;
            font-size: 1.05rem;
            margin-bottom: 10px;
        }

        .service-box p {
            color: var(--text-sub);
            font-size: 0.9rem;
            line-height: 1.7;
        }

        /* --- بخش دکمه تماس --- */
        .cta-wrapper {
            text-align: center;
            margin-top: 35px;
        }

        .btn-call {
            display: inline-flex;
            align-items: center;
            gap: 12px;
            background: var(--gold-gradient);
            color: #0d1322;
            font-weight: 800;
            font-size: 1.2rem;
            padding: 16px 45px;
            border-radius: 50px;
            text-decoration: none;
            box-shadow: 0 0 30px rgba(245, 158, 11, 0.4);
            transition: all 0.3s ease;
        }

        .btn-call:hover {
            transform: scale(1.05);
            box-shadow: 0 0 45px rgba(245, 158, 11, 0.7);
        }

        /* --- فوتر --- */
        footer {
            text-align: center;
            padding: 35px 20px;
            color: var(--text-sub);
            font-size: 0.88rem;
            border-top: 1px solid rgba(255, 255, 255, 0.08);
            background: rgba(5, 8, 16, 0.9);
        }

        .seo-keywords {
            margin-top: 18px;
            font-size: 0.78rem;
            color: #64748b;
            line-height: 2;
        }

        @media (max-width: 600px) {
            .hero h1 { font-size: 1.8rem; }
            .hero h2 { font-size: 1.05rem; }
            .card { padding: 22px; }
            .btn-call { font-size: 1rem; padding: 14px 30px; }
        }
    </style>
</head>
<body>

    <!-- پس‌زمینه امواج رادیویی -->
    <div class="radio-waves-bg">
        <div class="wave-line"></div>
    </div>

    <!-- بخش هیرو (بالای سایت) -->
    <header class="hero">
        <div class="antenna-container">
            <div class="pulse-ring"></div>
            <div class="pulse-ring"></div>
            <div class="pulse-ring"></div>
            
            <!-- آیکون وکتور موج رادیویی و آنتن -->
            <svg class="antenna-icon" viewBox="0 0 24 24">
                <defs>
                    <linearGradient id="goldGradient" x1="0%" y1="0%" x2="100%" y2="100%">
                        <stop offset="0%" stop-color="#f59e0b" />
                        <stop offset="100%" stop-color="#fef08a" />
                    </linearGradient>
                </defs>
                <path d="M12 3c-4.97 0-9 4.03-9 9 0 2.12.74 4.07 1.97 5.61L4.35 19.4c-.39.39-.39 1.02 0 1.41.39.39 1.02.39 1.41 0l1.9-1.9C9.18 19.58 10.54 20 12 20s2.82-.42 4.34-1.09l1.9 1.9c.39.39 1.02.39 1.41 0 .39-.39.39-1.02 0-1.41l-1.38-1.79C19.26 16.07 20 14.12 20 12c0-4.97-4.03-9-9-9zm0 2c3.87 0 7 3.13 7 7 0 1.52-.49 2.93-1.32 4.08l-2.09-2.09C15.82 13.38 16 12.71 16 12c0-2.21-1.79-4-4-4s-4 1.79-4 4c0 .71.18 1.38.41 1.99l-2.09 2.09C5.49 14.93 5 13.52 5 12c0-3.87 3.13-7 7-7zm0 6c.55 0 1 .45 1 1s-.45 1-1 1-1-.45-1-1 .45-1 1-1z"/>
            </svg>
        </div>

        <h1>میلاد یوسفی</h1>
        <h2>مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی</h2>

        <div class="badges">
            <span class="badge gold-badge">🤝 همکاری با شرکت امیدان صنعت</span>
            <span class="badge">📻 راه‌اندازی بیسیم موتورولا</span>
            <span class="badge">📍 قائمشهر | مازندران | سراسر ایران</span>
        </div>
    </header>

    <!-- کانتینر اصلی محتوا -->
    <main class="container">

        <!-- درباره من -->
        <section class="card">
            <h3 class="card-title">👨‍💻 درباره من | بیوگرافی حرفه‌ای</h3>
            <p>
                اینجانب <strong>میلاد یوسفی</strong>، **مهندس راه‌اندازی بیسیم** و متخصص طراحی، کانفیگ، نصب و راه‌اندازی شبکه‌های ارتباطی رادیویی با سال‌ها تجربه در پروژه‌های صنعتی، سازمانی و زیرساختی هستم. افتخار همکاری با **شرکت امیدان صنعت** را داشته و آماده ارائه خدمات تخصصی در استان مازندران (قائمشهر، ساری، بابل، آمل، چالوس و...) و تمامی استان‌های کشور می‌باشم.
            </p>
        </section>

        <!-- خدمات تخصصی -->
        <section class="card">
            <h3 class="card-title">🛠 خدمات تخصصی (Services)</h3>
            <div class="services-grid">
                <div class="service-box">
                    <h4>📡 راه‌اندازی بیسیم و شبکه‌های رادیویی</h4>
                    <p>مشاوره، طراحی، جانمایی و اجرای کامل شبکه‌های ارتباطی بیسیم دستی، خودرویی و ثابت.</p>
                </div>
                <div class="service-box">
                    <h4>📻 راه‌اندازی بیسیم موتورولا (Motorola)</h4>
                    <p>کانفیگ، برنامه‌ریزی (Programming)، فرکانس‌دهی و عیب‌یابی تخصصی تجهیزات برند موتورولا.</p>
                </div>
                <div class="service-box">
                    <h4>🏗 راه‌اندازی سایت و دکل‌های ارتباطی</h4>
                    <p>نصب تکرارکننده (Repeater)، دکل‌های ارتباطی، آنتن‌های دیجیتال/آنالوگ و تجهیز کامل سایت‌های رادیویی.</p>
                </div>
                <div class="service-box">
                    <h4>🔍 تست پوشش و بهینه‌سازی سیگنال</h4>
                    <p>تست سیگنالینگ، عیب‌یابی خطوط انتقال، آنتن‌ها، کابل‌ها و رفع تداخلات فرکانسی.</p>
                </div>
            </div>
        </section>

        <!-- همکاری سازمانی -->
        <section class="card">
            <h3 class="card-title">🏢 همکاری‌های سازمانی</h3>
            <p>
                🤝 <strong>همکاری با شرکت امیدان صنعت:</strong> ارائه خدمات تخصصی مهندسی، طراحی، تامین، نصب و راه‌اندازی شبکه‌های بیسیم پروژه‌های صنعتی و ارگان‌ها با همکاری شرکت امیدان صنعت.
            </p>
        </section>

        <!-- مناطق تحت پوشش -->
        <section class="card">
            <h3 class="card-title">📍 مناطق تحت پوشش خدمات</h3>
            <p>
                🏡 <strong>استان مازندران:</strong> قائمشهر (پایگاه اصلی)، ساری، بابل، آمل، بهشهر، بابلسر، تنکابن، چالوس، نوشهر، رامسر و كافة شهرهای استان.<br>
                🇮🇷 <strong>سراسر ایران:</strong> اجرا و راه‌اندازی پروژه‌های رادیویی در تمامی استان‌ها و مناطق صنعتی کشور.
            </p>
        </section>

        <!-- دکمه تماس -->
        <div class="cta-wrapper">
            <a href="tel:09048818508" class="btn-call">
                <span>📞 تماس و مشاوره مستقیم: 09048818508</span>
            </a>
        </div>

    </main>

    <!-- فوتر -->
    <footer>
        <p>© تمامی حقوق محفوظ است | میلاد یوسفی - مهندس راه‌اندازی بیسیم و شبکه‌های رادیویی</p>
        <div class="seo-keywords">
            مهندس بیسیم | راه اندازی بیسیم | مهندس راه اندازی بیسیم | راه اندازی بیسیم موتورولا | راه اندازی سایت بیسیم | بیسیم موتورولا مازندران | راه اندازی بیسیم قائمشهر | شرکت امیدان صنعت | تعمیرات بیسیم موتورولا | متخصص شبکه‌های رادیویی
        </div>
    </footer>

</body>
</html>
