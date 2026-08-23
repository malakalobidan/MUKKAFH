<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>مكافح | MUKAFIH — حلول ذكية للحماية من الحرائق</title>

<meta name="description"
content="مكافح — حلول متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والطائرات المسيّرة لحماية المنشآت ورفع مستوى السلامة.">

<meta name="keywords"
content="مكافح, MUKAFIH, مكافحة الحرائق, Fire Protection, AI Firefighting, Drones, Saudi Arabia">

<meta name="author" content="MUKAFIH">

<meta property="og:title" content="مكافح | MUKAFIH">
<meta property="og:description"
content="نبتكر اليوم لنحمي الغد — حلول ذكية ومتقدمة للحماية من الحرائق.">
<meta property="og:type" content="website">
<meta property="og:url" content="https://malakalobidan.github.io/MUKKAFH/">
<meta property="og:image" content="assets/mukafih-logo.png">

<link rel="icon" href="assets/mukafih-logo.png">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700;800;900&family=Montserrat:wght@400;500;600;700;800;900&display=swap" rel="stylesheet">

<style>

:root{
    --red:#e3262e;
    --red-dark:#b8171e;
    --black:#050505;
    --black2:#0b0b0b;
    --black3:#111111;
    --white:#ffffff;
    --gray:#a7a7a7;
    --gray2:#d5d5d5;
    --border:rgba(255,255,255,.10);
    --max:1240px;
    --radius:22px;
    --transition:.35s cubic-bezier(.2,.8,.2,1);
}

*{
    margin:0;
    padding:0;
    box-sizing:border-box;
}

html{
    scroll-behavior:smooth;
}

body{
    background:var(--black);
    color:#fff;
    font-family:"Cairo",sans-serif;
    overflow-x:hidden;
    line-height:1.8;
}

body.en{
    font-family:"Montserrat","Cairo",sans-serif;
    direction:ltr;
}

body.en .ar{
    display:none!important;
}

body:not(.en) .en-text{
    display:none!important;
}

img{
    max-width:100%;
    display:block;
}

a{
    text-decoration:none;
    color:inherit;
}

button,
input,
textarea,
select{
    font-family:inherit;
}

button{
    cursor:pointer;
}

::selection{
    background:var(--red);
    color:#fff;
}

.container{
    width:min(calc(100% - 40px),var(--max));
    margin:auto;
}

section{
    scroll-margin-top:90px;
}

.section{
    padding:120px 0;
}

.eyebrow{
    color:var(--red);
    font-size:13px;
    font-weight:800;
    letter-spacing:2px;
    display:flex;
    align-items:center;
    gap:10px;
    margin-bottom:18px;
}

.eyebrow:before{
    content:"";
    width:30px;
    height:2px;
    background:var(--red);
}

h2{
    font-size:clamp(40px,6vw,72px);
    line-height:1.05;
    letter-spacing:-2px;
    margin-bottom:25px;
}

.section-desc{
    max-width:720px;
    color:var(--gray);
    font-size:17px;
    line-height:2;
}

/* HEADER */

header{
    position:fixed;
    top:0;
    left:0;
    right:0;
    z-index:1000;
    transition:var(--transition);
    background:linear-gradient(to bottom,rgba(0,0,0,.75),transparent);
}

header.scrolled{
    background:rgba(5,5,5,.90);
    backdrop-filter:blur(18px);
    border-bottom:1px solid var(--border);
}

.nav{
    height:82px;
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:20px;
}

.logo{
    display:flex;
    align-items:center;
    gap:11px;
    flex-shrink:0;
}

.logo img{
    width:48px;
    height:48px;
    object-fit:contain;
}

.logo-text{
    display:flex;
    flex-direction:column;
    line-height:1.15;
}

.logo-ar{
    font-size:18px;
    font-weight:900;
}

.logo-en{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-size:9px;
    letter-spacing:2px;
    font-weight:800;
}

.nav-links{
    display:flex;
    align-items:center;
    gap:28px;
    list-style:none;
}

.nav-links a{
    color:#ddd;
    font-size:14px;
    transition:var(--transition);
    position:relative;
}

.nav-links a:after{
    content:"";
    position:absolute;
    bottom:-8px;
    right:0;
    width:0;
    height:2px;
    background:var(--red);
    transition:var(--transition);
}

body.en .nav-links a:after{
    right:auto;
    left:0;
}

.nav-links a:hover{
    color:#fff;
}

.nav-links a:hover:after{
    width:100%;
}

.nav-actions{
    display:flex;
    align-items:center;
    gap:10px;
}

.lang-btn{
    border:1px solid var(--border);
    background:rgba(255,255,255,.04);
    color:#fff;
    border-radius:999px;
    padding:8px 16px;
    font-weight:800;
    transition:var(--transition);
}

.lang-btn:hover{
    background:#fff;
    color:#000;
}

.menu-btn{
    display:none;
    background:none;
    border:0;
    color:#fff;
    font-size:28px;
}

/* HERO */

.hero{
    min-height:100vh;
    display:flex;
    align-items:center;
    position:relative;
    overflow:hidden;
}

.hero-image{
    position:absolute;
    inset:0;
    width:100%;
    height:100%;
    object-fit:cover;
    opacity:.40;
}

.hero-overlay{
    position:absolute;
    inset:0;
    background:
        linear-gradient(90deg,rgba(0,0,0,.96),rgba(0,0,0,.70),rgba(0,0,0,.20)),
        linear-gradient(0deg,rgba(0,0,0,.55),transparent);
}

body.en .hero-overlay{
    background:
        linear-gradient(90deg,rgba(0,0,0,.20),rgba(0,0,0,.70),rgba(0,0,0,.96)),
        linear-gradient(0deg,rgba(0,0,0,.55),transparent);
}

.hero-content{
    position:relative;
    z-index:2;
    padding-top:90px;
    max-width:900px;
}

.hero-kicker{
    color:var(--red);
    font-size:13px;
    letter-spacing:3px;
    font-weight:900;
    margin-bottom:20px;
}

.hero h1{
    font-size:clamp(50px,8vw,105px);
    line-height:.98;
    letter-spacing:-5px;
    font-weight:900;
    margin-bottom:30px;
}

