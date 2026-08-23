<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>مكافح | حلول ذكية للحماية من الحرائق</title>

<meta name="description"
content="مكافح - شركة تقنية ناشئة تطور حلولًا ذكية للحماية من الحرائق باستخدام الذكاء الاصطناعي والطائرات بدون طيار والتقنيات المتقدمة.">

<meta name="theme-color" content="#080808">

<style>

@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;500;600;700;800&family=Inter:wght@400;500;600;700;800&display=swap');

:root{
    --black:#070707;
    --dark:#0d0d0d;
    --dark2:#141414;
    --red:#d51f2f;
    --red2:#ff3445;
    --white:#ffffff;
    --muted:#a7a7a7;
    --line:rgba(255,255,255,.09);
    --glass:rgba(255,255,255,.045);
    --radius:24px;
    --container:1200px;
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
    scroll-behavior:smooth;
}

html{
    background:var(--black);
}

body{
    font-family:"Cairo",sans-serif;
    background:
        radial-gradient(circle at 85% 10%,rgba(213,31,47,.12),transparent 25%),
        var(--black);
    color:var(--white);
    overflow-x:hidden;
}

body.en{
    font-family:"Inter",sans-serif;
}

a{
    color:inherit;
    text-decoration:none;
}

img{
    max-width:100%;
    display:block;
}

button{
    font-family:inherit;
}

.container{
    width:min(var(--container),calc(100% - 40px));
    margin:auto;
}

.red{
    color:var(--red2);
}

/* ================= NAVBAR ================= */

.navbar{
    position:fixed;
    top:0;
    left:0;
    right:0;
    z-index:1000;
    background:rgba(7,7,7,.72);
    backdrop-filter:blur(18px);
    border-bottom:1px solid var(--line);
}

.nav-inner{
    height:78px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:30px;
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
}

.logo img{
    width:48px;
    height:48px;
    object-fit:contain;
}

.logo-text strong{
    display:block;
    font-size:19px;
    line-height:1;
}

.logo-text span{
    display:block;
    margin-top:5px;
    color:#888;
    font-size:9px;
    letter-spacing:2px;
    direction:ltr;
}

.nav-links{
    display:flex;
    gap:28px;
    align-items:center;
}

.nav-links a{
    color:#bdbdbd;
    font-size:14px;
    transition:.3s;
}

.nav-links a:hover{
    color:white;
}

.nav-actions{
    display:flex;
    align-items:center;
    gap:10px;
}

.lang-btn{
    border:1px solid rgba(255,255,255,.15);
    background:rgba(255,255,255,.04);
    color:white;
    border-radius:50px;
    padding:8px 15px;
    cursor:pointer;
    font-weight:700;
    transition:.3s;
}

.lang-btn:hover{
    border-color:var(--red);
}

.mobile-menu{
    display:none;
    background:none;
    border:0;
    color:white;
    font-size:27px;
    cursor:pointer;
}

/* ================= HERO ================= */

.hero{
    min-height:100vh;
    padding-top:78px;
    position:relative;
    display:flex;
    align-items:center;
    overflow:hidden;
}

.hero::before{
    content:"";
    position:absolute;
    width:650px;
    height:650px;
    background:radial-gradient(circle,rgba(213,31,47,.2),transparent 68%);
    top:-200px;
    right:-160px;
}

.hero-grid{
    display:grid;
    grid-template-columns:1fr 1.15fr;
    gap:55px;
    align-items:center;
    position:relative;
    z-index:2;
}

.hero-content{
    padding:60px 0;
}

.eyebrow{
    display:inline-flex;
    align-items:center;
    gap:10px;
    border:1px solid rgba(213,31,47,.35);
    background:rgba(213,31,47,.07);
    color:#ff6370;
    border-radius:50px;
    padding:7px 14px;
    font-size:12px;
    margin-bottom:25px;
}

.eyebrow-dot{
    width:7px;
    height:7px;
    border-radius:50%;
    background:var(--red2);
    box-shadow:0 0 15px var(--red);
}

.hero h1{
    font-size:clamp(42px,5vw,76px);
    line-height:1.08;
    font-weight:800;
    letter-spacing:-2px;
    margin-bottom:25px;
}

.hero h1 span{
    color:var(--red2);
}

.hero-description{
    color:#aaa;
    font-size:18px;
    line-height:2;
    max-width:600px;
    margin-bottom:35px;
}

.hero-buttons{
    display:flex;
    gap:13px;
    flex-wrap:wrap;
}

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    gap:10px;
    padding:14px 23px;
    border-radius:12px;
    font-size:14px;
    font-weight:700;
    cursor:pointer;
    transition:.3s;
}

.btn-primary{
    background:var(--red);
    color:white;
    box-shadow:0 10px 35px rgba(213,31,47,.22);
}

.btn-primary:hover{
    background:#ef2a3b;
    transform:translateY(-2px);
}

.btn-outline{
    border:1px solid rgba(255,255,255,.14);
    background:rgba(255,255,255,.035);
}

.btn-outline:hover{
    background:rgba(255,255,255,.08);
}

.hero-visual{
    position:relative;
}

.hero-image-wrap{
    position:relative;
    border-radius:32px;
    overflow:hidden;
    min-height:560px;
    background:
        linear-gradient(135deg,#161616,#080808);
    border:1px solid rgba(255,255,255,.1);
    box-shadow:0 35px 100px rgba(0,0,0,.5);
}

.hero-image-wrap::after{
    content:"";
    position:absolute;
    inset:0;
    background:
        linear-gradient(90deg,rgba(7,7,7,.65),transparent 60%),
        linear-gradient(0deg,rgba(7,7,7,.45),transparent 55%);
    pointer-events:none;
}

.hero-image{
    width:100%;
    height:560px;
    object-fit:cover;
}

.hero-tech-card{
    position:absolute;
    bottom:25px;
    right:25px;
    z-index:4;
    padding:18px 20px;
    width:240px;
    border-radius:18px;
    background:rgba(10,10,10,.8);
    backdrop-filter:blur(18px);
    border:1px solid rgba(255,255,255,.12);
}

.hero-tech-card small{
    color:#888;
    display:block;
    margin-bottom:5px;
}

.hero-tech-card strong{
    font-size:18px;
}

.tech-line{
    margin-top:12px;
    height:3px;
    background:#262626;
    border-radius:10px;
    overflow:hidden;
}

.tech-line span{
    display:block;
    width:86%;
    height:100%;
    background:var(--red);
}

/* ================= STATS ================= */

.stats{
    border-top:1px solid var(--line);
    border-bottom:1px solid var(--line);
    background:#0a0a0a;
}

.stats-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
}

.stat{
    padding:30px 20px;
    text-align:center;
    border-left:1px solid var(--line);
}

.stat:last-child{
    border-left:0;
}

.stat strong{
    font-size:30px;
    display:block;
}

.stat span{
    color:#858585;
    font-size:12px;
}

/* ================= GENERAL SECTIONS ================= */

