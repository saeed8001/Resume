<!DOCTYPE html>
<html lang="en" dir="ltr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Saeed Kakavandi | سعید کاکاوندی — Resume</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Oswald:wght@400;500;600;700&family=Inter:wght@300;400;500;600;700;800&family=Vazirmatn:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

<style>
    /* ============================================================
       DESIGN TOKENS
       Palette drawn from highway-guide-sign blue, ramp-metering
       signal amber, and engineering drafting paper — grounded in
       the subject's own work (traffic engineering / GIS / GPS).
       ============================================================ */
    :root {
        --ink: #1B2027;
        --ink-soft: #4B5563;
        --paper: #F5F4EF;
        --card: #FFFFFF;
        --route-blue: #14335C;
        --route-blue-2: #2C5C94;
        --signal-amber: #E2A63B;
        --go-green: #2E6E52;
        --line: #E1DDD1;
        --line-strong: #C9C3B2;
        --radius: 10px;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    html { scroll-behavior: smooth; }

    @media (prefers-reduced-motion: reduce) {
        html { scroll-behavior: auto; }
        * { transition: none !important; animation: none !important; }
    }

    body {
        background: var(--paper);
        color: var(--ink);
        font-family: 'Inter', sans-serif;
        line-height: 1.75;
        font-weight: 400;
    }

    html[dir="rtl"] body { font-family: 'Vazirmatn', sans-serif; }

    a { color: var(--route-blue-2); }

    :focus-visible {
        outline: 2px solid var(--signal-amber);
        outline-offset: 2px;
    }

    /* ---------------- language visibility ---------------- */
    .fa-content { display: none; }
    .en-content { display: block; }
    html[dir="rtl"] .fa-content { display: block; }
    html[dir="rtl"] .en-content { display: none; }

    /* inline elements (button labels, footer) need inline-flex, not block */
    span.en-content { display: inline-flex; }
    span.fa-content { display: none; }
    html[dir="rtl"] span.en-content { display: none; }
    html[dir="rtl"] span.fa-content { display: inline-flex; }

    /* ---------------- floating controls ---------------- */
    .controls {
        position: fixed;
        top: 18px;
        left: 18px;
        z-index: 1000;
        display: flex;
        gap: 10px;
    }
    html[dir="rtl"] .controls { left: auto; right: 18px; }

    .ctrl-btn {
        background: var(--card);
        color: var(--route-blue);
        border: 1.5px solid var(--route-blue);
        padding: 9px 16px;
        border-radius: 30px;
        font-family: inherit;
        font-weight: 600;
        font-size: 0.82rem;
        cursor: pointer;
        display: flex;
        align-items: center;
        gap: 7px;
        box-shadow: 0 2px 8px rgba(20,51,92,0.12);
        transition: transform 0.15s ease, background 0.15s ease, color 0.15s ease;
    }
    .ctrl-btn:hover { background: var(--route-blue); color: #fff; transform: translateY(-1px); }
    .ctrl-btn.primary { background: var(--signal-amber); border-color: var(--signal-amber); color: var(--route-blue); }
    .ctrl-btn.primary:hover { background: #cf9330; color: #fff; }

    /* ---------------- header / hero ---------------- */
    header {
        position: relative;
        background: linear-gradient(150deg, var(--route-blue) 0%, #0D2038 100%);
        color: #fff;
        padding: 96px 20px 64px;
        text-align: center;
        overflow: hidden;
    }
    header::before {
        content: '';
        position: absolute;
        inset: 0;
        background-image:
            linear-gradient(rgba(255,255,255,0.055) 1px, transparent 1px),
            linear-gradient(90deg, rgba(255,255,255,0.055) 1px, transparent 1px);
        background-size: 30px 30px;
        pointer-events: none;
    }
    header::after {
        content: '';
        position: absolute;
        width: 340px; height: 340px;
        border-radius: 50%;
        background: radial-gradient(circle, rgba(226,166,59,0.18) 0%, transparent 70%);
        top: -120px; right: -80px;
        pointer-events: none;
    }
    html[dir="rtl"] header::after { right: auto; left: -80px; }

    .hero-inner { position: relative; z-index: 2; }

    /* decorative motif replacing a photo slot — a small highway medallion
       flanked by dashed lane markings, echoing the mile-marker language
       used later in the timeline */
    .hero-motif {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: 14px;
        margin-bottom: 22px;
    }
    .hero-motif .lane {
        width: 56px;
        height: 0;
        border-top: 2px dashed rgba(255,255,255,0.32);
    }
    .hero-motif .medallion {
        width: 46px; height: 46px;
        border-radius: 50%;
        background: rgba(255,255,255,0.06);
        border: 1.5px solid rgba(226,166,59,0.55);
        display: flex; align-items: center; justify-content: center;
        color: var(--signal-amber);
        font-size: 1.05rem;
        box-shadow: 0 4px 14px rgba(0,0,0,0.25);
    }

    h1 {
        font-family: 'Oswald', sans-serif;
        font-size: 2.6rem;
        font-weight: 600;
        letter-spacing: 0.5px;
        margin-bottom: 8px;
        color: #fff;
    }
    html[dir="rtl"] h1 { font-family: 'Vazirmatn', sans-serif; font-weight: 700; letter-spacing: 0; }

    .tagline {
        font-size: 1.08rem;
        color: #C9D6E8;
        margin-bottom: 22px;
        font-weight: 300;
    }
    html[dir="rtl"] .tagline { font-weight: 400; }

    .route-strip {
        display: inline-block;
        background: var(--go-green);
        color: #fff;
        padding: 10px 26px;
        border-radius: 4px;
        border: 1.5px solid rgba(255,255,255,0.3);
        font-size: 0.86rem;
        letter-spacing: 0.2px;
        margin-bottom: 28px;
        max-width: 90%;
    }
    html[dir="rtl"] .route-strip { font-weight: 600; }

    .contact-bar {
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
        gap: 12px;
        font-size: 0.9rem;
    }
    .contact-bar a, .contact-bar span {
        color: #F1F5F9;
        text-decoration: none;
        display: inline-flex;
        align-items: center;
        gap: 8px;
        background: rgba(255,255,255,0.09);
        border: 1px solid rgba(255,255,255,0.15);
        padding: 8px 16px;
        border-radius: 20px;
        transition: background 0.15s ease, transform 0.15s ease;
    }
    .contact-bar a:hover { background: var(--signal-amber); color: var(--route-blue); border-color: var(--signal-amber); transform: translateY(-1px); }

    /* ---------------- layout ---------------- */
    .container {
        max-width: 900px;
        margin: -32px auto 60px;
        padding: 0 20px;
        position: relative;
        z-index: 3;
    }

    .card {
        background: var(--card);
        border-radius: var(--radius);
        border-top: 4px solid var(--route-blue-2);
        padding: 38px 40px;
        box-shadow: 0 10px 26px rgba(20,32,39,0.06);
        margin-bottom: 24px;
        border-inline: 1px solid #EDEAE0;
        border-bottom: 1px solid #EDEAE0;
    }
    .card.c-about   { border-top-color: var(--route-blue); }
    .card.c-edu     { border-top-color: var(--route-blue-2); }
    .card.c-teach   { border-top-color: var(--go-green); }
    .card.c-exp     { border-top-color: var(--signal-amber); }
    .card.c-honors  { border-top-color: var(--route-blue); }
    .card.c-skills  { border-top-color: var(--route-blue-2); }

    .section-title {
        display: flex;
        align-items: center;
        gap: 13px;
        color: var(--route-blue);
        font-family: 'Oswald', sans-serif;
        font-weight: 600;
        font-size: 1.28rem;
        text-transform: uppercase;
        letter-spacing: 0.5px;
        padding-bottom: 14px;
        margin-bottom: 26px;
        border-bottom: 2px dashed var(--line-strong);
    }
    html[dir="rtl"] .section-title { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; font-weight: 700; }

    .icon-badge {
        width: 32px; height: 32px;
        border-radius: 50%;
        flex-shrink: 0;
        display: flex; align-items: center; justify-content: center;
        color: #fff;
        font-size: 0.92rem;
        background: var(--route-blue);
    }
    .icon-badge.blue2 { background: var(--route-blue-2); }
    .icon-badge.green { background: var(--go-green); }
    .icon-badge.amber { background: var(--signal-amber); color: var(--route-blue); }

    .about-text { color: var(--ink-soft); text-align: justify; font-size: 1rem; }

    /* ---------------- timeline (mile-marker style) ---------------- */
    .timeline-item {
        position: relative;
        padding-bottom: 28px;
        padding-left: 26px;
        border-left: 2px dashed var(--line-strong);
    }
    html[dir="rtl"] .timeline-item { padding-left: 0; padding-right: 26px; border-left: none; border-right: 2px dashed var(--line-strong); }
    .timeline-item:last-child { border-color: transparent; padding-bottom: 0; }
    .timeline-item::before {
        content: '';
        position: absolute;
        top: 4px; left: -7px;
        width: 12px; height: 12px;
        background: var(--signal-amber);
        border: 2px solid #fff;
        box-shadow: 0 0 0 2px var(--route-blue-2);
        border-radius: 50%;
    }
    html[dir="rtl"] .timeline-item::before { left: auto; right: -7px; }

    .item-title { font-weight: 700; font-size: 1.08rem; color: var(--route-blue); margin-bottom: 4px; }
    .item-subtitle { color: var(--route-blue-2); font-weight: 600; font-size: 0.92rem; margin-bottom: 8px; }
    .item-subtitle a { color: inherit; text-decoration: underline dotted; text-underline-offset: 3px; }
    .item-meta {
        font-size: 0.8rem;
        color: var(--ink-soft);
        background: var(--paper);
        padding: 4px 12px;
        border-radius: 12px;
        display: inline-block;
        margin-bottom: 10px;
        font-weight: 600;
    }
    .item-meta.live { background: rgba(46,110,82,0.12); color: var(--go-green); }
    .timeline-item p { color: var(--ink-soft); font-size: 0.95rem; }
    .thesis-line { font-size: 0.95rem; color: var(--ink); margin-top: 4px; }
    .thesis-line strong { color: var(--route-blue); }
    .thesis-line a { text-decoration: underline dotted; text-underline-offset: 3px; }

    /* ---------------- honors cards ---------------- */
    .honor-card {
        display: flex;
        gap: 16px;
        padding: 18px 0;
        border-bottom: 1px solid var(--line);
    }
    .honor-card:last-child { border-bottom: none; padding-bottom: 0; }
    .honor-icon {
        flex-shrink: 0;
        width: 40px; height: 40px;
        border-radius: 50%;
        display: flex; align-items: center; justify-content: center;
        font-size: 1rem;
        color: #fff;
    }
    .honor-icon.award { background: var(--signal-amber); }
    .honor-icon.fellowship { background: var(--route-blue-2); }
    .honor-icon.grant { background: var(--go-green); }
    .honor-kicker {
        font-family: 'Oswald', sans-serif;
        font-size: 0.68rem;
        text-transform: uppercase;
        letter-spacing: 1.5px;
        font-weight: 600;
        margin-bottom: 4px;
    }
    html[dir="rtl"] .honor-kicker { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; font-weight: 700; }
    .honor-kicker.award { color: #B9832A; }
    .honor-kicker.fellowship { color: var(--route-blue-2); }
    .honor-kicker.grant { color: var(--go-green); }
    .honor-title { font-weight: 700; color: var(--route-blue); margin-bottom: 4px; font-size: 1rem; }
    .honor-title a { color: inherit; text-decoration: underline dotted; text-underline-offset: 3px; }
    .honor-body { color: var(--ink-soft); font-size: 0.93rem; }

    /* ---------------- skills (numeric, out of 10) ---------------- */
    .skill-group-title {
        font-family: 'Oswald', sans-serif;
        font-size: 0.78rem;
        text-transform: uppercase;
        letter-spacing: 1.5px;
        color: var(--ink-soft);
        margin: 22px 0 14px;
        font-weight: 600;
    }
    html[dir="rtl"] .skill-group-title { font-family: 'Vazirmatn', sans-serif; text-transform: none; letter-spacing: 0; }
    .skill-group-title:first-of-type { margin-top: 0; }

    .skill-row { display: flex; align-items: center; gap: 14px; margin-bottom: 13px; }
    html[dir="rtl"] .skill-row { flex-direction: row-reverse; }
    .skill-name { width: 178px; flex-shrink: 0; font-weight: 600; font-size: 0.9rem; }

    .skill-track {
        flex: 1;
        height: 10px;
        border-radius: 3px;
        position: relative;
        overflow: hidden;
        background: repeating-linear-gradient(90deg, var(--line) 0, var(--line) 8%, transparent 8%, transparent 10%);
    }
    .skill-fill {
        position: absolute;
        inset-inline-start: 0;
        top: 0; bottom: 0;
        background: linear-gradient(90deg, var(--route-blue-2), var(--signal-amber));
        -webkit-mask-image: repeating-linear-gradient(90deg, #000 0, #000 8%, transparent 8%, transparent 10%);
                mask-image: repeating-linear-gradient(90deg, #000 0, #000 8%, transparent 8%, transparent 10%);
    }
    .skill-score {
        width: 46px;
        flex-shrink: 0;
        text-align: center;
        font-family: 'Oswald', sans-serif;
        font-weight: 700;
        font-size: 0.92rem;
        color: var(--route-blue);
    }
    html[dir="rtl"] .skill-score { font-family: 'Vazirmatn', sans-serif; }
    .skill-score span { font-weight: 400; font-size: 0.72rem; color: var(--ink-soft); }

    /* ---------------- footer ---------------- */
    footer {
        text-align: center;
        color: var(--ink-soft);
        font-size: 0.8rem;
        padding-bottom: 40px;
    }

    /* ---------------- responsive ---------------- */
    @media (max-width: 640px) {
        header { padding: 90px 16px 52px; }
        h1 { font-size: 2rem; }
        .card { padding: 28px 22px; }
        .skill-name { width: 120px; font-size: 0.82rem; }
        .skill-score { width: 38px; font-size: 0.8rem; }
        .honor-card { flex-direction: column; }
        .hero-motif .lane { width: 30px; }
        .hero-motif .medallion { width: 38px; height: 38px; font-size: 0.92rem; }
    }

    /* ---------------- print (A4) ---------------- */
    @media print {
        @page { size: A4; margin: 13mm 12mm; }
        body { background: #fff; color: #000; }
        .controls { display: none !important; }
        .container { margin-top: 0; max-width: 100%; }
        header {
            background: none !important;
            color: #000 !important;
            padding: 0 0 16px;
            border-bottom: 2px solid var(--route-blue);
        }
        header::before, header::after { display: none !important; }
        .hero-motif { display: none !important; }
        h1 { color: #000 !important; }
        .tagline { color: #333 !important; }
        .route-strip, .contact-bar a, .contact-bar span {
            -webkit-print-color-adjust: exact; print-color-adjust: exact;
            box-shadow: none !important;
        }
        .contact-bar a, .contact-bar span { color: #000 !important; background: none !important; border: 1px solid #999 !important; }
        .card { box-shadow: none !important; border: 1px solid #ddd; border-top: 1px solid #ddd !important; padding: 18px 4px; margin-bottom: 10px; page-break-inside: avoid; }
        .section-title { color: #000 !important; }
        .item-title, .item-subtitle, .honor-title, .thesis-line strong { color: #000 !important; }
        .item-meta.live { background: none !important; }
        .skill-fill, .honor-icon, .icon-badge { -webkit-print-color-adjust: exact; print-color-adjust: exact; }
    }
</style>
</head>
<body>

<div class="controls">
    <button class="ctrl-btn" onclick="toggleLanguage()">
        <i class="fas fa-globe"></i>
        <span class="en-content">فارسی</span>
        <span class="fa-content">English</span>
    </button>
    <button class="ctrl-btn primary" onclick="window.print()">
        <i class="fas fa-print"></i>
        <span class="en-content">Save PDF</span>
        <span class="fa-content">ذخیره PDF</span>
    </button>
</div>

<header>
    <div class="hero-inner">
        <div class="hero-motif" aria-hidden="true">
            <span class="lane"></span>
            <span class="medallion"><i class="fas fa-road"></i></span>
            <span class="lane"></span>
        </div>

        <div class="en-content">
            <h1>Saeed Kakavandi</h1>
            <p class="tagline">Transportation Engineer &amp; Data Analyst</p>
            <div class="route-strip">Turning transportation data into safer, smarter roads</div>
            <div class="contact-bar">
                <a href="https://www.google.com/maps/place/Tehransar,+District+21,+Tehran,+Tehran+Province,+Iran/@35.6921918,51.2412539,14z/data=!3m1!4b1!4m6!3m5!1s0x3f8dfbebdac71fbb:0xe5a8ae53aa1e7b5!8m2!3d35.6928794!4d51.2541919!16s%2Fm%2F03d1vy8" target="_blank" rel="noopener"><i class="fas fa-map-marker-alt"></i> Tehran, Tehransar</a>
                <a href="tel:+989919719176"><i class="fas fa-phone"></i> +98 991 971 9176</a>
                <a href="mailto:saeedkakavandi8001@gmail.com"><i class="fas fa-envelope"></i> Email</a>
                <a href="https://www.linkedin.com/in/saeed-kakavandi/" target="_blank" rel="noopener"><i class="fab fa-linkedin"></i> LinkedIn</a>
            </div>
        </div>

        <div class="fa-content">
            <h1>سعید کاکاوندی</h1>
            <p class="tagline">مهندس حمل‌ونقل و تحلیل‌گر داده</p>
            <div class="route-strip">تبدیل داده‌های حمل‌ونقل به جاده‌هایی ایمن‌تر و هوشمندتر</div>
            <div class="contact-bar">
                <a href="https://www.google.com/maps/place/Tehransar,+District+21,+Tehran,+Tehran+Province,+Iran/@35.6921918,51.2412539,14z/data=!3m1!4b1!4m6!3m5!1s0x3f8dfbebdac71fbb:0xe5a8ae53aa1e7b5!8m2!3d35.6928794!4d51.2541919!16s%2Fm%2F03d1vy8" target="_blank" rel="noopener"><i class="fas fa-map-marker-alt"></i> تهران، تهرانسر</a>
                <a href="tel:+989919719176"><i class="fas fa-phone"></i> ۰۹۹۱۹۷۱۹۱۷۶</a>
                <a href="mailto:saeedkakavandi8001@gmail.com"><i class="fas fa-envelope"></i> ایمیل</a>
                <a href="https://www.linkedin.com/in/saeed-kakavandi/" target="_blank" rel="noopener"><i class="fab fa-linkedin"></i> لینکدین</a>
            </div>
        </div>
    </div>
</header>

<div class="container">

    <!-- ABOUT -->
    <div class="card c-about">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge"><i class="fas fa-user-tie"></i></span> About Me</h2>
            <p class="about-text">A transportation engineer and data scientist specializing in traffic-safety analytics and intelligent freeway operations. Currently pursuing an M.Sc. in Transportation Engineering at Amirkabir University of Technology, where a nationally co-funded thesis applies data-driven modeling to driving-history patterns in intercity bus crash prediction. Research spans large-scale GPS/FMS fleet analytics, fuzzy-logic ramp-metering control for freeway networks, and geospatial data engineering &mdash; pairing rigorous statistical methods with production-grade Python tooling to turn raw transportation data into actionable safety and mobility solutions.</p>
        </div>
        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge"><i class="fas fa-user-tie"></i></span> درباره من</h2>
            <p class="about-text">مهندس حمل‌ونقل و تحلیل‌گر داده با تمرکز بر ایمنی ترافیک و بهره‌برداری هوشمند از آزادراه‌ها. دانشجوی کارشناسی‌ارشد مهندسی حمل‌ونقل در دانشگاه صنعتی امیرکبیر هستم؛ جایی که پایان‌نامه‌ی حمایت‌مالی‌شده‌ام به مدل‌سازی داده‌محور اثر سابقه‌ی رانندگی در پیش‌بینی تصادفات اتوبوس‌های بین‌شهری اختصاص دارد. حوزه‌ی پژوهشی‌ام شامل تحلیل کلان‌مقیاس داده‌های GPS/FMS ناوگان اتوبوسرانی، طراحی کنترلر فازی برای کنترل رمپ آزادراهی و مهندسی داده‌های مکانی است؛ ترکیبی از روش‌های آماری دقیق و ابزارهای برنامه‌نویسی حرفه‌ای پایتون برای تبدیل داده‌های خام حمل‌ونقل به راهکارهای عملی ایمنی و تحرک‌پذیری.</p>
        </div>
    </div>

    <!-- EDUCATION -->
    <div class="card c-edu">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge blue2"><i class="fas fa-graduation-cap"></i></span> Education</h2>
            <div class="timeline-item">
                <div class="item-title">M.Sc. in Transportation Engineering</div>
                <div class="item-subtitle">Amirkabir University of Technology (AUT)</div>
                <div class="item-meta live">2024 &ndash; Present &nbsp;|&nbsp; GPA: 18.99/20</div>
                <p class="thesis-line"><strong>Thesis:</strong> A data-driven model to evaluate the effect of driving history in predicting intercity bus crashes<br>
                Supervisors: <a href="https://aut.ac.ir/cv/2325/%D8%B3%DB%8C%D8%AF-%D9%85%D8%AD%D9%85%D9%88%D8%AF-%D9%85%D8%B5%D8%A8%D8%A7%D8%AD-%D9%86%D9%85%DB%8C%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=2325&amp;mod=scv" target="_blank" rel="noopener">Dr. Mesbah</a> &amp; <a href="https://aut.ac.ir/cv/3020/%D8%B9%D9%84%DB%8C%D8%B1%D8%B6%D8%A7%20%D8%B5%D8%A7%D8%AF%D9%82%DB%8C%20%D8%B1%D8%A7%D8%AF" target="_blank" rel="noopener">Dr. Sadeghi-Rad</a> &nbsp;|&nbsp; Advisor: <a href="https://www.irc.ac.ir/fa-IR/Irc/5008/page/%D8%AF%DA%A9%D8%AA%D8%B1-%D9%84%DB%8C%D9%84%DB%8C-%D9%86%DB%8C%D8%A7%DA%A9%D8%A7%D9%86" target="_blank" rel="noopener">Dr. Niakan</a></p>
            </div>
            <div class="timeline-item" style="margin-top: 22px;">
                <div class="item-title">B.Sc. in Civil &amp; Environmental Engineering</div>
                <div class="item-subtitle">Amirkabir University of Technology (AUT)</div>
                <div class="item-meta">2020 &ndash; 2024 &nbsp;|&nbsp; GPA: 17.52/20</div>
                <p class="thesis-line"><strong>Project:</strong> Converting text address of Traffic Violations to geographical coordinates &nbsp;(Grade: 19.5/20)<br>
                Supervisor: <a href="https://aut.ac.ir/cv/2325/%D8%B3%DB%8C%D8%AF-%D9%85%D8%AD%D9%85%D9%88%D8%AF-%D9%85%D8%B5%D8%A8%D8%A7%D8%AD-%D9%86%D9%85%DB%8C%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=2325&amp;mod=scv" target="_blank" rel="noopener">Dr. Mesbah</a></p>
            </div>
        </div>
        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge blue2"><i class="fas fa-graduation-cap"></i></span> سوابق تحصیلی</h2>
            <div class="timeline-item">
                <div class="item-title">کارشناسی ارشد مهندسی حمل‌ونقل</div>
                <div class="item-subtitle">دانشگاه صنعتی امیرکبیر</div>
                <div class="item-meta live">۱۴۰۳ &ndash; تاکنون &nbsp;|&nbsp; معدل: ۱۸.۹۹/۲۰</div>
                <p class="thesis-line"><strong>پایان‌نامه:</strong> مدل‌سازی داده‌مبنای اثر سابقه رانندگی در پیش‌بینی تصادفات اتوبوس‌های بین‌شهری<br>
                به راهنمایی <a href="https://aut.ac.ir/cv/2325/%D8%B3%DB%8C%D8%AF-%D9%85%D8%AD%D9%85%D9%88%D8%AF-%D9%85%D8%B5%D8%A8%D8%A7%D8%AD-%D9%86%D9%85%DB%8C%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=2325&amp;mod=scv" target="_blank" rel="noopener">دکتر مصباح</a> و <a href="https://aut.ac.ir/cv/3020/%D8%B9%D9%84%DB%8C%D8%B1%D8%B6%D8%A7%20%D8%B5%D8%A7%D8%AF%D9%82%DB%8C%20%D8%B1%D8%A7%D8%AF" target="_blank" rel="noopener">دکتر صادقی‌راد</a> و مشاوره <a href="https://www.irc.ac.ir/fa-IR/Irc/5008/page/%D8%AF%DA%A9%D8%AA%D8%B1-%D9%84%DB%8C%D9%84%DB%8C-%D9%86%DB%8C%D8%A7%DA%A9%D8%A7%D9%86" target="_blank" rel="noopener">دکتر نیاکان</a></p>
            </div>
            <div class="timeline-item" style="margin-top: 22px;">
                <div class="item-title">کارشناسی مهندسی عمران و محیط‌زیست</div>
                <div class="item-subtitle">دانشگاه صنعتی امیرکبیر</div>
                <div class="item-meta">۱۳۹۹ &ndash; ۱۴۰۳ &nbsp;|&nbsp; معدل: ۱۷.۵۲/۲۰</div>
                <p class="thesis-line"><strong>پروژه کارشناسی:</strong> تبدیل آدرس‌های متنی تخلفات ترافیکی به مختصات جغرافیایی &nbsp;(نمره ۱۹.۵)<br>
                به راهنمایی <a href="https://aut.ac.ir/cv/2325/%D8%B3%DB%8C%D8%AF-%D9%85%D8%AD%D9%85%D9%88%D8%AF-%D9%85%D8%B5%D8%A8%D8%A7%D8%AD-%D9%86%D9%85%DB%8C%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=2325&amp;mod=scv" target="_blank" rel="noopener">دکتر مصباح</a></p>
            </div>
        </div>
    </div>

    <!-- TEACHING -->
    <div class="card c-teach">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge green"><i class="fas fa-chalkboard-teacher"></i></span> Teaching Assistantships</h2>
            <div class="timeline-item">
                <div class="item-title">TA &mdash; Operations Research (M.Sc. Level)</div>
                <div class="item-subtitle">Dept. of Road &amp; Transportation Engineering, AUT &mdash; under <a href="https://aut.ac.ir/cv/2035/%D8%A7%D9%85%DB%8C%D8%B1%20%DA%AF%D9%84%20%D8%B1%D9%88" target="_blank" rel="noopener">Dr. Amir Golrou</a></div>
                <div class="item-meta">Spring 2026</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">TA &mdash; Technical English (B.Sc. Level)</div>
                <div class="item-subtitle">Dept. of Road &amp; Transportation Engineering, AUT &mdash; under <a href="https://aut.ac.ir/cv/2035/%D8%A7%D9%85%DB%8C%D8%B1%20%DA%AF%D9%84%20%D8%B1%D9%88" target="_blank" rel="noopener">Dr. Amir Golrou</a></div>
                <div class="item-meta">Spring 2025</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">TA &mdash; Dynamics (B.Sc. Level)</div>
                <div class="item-subtitle">Geotechnical Engineering Dept., AUT &mdash; under <a href="https://aut.ac.ir/cv/26582/%D8%B3%D8%A7%D8%B1%D8%A7-%D8%AD%DB%8C%D8%AF%D8%B1%DB%8C-%DA%AF%D9%84%D9%81%D8%B2%D8%A7%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=26582&amp;mod=scv" target="_blank" rel="noopener">Dr. Sara Heidari</a></div>
                <div class="item-meta">3 Semesters (Fall 2023 &ndash; Fall 2024)</div>
            </div>
        </div>
        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge green"><i class="fas fa-chalkboard-teacher"></i></span> سوابق تدریس و دستیار آموزشی (TA)</h2>
            <div class="timeline-item">
                <div class="item-title">دستیار آموزشی درس تحقیق در عملیات (مقطع کارشناسی ارشد)</div>
                <div class="item-subtitle">گروه راه و ترابری، دانشگاه صنعتی امیرکبیر &mdash; تحت نظر <a href="https://aut.ac.ir/cv/2035/%D8%A7%D9%85%DB%8C%D8%B1%20%DA%AF%D9%84%20%D8%B1%D9%88" target="_blank" rel="noopener">دکتر امیر گلرو</a></div>
                <div class="item-meta">ترم ۱۴۰۴-۲</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">دستیار آموزشی درس زبان تخصصی (مقطع کارشناسی)</div>
                <div class="item-subtitle">گروه راه و ترابری، دانشگاه صنعتی امیرکبیر &mdash; تحت نظر <a href="https://aut.ac.ir/cv/2035/%D8%A7%D9%85%DB%8C%D8%B1%20%DA%AF%D9%84%20%D8%B1%D9%88" target="_blank" rel="noopener">دکتر امیر گلرو</a></div>
                <div class="item-meta">ترم ۱۴۰۳-۲</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">دستیار آموزشی درس دینامیک (مقطع کارشناسی)</div>
                <div class="item-subtitle">گروه ژئوتکنیک، دانشگاه صنعتی امیرکبیر &mdash; تحت نظر <a href="https://aut.ac.ir/cv/26582/%D8%B3%D8%A7%D8%B1%D8%A7-%D8%AD%DB%8C%D8%AF%D8%B1%DB%8C-%DA%AF%D9%84%D9%81%D8%B2%D8%A7%D9%86%DB%8C?slc_lang=fa&amp;&amp;cv=26582&amp;mod=scv" target="_blank" rel="noopener">دکتر سارا حیدری</a></div>
                <div class="item-meta">۳ ترم (از ۱۴۰۲-۱ تا ۱۴۰۳-۱)</div>
            </div>
        </div>
    </div>

    <!-- EXPERIENCE -->
    <div class="card c-exp">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge amber"><i class="fas fa-briefcase"></i></span> Work Experience</h2>
            <div class="timeline-item">
                <div class="item-title">Spatial Data Analysis Internship in Transportation</div>
                <div class="item-subtitle"><a href="https://armanzamin.com/" target="_blank" rel="noopener">Arman Zamin</a></div>
                <div class="item-meta live">July 2026 &ndash; Present</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">Physics Scientific Supervisor</div>
                <div class="item-subtitle"><a href="http://www.mandegaralborz.sch.ir/" target="_blank" rel="noopener">Mandegar Alborz High School</a></div>
                <div class="item-meta">Oct 2025 &ndash; Feb 2026</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">Retrofitting Inspection Intern &mdash; Azadi Stadium</div>
                <div class="item-subtitle"><a href="https://tadbirsahel.com/" target="_blank" rel="noopener">Tadbir Sahel Pars Co.</a></div>
                <div class="item-meta">July 2023 &ndash; Sept 2023</div>
                <p>Supervised micropile execution to prevent soil settlement, and contributed to stadium structure retrofitting to enhance spectator safety.</p>
            </div>
        </div>
        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge amber"><i class="fas fa-briefcase"></i></span> سوابق کاری</h2>
            <div class="timeline-item">
                <div class="item-title">کارآموزی تخصصی تحلیل داده‌های مکانی در حمل‌ونقل</div>
                <div class="item-subtitle"><a href="https://armanzamin.com/" target="_blank" rel="noopener">آرمان زمین (Arman Zamin)</a></div>
                <div class="item-meta live">تیر ۱۴۰۵ &ndash; تاکنون</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">ناظر علمی درس فیزیک</div>
                <div class="item-subtitle"><a href="http://www.mandegaralborz.sch.ir/" target="_blank" rel="noopener">دبیرستان ماندگار البرز</a></div>
                <div class="item-meta">مهر ۱۴۰۴ &ndash; بهمن ۱۴۰۴</div>
            </div>
            <div class="timeline-item">
                <div class="item-title">کارآموز نظارت مقاوم‌سازی ورزشگاه آزادی</div>
                <div class="item-subtitle"><a href="https://tadbirsahel.com/" target="_blank" rel="noopener">شرکت تدبیر ساحل پارس</a></div>
                <div class="item-meta">تیر ۱۴۰۲ &ndash; شهریور ۱۴۰۲</div>
                <p>نظارت بر اجرای میکروپایل‌ها جهت جلوگیری از نشست زمین، نوسازی سکوها و مقاوم‌سازی گالری‌ها جهت ارتقای ایمنی تماشاگران.</p>
            </div>
        </div>
    </div>

    <!-- HONORS -->
    <div class="card c-honors">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge"><i class="fas fa-trophy"></i></span> Honors &amp; Achievements</h2>

            <div class="honor-card">
                <div class="honor-icon award"><i class="fas fa-award"></i></div>
                <div>
                    <div class="honor-kicker award">Award</div>
                    <div class="honor-title">Selected Researcher &mdash; Amirkabir University of Technology (2025)</div>
                    <div class="honor-body">The B.Sc. project &ldquo;Converting text address of Traffic Violations to geographical coordinates&rdquo; was selected as an outstanding project at the university level.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon award"><i class="fas fa-trophy"></i></div>
                <div>
                    <div class="honor-kicker award">Competition</div>
                    <div class="honor-title">First Place Team &mdash; 3rd National Problem-Oriented Rahi Sho Competition</div>
                    <div class="honor-body">Project: Improving the Speed and Quality of Transportation of Agricultural Inputs, Day-Old Chicks, Live Poultry, and Post-Slaughter Transport (2026).</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon fellowship"><i class="fas fa-star"></i></div>
                <div>
                    <div class="honor-kicker fellowship">Fellowship</div>
                    <div class="honor-title">Shahid Ahmadi-Roshan Plan &mdash; <a href="https://bmn.ir/" target="_blank" rel="noopener">National Elites Foundation</a></div>
                    <div class="honor-body">Member of the Problem-Oriented Research/Technology Core Development Plan; currently participating in a freeway ramp-coordination project under this plan, supervised by Dr. Mesbah, with a particular focus on developing the fuzzy logic controller.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon fellowship"><i class="fas fa-star"></i></div>
                <div>
                    <div class="honor-kicker fellowship">Fellowship</div>
                    <div class="honor-title">Shahid Vezvaei Plan &mdash; <a href="https://bmn.ir/" target="_blank" rel="noopener">National Elites Foundation</a></div>
                    <div class="honor-body">Member of the national plan supporting scientific &amp; cultural activities of talented students; recognized as a top student based on academic record and awarded financial support.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon grant"><i class="fas fa-hand-holding-dollar"></i></div>
                <div>
                    <div class="honor-kicker grant">Research Grant</div>
                    <div class="honor-title">Sponsorship &mdash; Insurance Research Institute</div>
                    <div class="honor-body">The M.Sc. thesis &ldquo;A data-driven model to evaluate the effect of driving history in predicting intercity bus crashes&rdquo; has been approved and financially supported by this institute.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon grant"><i class="fas fa-hand-holding-dollar"></i></div>
                <div>
                    <div class="honor-kicker grant">Research Grant</div>
                    <div class="honor-title">Sponsorship &mdash; Road Maintenance &amp; Transportation Organization</div>
                    <div class="honor-body">The same M.Sc. thesis has also been approved and financially supported by this organization.</div>
                </div>
            </div>
        </div>

        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge"><i class="fas fa-trophy"></i></span> دستاوردها و افتخارات</h2>

            <div class="honor-card">
                <div class="honor-icon award"><i class="fas fa-award"></i></div>
                <div>
                    <div class="honor-kicker award">افتخار</div>
                    <div class="honor-title">پژوهشگر برگزیده دانشگاه صنعتی امیرکبیر (۱۴۰۴)</div>
                    <div class="honor-body">پروژه کارشناسی با عنوان «تبدیل آدرس‌های متنی تخلفات ترافیکی به مختصات جغرافیایی» در سطح دانشگاه به‌عنوان پروژه برگزیده انتخاب شد.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon award"><i class="fas fa-trophy"></i></div>
                <div>
                    <div class="honor-kicker award">مسابقه</div>
                    <div class="honor-title">تیم اول در سومین مسابقه ملی مسئله‌محور راهی شو</div>
                    <div class="honor-body">پروژه: بهبود در سرعت و کیفیت حمل‌ونقل نهاده‌ها، جوجه یک‌روزه، مرغ زنده و حمل پس از کشتار (۱۴۰۵).</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon fellowship"><i class="fas fa-star"></i></div>
                <div>
                    <div class="honor-kicker fellowship">بورس پژوهشی</div>
                    <div class="honor-title">طرح شهید احمدی روشن &mdash; <a href="https://bmn.ir/" target="_blank" rel="noopener">بنیاد ملی نخبگان</a></div>
                    <div class="honor-body">عضو طرح توسعه هسته‌های مسأله‌محور پژوهشی/فناورانه؛ در حال حاضر در پروژه هماهنگ‌سازی رمپ آزادراهی ذیل این طرح، تحت نظارت دکتر مصباح فعالیت دارم و به‌طور ویژه بر توسعه‌ی کنترلر فازی این پروژه متمرکز هستم.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon fellowship"><i class="fas fa-star"></i></div>
                <div>
                    <div class="honor-kicker fellowship">بورس پژوهشی</div>
                    <div class="honor-title">طرح شهید وزوایی &mdash; <a href="https://bmn.ir/" target="_blank" rel="noopener">بنیاد ملی نخبگان</a></div>
                    <div class="honor-body">عضو طرح پشتیبانی از فعالیت‌های علمی و فرهنگی دانشجویان مستعد تحصیلی کشور؛ براساس سوابق تحصیلی به‌عنوان دانشجوی برتر شناخته شده و مورد حمایت مالی قرار گرفته‌ام.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon grant"><i class="fas fa-hand-holding-dollar"></i></div>
                <div>
                    <div class="honor-kicker grant">کمک‌هزینه پژوهشی</div>
                    <div class="honor-title">قرارداد حمایتی با پژوهشکده بیمه</div>
                    <div class="honor-body">پایان‌نامه کارشناسی‌ارشد با عنوان «مدل‌سازی داده‌مبنای اثر سابقه رانندگی در پیش‌بینی تصادفات اتوبوس‌های بین‌شهری» مورد تأیید و تحت حمایت مالی این مؤسسه قرار گرفته است.</div>
                </div>
            </div>
            <div class="honor-card">
                <div class="honor-icon grant"><i class="fas fa-hand-holding-dollar"></i></div>
                <div>
                    <div class="honor-kicker grant">کمک‌هزینه پژوهشی</div>
                    <div class="honor-title">قرارداد حمایتی با سازمان راهداری و حمل‌ونقل جاده‌ای</div>
                    <div class="honor-body">پایان‌نامه کارشناسی‌ارشد فوق، مورد تأیید و تحت حمایت مالی این سازمان نیز قرار گرفته است.</div>
                </div>
            </div>
        </div>
    </div>

    <!-- SKILLS -->
    <div class="card c-skills">
        <div class="en-content">
            <h2 class="section-title"><span class="icon-badge blue2"><i class="fas fa-laptop-code"></i></span> Technical Skills</h2>

            <div class="skill-group-title">Software &amp; Analysis Tools</div>
            <div class="skill-row"><div class="skill-name">Python</div><div class="skill-track"><div class="skill-fill" style="width:90%"></div></div><div class="skill-score">9<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">VISSIM &amp; VISSUM</div><div class="skill-track"><div class="skill-fill" style="width:70%"></div></div><div class="skill-score">7<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">Civil3D &amp; AutoCAD</div><div class="skill-track"><div class="skill-fill" style="width:70%"></div></div><div class="skill-score">7<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">Microsoft Office</div><div class="skill-track"><div class="skill-fill" style="width:80%"></div></div><div class="skill-score">8<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">SUMO</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">4<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">ArcGIS</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">4<span>/10</span></div></div>
            <div class="skill-row"><div class="skill-name">QGIS</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">4<span>/10</span></div></div>

            <div class="skill-group-title">Languages</div>
            <div class="skill-row"><div class="skill-name">English</div><div class="skill-track"><div class="skill-fill" style="width:90%"></div></div><div class="skill-score">9<span>/10</span></div></div>
        </div>
        <div class="fa-content">
            <h2 class="section-title"><span class="icon-badge blue2"><i class="fas fa-laptop-code"></i></span> مهارت‌های تخصصی</h2>

            <div class="skill-group-title">نرم‌افزار و ابزارهای تحلیل</div>
            <div class="skill-row"><div class="skill-name">Python</div><div class="skill-track"><div class="skill-fill" style="width:90%"></div></div><div class="skill-score">۹<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">Vissim &amp; Vissum</div><div class="skill-track"><div class="skill-fill" style="width:70%"></div></div><div class="skill-score">۷<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">Civil3D &amp; AutoCAD</div><div class="skill-track"><div class="skill-fill" style="width:70%"></div></div><div class="skill-score">۷<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">Microsoft Office</div><div class="skill-track"><div class="skill-fill" style="width:80%"></div></div><div class="skill-score">۸<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">Sumo</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">۴<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">ArcGIS</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">۴<span>/۱۰</span></div></div>
            <div class="skill-row"><div class="skill-name">QGIS</div><div class="skill-track"><div class="skill-fill" style="width:40%"></div></div><div class="skill-score">۴<span>/۱۰</span></div></div>

            <div class="skill-group-title">زبان</div>
            <div class="skill-row"><div class="skill-name">انگلیسی</div><div class="skill-track"><div class="skill-fill" style="width:90%"></div></div><div class="skill-score">۹<span>/۱۰</span></div></div>
        </div>
    </div>

    <footer>
        <span class="en-content">Saeed Kakavandi &middot; Tehran, Iran</span>
        <span class="fa-content">سعید کاکاوندی &middot; تهران، ایران</span>
    </footer>

</div>

<script>
    function toggleLanguage() {
        const html = document.documentElement;
        if (html.getAttribute('dir') === 'rtl') {
            html.setAttribute('lang', 'en');
            html.setAttribute('dir', 'ltr');
        } else {
            html.setAttribute('lang', 'fa');
            html.setAttribute('dir', 'rtl');
        }
    }
</script>

</body>
</html>