.hero h1 span{
    color:var(--red);
}

.hero-text{
    max-width:680px;
    color:#d0d0d0;
    font-size:18px;
    line-height:2;
    margin-bottom:35px;
}

.buttons{
    display:flex;
    flex-wrap:wrap;
    gap:13px;
}

.btn{
    min-height:52px;
    padding:0 25px;
    display:inline-flex;
    align-items:center;
    justify-content:center;
    border-radius:999px;
    font-weight:800;
    transition:var(--transition);
}

.btn-primary{
    background:var(--red);
    color:#fff;
    box-shadow:0 15px 40px rgba(227,38,46,.18);
}

.btn-primary:hover{
    background:#ff3038;
    transform:translateY(-3px);
}

.btn-outline{
    border:1px solid rgba(255,255,255,.25);
    background:rgba(255,255,255,.04);
    color:#fff;
}

.btn-outline:hover{
    background:#fff;
    color:#000;
}

/* ABOUT */

.about-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:70px;
    align-items:center;
}

.about-image{
    border-radius:var(--radius);
    overflow:hidden;
    border:1px solid var(--border);
    background:#111;
}

.about-image img{
    width:100%;
    height:540px;
    object-fit:cover;
}

.about-content p{
    color:var(--gray);
    font-size:17px;
    line-height:2;
    margin-bottom:25px;
}

.values{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:12px;
    margin-top:30px;
}

.value{
    border:1px solid var(--border);
    background:rgba(255,255,255,.025);
    border-radius:16px;
    padding:20px;
}

.value strong{
    color:var(--red);
    display:block;
    font-size:13px;
    margin-bottom:5px;
}

.value span{
    font-weight:800;
}

/* SOLUTIONS */

.solutions-grid{
    display:grid;
    grid-template-columns:repeat(2,1fr);
    gap:18px;
    margin-top:55px;
}

.card{
    position:relative;
    padding:35px;
    border:1px solid var(--border);
    background:linear-gradient(145deg,#111,#090909);
    border-radius:var(--radius);
    min-height:260px;
    transition:var(--transition);
    overflow:hidden;
}

.card:before{
    content:"";
    position:absolute;
    width:150px;
    height:150px;
    border-radius:50%;
    background:var(--red);
    filter:blur(80px);
    opacity:0;
    top:-60px;
    right:-60px;
    transition:var(--transition);
}

.card:hover{
    transform:translateY(-7px);
    border-color:rgba(227,38,46,.35);
}

.card:hover:before{
    opacity:.18;
}

.card-number{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-size:13px;
    font-weight:900;
    margin-bottom:25px;
}

.card h3{
    font-size:25px;
    margin-bottom:13px;
    position:relative;
}

.card p{
    color:var(--gray);
    line-height:1.9;
    position:relative;
}

/* TECHNOLOGY */

.tech{
    background:#090909;
}

.tech-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:70px;
    align-items:center;
}

.tech-image{
    border-radius:var(--radius);
    overflow:hidden;
    border:1px solid var(--border);
}

.tech-image img{
    width:100%;
    height:580px;
    object-fit:cover;
}

.tech-list{
    margin-top:35px;
    display:grid;
    gap:13px;
}

.tech-item{
    display:flex;
    gap:18px;
    align-items:flex-start;
    padding:20px;
    border:1px solid var(--border);
    border-radius:16px;
    background:rgba(255,255,255,.025);
}

.tech-number{
    width:38px;
    height:38px;
    display:grid;
    place-items:center;
    background:var(--red);
    border-radius:50%;
    font-size:12px;
    font-weight:900;
    flex-shrink:0;
}

.tech-item h3{
    font-size:17px;
    margin-bottom:3px;
}

.tech-item p{
    color:var(--gray);
    font-size:14px;
}

/* PROCESS */

.process-grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:12px;
    margin-top:55px;
}

.process{
    padding:25px 20px;
    border:1px solid var(--border);
    border-radius:18px;
    background:#0c0c0c;
    min-height:210px;
}

.process-number{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-size:13px;
    font-weight:900;
    margin-bottom:30px;
}

.process h3{
    font-size:18px;
    margin-bottom:10px;
}

.process p{
    color:var(--gray);
    font-size:13px;
    line-height:1.8;
}

/* SECTORS */

.sectors{
    background:#090909;
}

.sectors-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:16px;
    margin-top:55px;
}

.sector{
    min-height:250px;
    position:relative;
    overflow:hidden;
    border-radius:20px;
    border:1px solid var(--border);
}

.sector img{
    position:absolute;
    inset:0;
    width:100%;
    height:100%;
    object-fit:cover;
    opacity:.55;
    transition:var(--transition);
}

.sector:after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(0deg,#000,transparent 70%);
}

.sector:hover img{
    transform:scale(1.06);
    opacity:.72;
}

.sector-content{
    position:absolute;
    z-index:2;
    bottom:22px;
    right:22px;
    left:22px;
}

body.en .sector-content{
    right:auto;
    left:22px;
}

.sector-number{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-size:12px;
    font-weight:900;
}

.sector h3{
    font-size:20px;
    margin-top:4px;
}

/* ACHIEVEMENTS */

.achievements-intro{
    display:flex;
    justify-content:space-between;
    gap:40px;
    align-items:end;
}

.geneva{
    margin-top:55px;
    display:grid;
    grid-template-columns:1.1fr .9fr;
    border:1px solid var(--border);
    border-radius:var(--radius);
    overflow:hidden;
    background:#0d0d0d;
}

.geneva-image img{
    width:100%;
    height:500px;
    object-fit:cover;
}

.geneva-content{
    padding:50px;
    display:flex;
    flex-direction:column;
    justify-content:center;
}

.medal{
    font-size:50px;
    margin-bottom:10px;
}

.geneva-content small{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-weight:800;
    letter-spacing:1px;
}

.geneva-content h3{
    font-size:40px;
    line-height:1.2;
    margin:12px 0;
}

.geneva-content p{
    color:var(--gray);
}

.awards{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:12px;
    margin-top:15px;
}