section{
    padding:110px 0;
}

.section-head{
    max-width:760px;
    margin-bottom:55px;
}

.section-kicker{
    color:var(--red2);
    font-size:12px;
    font-weight:800;
    letter-spacing:1px;
    margin-bottom:12px;
}

.section-title{
    font-size:clamp(30px,4vw,48px);
    line-height:1.25;
    margin-bottom:18px;
}

.section-description{
    color:#919191;
    line-height:2;
    font-size:15px;
}

/* ================= ABOUT ================= */

.about-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:70px;
    align-items:center;
}

.about-card{
    position:relative;
    min-height:460px;
    border-radius:30px;
    background:
        linear-gradient(135deg,#151515,#090909);
    border:1px solid var(--line);
    overflow:hidden;
}

.about-card::before{
    content:"M";
    position:absolute;
    font-size:300px;
    font-weight:900;
    color:rgba(213,31,47,.055);
    left:20px;
    bottom:-80px;
}

.about-card img{
    width:100%;
    height:460px;
    object-fit:cover;
    opacity:.9;
}

.about-content p{
    color:#999;
    line-height:2.1;
    font-size:16px;
    margin-bottom:28px;
}

.check-list{
    display:grid;
    gap:14px;
}

.check{
    display:flex;
    align-items:flex-start;
    gap:12px;
    color:#d0d0d0;
    font-size:14px;
}

.check-icon{
    width:22px;
    height:22px;
    border-radius:7px;
    flex:none;
    display:grid;
    place-items:center;
    background:rgba(213,31,47,.12);
    color:var(--red2);
}

/* ================= SOLUTIONS ================= */

.services{
    background:#090909;
}

.services-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.service-card{
    position:relative;
    padding:32px;
    min-height:290px;
    border-radius:24px;
    background:linear-gradient(145deg,#161616,#0d0d0d);
    border:1px solid var(--line);
    transition:.35s;
    overflow:hidden;
}

.service-card:hover{
    transform:translateY(-7px);
    border-color:rgba(213,31,47,.4);
}

.service-number{
    color:#555;
    font-size:13px;
    font-weight:800;
    direction:ltr;
}

.service-icon{
    width:58px;
    height:58px;
    display:grid;
    place-items:center;
    border-radius:17px;
    background:rgba(213,31,47,.1);
    border:1px solid rgba(213,31,47,.15);
    color:var(--red2);
    font-size:25px;
    margin:25px 0;
}

.service-card h3{
    font-size:20px;
    margin-bottom:12px;
}

.service-card p{
    color:#888;
    line-height:1.9;
    font-size:14px;
}

/* ================= TECHNOLOGY ================= */

.tech-grid{
    display:grid;
    grid-template-columns:1.1fr .9fr;
    gap:55px;
    align-items:center;
}

.tech-image{
    border-radius:30px;
    overflow:hidden;
    border:1px solid var(--line);
    min-height:500px;
}

.tech-image img{
    width:100%;
    height:500px;
    object-fit:cover;
}

.tech-features{
    display:grid;
    gap:18px;
}

.tech-feature{
    display:flex;
    gap:18px;
    padding:20px;
    border:1px solid var(--line);
    border-radius:18px;
    background:rgba(255,255,255,.025);
}

.tech-feature-icon{
    width:45px;
    height:45px;
    border-radius:13px;
    display:grid;
    place-items:center;
    background:rgba(213,31,47,.1);
    color:var(--red2);
    flex:none;
}

.tech-feature h4{
    margin-bottom:6px;
}

.tech-feature p{
    color:#777;
    font-size:13px;
    line-height:1.8;
}

/* ================= HOW IT WORKS ================= */

.process{
    background:#090909;
}

.process-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
}

.process-step{
    padding:30px 22px;
    border:1px solid var(--line);
    border-radius:20px;
    background:#101010;
    position:relative;
}

.process-step::after{
    content:"";
    position:absolute;
    top:45px;
    left:-18px;
    width:20px;
    height:1px;
    background:#333;
}

.process-step:last-child::after{
    display:none;
}

.process-number{
    color:var(--red2);
    font-size:13px;
    font-weight:800;
    margin-bottom:25px;
}

.process-step h3{
    margin-bottom:10px;
}

.process-step p{
    color:#777;
    font-size:13px;
    line-height:1.8;
}

/* ================= SECTORS ================= */

.sectors-grid{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:15px;
}

.sector{
    position:relative;
    min-height:260px;
    border-radius:22px;
    overflow:hidden;
    border:1px solid var(--line);
}

.sector img{
    width:100%;
    height:100%;
    min-height:260px;
    object-fit:cover;
    transition:.5s;
}

.sector:hover img{
    transform:scale(1.07);
}

.sector::after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(0deg,rgba(0,0,0,.9),transparent 70%);
}

.sector-content{
    position:absolute;
    z-index:2;
    bottom:20px;
    right:20px;
    left:20px;
}

.sector-content h3{
    font-size:17px;
}

.sector-content p{
    color:#aaa;
    font-size:11px;
    margin-top:5px;
}

/* ================= WHY US ================= */

.why{
    background:
        radial-gradient(circle at 20% 50%,rgba(213,31,47,.08),transparent 35%),
        #090909;
}

.why-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:70px;
    align-items:center;
}

.why-list{
    display:grid;
    gap:15px;
}

.why-item{
    padding:22px;
    border:1px solid var(--line);
    border-radius:18px;
    display:flex;
    gap:16px;
    background:rgba(255,255,255,.025);
}

.why-item-number{
    width:35px;
    height:35px;
    border-radius:11px;
    display:grid;
    place-items:center;
    background:var(--red);
    font-size:12px;
    font-weight:800;
    flex:none;
}

.why-item h3{
    font-size:15px;
    margin-bottom:5px;
}

.why-item p{
    color:#777;
    font-size:12px;
    line-height:1.8;
}

/* ================= AWARDS ================= */

.awards{
    background:#070707;
}

.awards-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.award-card{
    border:1px solid var(--line);
    border-radius:22px;
    overflow:hidden;
    background:#101010;
    cursor:pointer;
    transition:.35s;
}

.award-card:hover{
    transform:translateY(-6px);
    border-color:rgba(213,31,47,.45);
}

.award-image{
    height:230px;
    background:#151515;
    overflow:hidden;
}

.award-image img{
    width:100%;
    height:100%;
    object-fit:cover;
    transition:.5s;
}

.award-card:hover .award-image img{
    transform:scale(1.04);
}

.award-info{
    padding:20px;
}

.award-info small{
    color:var(--red2);
    font-size:11px;
}

.award-info h3{
    margin-top:7px;
    font-size:16px;
}

.award-info p{
    color:#777;
    font-size:12px;
    margin-top:7px;
    line-height:1.7;
}

/* ================= MILESTONES ================= */

.timeline{
    position:relative;
    max-width:900px;
    margin:auto;
}

.timeline::before{
    content:"";
    position:absolute;
    top:0;
    bottom:0;
    right:16px;
    width:1px;
    background:#292929;
}

.timeline-item{
    position:relative;
    padding-right:55px;
    margin-bottom:38px;
}

.timeline-dot{
    position:absolute;
    right:8px;
    top:4px;
    width:17px;
    height:17px;
    border-radius:50%;
    background:var(--red);
    border:4px solid #070707;
    box-shadow:0 0 0 1px var(--red);
}

.timeline-year{
    color:var(--red2);
    font-size:12px;
    font-weight:800;
}

.timeline-item h3{
    margin:7px 0;
}

.timeline-item p{
    color:#777;
    font-size:13px;
    line-height:1.9;
}

/* ================= MEDIA ================= */

.media-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:18px;
}

.media-card{
    border:1px solid var(--line);
    border-radius:20px;
    padding:25px;
    background:#101010;
}

.media-card span{
    font-size:28px;
    color:var(--red2);
}

.media-card h3{
    margin:15px 0 8px;
}

.media-card p{
    color:#777;
    font-size:12px;
    line-height:1.8;
}

/* ================= CONTACT ================= */

.contact{
    background:
        linear-gradient(135deg,rgba(213,31,47,.12),transparent 45%),
        #0b0b0b;
}

.contact-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:50px;
    align-items:start;
}

.contact-info{
    padding-top:10px;
}

.contact-info p{
    color:#888;
    line-height:2;
    margin:20px 0 30px;
}

.socials{
    display:flex;
    flex-wrap:wrap;
    gap:10px;
}

.social{
    padding:11px 15px;
    border:1px solid var(--line);
    border-radius:12px;
    background:rgba(255,255,255,.025);
    font-size:12px;
    transition:.3s;
}

.social:hover{
    border-color:var(--red);
    transform:translateY(-2px);
}

.contact-form{
    background:#101010;
    border:1px solid var(--line);
    padding:30px;
    border-radius:25px;
}

.form-group{
    margin-bottom:17px;
}

.form-group label{
    display:block;
    color:#aaa;
    font-size:12px;
    margin-bottom:7px;
}

.form-group input,
.form-group textarea{
    width:100%;
    background:#080808;
    border:1px solid #222;
    color:white;
    border-radius:12px;
    padding:14px;
    font-family:inherit;
    outline:none;
    transition:.3s;
}

.form-group input:focus,
.form-group textarea:focus{
    border-color:var(--red);
}

.form-group textarea{
    min-height:140px;
    resize:vertical;
}

/* ================= FOOTER ================= */

footer{
    padding:35px 0;
    border-top:1px solid var(--line);
    background:#050505;
}

.footer-inner{
    display:flex;
    justify-content:space-between;
    align-items:center;
    gap:20px;
}

.footer-inner p{
    color:#666;
    font-size:11px;
}

.footer-brand{
    font-weight:800;
}

.footer-brand span{
    color:var(--red2);
}

/* ================= MODAL ================= */

.modal{
    position:fixed;
    inset:0;
    z-index:3000;
    background:rgba(0,0,0,.88);
    backdrop-filter:blur(10px);
    display:none;
    place-items:center;
    padding:25px;
}

.modal.active{
    display:grid;
}

.modal-content{
    position:relative;
    max-width:900px;
    max-height:90vh;
}

.modal-content img{
    max-height:85vh;
    width:auto;
    max-width:100%;
    border-radius:15px;
}

.modal-close{
    position:absolute;
    top:-45px;
    left:0;
    width:38px;
    height:38px;
    border-radius:50%;
    border:1px solid #444;
    background:#111;
    color:white;
    cursor:pointer;
    font-size:20px;
}

/* ================= MOBILE ================= */

@media(max-width:950px){

    .nav-links{
        position:absolute;
        top:78px;
        right:20px;
        left:20px;
        display:none;
        flex-direction:column;
        align-items:stretch;
        padding:20px;
        border:1px solid var(--line);
        background:#0d0d0d;
        border-radius:18px;
    }

    .nav-links.active{
        display:flex;
    }

    .mobile-menu{
        display:block;
    }

    .hero-grid,
    .about-grid,
    .tech-grid,
    .why-grid,
    .contact-grid{
        grid-template-columns:1fr;
    }

    .hero{
        min-height:auto;
    }

    .hero-content{
        padding-top:80px;
    }

    .hero-image-wrap,
    .hero-image{
        min-height:400px;
        height:400px;
    }

    .services-grid,
    .awards-grid,
    .media-grid{
        grid-template-columns:1fr 1fr;
    }

    .process-grid{
        grid-template-columns:1fr 1fr;
    }

    .sectors-grid{
        grid-template-columns:1fr 1fr;
    }

    .process-step::after{
        display:none;
    }
}

@media(max-width:600px){

    .container{
        width:min(100% - 28px,var(--container));
    }

    section{
        padding:75px 0;
    }

    .hero h1{
        font-size:43px;
    }

    .hero-description{
        font-size:15px;
    }

    .stats-grid{
        grid-template-columns:1fr 1fr;
    }

    .stat{
        border-bottom:1px solid var(--line);
    }

    .services-grid,
    .awards-grid,
    .media-grid,
    .process-grid,
    .sectors-grid{
        grid-template-columns:1fr;
    }

    .hero-tech-card{
        right:15px;
        bottom:15px;
    }

    .footer-inner{
        flex-direction:column;
        text-align:center;
    }
}

</style>
</head>

<body>

<!-- ================= NAVBAR ================= -->

<header class="navbar">

<div class="container nav-inner">

<a href="#home" class="logo">

<img src="assets/mukafih-logo.png" alt="مكافح">

<div class="logo-text">
<strong>مكافح</strong>
<span>MUKAFIH • FIRE PROTECTION</span>
</div>

</a>

<nav class="nav-links" id="navLinks">

<a href="#about" data-ar="من نحن" data-en="About Us">من نحن</a>

<a href="#solutions" data-ar="الحلول" data-en="Solutions">الحلول</a>

<a href="#technology" data-ar="التقنية" data-en="Technology">التقنية</a>

<a href="#sectors" data-ar="القطاعات" data-en="Sectors">القطاعات</a>

<a href="#awards" data-ar="الإنجازات" data-en="Achievements">الإنجازات</a>

<a href="#contact" data-ar="تواصل معنا" data-en="Contact">تواصل معنا</a>

</nav>

<div class="nav-actions">

<button class="lang-btn" id="languageBtn" onclick="toggleLanguage()">
EN
</button>

<button class="mobile-menu" onclick="toggleMenu()">
☰
</button>

</div>

</div>
</header>


<!-- ================= HERO ================= -->

<main>

<section class="hero" id="home">

<div class="container hero-grid">

<div class="hero-content">

<div class="eyebrow">

<span class="eyebrow-dot"></span>

<span
data-ar="تقنيات ذكية للحماية من الحرائق"
data-en="Smart Fire Protection Technology">
تقنيات ذكية للحماية من الحرائق
</span>