.award{
    border:1px solid var(--border);
    background:#0d0d0d;
    padding:25px;
    border-radius:18px;
    min-height:180px;
}

.award-number{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-size:12px;
    font-weight:900;
}

.award h4{
    margin-top:20px;
    font-size:16px;
}

.award p{
    color:var(--gray);
    font-size:13px;
    margin-top:8px;
}

.timeline{
    margin-top:35px;
    display:grid;
    gap:12px;
}

.timeline-item{
    display:grid;
    grid-template-columns:100px 1fr;
    gap:20px;
    padding:22px;
    border:1px solid var(--border);
    border-radius:16px;
    background:#0b0b0b;
}

.timeline-year{
    color:var(--red);
    font-family:Montserrat,sans-serif;
    font-weight:900;
}

.timeline-item h4{
    font-size:17px;
}

.timeline-item p{
    color:var(--gray);
    font-size:14px;
}

/* PRESENCE */

.presence{
    margin-top:45px;
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
}

.presence-image{
    border-radius:var(--radius);
    overflow:hidden;
    border:1px solid var(--border);
}

.presence-image img{
    width:100%;
    height:450px;
    object-fit:cover;
}

.presence-content p{
    color:var(--gray);
    font-size:16px;
    line-height:2;
}

/* CONTACT */

.contact{
    background:
        radial-gradient(circle at 80% 30%,rgba(227,38,46,.12),transparent 30%),
        #080808;
}

.contact-grid{
    display:grid;
    grid-template-columns:.8fr 1.2fr;
    gap:70px;
    align-items:start;
}

.contact-copy p{
    color:var(--gray);
    line-height:2;
    font-size:17px;
}

.email{
    margin-top:25px;
    color:#fff;
    font-family:Montserrat,sans-serif;
    font-weight:700;
    direction:ltr;
    text-align:right;
}

.socials{
    display:flex;
    gap:10px;
    flex-wrap:wrap;
    margin-top:30px;
}

.social{
    border:1px solid var(--border);
    border-radius:999px;
    padding:9px 17px;
    color:#ddd;
    transition:var(--transition);
    font-size:13px;
}

.social:hover{
    background:#fff;
    color:#000;
}

.contact-form{
    background:#0d0d0d;
    border:1px solid var(--border);
    border-radius:var(--radius);
    padding:35px;
}

.form-grid{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:15px;
}

.field{
    display:flex;
    flex-direction:column;
    gap:7px;
}

.field.full{
    grid-column:1/-1;
}

.field label{
    color:#ddd;
    font-size:13px;
    font-weight:700;
}

.field input,
.field textarea,
.field select{
    width:100%;
    border:1px solid var(--border);
    background:#080808;
    color:#fff;
    border-radius:12px;
    padding:14px 15px;
    outline:none;
    transition:var(--transition);
}

.field input:focus,
.field textarea:focus,
.field select:focus{
    border-color:var(--red);
    box-shadow:0 0 0 3px rgba(227,38,46,.08);
}

.field textarea{
    min-height:150px;
    resize:vertical;
}

.submit{
    margin-top:18px;
    width:100%;
    border:0;
    background:var(--red);
    color:#fff;
    padding:15px;
    border-radius:12px;
    font-weight:900;
    transition:var(--transition);
}

.submit:hover{
    background:#ff3038;
}

.form-note{
    margin-top:12px;
    text-align:center;
    color:#777;
    font-size:12px;
}

/* FOOTER */

footer{
    border-top:1px solid var(--border);
    padding:35px 0;
    background:#050505;
}

.footer{
    display:flex;
    align-items:center;
    justify-content:space-between;
    gap:20px;
}

.footer-brand{
    font-weight:900;
}

.footer-brand span{
    color:var(--red);
}

.footer-copy{
    color:#666;
    font-size:12px;
}

.footer-social{
    display:flex;
    gap:12px;
}

.footer-social a{
    color:#888;
    font-family:Montserrat,sans-serif;
    font-size:12px;
    transition:var(--transition);
}

.footer-social a:hover{
    color:#fff;
}

/* TOP BUTTON */

.top{
    position:fixed;
    bottom:25px;
    left:25px;
    width:45px;
    height:45px;
    border-radius:50%;
    border:1px solid var(--border);
    background:#111;
    color:#fff;
    z-index:500;
    opacity:0;
    visibility:hidden;
    transition:var(--transition);
}

.top.show{
    opacity:1;
    visibility:visible;
}

.top:hover{
    background:var(--red);
}

/* ANIMATION */

.reveal{
    opacity:0;
    transform:translateY(25px);
    transition:opacity .8s ease,transform .8s ease;
}

.reveal.visible{
    opacity:1;
    transform:none;
}

/* MOBILE */

@media(max-width:1000px){

    .nav-links{
        position:absolute;
        top:82px;
        left:20px;
        right:20px;
        background:#0b0b0b;
        border:1px solid var(--border);
        border-radius:18px;
        padding:20px;
        display:none;
        flex-direction:column;
        align-items:stretch;
        gap:0;
    }

    .nav-links.open{
        display:flex;
    }

    .nav-links a{
        display:block;
        padding:13px 5px;
    }

    .menu-btn{
        display:block;
    }

    .about-grid,
    .tech-grid,
    .contact-grid,
    .presence{
        grid-template-columns:1fr;
    }

    .process-grid{
        grid-template-columns:repeat(2,1fr);
    }

    .awards{
        grid-template-columns:repeat(2,1fr);
    }

    .geneva{
        grid-template-columns:1fr;
    }

    .sectors-grid{
        grid-template-columns:repeat(2,1fr);
    }

}