</div>

<h1
data-ar="نبتكر اليوم<br>لنحمي <span>الغد</span>"
data-en="Innovating Today<br>to Protect <span>Tomorrow</span>">

نبتكر اليوم<br>لنحمي <span>الغد</span>

</h1>

<p class="hero-description"
data-ar="مكافح شركة تقنية ناشئة تطور حلولًا ذكية ومتقدمة للحماية من الحرائق، تجمع بين الذكاء الاصطناعي والطائرات بدون طيار والتقنيات الحديثة لتعزيز سرعة الاستجابة ورفع مستوى السلامة."
data-en="Mukafih is a technology startup developing intelligent fire protection solutions that combine artificial intelligence, autonomous drones and advanced technologies to improve response and safety.">

مكافح شركة تقنية ناشئة تطور حلولًا ذكية ومتقدمة للحماية من الحرائق، تجمع بين الذكاء الاصطناعي والطائرات بدون طيار والتقنيات الحديثة لتعزيز سرعة الاستجابة ورفع مستوى السلامة.

</p>

<div class="hero-buttons">

<a href="#contact" class="btn btn-primary"
data-ar="تواصل معنا"
data-en="Contact Us">
تواصل معنا
</a>

<a href="#technology" class="btn btn-outline"
data-ar="اكتشف تقنيتنا"
data-en="Explore Our Technology">
اكتشف تقنيتنا
</a>

</div>

</div>


<div class="hero-visual">

<div class="hero-image-wrap">

<img
src="assets/hero-drone-truck.png"
class="hero-image"
alt="Mukafih Fire Protection Technology">

<div class="hero-tech-card">

<small
data-ar="منظومة الحماية الذكية"
data-en="Smart Protection System">
منظومة الحماية الذكية
</small>

<strong>AI • DRONE • FIRE SAFETY</strong>

<div class="tech-line">
<span></span>
</div>

</div>

</div>

</div>

</div>

</section>


<!-- ================= STATS ================= -->

<div class="stats">

<div class="container stats-grid">

<div class="stat">
<strong>AI</strong>
<span data-ar="ذكاء اصطناعي" data-en="Artificial Intelligence">
ذكاء اصطناعي
</span>
</div>

<div class="stat">
<strong>3D</strong>
<span data-ar="خرائط ثلاثية الأبعاد" data-en="3D Mapping">
خرائط ثلاثية الأبعاد
</span>
</div>

<div class="stat">
<strong>UWB</strong>
<span data-ar="تموضع داخلي متقدم" data-en="Advanced Indoor Positioning">
تموضع داخلي متقدم
</span>
</div>

<div class="stat">
<strong>24/7</strong>
<span data-ar="استعداد للحماية" data-en="Protection Readiness">
استعداد للحماية
</span>
</div>

</div>

</div>


<!-- ================= ABOUT ================= -->

<section id="about">

<div class="container about-grid">

<div class="about-card">

<img src="assets/technology.png" alt="Mukafih">

</div>


<div class="about-content">

<div class="section-head">

<div class="section-kicker"
data-ar="من نحن"
data-en="ABOUT US">
من نحن
</div>

<h2 class="section-title"
data-ar="حماية أكثر ذكاءً تبدأ من التقنية."
data-en="Smarter protection starts with technology.">
حماية أكثر ذكاءً تبدأ من التقنية.
</h2>

</div>

<p
data-ar="نحن في مكافح نؤمن أن مستقبل الحماية من الحرائق يعتمد على الجمع بين الخبرة والتقنية والقدرة على الاستجابة في الوقت المناسب. لذلك نعمل على تطوير حلول متقدمة تساعد المنشآت على اكتشاف المخاطر والتعامل معها بذكاء وكفاءة."
data-en="At Mukafih, we believe the future of fire protection lies in combining expertise, technology and timely response. We develop advanced solutions that help facilities detect risks and respond intelligently and efficiently.">

نحن في مكافح نؤمن أن مستقبل الحماية من الحرائق يعتمد على الجمع بين الخبرة والتقنية والقدرة على الاستجابة في الوقت المناسب. لذلك نعمل على تطوير حلول متقدمة تساعد المنشآت على اكتشاف المخاطر والتعامل معها بذكاء وكفاءة.

</p>

<div class="check-list">

<div class="check">
<div class="check-icon">✓</div>
<span data-ar="حلول تقنية متقدمة للحماية من الحرائق"
data-en="Advanced fire protection technology">
حلول تقنية متقدمة للحماية من الحرائق
</span>
</div>

<div class="check">
<div class="check-icon">✓</div>
<span data-ar="دمج الذكاء الاصطناعي مع أنظمة الحماية"
data-en="AI-powered protection systems">
دمج الذكاء الاصطناعي مع أنظمة الحماية
</span>
</div>

<div class="check">
<div class="check-icon">✓</div>
<span data-ar="تركيز على البيئات الصناعية والمنشآت عالية الخطورة"
data-en="Designed for industrial and high-risk environments">
تركيز على البيئات الصناعية والمنشآت عالية الخطورة
</span>
</div>

<div class="check">
<div class="check-icon">✓</div>
<span data-ar="ابتكار سعودي برؤية مستقبلية"
data-en="Saudi innovation with a future-focused vision">
ابتكار سعودي برؤية مستقبلية
</span>
</div>

</div>

</div>

</div>

</section>


<!-- ================= SOLUTIONS ================= -->

<section class="services" id="solutions">

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="حلولنا"
data-en="OUR SOLUTIONS">
حلولنا
</div>

<h2 class="section-title"
data-ar="من الكشف المبكر إلى الاستجابة الذكية."
data-en="From early detection to intelligent response.">
من الكشف المبكر إلى الاستجابة الذكية.
</h2>

<p class="section-description"
data-ar="نطور منظومة متكاملة تساعد المنشآت على رفع مستوى السلامة والاستجابة للمخاطر باستخدام تقنيات حديثة."
data-en="We develop integrated solutions that help facilities improve safety and respond to risks using advanced technologies.">
نطور منظومة متكاملة تساعد المنشآت على رفع مستوى السلامة والاستجابة للمخاطر باستخدام تقنيات حديثة.
</p>

</div>


<div class="services-grid">

<div class="service-card">

<div class="service-number">01</div>

<div class="service-icon">◉</div>

<h3
data-ar="الكشف الذكي عن الحرائق"
data-en="Intelligent Fire Detection">
الكشف الذكي عن الحرائق
</h3>

<p
data-ar="استخدام تقنيات الاستشعار والرؤية الحاسوبية والتصوير الحراري للمساعدة في التعرف على مؤشرات الحريق في وقت مبكر."
data-en="Using sensing technologies, computer vision and thermal imaging to identify fire indicators at an early stage.">
استخدام تقنيات الاستشعار والرؤية الحاسوبية والتصوير الحراري للمساعدة في التعرف على مؤشرات الحريق في وقت مبكر.
</p>

</div>


<div class="service-card">

<div class="service-number">02</div>

<div class="service-icon">✦</div>

<h3
data-ar="الطائرات بدون طيار"
data-en="Firefighting Drones">
الطائرات بدون طيار
</h3>

<p
data-ar="طائرات ذكية مصممة للعمل داخل البيئات التي قد تشكل خطرًا على فرق الاستجابة، مع قدرات استكشاف ومراقبة واستجابة."
data-en="Intelligent drones designed to operate in environments that may be hazardous for response teams, providing inspection, monitoring and response capabilities.">
طائرات ذكية مصممة للعمل داخل البيئات التي قد تشكل خطرًا على فرق الاستجابة، مع قدرات استكشاف ومراقبة واستجابة.
</p>

</div>


<div class="service-card">

<div class="service-number">03</div>

<div class="service-icon">AI</div>

<h3
data-ar="الذكاء الاصطناعي والرؤية الحاسوبية"
data-en="AI & Computer Vision">
الذكاء الاصطناعي والرؤية الحاسوبية
</h3>

<p
data-ar="تحليل البيانات والصور والقراءات الحسية للمساعدة في اتخاذ قرارات أسرع وأكثر دقة أثناء حالات الطوارئ."
data-en="Analyzing visual, sensor and environmental data to support faster and more informed decisions during emergencies.">
تحليل البيانات والصور والقراءات الحسية للمساعدة في اتخاذ قرارات أسرع وأكثر دقة أثناء حالات الطوارئ.
</p>

</div>

</div>

</div>

</section>


<!-- ================= TECHNOLOGY ================= -->

<section id="technology">

<div class="container tech-grid">

<div class="tech-image">

<img src="assets/drone.png" alt="Mukafih Smart Firefighting Drone">

</div>


<div>

<div class="section-head">

<div class="section-kicker"
data-ar="التقنية"
data-en="TECHNOLOGY">
التقنية
</div>

<h2 class="section-title"
data-ar="مصممة للبيئات التي لا يكفي فيها الحل التقليدي."
data-en="Built for environments where traditional protection is not enough.">
مصممة للبيئات التي لا يكفي فيها الحل التقليدي.
</h2>

<p class="section-description"
data-ar="تعتمد منظومة مكافح على مجموعة من التقنيات التي تمكّن الأنظمة من العمل في البيئات الداخلية المعقدة حتى في ظروف يصعب فيها الاعتماد على GPS."
data-en="Mukafih's system combines multiple technologies designed to operate in complex indoor environments where GPS-based positioning may not be available.">
تعتمد منظومة مكافح على مجموعة من التقنيات التي تمكّن الأنظمة من العمل في البيئات الداخلية المعقدة حتى في ظروف يصعب فيها الاعتماد على GPS.
</p>

</div>


<div class="tech-features">

<div class="tech-feature">

<div class="tech-feature-icon">3D</div>

<div>

<h4
data-ar="الخرائط ثلاثية الأبعاد"
data-en="3D Mapping">
الخرائط ثلاثية الأبعاد
</h4>

<p
data-ar="بناء وفهم البيئة الداخلية للمساعدة على الملاحة وتحديد موقع الخطر."
data-en="Building and understanding indoor environments to support navigation and hazard localization.">
بناء وفهم البيئة الداخلية للمساعدة على الملاحة وتحديد موقع الخطر.
</p>

</div>

</div>


<div class="tech-feature">

<div class="tech-feature-icon">◎</div>

<div>

<h4>SLAM + UWB</h4>

<p
data-ar="تقنيات للتموضع والملاحة في البيئات الداخلية المعقدة."
data-en="Positioning and navigation technologies for complex indoor environments.">
تقنيات للتموضع والملاحة في البيئات الداخلية المعقدة.
</p>

</div>

</div>


<div class="tech-feature">

<div class="tech-feature-icon">IR</div>

<div>

<h4
data-ar="التصوير الحراري"
data-en="Thermal Imaging">
التصوير الحراري
</h4>

<p
data-ar="الاستفادة من البيانات الحرارية للمساعدة في تقييم مؤشرات الحرارة ومصادر الخطر."
data-en="Using thermal data to support heat assessment and hazard identification.">
الاستفادة من البيانات الحرارية للمساعدة في تقييم مؤشرات الحرارة ومصادر الخطر.
</p>

</div>

</div>


<div class="tech-feature">

<div class="tech-feature-icon">AI</div>

<div>

<h4
data-ar="تحقق متعدد المستشعرات"
data-en="Multi-Sensor Verification">
تحقق متعدد المستشعرات
</h4>

<p
data-ar="دمج البيانات الحرارية والبصرية وبيانات العمق للمساعدة على تقليل الإنذارات الكاذبة."
data-en="Combining thermal, visual and depth data to help reduce false alarms.">
دمج البيانات الحرارية والبصرية وبيانات العمق للمساعدة على تقليل الإنذارات الكاذبة.
</p>

</div>

</div>

</div>

</div>

</div>

</section>


<!-- ================= PROCESS ================= -->

<section class="process">

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="كيف تعمل المنظومة؟"
data-en="HOW IT WORKS">
كيف تعمل المنظومة؟
</div>

<h2 class="section-title"
data-ar="استجابة ذكية تبدأ من لحظة اكتشاف الخطر."
data-en="Intelligent response starts the moment a risk is detected.">
استجابة ذكية تبدأ من لحظة اكتشاف الخطر.
</h2>

</div>


<div class="process-grid">

<div class="process-step">

<div class="process-number">01</div>

<h3
data-ar="اكتشاف"
data-en="Detect">
اكتشاف
</h3>

<p
data-ar="تلتقط المستشعرات مؤشرات الحرارة أو الدخان أو الخطر."
data-en="Sensors identify heat, smoke or other fire indicators.">
تلتقط المستشعرات مؤشرات الحرارة أو الدخان أو الخطر.
</p>

</div>


<div class="process-step">

<div class="process-number">02</div>

<h3
data-ar="تحليل"
data-en="Analyze">
تحليل
</h3>

<p
data-ar="يتم تحليل البيانات باستخدام أنظمة الذكاء الاصطناعي والرؤية الحاسوبية."
data-en="AI and computer vision systems analyze the collected data.">
يتم تحليل البيانات باستخدام أنظمة الذكاء الاصطناعي والرؤية الحاسوبية.
</p>

</div>


<div class="process-step">

<div class="process-number">03</div>

<h3
data-ar="تحديد الموقع"
data-en="Locate">
تحديد الموقع
</h3>

<p
data-ar="تساعد الخرائط والأنظمة الملاحية على تحديد موقع الخطر داخل المنشأة."
data-en="Mapping and navigation systems help locate the hazard inside the facility.">
تساعد الخرائط والأنظمة الملاحية على تحديد موقع الخطر داخل المنشأة.
</p>

</div>


<div class="process-step">

<div class="process-number">04</div>

<h3
data-ar="الاستجابة"
data-en="Respond">
الاستجابة
</h3>