@media(max-width:650px){

    .container{
        width:min(calc(100% - 28px),var(--max));
    }

    .section{
        padding:85px 0;
    }

    .nav{
        height:72px;
    }

    .nav-links{
        top:72px;
    }

    .hero{
        min-height:850px;
    }

    .hero h1{
        font-size:52px;
        letter-spacing:-3px;
    }

    .hero-text{
        font-size:15px;
    }

    .buttons{
        flex-direction:column;
        align-items:stretch;
    }

    .btn{
        width:100%;
    }

    .about-image img,
    .tech-image img{
        height:350px;
    }

    .values{
        grid-template-columns:1fr;
    }

    .solutions-grid{
        grid-template-columns:1fr;
    }

    .process-grid{
        grid-template-columns:1fr;
    }

    .sectors-grid{
        grid-template-columns:1fr;
    }

    .awards{
        grid-template-columns:1fr;
    }

    .geneva-content{
        padding:30px;
    }

    .geneva-content h3{
        font-size:30px;
    }

    .timeline-item{
        grid-template-columns:1fr;
        gap:5px;
    }

    .form-grid{
        grid-template-columns:1fr;
    }

    .field.full{
        grid-column:auto;
    }

    .contact-form{
        padding:22px;
    }

    .footer{
        flex-direction:column;
        align-items:flex-start;
    }

    .top{
        left:auto;
        right:18px;
        bottom:18px;
    }

}

</style>
</head>

<body>

<!-- HEADER -->

<header id="header">

<div class="container nav">

<a href="#home" class="logo">

<img src="assets/mukafih-logo.png" alt="شعار مكافح MUKAFIH">

<div class="logo-text">
<span class="logo-ar ar">مكافح</span>
<span class="logo-ar en-text">MUKAFIH</span>

<span class="logo-en">FIRE PROTECTION</span>
</div>

</a>

<nav>

<ul class="nav-links" id="navLinks">

<li>
<a href="#home">
<span class="ar">الرئيسية</span>
<span class="en-text">Home</span>
</a>
</li>

<li>
<a href="#about">
<span class="ar">من نحن</span>
<span class="en-text">About</span>
</a>
</li>

<li>
<a href="#solutions">
<span class="ar">الحلول</span>
<span class="en-text">Solutions</span>
</a>
</li>

<li>
<a href="#technology">
<span class="ar">التقنية</span>
<span class="en-text">Technology</span>
</a>
</li>

<li>
<a href="#sectors">
<span class="ar">القطاعات</span>
<span class="en-text">Sectors</span>
</a>
</li>

<li>
<a href="#achievements">
<span class="ar">الإنجازات</span>
<span class="en-text">Achievements</span>
</a>
</li>

<li>
<a href="#contact">
<span class="ar">تواصل معنا</span>
<span class="en-text">Contact</span>
</a>
</li>

</ul>

</nav>

<div class="nav-actions">

<button class="lang-btn" id="langBtn" type="button">
EN
</button>

<button class="menu-btn" id="menuBtn" type="button" aria-label="القائمة">
☰
</button>

</div>

</div>

</header>


<!-- HERO -->

<main>

<section class="hero" id="home">

<img
src="assets/hero-drone.jpg"
alt="MUKAFIH Smart Firefighting Drone"
class="hero-image"
>

<div class="hero-overlay"></div>

<div class="container">

<div class="hero-content reveal">

<div class="hero-kicker">
<span class="ar">تقنية سعودية للحماية الذكية</span>
<span class="en-text">SAUDI SMART FIRE PROTECTION TECHNOLOGY</span>
</div>

<h1>

<span class="ar">
نبتكر اليوم<br>
<span>لنحمي الغد.</span>
</span>

<span class="en-text">
INNOVATE TODAY.<br>
<span>PROTECT TOMORROW.</span>
</span>

</h1>

<p class="hero-text">

<span class="ar">
حلول متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والأتمتة لحماية المنشآت ورفع مستوى السلامة.
</span>

<span class="en-text">
Advanced fire protection solutions combining engineering, artificial intelligence and automation to protect facilities and enhance safety.
</span>

</p>

<div class="buttons">

<a href="#solutions" class="btn btn-primary">

<span class="ar">اكتشف حلولنا</span>
<span class="en-text">Explore Our Solutions</span>

</a>

<a href="#contact" class="btn btn-outline">

<span class="ar">تواصل مع مكافح</span>
<span class="en-text">Contact MUKAFIH</span>

</a>

</div>

</div>

</div>

</section>


<!-- ABOUT -->

<section class="section" id="about">

<div class="container">

<div class="about-grid">

<div class="about-image reveal">

<img
src="assets/about-mukafih.jpg"
alt="عن شركة مكافح"
loading="lazy"
>

</div>

<div class="about-content reveal">

<div class="eyebrow">
<span class="ar">من نحن</span>
<span class="en-text">ABOUT US</span>
</div>

<h2>

<span class="ar">
الحماية لم تعد<br>
تنتظر وقوع الحريق.
</span>

<span class="en-text">
Protection should never<br>
wait for a fire.
</span>

</h2>

<p>

<span class="ar">
نحن في مكافح نؤمن بقوة الابتكار والتقنية في تطوير مستقبل أكثر أمانًا. نعمل على تقديم حلول متقدمة للحماية من الحرائق مصممة للبيئات التي تتطلب سرعة الاستجابة وذكاء القرار.
</span>

<span class="en-text">
At MUKAFIH, we believe in the power of innovation and technology to build a safer future. We develop advanced fire protection solutions for environments where rapid response and intelligent decision-making are essential.
</span>

</p>

<p>

<span class="ar">
نمـزج بين الأنظمة الهندسية والتقنيات الذكية لنمنح المنشآت مستوى أعلى من الرصد والتحليل والاستجابة.
</span>

<span class="en-text">
We combine engineering systems with intelligent technologies to provide facilities with enhanced monitoring, analysis and response capabilities.
</span>

</p>

<div class="values">

<div class="value">
<strong>01</strong>
<span class="ar">الابتكار</span>
<span class="en-text">Innovation</span>
</div>

<div class="value">
<strong>02</strong>
<span class="ar">السلامة</span>
<span class="en-text">Safety</span>
</div>

<div class="value">
<strong>03</strong>
<span class="ar">الاستجابة الذكية</span>
<span class="en-text">Smart Response</span>
</div>

</div>

</div>

</div>

</div>

</section>


<!-- SOLUTIONS -->

<section class="section" id="solutions">

<div class="container">

<div class="eyebrow">
<span class="ar">حلول مكافح</span>
<span class="en-text">MUKAFIH SOLUTIONS</span>
</div>

<h2>

<span class="ar">
حلول مصممة<br>
للخطر الحقيقي.
</span>