<p
data-ar="تتجه المنظومة نحو موقع الخطر لدعم الاستجابة الأولية وتقليل زمن الوصول."
data-en="The system moves toward the hazard to support initial response and reduce response time.">
تتجه المنظومة نحو موقع الخطر لدعم الاستجابة الأولية وتقليل زمن الوصول.
</p>

</div>

</div>

</div>

</section>


<!-- ================= SECTORS ================= -->

<section id="sectors">

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="القطاعات"
data-en="INDUSTRIES">
القطاعات
</div>

<h2 class="section-title"
data-ar="حلول مصممة للبيئات عالية الخطورة."
data-en="Solutions designed for high-risk environments.">
حلول مصممة للبيئات عالية الخطورة.
</h2>

</div>


<div class="sectors-grid">

<div class="sector">

<img src="assets/factory.jpg" alt="Factories">

<div class="sector-content">

<h3
data-ar="المصانع والمنشآت الصناعية"
data-en="Factories & Industrial Facilities">
المصانع والمنشآت الصناعية
</h3>

<p
data-ar="مراقبة واستجابة في البيئات التشغيلية المعقدة."
data-en="Monitoring and response in complex operational environments.">
مراقبة واستجابة في البيئات التشغيلية المعقدة.
</p>

</div>

</div>


<div class="sector">

<img src="assets/warehouse.jpg" alt="Warehouses">

<div class="sector-content">

<h3
data-ar="المستودعات"
data-en="Warehouses">
المستودعات
</h3>

<p
data-ar="الوصول إلى المناطق المرتفعة والعميقة التي يصعب الوصول إليها."
data-en="Accessing elevated and difficult-to-reach areas.">
الوصول إلى المناطق المرتفعة والعميقة التي يصعب الوصول إليها.
</p>

</div>

</div>


<div class="sector">

<img src="assets/data-center.jpg" alt="Data Centers">

<div class="sector-content">

<h3
data-ar="مراكز البيانات"
data-en="Data Centers">
مراكز البيانات
</h3>

<p
data-ar="استجابة أولية مع مراعاة حساسية المعدات."
data-en="Initial response while considering sensitive equipment.">
استجابة أولية مع مراعاة حساسية المعدات.
</p>

</div>

</div>


<div class="sector">

<img src="assets/electrical-room.jpg" alt="Electrical Rooms">

<div class="sector-content">

<h3
data-ar="غرف الكهرباء والمحطات"
data-en="Electrical Rooms & Substations">
غرف الكهرباء والمحطات
</h3>

<p
data-ar="حلول للبيئات المغلقة والمعقدة التي لا يتوفر فيها GPS."
data-en="Solutions for enclosed and complex environments without GPS.">
حلول للبيئات المغلقة والمعقدة التي لا يتوفر فيها GPS.
</p>

</div>

</div>

</div>

</div>

</section>


<!-- ================= WHY US ================= -->

<section class="why">

<div class="container why-grid">

<div>

<div class="section-kicker"
data-ar="لماذا مكافح؟"
data-en="WHY MUKAFIH">
لماذا مكافح؟
</div>

<h2 class="section-title"
data-ar="لأن السلامة لا تحتمل الانتظار."
data-en="Because safety cannot wait.">
لأن السلامة لا تحتمل الانتظار.
</h2>

<p class="section-description"
data-ar="نحن لا نضيف التقنية لمجرد التقنية؛ بل نوظفها لحل مشكلة حقيقية في الاستجابة للحرائق وحماية الأرواح والأصول."
data-en="We do not use technology for technology's sake. We apply it to solve real fire-response challenges and protect people and assets.">
نحن لا نضيف التقنية لمجرد التقنية؛ بل نوظفها لحل مشكلة حقيقية في الاستجابة للحرائق وحماية الأرواح والأصول.
</p>

</div>


<div class="why-list">

<div class="why-item">

<div class="why-item-number">01</div>

<div>

<h3
data-ar="ابتكار تقني"
data-en="Technology-driven innovation">
ابتكار تقني
</h3>

<p
data-ar="دمج الذكاء الاصطناعي والطائرات بدون طيار وتقنيات الاستشعار."
data-en="Combining AI, drones and advanced sensing technologies.">
دمج الذكاء الاصطناعي والطائرات بدون طيار وتقنيات الاستشعار.
</p>

</div>

</div>


<div class="why-item">

<div class="why-item-number">02</div>

<div>

<h3
data-ar="حلول مخصصة"
data-en="Purpose-built solutions">
حلول مخصصة
</h3>

<p
data-ar="تصميم المنظومة وفق طبيعة البيئة والمخاطر الموجودة داخل المنشأة."
data-en="Solutions designed around the facility's environment and risk profile.">
تصميم المنظومة وفق طبيعة البيئة والمخاطر الموجودة داخل المنشأة.
</p>

</div>

</div>


<div class="why-item">

<div class="why-item-number">03</div>

<div>

<h3
data-ar="استجابة أسرع"
data-en="Faster response">
استجابة أسرع
</h3>

<p
data-ar="الهدف هو تقليل الزمن بين اكتشاف الخطر والوصول إليه."
data-en="Our goal is to reduce the time between detecting a hazard and reaching it.">
الهدف هو تقليل الزمن بين اكتشاف الخطر والوصول إليه.
</p>

</div>

</div>


<div class="why-item">

<div class="why-item-number">04</div>

<div>

<h3
data-ar="ابتكار سعودي"
data-en="Saudi innovation">
ابتكار سعودي
</h3>

<p
data-ar="نبني تقنية محلية قادرة على المنافسة والتوسع مستقبلًا."
data-en="Building local technology with the potential to compete and scale.">
نبني تقنية محلية قادرة على المنافسة والتوسع مستقبلًا.
</p>

</div>

</div>

</div>

</div>

</section>


<!-- ================= AWARDS ================= -->

<section class="awards" id="awards">

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="الإنجازات والجوائز"
data-en="ACHIEVEMENTS & AWARDS">
الإنجازات والجوائز
</div>

<h2 class="section-title"
data-ar="إنجازات تعكس رحلة الابتكار."
data-en="Milestones that reflect our innovation journey.">
إنجازات تعكس رحلة الابتكار.
</h2>

<p class="section-description"
data-ar="من الاحتضان والبرامج الريادية إلى المشاركات والمعارض والجوائز الدولية."
data-en="From incubation and entrepreneurship programs to exhibitions and international awards.">
من الاحتضان والبرامج الريادية إلى المشاركات والمعارض والجوائز الدولية.
</p>

</div>


<div class="awards-grid">


<div class="award-card" onclick="openModal('assets/award-geneva.jpg')">

<div class="award-image">
<img src="assets/award-geneva.jpg" alt="Geneva Gold Medal">
</div>

<div class="award-info">

<small>INTERNATIONAL</small>

<h3
data-ar="معرض جنيف الدولي للاختراعات"
data-en="Geneva International Exhibition of Inventions">
معرض جنيف الدولي للاختراعات
</h3>