<span class="en-text">
Solutions designed<br>
for real-world risk.
</span>

</h2>

<p class="section-desc">

<span class="ar">
من الكشف المبكر إلى الاستجابة، نطور منظومة حماية تتناسب مع طبيعة المنشأة ودرجة المخاطر فيها.
</span>

<span class="en-text">
From early detection to response, we develop protection systems tailored to each facility and its specific risk profile.
</span>

</p>

<div class="solutions-grid">

<div class="card reveal">

<div class="card-number">01</div>

<h3>
<span class="ar">الحماية الذكية بالطائرات المسيّرة</span>
<span class="en-text">Smart Drone Fire Protection</span>
</h3>

<p>
<span class="ar">
حلول جوية ذكية للعمل داخل البيئات الصناعية والمنشآت المغلقة، للمساعدة في اكتشاف الحريق والتحقق منه والاستجابة المبكرة.
</span>

<span class="en-text">
Intelligent aerial solutions designed for industrial and enclosed environments to support fire detection, verification and early response.
</span>
</p>

</div>


<div class="card reveal">

<div class="card-number">02</div>

<h3>
<span class="ar">أنظمة مكافحة الحرائق</span>
<span class="en-text">Firefighting Systems</span>
</h3>

<p>
<span class="ar">
حلول حماية متقدمة مصممة وفق طبيعة كل منشأة واحتياجاتها التشغيلية.
</span>

<span class="en-text">
Advanced protection solutions designed according to each facility's environment and operational requirements.
</span>
</p>

</div>


<div class="card reveal">

<div class="card-number">03</div>

<h3>
<span class="ar">الذكاء الاصطناعي والكشف المبكر</span>
<span class="en-text">AI & Early Detection</span>
</h3>

<p>
<span class="ar">
توظيف الرؤية الحاسوبية والذكاء الاصطناعي لتحليل البيئة واكتشاف مؤشرات الخطر.
</span>

<span class="en-text">
Using computer vision and artificial intelligence to analyze environments and identify signs of potential hazards.
</span>
</p>

</div>


<div class="card reveal">

<div class="card-number">04</div>

<h3>
<span class="ar">حلول المنشآت الصناعية</span>
<span class="en-text">Industrial Facility Solutions</span>
</h3>

<p>
<span class="ar">
منظومات حماية للبيئات التي تتطلب مستويات عالية من المراقبة والاستجابة والسلامة.
</span>

<span class="en-text">
Protection systems for environments requiring advanced monitoring, response and safety capabilities.
</span>
</p>

</div>

</div>

</div>

</section>


<!-- TECHNOLOGY -->

<section class="section tech" id="technology">

<div class="container">

<div class="tech-grid">

<div class="tech-image reveal">

<img
src="assets/mukafih-technology.jpg"
alt="تقنية مكافح"
loading="lazy"
>

</div>

<div class="reveal">

<div class="eyebrow">
<span class="ar">التقنية</span>
<span class="en-text">TECHNOLOGY</span>
</div>

<h2>

<span class="ar">
عندما تصبح<br>
كل ثانية مهمة.
</span>

<span class="en-text">
When every<br>
second matters.
</span>

</h2>

<p class="section-desc">

<span class="ar">
صممت منظومة مكافح لتعمل في البيئات التي قد تكون فيها الاستجابة البشرية صعبة أو محفوفة بالمخاطر.
</span>

<span class="en-text">
MUKAFIH is designed for environments where human response can be difficult, delayed or exposed to significant risk.
</span>

</p>

<div class="tech-list">

<div class="tech-item">

<div class="tech-number">01</div>

<div>
<h3>
<span class="ar">رصد وتحليل ذكي</span>
<span class="en-text">Smart Monitoring & Analysis</span>
</h3>

<p>
<span class="ar">مراقبة البيئة وتحليل مؤشرات الخطر.</span>
<span class="en-text">Monitoring environments and analyzing risk indicators.</span>
</p>
</div>

</div>


<div class="tech-item">

<div class="tech-number">02</div>

<div>
<h3>
<span class="ar">خرائط ثلاثية الأبعاد</span>
<span class="en-text">3D Mapping</span>
</h3>

<p>
<span class="ar">بناء خرائط ثلاثية الأبعاد للبيئات الداخلية.</span>
<span class="en-text">Building three-dimensional maps of indoor environments.</span>
</p>
</div>

</div>


<div class="tech-item">

<div class="tech-number">03</div>

<div>
<h3>
<span class="ar">استجابة سريعة</span>
<span class="en-text">Rapid Response</span>
</h3>

<p>
<span class="ar">تحديد الخطر والمساعدة في تفعيل الاستجابة المناسبة.</span>
<span class="en-text">Identifying hazards and supporting the appropriate response.</span>
</p>
</div>

</div>


<div class="tech-item">

<div class="tech-number">04</div>

<div>
<h3>
<span class="ar">ملاحة للبيئات الداخلية</span>
<span class="en-text">Indoor Navigation</span>
</h3>

<p>
<span class="ar">الملاحة في البيئات التي لا يتوفر فيها GPS.</span>
<span class="en-text">Navigation in environments where GPS may not be available.</span>
</p>
</div>

</div>

</div>

</div>

</div>

</div>

</section>


<!-- PROCESS -->

<section class="section">

<div class="container">

<div class="eyebrow">
<span class="ar">كيف تعمل مكافح؟</span>
<span class="en-text">HOW IT WORKS</span>
</div>

<h2>

<span class="ar">
من الرصد<br>
إلى الاستجابة.
</span>

<span class="en-text">
From detection<br>
to response.
</span>

</h2>

<div class="process-grid">

<div class="process reveal">
<div class="process-number">01</div>
<h3>
<span class="ar">الرصد</span>
<span class="en-text">Detection</span>
</h3>
<p>
<span class="ar">مراقبة البيئة واكتشاف مؤشرات الخطر.</span>
<span class="en-text">Monitoring the environment and detecting risk indicators.</span>
</p>
</div>


<div class="process reveal">
<div class="process-number">02</div>
<h3>
<span class="ar">التحليل</span>
<span class="en-text">Analysis</span>
</h3>
<p>
<span class="ar">تحليل البيانات وتحديد طبيعة الحدث.</span>
<span class="en-text">Analyzing data and identifying the nature of the event.</span>
</p>
</div>


<div class="process reveal">
<div class="process-number">03</div>
<h3>
<span class="ar">تحديد الموقع</span>
<span class="en-text">Localization</span>
</h3>
<p>
<span class="ar">تحديد موقع الخطر داخل المنشأة.</span>
<span class="en-text">Locating the hazard inside the facility.</span>
</p>
</div>


<div class="process reveal">
<div class="process-number">04</div>
<h3>
<span class="ar">الاستجابة</span>
<span class="en-text">Response</span>
</h3>
<p>
<span class="ar">تفعيل منظومة الاستجابة المناسبة.</span>
<span class="en-text">Activating the appropriate response system.</span>
</p>
</div>


<div class="process reveal">
<div class="process-number">05</div>
<h3>
<span class="ar">الحماية</span>
<span class="en-text">Protection</span>
</h3>
<p>
<span class="ar">المساعدة في الحد من انتشار الخطر وتقليل المخاطر.</span>
<span class="en-text">Helping limit hazard spread and reduce risks.</span>
</p>
</div>

</div>

</div>

</section>


<!-- SECTORS -->

<section class="section sectors" id="sectors">

<div class="container">

<div class="eyebrow">
<span class="ar">القطاعات</span>
<span class="en-text">SECTORS</span>
</div>

<h2>

<span class="ar">
حماية تتكيف<br>
مع بيئتك.
</span>

<span class="en-text">
Protection adapted<br>
to your environment.
</span>

</h2>

<p class="section-desc">

<span class="ar">
حلول موجهة للبيئات التي تتطلب مستويات متقدمة من المراقبة والاستجابة.
</span>

<span class="en-text">
Solutions designed for environments requiring advanced monitoring and response capabilities.
</span>

</p>

<div class="sectors-grid">

<div class="sector reveal">
<img src="assets/sector-factory.jpg" alt="المصانع" loading="lazy">
<div class="sector-content">
<div class="sector-number">01</div>
<h3>
<span class="ar">المصانع</span>
<span class="en-text">Factories</span>
</h3>
</div>
</div>


<div class="sector reveal">
<img src="assets/sector-warehouse.jpg" alt="المستودعات" loading="lazy">
<div class="sector-content">
<div class="sector-number">02</div>
<h3>
<span class="ar">المستودعات</span>
<span class="en-text">Warehouses</span>
</h3>
</div>
</div>


<div class="sector reveal">
<img src="assets/sector-power.jpg" alt="غرف الكهرباء والمحطات" loading="lazy">
<div class="sector-content">
<div class="sector-number">03</div>
<h3>
<span class="ar">غرف الكهرباء والمحطات</span>
<span class="en-text">Power Facilities</span>
</h3>
</div>
</div>


<div class="sector reveal">
<img src="assets/sector-datacenter.jpg" alt="مراكز البيانات" loading="lazy">
<div class="sector-content">
<div class="sector-number">04</div>
<h3>
<span class="ar">مراكز البيانات</span>
<span class="en-text">Data Centers</span>
</h3>
</div>
</div>


<div class="sector reveal">
<img src="assets/sector-tunnel.jpg" alt="الأنفاق والمرافق المغلقة" loading="lazy">
<div class="sector-content">
<div class="sector-number">05</div>
<h3>
<span class="ar">الأنفاق والمرافق المغلقة</span>
<span class="en-text">Tunnels & Enclosed Facilities</span>
</h3>
</div>
</div>


<div class="sector reveal">
<img src="assets/sector-industrial.jpg" alt="المنشآت عالية الخطورة" loading="lazy">
<div class="sector-content">
<div class="sector-number">06</div>
<h3>
<span class="ar">المنشآت عالية الخطورة</span>
<span class="en-text">High-Risk Facilities</span>
</h3>
</div>
</div>

</div>

</div>

</section>


<!-- ACHIEVEMENTS -->

<section class="section" id="achievements">

<div class="container">

<div class="achievements-intro">

<div>

<div class="eyebrow">
<span class="ar">الإنجازات والتكريمات</span>
<span class="en-text">ACHIEVEMENTS & RECOGNITION</span>
</div>

<h2>

<span class="ar">
إنجازات<br>
تصنع الثقة.
</span>

<span class="en-text">
Achievements<br>
that build trust.
</span>

</h2>

</div>

<p class="section-desc">

<span class="ar">
من الاحتضان والتأهل إلى التقدير الدولي، نواصل بناء رحلة مكافح بخطوات موثقة.
</span>

<span class="en-text">
From incubation and national competitions to international recognition, MUKAFIH continues to build its journey through documented milestones.
</span>

</p>

</div>


<div class="geneva reveal">

<div class="geneva-image">

<img
src="assets/geneva-gold-medal.jpg"
alt="الميدالية الذهبية مع مرتبة الشرف - معرض جنيف الدولي للاختراعات"
loading="lazy"
>

</div>

<div class="geneva-content">

<div class="medal">🥇</div>

<small>
51ST GENEVA INTERNATIONAL EXHIBITION OF INVENTIONS
</small>

<h3>

<span class="ar">
الميدالية الذهبية<br>
مع مرتبة الشرف
</span>

<span class="en-text">
Gold Medal<br>
with Honors
</span>

</h3>

<p>

<span class="ar">
تكريم دولي يبرز قيمة الابتكار الذي تقدمه مكافح.
</span>

<span class="en-text">
International recognition highlighting the innovation delivered by MUKAFIH.
</span>

</p>

</div>

</div>


<div class="awards">

<div class="award reveal">

<div class="award-number">01</div>

<h4>
<span class="ar">جائزة خاصة</span>
<span class="en-text">Special Award</span>
</h4>

<p>
THE HONG KONG UNIVERSITY OF SCIENCE AND TECHNOLOGY
</p>

</div>


<div class="award reveal">

<div class="award-number">02</div>

<h4>
<span class="ar">شهادة وميدالية</span>
<span class="en-text">Certificate & Medal</span>
</h4>