<p
data-ar="الميدالية الذهبية مع مرتبة الشرف."
data-en="Gold Medal with Honors.">
الميدالية الذهبية مع مرتبة الشرف.
</p>

</div>

</div>


<div class="award-card" onclick="openModal('assets/award-hkust.jpg')">

<div class="award-image">
<img src="assets/award-hkust.jpg" alt="HKUST Award">
</div>

<div class="award-info">

<small>SPECIAL AWARD</small>

<h3>
THE HONG KONG UNIVERSITY OF SCIENCE AND TECHNOLOGY
</h3>

<p
data-ar="جائزة خاصة عن الابتكار."
data-en="Special award recognizing the innovation.">
جائزة خاصة عن الابتكار.
</p>

</div>

</div>


<div class="award-card" onclick="openModal('assets/award-french.jpg')">

<div class="award-image">
<img src="assets/award-french.jpg" alt="French Inventors Federation">
</div>

<div class="award-info">

<small>SPECIAL AWARD</small>

<h3
data-ar="الاتحاد الفرنسي للمخترعين"
data-en="French Inventors Federation">
الاتحاد الفرنسي للمخترعين
</h3>

<p
data-ar="شهادة وميدالية، مع الإشارة إلى الاختراع ضمن أفضل الاختراعات في المعرض."
data-en="Certificate and medal, with recognition among the leading inventions at the exhibition.">
شهادة وميدالية، مع الإشارة إلى الاختراع ضمن أفضل الاختراعات في المعرض.
</p>

</div>

</div>


<div class="award-card" onclick="openModal('assets/award-malaysia.jpg')">

<div class="award-image">
<img src="assets/award-malaysia.jpg" alt="Malaysia Special Award">
</div>

<div class="award-info">

<small>SPECIAL AWARD</small>

<h3
data-ar="جائزة الوفد الماليزي"
data-en="Malaysia Delegation Special Award">
جائزة الوفد الماليزي
</h3>

<p
data-ar="جائزة خاصة ضمن معرض جنيف الدولي."
data-en="Special award presented during the Geneva exhibition.">
جائزة خاصة ضمن معرض جنيف الدولي.
</p>

</div>

</div>


<div class="award-card" onclick="openModal('assets/award-qassim.jpg')">

<div class="award-image">
<img src="assets/award-qassim.jpg" alt="Qassim University Award">
</div>

<div class="award-info">

<small>SPECIAL AWARD</small>

<h3
data-ar="جامعة القصيم"
data-en="Qassim University">
جامعة القصيم
</h3>

<p
data-ar="جائزة خاصة تقديرًا للابتكار."
data-en="Special award recognizing the innovation.">
جائزة خاصة تقديرًا للابتكار.
</p>

</div>

</div>


<div class="award-card" onclick="openModal('assets/enjaz.jpg')">

<div class="award-image">
<img src="assets/enjaz.jpg" alt="Enjaz Saudi">
</div>

<div class="award-info">

<small>2026</small>

<h3
data-ar="إنجاز السعودية"
data-en="Enjaz Saudi">
إنجاز السعودية
</h3>

<p
data-ar="التأهل إلى نهائيات مسابقة فكرة."
data-en="Finalist in the Idea Competition.">
التأهل إلى نهائيات مسابقة فكرة.
</p>

</div>

</div>

</div>

</div>

</section>


<!-- ================= TIMELINE ================= -->

<section>

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="رحلتنا"
data-en="OUR JOURNEY">
رحلتنا
</div>

<h2 class="section-title"
data-ar="من الفكرة إلى الابتكار."
data-en="From idea to innovation.">
من الفكرة إلى الابتكار.
</h2>

</div>


<div class="timeline">


<div class="timeline-item">

<div class="timeline-dot"></div>

<div class="timeline-year">2025</div>

<h3
data-ar="برنامج الاحتضان في CEIES"
data-en="CEIES Incubation Program">
برنامج الاحتضان في CEIES
</h3>

<p
data-ar="الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز خلال عام 2025."
data-en="Incubation at the Center of Excellence in Engineering and Electrical Systems at King Abdulaziz University during 2025.">
الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز خلال عام 2025.
</p>

</div>


<div class="timeline-item">

<div class="timeline-dot"></div>

<div class="timeline-year">2026</div>

<h3
data-ar="إنجاز السعودية"
data-en="Enjaz Saudi">
إنجاز السعودية
</h3>

<p
data-ar="التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية."
data-en="Reached the finals of Enjaz Saudi's Idea Competition.">
التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية.
</p>

</div>


<div class="timeline-item">

<div class="timeline-dot"></div>

<div class="timeline-year">2026</div>

<h3
data-ar="المؤتمر الأول للابتكار وريادة الأعمال"
data-en="First Innovation & Entrepreneurship Conference">
المؤتمر الأول للابتكار وريادة الأعمال
</h3>

<p
data-ar="التواجد ضمن أفضل 20 مشروعًا رياديًا والمشاركة في المعرض."
data-en="Selected among the Top 20 entrepreneurial projects and participated in the exhibition.">
التواجد ضمن أفضل 20 مشروعًا رياديًا والمشاركة في المعرض.
</p>

</div>


<div class="timeline-item">

<div class="timeline-dot"></div>

<div class="timeline-year">2026</div>

<h3
data-ar="معرض جنيف الدولي للاختراعات"
data-en="Geneva International Exhibition of Inventions">
معرض جنيف الدولي للاختراعات
</h3>

<p
data-ar="الحصول على الميدالية الذهبية مع مرتبة الشرف، إضافة إلى ثلاث جوائز خاصة دولية وجائزة خاصة من جامعة القصيم."
data-en="Won a Gold Medal with Honors, along with international special awards and a special award from Qassim University.">
الحصول على الميدالية الذهبية مع مرتبة الشرف، إضافة إلى ثلاث جوائز خاصة دولية وجائزة خاصة من جامعة القصيم.
</p>

</div>


<div class="timeline-item">

<div class="timeline-dot"></div>

<div class="timeline-year">2026</div>

<h3
data-ar="تمثيل مركز الابتكار وريادة الأعمال"
data-en="Representing the Innovation & Entrepreneurship Center">
تمثيل مركز الابتكار وريادة الأعمال
</h3>

<p
data-ar="تمثيل مركز الابتكار وريادة الأعمال بجامعة الملك عبدالعزيز في ملتقى تمكين المستقبل."
data-en="Represented King Abdulaziz University's Innovation and Entrepreneurship Center at the Future Empowerment Forum.">
تمثيل مركز الابتكار وريادة الأعمال بجامعة الملك عبدالعزيز في ملتقى تمكين المستقبل.
</p>

</div>

</div>

</div>

</section>


<!-- ================= MEDIA ================= -->

<section class="services">

<div class="container">

<div class="section-head">

<div class="section-kicker"
data-ar="الحضور والظهور"
data-en="MEDIA & PRESENCE">
الحضور والظهور
</div>

<h2 class="section-title"
data-ar="من الابتكار إلى المجتمع."
data-en="Taking innovation beyond the lab.">
من الابتكار إلى المجتمع.
</h2>

</div>


<div class="media-grid">


<div class="media-card">

<span>01</span>

<h3
data-ar="لقاء صاحب السمو الأمير سعود بن جلوي"
data-en="Meeting with HRH Prince Saud bin Jalawi">
لقاء صاحب السمو الأمير سعود بن جلوي
</h3>

<p
data-ar="لقاء بعد الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز."
data-en="A meeting following the Geneva achievement, attended by the President of King Abdulaziz University.">
لقاء بعد الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز.
</p>

</div>


<div class="media-card">

<span>02</span>

<h3
data-ar="إذاعة الرياض"
data-en="Riyadh Radio">
إذاعة الرياض
</h3>

<p
data-ar="المشاركة في برنامج فرسان التمكين."
data-en="Participation in the Faris Al-Tamkeen program.">
المشاركة في برنامج فرسان التمكين.
</p>

</div>


<div class="media-card">

<span>03</span>

<h3
data-ar="أسبوع ريادة الأعمال – غرفة جدة"
data-en="Entrepreneurship Week – Jeddah Chamber">
أسبوع ريادة الأعمال – غرفة جدة
</h3>

<p
data-ar="المشاركة ضمن فعاليات أسبوع ريادة الأعمال."
data-en="Participation in Entrepreneurship Week activities.">
المشاركة ضمن فعاليات أسبوع ريادة الأعمال.
</p>

</div>

</div>

</div>

</section>


<!-- ================= CONTACT ================= -->

<section class="contact" id="contact">

<div class="container contact-grid">


<div class="contact-info">

<div class="section-kicker"
data-ar="تواصل معنا"
data-en="CONTACT US">
تواصل معنا
</div>

<h2 class="section-title"
data-ar="لنبدأ محادثة تصنع فرقًا."
data-en="Let's start a conversation that makes a difference.">
لنبدأ محادثة تصنع فرقًا.
</h2>

<p
data-ar="نحن هنا للإجابة على استفساراتكم ومناقشة فرص التعاون والشراكات. يسعدنا تواصلكم معنا."
data-en="We are here to answer your questions and discuss opportunities for collaboration and partnerships.">
نحن هنا للإجابة على استفساراتكم ومناقشة فرص التعاون والشراكات. يسعدنا تواصلكم معنا.
</p>


<div class="socials">

<a class="social"
href="https://x.com/muk_fh"
target="_blank">
X
</a>

<a class="social"
href="https://www.instagram.com/muk.fh"
target="_blank">
Instagram
</a>

<a class="social"
href="https://www.linkedin.com/company/mokfeh/"
target="_blank">
LinkedIn
</a>

<a class="social"
href="https://www.tiktok.com/@muk.fh"
target="_blank">
TikTok
</a>

</div>

</div>


<form class="contact-form" onsubmit="sendMessage(event)">

<div class="form-group">

<label
data-ar="الاسم الكامل"
data-en="Full Name">
الاسم الكامل
</label>

<input
type="text"
required
placeholder="الاسم الكامل"
data-placeholder-ar="الاسم الكامل"
data-placeholder-en="Full Name">

</div>


<div class="form-group">

<label
data-ar="البريد الإلكتروني"
data-en="Email">
البريد الإلكتروني
</label>

<input
type="email"
required
placeholder="البريد الإلكتروني"
data-placeholder-ar="البريد الإلكتروني"
data-placeholder-en="Email">

</div>


<div class="form-group">

<label
data-ar="الرسالة"
data-en="Message">
الرسالة
</label>

<textarea
required
placeholder="اكتب رسالتك هنا..."
data-placeholder-ar="اكتب رسالتك هنا..."
data-placeholder-en="Write your message here..."></textarea>

</div>


<button class="btn btn-primary" type="submit"
data-ar="إرسال الرسالة"
data-en="Send Message">
إرسال الرسالة
</button>

</form>

</div>

</section>

</main>


<!-- ================= FOOTER ================= -->

<footer>

<div class="container footer-inner">

<div class="footer-brand">
<span>مكافح</span> MUKAFIH
</div>

<p
data-ar="© 2026 مكافح. جميع الحقوق محفوظة."
data-en="© 2026 Mukafih. All rights reserved.">
© 2026 مكافح. جميع الحقوق محفوظة.
</p>

<p>
FIRE PROTECTION COMPANY
</p>

</div>

</footer>


<!-- ================= IMAGE MODAL ================= -->

<div class="modal" id="imageModal" onclick="closeModal()">

<div class="modal-content" onclick="event.stopPropagation()">

<button class="modal-close" onclick="closeModal()">×</button>

<img id="modalImage" src="" alt="Award">

</div>

</div>


<script>

/* ================= LANGUAGE ================= */

let currentLanguage = "ar";

function toggleLanguage(){

    currentLanguage = currentLanguage === "ar" ? "en" : "ar";

    document.documentElement.lang = currentLanguage;
    document.documentElement.dir =
        currentLanguage === "ar" ? "rtl" : "ltr";

    document.body.classList.toggle(
        "en",
        currentLanguage === "en"
    );

    document.querySelectorAll("[data-ar]").forEach(el => {

        const text = el.getAttribute(
            "data-" + currentLanguage
        );

        if(text){
            el.innerHTML = text;
        }

    });


    document.querySelectorAll(
        "input[data-placeholder-ar], textarea[data-placeholder-ar]"
    ).forEach(el => {

        const placeholder = el.getAttribute(
            "data-placeholder-" + currentLanguage
        );

        if(placeholder){
            el.placeholder = placeholder;
        }

    });


    document.getElementById("languageBtn").textContent =
        currentLanguage === "ar" ? "EN" : "عربي";

}


/* ================= MOBILE MENU ================= */

function toggleMenu(){

    document
        .getElementById("navLinks")
        .classList.toggle("active");

}


/* close mobile menu after clicking */

document.querySelectorAll(".nav-links a").forEach(link => {

    link.addEventListener("click", () => {

        document
            .getElementById("navLinks")
            .classList.remove("active");

    });

});


/* ================= AWARD MODAL ================= */

function openModal(image){

    document
        .getElementById("modalImage")
        .src = image;

    document
        .getElementById("imageModal")
        .classList.add("active");

}


function closeModal(){

    document
        .getElementById("imageModal")
        .classList.remove("active");

}


/* ================= CONTACT ================= */

function sendMessage(event){

    event.preventDefault();

    const message =
        currentLanguage === "ar"
        ? "شكرًا لتواصلكم مع مكافح. سيتم التواصل معكم قريبًا."
        : "Thank you for contacting Mukafih. We will get back to you soon.";

    alert(message);

}


/* ================= ESC KEY ================= */

document.addEventListener("keydown", function(e){

    if(e.key === "Escape"){
        closeModal();
    }

});

</script>

</body>
</html>