<p>
Fédération Française des Inventeurs
<br>
French Inventors Federation
</p>

</div>


<div class="award reveal">

<div class="award-number">03</div>

<h4>
<span class="ar">جائزة خاصة</span>
<span class="en-text">Special Award</span>
</h4>

<p>
Malaysia Delegation
</p>

</div>


<div class="award reveal">

<div class="award-number">04</div>

<h4>
<span class="ar">جائزة خاصة</span>
<span class="en-text">Special Award</span>
</h4>

<p>
<span class="ar">جامعة القصيم — المملكة العربية السعودية</span>
<span class="en-text">Qassim University — Saudi Arabia</span>
</p>

</div>

</div>


<div class="timeline">

<div class="timeline-item reveal">

<div class="timeline-year">2025</div>

<div>

<h4>
<span class="ar">برنامج الاحتضان — CEIES · جامعة الملك عبدالعزيز</span>
<span class="en-text">CEIES Incubation Program · King Abdulaziz University</span>
</h4>

<p>
<span class="ar">
برنامج الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز، خلال الفترة من يناير إلى ديسمبر 2025.
</span>

<span class="en-text">
Incubation program at the Center of Excellence in Engineering and Electrical Systems at King Abdulaziz University, from January to December 2025.
</span>
</p>

</div>

</div>


<div class="timeline-item reveal">

<div class="timeline-year">2026</div>

<div>

<h4>
<span class="ar">إنجاز السعودية — التأهل للنهائيات</span>
<span class="en-text">Injaz Saudi Arabia — Finalist</span>
</h4>

<p>
<span class="ar">
التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية 2026.
</span>

<span class="en-text">
Qualified for the finals of the Fikra competition by Injaz Saudi Arabia 2026.
</span>
</p>

</div>

</div>


<div class="timeline-item reveal">

<div class="timeline-year">TOP 20</div>

<div>

<h4>
<span class="ar">المؤتمر الأول للابتكار وريادة الأعمال — جامعة الملك عبدالعزيز</span>
<span class="en-text">First Innovation & Entrepreneurship Conference</span>
</h4>

<p>
<span class="ar">
كنا ضمن أفضل 20 مشروعًا رياديًا مشاركًا في المؤتمر والمعرض.
</span>

<span class="en-text">
Selected among the Top 20 entrepreneurial projects participating in the conference and exhibition.
</span>
</p>

</div>

</div>


<div class="timeline-item reveal">

<div class="timeline-year">+</div>

<div>

<h4>
<span class="ar">حضور ومشاركات ريادية</span>
<span class="en-text">Entrepreneurial Presence</span>
</h4>

<p>
<span class="ar">
المشاركة في غرفة جدة ضمن فعاليات أسبوع ريادة الأعمال، ومعرض رواد الأعمال في كلية العلوم، وHack4Earth، وملتقى تمكين المستقبل.
</span>

<span class="en-text">
Participation in Jeddah Chamber Entrepreneurship Week, the Entrepreneurs Exhibition at the College of Science, Hack4Earth and the Future Empowerment Forum.
</span>
</p>

</div>

</div>

</div>


<!-- OFFICIAL PRESENCE -->

<div class="presence">

<div class="presence-image reveal">

<img
src="assets/mukafih-official-meeting.jpg"
alt="لقاء مكافح الرسمي"
loading="lazy"
>

</div>

<div class="presence-content reveal">

<div class="eyebrow">
<span class="ar">حضور رسمي وإعلامي</span>
<span class="en-text">OFFICIAL & MEDIA PRESENCE</span>
</div>

<h2>

<span class="ar">
من الابتكار<br>
إلى الحضور.
</span>

<span class="en-text">
From innovation<br>
to impact.
</span>

</h2>

<p>

<span class="ar">
حظيت مكافح بحضور وتمثيل في مناسبات وبرامج تعكس رحلتها في الابتكار وريادة الأعمال، من بينها لقاء صاحب السمو الأمير سعود بن جلوي محافظ جدة عقب الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز د. طريف الأعمى.
</span>

<span class="en-text">
MUKAFIH has been represented across events and programs reflecting its innovation and entrepreneurship journey, including a meeting with His Highness Prince Saud bin Jalawi, Governor of Jeddah, following the Geneva International Exhibition of Inventions, in the presence of the President of King Abdulaziz University, Dr. Tareef Al-Ama.
</span>

</p>

<div class="buttons" style="margin-top:25px;">

<a href="#contact" class="btn btn-primary">

<span class="ar">ابدأ محادثة مع مكافح</span>
<span class="en-text">Start a Conversation</span>

</a>

</div>

</div>

</div>

</div>

</section>


<!-- CONTACT -->

<section class="section contact" id="contact">

<div class="container">

<div class="contact-grid">

<div class="contact-copy reveal">

<div class="eyebrow">

<span class="ar">تواصل معنا</span>
<span class="en-text">CONTACT US</span>

</div>

<h2>

<span class="ar">
هل منشأتك مستعدة<br>
للخطر قبل وقوعه؟
</span>

<span class="en-text">
Is your facility ready<br>
before danger strikes?
</span>

</h2>

<p>

<span class="ar">
نحن هنا للإجابة على استفساراتكم ومناقشة فرص التعاون المشترك. يسعدنا اتصالكم بنا في أي وقت.
</span>

<span class="en-text">
We are here to answer your questions and discuss opportunities for collaboration. We would be pleased to hear from you.
</span>

</p>

<div class="email">
mkafh2024@gmail.com
</div>

<div class="socials">

<a class="social"
href="https://x.com/muk_fh?s=21"
target="_blank"
rel="noopener noreferrer">
X
</a>

<a class="social"
href="https://www.instagram.com/muk.fh/"
target="_blank"
rel="noopener noreferrer">
Instagram
</a>

<a class="social"
href="https://www.linkedin.com/company/mokfeh/"
target="_blank"
rel="noopener noreferrer">
LinkedIn
</a>

<a class="social"
href="https://www.tiktok.com/@muk.fh"
target="_blank"
rel="noopener noreferrer">
TikTok
</a>

</div>

</div>


<!-- FORM -->

<div class="contact-form reveal">

<form
action="https://formsubmit.co/mkafh2024@gmail.com"
method="POST"
>

<input type="hidden" name="_subject" value="رسالة جديدة من موقع مكافح | MUKAFIH">

<input type="hidden" name="_template" value="table">

<input type="hidden" name="_captcha" value="false">

<input
type="hidden"
name="_next"
value="https://malakalobidan.github.io/MUKKAFH/?sent=true#contact"
>

<div class="form-grid">

<div class="field">

<label>

<span class="ar">الاسم الكامل</span>
<span class="en-text">Full Name</span>

</label>

<input
type="text"
name="name"
placeholder="الاسم الكامل"
required
>

</div>


<div class="field">

<label>

<span class="ar">البريد الإلكتروني</span>
<span class="en-text">Email Address</span>

</label>

<input
type="email"
name="email"
placeholder="name@example.com"
dir="ltr"
required
>

</div>


<div class="field">

<label>

<span class="ar">الشركة</span>
<span class="en-text">Company</span>

</label>

<input
type="text"
name="company"
placeholder="اسم الشركة"
>

</div>


<div class="field">

<label>

<span class="ar">القطاع</span>
<span class="en-text">Sector</span>

</label>

<select name="sector">

<option value="">
اختر القطاع
</option>

<option value="Factories">
المصانع
</option>

<option value="Warehouses">
المستودعات
</option>

<option value="Power">
غرف الكهرباء والمحطات
</option>

<option value="Data Centers">
مراكز البيانات
</option>

<option value="Tunnels">
الأنفاق والمرافق المغلقة
</option>

<option value="High Risk Facilities">
المنشآت عالية الخطورة
</option>

<option value="Other">
أخرى
</option>

</select>

</div>


<div class="field full">

<label>

<span class="ar">الرسالة</span>
<span class="en-text">Message</span>

</label>

<textarea
name="message"
placeholder="اكتب رسالتك هنا..."
required
></textarea>

</div>

</div>

<button class="submit" type="submit">

<span class="ar">إرسال الرسالة</span>
<span class="en-text">Send Message</span>

</button>

<div class="form-note">

<span class="ar">
سيتم إرسال رسالتك مباشرة إلى فريق مكافح.
</span>

<span class="en-text">
Your message will be sent directly to the MUKAFIH team.
</span>

</div>

</form>

</div>

</div>

</div>

</section>

</main>


<!-- FOOTER -->

<footer>

<div class="container footer">

<div class="footer-brand">

<span>مكافح</span>
&nbsp; MUKAFIH

</div>

<div class="footer-copy">
© 2026 MUKAFIH. All Rights Reserved.
</div>

<div class="footer-social">

<a href="https://x.com/muk_fh?s=21" target="_blank" rel="noopener">X</a>

<a href="https://www.instagram.com/muk.fh/" target="_blank" rel="noopener">IG</a>

<a href="https://www.linkedin.com/company/mokfeh/" target="_blank" rel="noopener">IN</a>

<a href="https://www.tiktok.com/@muk.fh" target="_blank" rel="noopener">TT</a>

</div>

</div>

</footer>


<button
class="top"
id="topBtn"
aria-label="العودة إلى الأعلى"
>
↑
</button>


<script>

/* ===============================
   LANGUAGE
================================ */

const langBtn = document.getElementById("langBtn");

function setLanguage(lang){

    if(lang === "en"){

        document.body.classList.add("en");
        document.documentElement.lang = "en";
        document.documentElement.dir = "ltr";
        langBtn.textContent = "AR";

        localStorage.setItem("mukafih-language","en");

    }else{

        document.body.classList.remove("en");
        document.documentElement.lang = "ar";
        document.documentElement.dir = "rtl";
        langBtn.textContent = "EN";

        localStorage.setItem("mukafih-language","ar");
    }
}

langBtn.addEventListener("click",()=>{

    const current =
        document.body.classList.contains("en")
        ? "ar"
        : "en";

    setLanguage(current);

});


const savedLanguage =
    localStorage.getItem("mukafih-language");

if(savedLanguage === "en"){
    setLanguage("en");
}else{
    setLanguage("ar");
}


/* ===============================
   HEADER
================================ */

const header =
    document.getElementById("header");

window.addEventListener("scroll",()=>{

    if(window.scrollY > 40){
        header.classList.add("scrolled");
    }else{
        header.classList.remove("scrolled");
    }

});


/* ===============================
   MOBILE MENU
================================ */

const menuBtn =
    document.getElementById("menuBtn");

const navLinks =
    document.getElementById("navLinks");

menuBtn.addEventListener("click",()=>{

    navLinks.classList.toggle("open");

});

document.querySelectorAll(".nav-links a")
.forEach(link=>{

    link.addEventListener("click",()=>{

        navLinks.classList.remove("open");

    });

});


/* ===============================
   REVEAL ANIMATION
================================ */

const observer =
    new IntersectionObserver(
        entries=>{

            entries.forEach(entry=>{

                if(entry.isIntersecting){

                    entry.target.classList.add("visible");

                }

            });

        },
        {
            threshold:.12
        }
    );


document.querySelectorAll(".reveal")
.forEach(element=>{

    observer.observe(element);

});


/* ===============================
   TOP BUTTON
================================ */

const topBtn =
    document.getElementById("topBtn");

window.addEventListener("scroll",()=>{

    if(window.scrollY > 600){

        topBtn.classList.add("show");

    }else{

        topBtn.classList.remove("show");

    }

});


topBtn.addEventListener("click",()=>{

    window.scrollTo({
        top:0,
        behavior:"smooth"
    });

});


/* ===============================
   SUCCESS MESSAGE
================================ */

const params =
    new URLSearchParams(window.location.search);

if(params.get("sent") === "true"){

    setTimeout(()=>{

        alert(
            document.body.classList.contains("en")
            ? "Thank you. Your message has been sent successfully."
            : "شكرًا لك، تم إرسال رسالتك بنجاح إلى فريق مكافح."
        );

        window.history.replaceState(
            {},
            document.title,
            window.location.pathname + "#contact"
        );

    },500);

}

</script>

</body>
</html>
