# MUKKAFH
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>مكافح | MUKAFIH — Fire Protection Company</title>

<meta name="description"
content="مكافح — حلول ذكية ومتقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والأتمتة.">

<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;500;600;700;800&display=swap" rel="stylesheet">

<style>

:root{
    --red:#e21d35;
    --red2:#ff3048;
    --black:#070809;
    --dark:#0d0f11;
    --dark2:#131518;
    --white:#ffffff;
    --off:#f4f4f1;
    --gray:#777;
    --line:#27292c;
    --shadow:0 20px 60px rgba(0,0,0,.25);
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
    font-family:"Cairo",sans-serif;
    background:var(--off);
    color:#111;
    overflow-x:hidden;
}

body.en{
    direction:ltr;
}

img{
    width:100%;
    display:block;
}

a{
    text-decoration:none;
    color:inherit;
}

button,
input,
textarea{
    font-family:inherit;
}

button{
    cursor:pointer;
}


/* =========================
   LOADER
========================= */

#loader{
    position:fixed;
    inset:0;
    z-index:99999;
    background:#070809;
    color:white;
    display:flex;
    flex-direction:column;
    align-items:center;
    justify-content:center;
    transition:.7s ease;
}

#loader.hide{
    opacity:0;
    visibility:hidden;
}

.loader-logo{
    width:65px;
    height:65px;
    border:1px solid var(--red);
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
    font-size:30px;
    font-weight:800;
    margin-bottom:15px;
}

.loader-name{
    font-size:10px;
    letter-spacing:4px;
    color:#aaa;
}


/* =========================
   HEADER
========================= */

header{
    position:fixed;
    top:0;
    left:0;
    right:0;
    height:82px;
    padding:0 6vw;
    display:flex;
    align-items:center;
    justify-content:space-between;
    z-index:5000;
    color:white;
    transition:.35s;
}

header.scrolled{
    height:70px;
    background:rgba(7,8,9,.93);
    backdrop-filter:blur(18px);
    border-bottom:1px solid rgba(255,255,255,.08);
}

.logo{
    display:flex;
    align-items:center;
    gap:12px;
}

.logo-box{
    width:40px;
    height:40px;
    border:1px solid var(--red);
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:800;
    font-size:19px;
}

.logo-text strong{
    display:block;
    font-size:17px;
    line-height:1;
}

.logo-text small{
    display:block;
    font-size:7px;
    letter-spacing:1.5px;
    color:#aaa;
    margin-top:5px;
    direction:ltr;
}

nav{
    display:flex;
    align-items:center;
    gap:27px;
}

nav a{
    font-size:11px;
    color:#ccc;
    transition:.25s;
}

nav a:hover{
    color:white;
}

nav a.active{
    color:var(--red);
}

.header-actions{
    display:flex;
    align-items:center;
    gap:10px;
}

.language-btn{
    color:white;
    background:transparent;
    border:1px solid rgba(255,255,255,.3);
    border-radius:30px;
    padding:7px 15px;
    font-size:10px;
}

.menu{
    display:none;
    border:0;
    background:none;
    width:30px;
}

.menu span{
    height:1px;
    background:white;
    display:block;
    margin:6px 0;
}


/* =========================
   HERO
========================= */

.hero{
    min-height:100vh;
    position:relative;
    display:flex;
    align-items:center;
    overflow:hidden;
    background:#050607;
    color:white;
}

.hero-image{
    position:absolute;
    inset:0;
    z-index:0;
}

.hero-image img{
    width:100%;
    height:100%;
    object-fit:cover;
    opacity:.58;
}

.hero-bg{
    position:absolute;
    inset:0;
    background:
        radial-gradient(circle at 75% 45%,rgba(226,29,53,.25),transparent 25%),
        linear-gradient(90deg,#050607 5%,rgba(5,6,7,.82) 48%,rgba(5,6,7,.2));
    z-index:1;
}

.hero-grid{
    position:absolute;
    inset:0;
    z-index:2;
    background-image:
        linear-gradient(rgba(255,255,255,.035) 1px,transparent 1px),
        linear-gradient(90deg,rgba(255,255,255,.035) 1px,transparent 1px);
    background-size:70px 70px;
    mask-image:linear-gradient(to right,black,transparent);
}

.hero-content{
    position:relative;
    z-index:4;
    width:min(800px,88vw);
    margin-right:8vw;
}

body.en .hero-content{
    margin-right:0;
    margin-left:8vw;
}

.eyebrow{
    display:flex;
    align-items:center;
    gap:10px;
    color:#aaa;
    font-size:10px;
    letter-spacing:1.5px;
    margin-bottom:25px;
}

.eyebrow span:first-child{
    width:28px;
    height:1px;
    background:var(--red);
}

.hero h1{
    font-size:clamp(48px,7vw,100px);
    line-height:1.05;
    letter-spacing:-4px;
    font-weight:500;
}

.hero h1 strong{
    color:var(--red);
    font-weight:800;
}

.hero-description{
    max-width:600px;
    color:#c4c4c4;
    font-size:14px;
    line-height:2;
    margin:28px 0 35px;
}

.buttons{
    display:flex;
    gap:12px;
    flex-wrap:wrap;
}

.btn{
    display:inline-flex;
    align-items:center;
    justify-content:center;
    padding:13px 25px;
    font-size:11px;
    font-weight:700;
    border:1px solid transparent;
    transition:.3s;
}

.btn-red{
    background:var(--red);
    color:white;
}

.btn-red:hover{
    background:var(--red2);
    transform:translateY(-3px);
}

.btn-outline{
    border-color:rgba(255,255,255,.3);
    color:white;
}

.btn-outline:hover{
    border-color:white;
}

.hero-bottom{
    position:absolute;
    bottom:35px;
    left:8vw;
    right:8vw;
    z-index:5;
    display:flex;
    justify-content:space-between;
    align-items:center;
    color:#777;
    font-size:9px;
}

.scroll{
    display:flex;
    align-items:center;
    gap:10px;
}

.scroll i{
    width:1px;
    height:40px;
    background:#777;
}


/* =========================
   GENERAL
========================= */

section{
    position:relative;
    padding:130px 8vw;
}

.section-number{
    color:var(--red);
    font-size:10px;
    letter-spacing:2px;
    margin-bottom:25px;
}

.section-title{
    font-size:clamp(40px,5.5vw,76px);
    line-height:1.18;
    letter-spacing:-2px;
}

.section-title em{
    color:var(--red);
    font-style:normal;
}

.section-description{
    color:#777;
    font-size:13px;
    line-height:2;
    max-width:450px;
}


/* =========================
   ABOUT
========================= */

.about{
    background:var(--off);
    min-height:720px;
}

.about-grid{
    display:grid;
    grid-template-columns:1.2fr .8fr;
    gap:90px;
    align-items:center;
}

.about-copy{
    padding-top:20px;
}

.about-copy p{
    color:#666;
    font-size:14px;
    line-height:2.1;
    margin-bottom:18px;
    max-width:520px;
}

.pillars{
    margin-top:80px;
    border-top:1px solid #ddd;
    display:grid;
    grid-template-columns:repeat(3,1fr);
}

.pillar{
    padding-top:20px;
}

.pillar span{
    color:var(--red);
    font-size:9px;
}

.pillar strong{
    display:block;
    margin-top:10px;
    font-size:14px;
}


/* =========================
   SOLUTIONS
========================= */

.dark{
    background:var(--black);
    color:white;
}

.section-heading{
    display:flex;
    justify-content:space-between;
    gap:50px;
    align-items:flex-end;
    margin-bottom:60px;
}

.section-heading .section-description{
    max-width:370px;
}

.solutions-grid{
    display:grid;
    grid-template-columns:1.5fr 1fr 1fr;
    gap:1px;
    background:#292b2e;
}

.solution{
    min-height:330px;
    background:#0d0f11;
    padding:32px;
    position:relative;
    display:flex;
    flex-direction:column;
    justify-content:flex-end;
    overflow:hidden;
}

.solution.big{
    min-height:660px;
    grid-row:span 2;
}

.solution-image{
    position:absolute;
    inset:0;
}

.solution-image img{
    width:100%;
    height:100%;
    object-fit:cover;
    opacity:.5;
}

.solution-image:after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(0deg,#0b0c0d,transparent 75%);
}

.solution-content{
    position:relative;
    z-index:2;
}

.solution-number{
    position:absolute;
    top:25px;
    right:30px;
    color:var(--red);
    font-size:10px;
}

.solution-icon{
    position:absolute;
    top:28px;
    left:30px;
    color:var(--red);
    font-size:25px;
}

.solution h3{
    font-size:19px;
    margin-bottom:12px;
}

.solution p{
    color:#858585;
    font-size:11px;
    line-height:1.9;
}


/* =========================
   TECHNOLOGY
========================= */

.technology{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:90px;
    align-items:center;
    background:var(--off);
}

.tech-visual{
    height:600px;
    background:#0b0d0f;
    position:relative;
    overflow:hidden;
}

.tech-visual img{
    height:100%;
    object-fit:cover;
    opacity:.55;
}

.radar{
    position:absolute;
    width:300px;
    height:300px;
    border:1px solid rgba(226,29,53,.5);
    border-radius:50%;
    top:50%;
    left:50%;
    transform:translate(-50%,-50%);
    box-shadow:
        0 0 0 50px rgba(226,29,53,.03),
        0 0 0 100px rgba(226,29,53,.02);
}

.radar:after{
    content:"";
    position:absolute;
    left:50%;
    top:50%;
    width:50%;
    height:1px;
    background:var(--red);
    transform-origin:left;
    animation:radar 4s linear infinite;
}

@keyframes radar{
    to{
        transform:rotate(360deg);
    }
}

.tech-tag{
    position:absolute;
    background:#08090a;
    color:white;
    border-right:2px solid var(--red);
    padding:9px 13px;
    font-size:9px;
}

body.en .tech-tag{
    border-right:0;
    border-left:2px solid var(--red);
}

.tech-tag small{
    display:block;
    color:#666;
    font-size:7px;
}

.tag1{
    top:22%;
    right:12%;
}

.tag2{
    bottom:27%;
    left:10%;
}

.tag3{
    bottom:13%;
    right:20%;
}

.tech-copy p{
    margin:25px 0 35px;
    color:#666;
    line-height:2;
    font-size:13px;
    max-width:500px;
}

.tech-list{
    border-top:1px solid #ddd;
}

.tech-list div{
    border-bottom:1px solid #ddd;
    padding:15px 0;
    display:flex;
    gap:18px;
    font-size:11px;
}

.tech-list b{
    color:var(--red);
    font-size:9px;
}


/* =========================
   PROCESS
========================= */

.process{
    overflow:hidden;
}

.process-line{
    height:1px;
    background:#292b2e;
    position:absolute;
    left:8vw;
    right:8vw;
    top:300px;
}

.process-grid{
    display:grid;
    grid-template-columns:repeat(5,1fr);
    gap:25px;
    position:relative;
}

.process-item span{
    color:var(--red);
    font-size:10px;
}

.process-icon{
    width:50px;
    height:50px;
    border:1px solid #34363a;
    border-radius:50%;
    display:flex;
    align-items:center;
    justify-content:center;
    background:var(--black);
    margin:35px 0 20px;
    color:#fff;
}

.process-item h3{
    font-size:16px;
}

.process-item p{
    color:#777;
    font-size:10px;
    line-height:1.9;
    margin-top:10px;
}


/* =========================
   SECTORS
========================= */

.sectors{
    background:var(--off);
}

.sectors-grid{
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:15px;
    margin-top:60px;
}

.sector{
    height:300px;
    position:relative;
    overflow:hidden;
    background:#111;
}

.sector img{
    height:100%;
    object-fit:cover;
    opacity:.7;
    transition:.5s;
}

.sector:hover img{
    transform:scale(1.07);
    opacity:.9;
}

.sector:after{
    content:"";
    position:absolute;
    inset:0;
    background:linear-gradient(0deg,rgba(0,0,0,.9),transparent 65%);
}

.sector-number{
    position:absolute;
    z-index:2;
    top:20px;
    right:20px;
    color:var(--red);
    font-size:9px;
}

.sector h3{
    position:absolute;
    z-index:2;
    bottom:22px;
    right:22px;
    left:22px;
    color:white;
    font-size:18px;
}


/* =========================
   ACHIEVEMENTS
========================= */

.achievements{
    background:#090a0b;
}

.award-main{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:50px;
    align-items:center;
    margin-bottom:55px;
}

.award-image{
    height:400px;
    background:#111;
    position:relative;
    overflow:hidden;
}

.award-image img{
    height:100%;
    object-fit:cover;
}

.award-image .medal{
    position:absolute;
    inset:0;
    display:flex;
    justify-content:center;
    align-items:center;
    font-size:80px;
    background:rgba(0,0,0,.12);
}

.award-label{
    color:var(--red);
    font-size:9px;
    letter-spacing:1.2px;
}

.award-title{
    font-size:clamp(40px,5vw,70px);
    line-height:1.15;
    margin:20px 0;
}

.award-copy{
    color:#777;
    font-size:12px;
    line-height:2;
}

.awards{
    display:grid;
    grid-template-columns:repeat(4,1fr);
    gap:1px;
    background:#292b2e;
}

.award-card{
    background:#0d0f11;
    min-height:200px;
    padding:30px;
}

.award-card span{
    color:var(--red);
    font-size:9px;
}

.award-card h4{
    margin-top:25px;
    font-size:16px;
}

.award-card p{
    color:#777;
    font-size:9px;
    line-height:1.9;
    margin-top:10px;
}

.timeline{
    margin-top:70px;
    display:grid;
    grid-template-columns:repeat(3,1fr);
    gap:45px;
}

.timeline-item{
    border-top:1px solid #333;
    padding-top:18px;
}

.timeline-year{
    color:var(--red);
    font-size:9px;
}

.timeline-item h4{
    margin:12px 0;
}

.timeline-item p{
    color:#777;
    font-size:10px;
    line-height:1.9;
}

.recognition{
    border-top:1px solid #292b2e;
    border-bottom:1px solid #292b2e;
    margin-top:65px;
    padding:23px 0;
    display:flex;
    justify-content:space-between;
    flex-wrap:wrap;
    gap:20px;
    color:#777;
    font-size:10px;
}


/* =========================
   OFFICIAL PRESENCE
========================= */

.presence{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:80px;
    align-items:center;
}

.presence-image{
    height:520px;
    background:#111;
    overflow:hidden;
}

.presence-image img{
    height:100%;
    object-fit:cover;
}

.presence-copy p{
    color:#666;
    font-size:13px;
    line-height:2.1;
    margin:25px 0 30px;
}

.text-link{
    font-size:11px;
    font-weight:700;
    border-bottom:1px solid var(--red);
    padding-bottom:5px;
}


/* =========================
   CONTACT
========================= */

.contact{
    background:#08090a;
    color:white;
    text-align:center;
    overflow:hidden;
}

.contact-bg{
    position:absolute;
    inset:0;
    background-image:
        linear-gradient(rgba(255,255,255,.03) 1px,transparent 1px),
        linear-gradient(90deg,rgba(255,255,255,.03) 1px,transparent 1px);
    background-size:70px 70px;
}

.contact-content{
    position:relative;
    z-index:2;
    max-width:950px;
    margin:auto;
}

.contact .eyebrow{
    justify-content:center;
}

.contact-description{
    color:#777;
    font-size:12px;
    margin:25px auto 40px;
    max-width:500px;
}

form{
    max-width:720px;
    margin:auto;
    text-align:right;
}

body.en form{
    text-align:left;
}

.form-row{
    display:grid;
    grid-template-columns:1fr 1fr;
    gap:10px;
    margin-bottom:10px;
}

input,
textarea{
    width:100%;
    background:#111315;
    border:1px solid #292b2e;
    color:white;
    padding:14px;
    outline:none;
    font-size:10px;
}

input:focus,
textarea:focus{
    border-color:var(--red);
}

textarea{
    min-height:130px;
    resize:vertical;
    margin-bottom:12px;
}

.form-message{
    color:var(--red);
    font-size:10px;
    margin-top:10px;
}


/* =========================
   FOOTER
========================= */

footer{
    background:#050506;
    color:#777;
    padding:35px 8vw;
    display:grid;
    grid-template-columns:1fr 1fr auto auto;
    align-items:center;
    gap:30px;
    border-top:1px solid #17191b;
}

.footer-logo{
    display:flex;
    align-items:center;
    gap:12px;
    color:white;
}

.footer-logo-box{
    width:35px;
    height:35px;
    border:1px solid var(--red);
    display:flex;
    align-items:center;
    justify-content:center;
    font-weight:800;
}

.footer-logo strong{
    display:block;
    font-size:15px;
}

.footer-logo small{
    font-size:7px;
    letter-spacing:1px;
}

.footer-tagline{
    font-size:10px;
}

.socials{
    display:flex;
    gap:8px;
}

.socials a{
    width:32px;
    height:32px;
    border:1px solid #292b2e;
    display:flex;
    align-items:center;
    justify-content:center;
    color:white;
    font-size:9px;
    transition:.25s;
}

.socials a:hover{
    border-color:var(--red);
    color:var(--red);
}

.copyright{
    font-size:8px;
}


/* =========================
   ANIMATIONS
========================= */

.reveal{
    opacity:0;
    transform:translateY(30px);
    transition:1s ease;
}

.reveal.show{
    opacity:1;
    transform:translateY(0);
}


/* =========================
   MOBILE
========================= */

@media(max-width:1000px){

    nav{
        gap:15px;
    }

    .solutions-grid{
        grid-template-columns:1fr 1fr;
    }

    .solution.big{
        grid-row:span 2;
    }

    .technology,
    .presence{
        grid-template-columns:1fr;
    }

    .process-grid{
        grid-template-columns:repeat(5,170px);
        overflow-x:auto;
        padding-bottom:20px;
    }

    .process-line{
        display:none;
    }

    .awards{
        grid-template-columns:1fr 1fr;
    }

    footer{
        grid-template-columns:1fr 1fr;
    }
}

@media(max-width:760px){

    header{
        padding:0 5vw;
    }

    nav{
        display:none;
        position:absolute;
        top:70px;
        left:5vw;
        right:5vw;
        background:rgba(8,9,10,.98);
        padding:20px;
        flex-direction:column;
        align-items:stretch;
        border:1px solid #292b2e;
    }

    nav.open{
        display:flex;
    }

    .menu{
        display:block;
    }

    .hero-content{
        margin-right:6vw;
        margin-left:6vw;
    }

    body.en .hero-content{
        margin-left:6vw;
        margin-right:6vw;
    }

    .hero h1{
        font-size:53px;
    }

    section{
        padding:90px 6vw;
    }

    .about-grid{
        grid-template-columns:1fr;
        gap:40px;
    }

    .pillars{
        margin-top:50px;
    }

    .section-heading{
        display:block;
    }

    .section-heading .section-description{
        margin-top:25px;
    }

    .solutions-grid{
        grid-template-columns:1fr;
    }

    .solution.big{
        grid-row:auto;
        min-height:500px;
    }

    .tech-visual{
        height:380px;
    }

    .sectors-grid{
        grid-template-columns:1fr;
    }

    .sector{
        height:260px;
    }

    .award-main{
        grid-template-columns:1fr;
    }

    .award-image{
        height:300px;
    }

    .awards,
    .timeline{
        grid-template-columns:1fr;
    }

    .presence-image{
        height:340px;
    }

    .form-row{
        grid-template-columns:1fr;
    }

    .section-title{
        font-size:44px;
    }

    footer{
        grid-template-columns:1fr;
        text-align:center;
    }

    .footer-logo,
    .socials{
        justify-content:center;
    }

}

</style>
</head>

<body>

<!-- LOADER -->
<div id="loader">
    <div class="loader-logo">M</div>
    <div class="loader-name">MUKAFIH</div>
</div>


<!-- HEADER -->
<header id="header">

    <a href="#home" class="logo">

        <div class="logo-box">M</div>

        <div class="logo-text">
            <strong>مكافح</strong>
            <small>MUKAFIH · FIRE PROTECTION</small>
        </div>

    </a>


    <nav id="nav">

        <a href="#home">الرئيسية</a>
        <a href="#about">من نحن</a>
        <a href="#solutions">الحلول</a>
        <a href="#technology">التقنية</a>
        <a href="#sectors">القطاعات</a>
        <a href="#achievements">الإنجازات</a>
        <a href="#contact">تواصل معنا</a>

    </nav>


    <div class="header-actions">

        <button id="languageBtn" class="language-btn">
            EN
        </button>

        <button id="menuBtn" class="menu">
            <span></span>
            <span></span>
            <span></span>
        </button>

    </div>

</header>


<main>


<!-- =========================
 HERO
========================= -->

<section class="hero" id="home">

    <div class="hero-image">
        <img src="images/hero-drone.jpg"
             alt="MUKAFIH Smart Firefighting Drone"
             onerror="this.style.display='none'">
    </div>

    <div class="hero-bg"></div>
    <div class="hero-grid"></div>


    <div class="hero-content reveal">

        <div class="eyebrow">
            <span></span>
            <span
                data-ar="تقنية سعودية للحماية الذكية"
                data-en="Saudi technology for intelligent protection">
                تقنية سعودية للحماية الذكية
            </span>
        </div>


        <h1>

            <span
                data-ar="نبتكر اليوم"
                data-en="We innovate today">
                نبتكر اليوم
            </span>

            <br>

            <strong
                data-ar="لنحمي الغد."
                data-en="to protect tomorrow.">
                لنحمي الغد.
            </strong>

        </h1>


        <p class="hero-description"
           data-ar="حلول متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والأتمتة لحماية المنشآت ورفع مستوى السلامة."
           data-en="Advanced fire protection solutions combining engineering, artificial intelligence and automation to protect facilities and elevate safety.">

            حلول متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والأتمتة لحماية المنشآت ورفع مستوى السلامة.

        </p>


        <div class="buttons">

            <a href="#solutions" class="btn btn-red"
               data-ar="اكتشف حلولنا"
               data-en="Explore our solutions">
                اكتشف حلولنا
            </a>

            <a href="#contact" class="btn btn-outline"
               data-ar="تواصل مع مكافح"
               data-en="Talk to MUKAFIH">
                تواصل مع مكافح
            </a>

        </div>

    </div>


    <div class="hero-bottom">

        <span>MUKAFIH · 01</span>

        <div class="scroll">
            <i></i>
            <span
                data-ar="اكتشف المزيد"
                data-en="Scroll to explore">
                اكتشف المزيد
            </span>
        </div>

    </div>

</section>



<!-- =========================
 ABOUT
========================= -->

<section class="about" id="about">

    <div class="section-number">01</div>

    <div class="about-grid">

        <div class="reveal">

            <div class="eyebrow">
                <span></span>

                <span
                    data-ar="من نحن"
                    data-en="About MUKAFIH">
                    من نحن
                </span>

            </div>

            <h2 class="section-title"
                data-ar="الحماية لم تعد<br><em>تنتظر وقوع الحريق.</em>"
                data-en="Protection no longer<br><em>waits for fire to happen.</em>">

                الحماية لم تعد
                <br>
                <em>تنتظر وقوع الحريق.</em>

            </h2>

        </div>


        <div class="about-copy reveal">

            <p
                data-ar="نحن في مكافح نؤمن بقوة الابتكار والتقنية في تطوير مستقبل أكثر أمانًا. نعمل على تقديم حلول متقدمة للحماية من الحرائق مصممة للبيئات التي تتطلب سرعة الاستجابة وذكاء القرار."
                data-en="At MUKAFIH, we believe in the power of innovation and technology to build a safer future. We deliver advanced fire protection solutions designed for environments that demand rapid response and intelligent decision-making.">

                نحن في مكافح نؤمن بقوة الابتكار والتقنية في تطوير مستقبل أكثر أمانًا. نعمل على تقديم حلول متقدمة للحماية من الحرائق مصممة للبيئات التي تتطلب سرعة الاستجابة وذكاء القرار.

            </p>


            <p
                data-ar="نمـزج بين الأنظمة الهندسية والتقنيات الذكية لنمنح المنشآت مستوى أعلى من الرصد والتحليل والاستجابة."
                data-en="We combine engineering systems with intelligent technologies to give facilities a higher level of monitoring, analysis and response.">

                نمـزج بين الأنظمة الهندسية والتقنيات الذكية لنمنح المنشآت مستوى أعلى من الرصد والتحليل والاستجابة.

            </p>

        </div>

    </div>


    <div class="pillars">

        <div class="pillar">
            <span>01</span>
            <strong
                data-ar="الابتكار"
                data-en="Innovation">
                الابتكار
            </strong>
        </div>

        <div class="pillar">
            <span>02</span>
            <strong
                data-ar="السلامة"
                data-en="Safety">
                السلامة
            </strong>
        </div>

        <div class="pillar">
            <span>03</span>
            <strong
                data-ar="الاستجابة الذكية"
                data-en="Smart Response">
                الاستجابة الذكية
            </strong>
        </div>

    </div>

</section>



<!-- =========================
 SOLUTIONS
========================= -->

<section class="dark" id="solutions">

    <div class="section-heading">

        <div>

            <div class="eyebrow">
                <span></span>

                <span
                    data-ar="حلول مكافح"
                    data-en="MUKAFIH Solutions">
                    حلول مكافح
                </span>

            </div>

            <h2 class="section-title"
                data-ar="حلول مصممة<br>للخطر الحقيقي."
                data-en="Solutions designed<br>for real-world risk.">

                حلول مصممة
                <br>
                للخطر الحقيقي.

            </h2>

        </div>


        <p class="section-description"
           data-ar="من الكشف المبكر إلى الاستجابة، نطور منظومة حماية تتناسب مع طبيعة المنشأة ودرجة المخاطر فيها."
           data-en="From early detection to response, we build protection systems tailored to each facility and its risk profile.">

            من الكشف المبكر إلى الاستجابة، نطور منظومة حماية تتناسب مع طبيعة المنشأة ودرجة المخاطر فيها.

        </p>

    </div>


    <div class="solutions-grid">


        <!-- DRONE -->

        <article class="solution big">

            <div class="solution-image">

                <img src="images/drone.jpg"
                     alt="MUKAFIH Drone"
                     onerror="this.style.display='none'">

            </div>

            <span class="solution-number">01</span>

            <div class="solution-content">

                <h3
                    data-ar="الحماية الذكية بالطائرات المسيّرة"
                    data-en="Smart Drone Fire Protection">

                    الحماية الذكية بالطائرات المسيّرة

                </h3>

                <p
                    data-ar="حلول جوية ذكية للعمل داخل البيئات الصناعية والمنشآت المغلقة، للمساعدة في اكتشاف الحريق والتحقق منه والاستجابة المبكرة."
                    data-en="Intelligent aerial solutions for industrial and enclosed environments, supporting fire detection, verification and early response.">

                    حلول جوية ذكية للعمل داخل البيئات الصناعية والمنشآت المغلقة، للمساعدة في اكتشاف الحريق والتحقق منه والاستجابة المبكرة.

                </p>

            </div>

        </article>


        <!-- SYSTEMS -->

        <article class="solution">

            <span class="solution-number">02</span>

            <div class="solution-icon">⌁</div>

            <div class="solution-content">

                <h3
                    data-ar="أنظمة مكافحة الحرائق"
                    data-en="Firefighting Systems">

                    أنظمة مكافحة الحرائق

                </h3>

                <p
                    data-ar="حلول حماية متقدمة مصممة وفق طبيعة كل منشأة واحتياجاتها التشغيلية."
                    data-en="Advanced protection systems tailored to each facility and its operational needs.">

                    حلول حماية متقدمة مصممة وفق طبيعة كل منشأة واحتياجاتها التشغيلية.

                </p>

            </div>

        </article>


        <!-- AI -->

        <article class="solution">

            <span class="solution-number">03</span>

            <div class="solution-icon">AI</div>

            <div class="solution-content">

                <h3
                    data-ar="الذكاء الاصطناعي والكشف المبكر"
                    data-en="AI & Early Detection">

                    الذكاء الاصطناعي والكشف المبكر

                </h3>

                <p
                    data-ar="توظيف الرؤية الحاسوبية والذكاء الاصطناعي لتحليل البيئة واكتشاف مؤشرات الخطر."
                    data-en="Computer vision and AI technologies analyze environments and identify risk indicators.">

                    توظيف الرؤية الحاسوبية والذكاء الاصطناعي لتحليل البيئة واكتشاف مؤشرات الخطر.

                </p>

            </div>

        </article>


        <!-- INDUSTRIAL -->

        <article class="solution">

            <span class="solution-number">04</span>

            <div class="solution-icon">◈</div>

            <div class="solution-content">

                <h3
                    data-ar="حلول المنشآت الصناعية"
                    data-en="Industrial Facility Solutions">

                    حلول المنشآت الصناعية

                </h3>

                <p
                    data-ar="منظومات حماية للبيئات التي تتطلب مستويات عالية من المراقبة والاستجابة والسلامة."
                    data-en="Protection systems for environments requiring high levels of monitoring, response and safety.">

                    منظومات حماية للبيئات التي تتطلب مستويات عالية من المراقبة والاستجابة والسلامة.

                </p>

            </div>

        </article>

    </div>

</section>



<!-- =========================
 TECHNOLOGY
========================= -->

<section class="technology" id="technology">

    <div class="tech-visual reveal">

        <img src="images/technology-drone.jpg"
             alt="MUKAFIH Technology"
             onerror="this.style.display='none'">

        <div class="radar"></div>

        <div class="tech-tag tag1">
            AI
            <small>ANALYSIS</small>
        </div>

        <div class="tech-tag tag2">
            3D
            <small>MAPPING</small>
        </div>

        <div class="tech-tag tag3">
            LIVE
            <small>RESPONSE</small>
        </div>

    </div>


    <div class="tech-copy reveal">

        <div class="section-number">02</div>

        <div class="eyebrow">

            <span></span>

            <span
                data-ar="التقنية"
                data-en="Technology">
                التقنية
            </span>

        </div>


        <h2 class="section-title"
            data-ar="عندما تصبح<br><em>كل ثانية مهمة.</em>"
            data-en="When<br><em>every second matters.</em>">

            عندما تصبح
            <br>
            <em>كل ثانية مهمة.</em>

        </h2>


        <p
            data-ar="صممت منظومة مكافح لتعمل في البيئات التي قد تكون فيها الاستجابة البشرية صعبة أو محفوفة بالمخاطر."
            data-en="MUKAFIH's system is designed for environments where human response may be difficult or hazardous.">

            صممت منظومة مكافح لتعمل في البيئات التي قد تكون فيها الاستجابة البشرية صعبة أو محفوفة بالمخاطر.

        </p>


        <div class="tech-list">

            <div>
                <b>01</b>
                <span
                    data-ar="رصد وتحليل ذكي"
                    data-en="Intelligent monitoring & analysis">
                    رصد وتحليل ذكي
                </span>
            </div>

            <div>
                <b>02</b>
                <span
                    data-ar="خرائط ثلاثية الأبعاد للبيئات الداخلية"
                    data-en="3D mapping for indoor environments">
                    خرائط ثلاثية الأبعاد للبيئات الداخلية
                </span>
            </div>

            <div>
                <b>03</b>
                <span
                    data-ar="استجابة سريعة عند اكتشاف الخطر"
                    data-en="Rapid response upon risk detection">
                    استجابة سريعة عند اكتشاف الخطر
                </span>
            </div>

            <div>
                <b>04</b>
                <span
                    data-ar="ملاحة مناسبة للبيئات التي لا يتوفر فيها GPS"
                    data-en="Navigation for GPS-denied environments">
                    ملاحة مناسبة للبيئات التي لا يتوفر فيها GPS
                </span>
            </div>

        </div>

    </div>

</section>



<!-- =========================
 HOW IT WORKS
========================= -->

<section class="dark process">

    <div class="section-number">03</div>

    <div class="section-heading">

        <div>

            <div class="eyebrow">

                <span></span>

                <span
                    data-ar="كيف تعمل مكافح؟"
                    data-en="How MUKAFIH works">
                    كيف تعمل مكافح؟
                </span>

            </div>

            <h2 class="section-title"
                data-ar="من الرصد<br>إلى الاستجابة."
                data-en="From detection<br>to response.">

                من الرصد
                <br>
                إلى الاستجابة.

            </h2>

        </div>

    </div>


    <div class="process-line"></div>


    <div class="process-grid">

        <div class="process-item">
            <span>01</span>
            <div class="process-icon">◉</div>

            <h3 data-ar="الرصد" data-en="Detect">
                الرصد
            </h3>

            <p
                data-ar="مراقبة البيئة واكتشاف مؤشرات الخطر."
                data-en="Monitor the environment and identify risk indicators.">
                مراقبة البيئة واكتشاف مؤشرات الخطر.
            </p>
        </div>


        <div class="process-item">
            <span>02</span>
            <div class="process-icon">AI</div>

            <h3 data-ar="التحليل" data-en="Analyze">
                التحليل
            </h3>

            <p
                data-ar="تحليل البيانات وتحديد طبيعة الحدث."
                data-en="Analyze data and determine the nature of the event.">
                تحليل البيانات وتحديد طبيعة الحدث.
            </p>
        </div>


        <div class="process-item">
            <span>03</span>
            <div class="process-icon">⌖</div>

            <h3 data-ar="تحديد الموقع" data-en="Locate">
                تحديد الموقع
            </h3>

            <p
                data-ar="تحديد موقع الخطر داخل المنشأة."
                data-en="Locate the risk within the facility.">
                تحديد موقع الخطر داخل المنشأة.
            </p>
        </div>


        <div class="process-item">
            <span>04</span>
            <div class="process-icon">↗</div>

            <h3 data-ar="الاستجابة" data-en="Respond">
                الاستجابة
            </h3>

            <p
                data-ar="تفعيل منظومة الاستجابة المناسبة."
                data-en="Initiate the appropriate response system.">
                تفعيل منظومة الاستجابة المناسبة.
            </p>
        </div>


        <div class="process-item">
            <span>05</span>
            <div class="process-icon">✓</div>

            <h3 data-ar="الحماية" data-en="Protect">
                الحماية
            </h3>

            <p
                data-ar="المساعدة في الحد من انتشار الخطر وتقليل المخاطر."
                data-en="Help limit risk spread and reduce exposure.">
                المساعدة في الحد من انتشار الخطر وتقليل المخاطر.
            </p>
        </div>

    </div>

</section>



<!-- =========================
 SECTORS
========================= -->

<section class="sectors" id="sectors">

    <div class="section-heading">

        <div>

            <div class="eyebrow">

                <span></span>

                <span
                    data-ar="القطاعات"
                    data-en="Sectors">
                    القطاعات
                </span>

            </div>

            <h2 class="section-title"
                data-ar="حماية تتكيف<br>مع بيئتك."
                data-en="Protection that adapts<br>to your environment.">

                حماية تتكيف
                <br>
                مع بيئتك.

            </h2>

        </div>


        <p class="section-description"
           data-ar="حلول موجهة للبيئات التي تتطلب مستويات متقدمة من المراقبة والاستجابة."
           data-en="Solutions for environments that demand advanced monitoring and response.">

            حلول موجهة للبيئات التي تتطلب مستويات متقدمة من المراقبة والاستجابة.

        </p>

    </div>


    <div class="sectors-grid">

        <div class="sector">
            <img src="images/factory.jpg" alt="Factory">
            <span class="sector-number">01</span>
            <h3 data-ar="المصانع" data-en="Factories">المصانع</h3>
        </div>

        <div class="sector">
            <img src="images/warehouse.jpg" alt="Warehouse">
            <span class="sector-number">02</span>
            <h3 data-ar="المستودعات" data-en="Warehouses">المستودعات</h3>
        </div>

        <div class="sector">
            <img src="images/power-room.jpg" alt="Power Facility">
            <span class="sector-number">03</span>
            <h3 data-ar="غرف الكهرباء والمحطات" data-en="Power Rooms & Substations">غرف الكهرباء والمحطات</h3>
        </div>

        <div class="sector">
            <img src="images/data-center.jpg" alt="Data Center">
            <span class="sector-number">04</span>
            <h3 data-ar="مراكز البيانات" data-en="Data Centers">مراكز البيانات</h3>
        </div>

        <div class="sector">
            <img src="images/tunnel.jpg" alt="Tunnel">
            <span class="sector-number">05</span>
            <h3 data-ar="الأنفاق والمرافق المغلقة" data-en="Tunnels & Enclosed Facilities">الأنفاق والمرافق المغلقة</h3>
        </div>

        <div class="sector">
            <img src="images/industrial-site.jpg" alt="Industrial Facility">
            <span class="sector-number">06</span>
            <h3 data-ar="المنشآت عالية الخطورة" data-en="High-Risk Facilities">المنشآت عالية الخطورة</h3>
        </div>

    </div>

</section>



<!-- =========================
 ACHIEVEMENTS
========================= -->

<section class="achievements dark" id="achievements">

    <div class="section-heading">

        <div>

            <div class="eyebrow">

                <span></span>

                <span
                    data-ar="الإنجازات والتكريمات"
                    data-en="Achievements & Recognition">
                    الإنجازات والتكريمات
                </span>

            </div>

            <h2 class="section-title"
                data-ar="إنجازات<br><em>تصنع الثقة.</em>"
                data-en="Achievements<br><em>that build trust.</em>">

                إنجازات
                <br>
                <em>تصنع الثقة.</em>

            </h2>

        </div>


        <p class="section-description"
           data-ar="من الاحتضان والتأهل إلى التقدير الدولي، نواصل بناء رحلة مكافح بخطوات موثقة."
           data-en="From incubation and competition to international recognition, MUKAFIH continues its documented journey forward.">

            من الاحتضان والتأهل إلى التقدير الدولي، نواصل بناء رحلة مكافح بخطوات موثقة.

        </p>

    </div>


    <!-- GENEVA -->

    <div class="award-main">

        <div class="award-image">

            <img src="images/geneva-gold-medal.jpg"
                 alt="Geneva Gold Medal"
                 onerror="this.style.display='none'">

            <div class="medal">🥇</div>

        </div>


        <div class="reveal">

            <div class="award-label">
                51st GENEVA INTERNATIONAL EXHIBITION OF INVENTIONS
            </div>

            <h3 class="award-title"
                data-ar="الميدالية الذهبية<br>مع مرتبة الشرف"
                data-en="Gold Medal<br>with Honors">

                الميدالية الذهبية
                <br>
                مع مرتبة الشرف

            </h3>

            <p class="award-copy"
               data-ar="تكريم دولي يبرز قيمة الابتكار الذي تقدمه مكافح."
               data-en="International recognition highlighting the value of MUKAFIH's innovation.">

                تكريم دولي يبرز قيمة الابتكار الذي تقدمه مكافح.

            </p>

        </div>

    </div>


    <!-- SPECIAL AWARDS -->

    <div class="awards">

        <article class="award-card">

            <span>01</span>

            <h4>Special Award</h4>

            <p>
                THE HONG KONG UNIVERSITY
                OF SCIENCE AND TECHNOLOGY
            </p>

        </article>


        <article class="award-card">

            <span>02</span>

            <h4
                data-ar="شهادة وميدالية"
                data-en="Certificate & Medal">
                شهادة وميدالية
            </h4>

            <p>
                Fédération Française des Inventeurs
                <br><br>
                French Inventors Federation
            </p>

        </article>


        <article class="award-card">

            <span>03</span>

            <h4>Special Award</h4>

            <p>
                Malaysia Delegation
            </p>

        </article>


        <article class="award-card">

            <span>04</span>

            <h4>Special Award</h4>

            <p
                data-ar="جامعة القصيم — المملكة العربية السعودية"
                data-en="Qassim University — Saudi Arabia">
                جامعة القصيم — المملكة العربية السعودية
            </p>

        </article>

    </div>


    <!-- TIMELINE -->

    <div class="timeline">

        <div class="timeline-item">

            <div class="timeline-year">2025</div>

            <h4>
                CEIES · KAU
            </h4>

            <p
                data-ar="برنامج الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز، خلال الفترة من يناير إلى ديسمبر 2025."
                data-en="Incubation at CEIES, King Abdulaziz University, from January to December 2025.">

                برنامج الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز، خلال الفترة من يناير إلى ديسمبر 2025.

            </p>

        </div>


        <div class="timeline-item">

            <div class="timeline-year">2026</div>

            <h4
                data-ar="إنجاز السعودية"
                data-en="Enjaz Saudi Arabia">
                إنجاز السعودية
            </h4>

            <p
                data-ar="التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية 2026."
                data-en="Finalist in the Fikra competition by Enjaz Saudi Arabia 2026.">

                التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية 2026.

            </p>

        </div>


        <div class="timeline-item">

            <div class="timeline-year">2026</div>

            <h4>Top 20</h4>

            <p
                data-ar="كنا ضمن أفضل 20 مشروعًا رياديًا مشاركًا في المؤتمر الأول للابتكار وريادة الأعمال بجامعة الملك عبدالعزيز."
                data-en="Selected among the Top 20 entrepreneurial projects at the 1st Innovation & Entrepreneurship Conference at KAU.">

                كنا ضمن أفضل 20 مشروعًا رياديًا مشاركًا في المؤتمر الأول للابتكار وريادة الأعمال بجامعة الملك عبدالعزيز.

            </p>

        </div>

    </div>


    <div class="recognition">

        <span
            data-ar="غرفة جدة"
            data-en="Jeddah Chamber">
            غرفة جدة
        </span>

        <span
            data-ar="معرض رواد الأعمال"
            data-en="Entrepreneurs Exhibition">
            معرض رواد الأعمال
        </span>

        <span>Hack4Earth</span>

        <span
            data-ar="ملتقى تمكين المستقبل"
            data-en="Future Empowerment Forum">
            ملتقى تمكين المستقبل
        </span>

        <span
            data-ar="إذاعة الرياض"
            data-en="Riyadh Radio">
            إذاعة الرياض
        </span>

    </div>

</section>



<!-- =========================
 OFFICIAL PRESENCE
========================= -->

<section class="presence">

    <div class="presence-image reveal">

        <img src="images/official-meeting.jpg"
             alt="MUKAFIH Official Meeting"
             onerror="this.style.display='none'">

    </div>


    <div class="reveal">

        <div class="eyebrow">

            <span></span>

            <span
                data-ar="حضور رسمي وإعلامي"
                data-en="Official & Media Presence">
                حضور رسمي وإعلامي
            </span>

        </div>


        <h2 class="section-title"
            data-ar="من الابتكار<br>إلى <em>الحضور.</em>"
            data-en="From innovation<br>to <em>impact.</em>">

            من الابتكار
            <br>
            إلى <em>الحضور.</em>

        </h2>


        <p class="section-description"
           data-ar="حظيت مكافح بحضور وتمثيل في مناسبات وبرامج تعكس رحلتها في الابتكار وريادة الأعمال، من بينها لقاء صاحب السمو الأمير سعود بن جلوي محافظ جدة عقب الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز د. طريف الأعمى."
           data-en="MUKAFIH has been represented across initiatives reflecting its innovation and entrepreneurship journey, including a meeting with H.H. Prince Saud bin Jalawi, Governor of Jeddah, following the Geneva win, attended by KAU President Dr. Tareef Al-Aama.">

            حظيت مكافح بحضور وتمثيل في مناسبات وبرامج تعكس رحلتها في الابتكار وريادة الأعمال، من بينها لقاء صاحب السمو الأمير سعود بن جلوي محافظ جدة عقب الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز د. طريف الأعمى.

        </p>


        <br>

        <a href="#contact" class="text-link"
           data-ar="ابدأ محادثة مع مكافح ←"
           data-en="Start a conversation with MUKAFIH →">

            ابدأ محادثة مع مكافح ←

        </a>

    </div>

</section>



<!-- =========================
 CONTACT
========================= -->

<section class="contact" id="contact">

    <div class="contact-bg"></div>

    <div class="contact-content reveal">

        <div class="eyebrow">

            <span></span>

            <span
                data-ar="تواصل معنا"
                data-en="Contact us">
                تواصل معنا
            </span>

            <span></span>

        </div>


        <h2 class="section-title"
            data-ar="هل منشأتك مستعدة<br><em>للخطر قبل وقوعه؟</em>"
            data-en="Is your facility ready<br><em>before the risk happens?</em>">

            هل منشأتك مستعدة
            <br>
            <em>للخطر قبل وقوعه؟</em>

        </h2>


        <p class="contact-description"
           data-ar="دعنا نناقش احتياجات منشأتك ونبني معًا مستوى حماية أكثر ذكاءً."
           data-en="Let's discuss your facility's needs and build a smarter level of protection together.">

            دعنا نناقش احتياجات منشأتك ونبني معًا مستوى حماية أكثر ذكاءً.

        </p>


        <form id="contactForm">

            <div class="form-row">

                <input
                    type="text"
                    required
                    data-ar-placeholder="الاسم الكامل"
                    data-en-placeholder="Full name"
                    placeholder="الاسم الكامل">

                <input
                    type="email"
                    required
                    data-ar-placeholder="البريد الإلكتروني"
                    data-en-placeholder="Email address"
                    placeholder="البريد الإلكتروني">

            </div>


            <div class="form-row">

                <input
                    type="text"
                    data-ar-placeholder="الشركة"
                    data-en-placeholder="Company"
                    placeholder="الشركة">

                <input
                    type="text"
                    data-ar-placeholder="القطاع"
                    data-en-placeholder="Industry"
                    placeholder="القطاع">

            </div>


            <textarea
                required
                data-ar-placeholder="كيف يمكننا مساعدتك؟"
                data-en-placeholder="How can we help?"
                placeholder="كيف يمكننا مساعدتك؟"></textarea>


            <button
                class="btn btn-red"
                type="submit"
                data-ar="إرسال الرسالة"
                data-en="Send message">

                إرسال الرسالة

            </button>


            <div id="formMessage" class="form-message"></div>

        </form>

    </div>

</section>

</main>



<!-- =========================
 FOOTER
========================= -->

<footer>

    <div class="footer-logo">

        <div class="footer-logo-box">M</div>

        <div>

            <strong>مكافح</strong>

            <small>
                MUKAFIH · FIRE PROTECTION COMPANY
            </small>

        </div>

    </div>


    <div class="footer-tagline"
         data-ar="نبتكر اليوم لنحمي الغد."
         data-en="We innovate today to protect tomorrow.">

        نبتكر اليوم لنحمي الغد.

    </div>


    <div class="socials">

        <a href="https://x.com/muk_fh"
           target="_blank"
           rel="noopener">
            X
        </a>

        <a href="https://www.instagram.com/muk.fh/"
           target="_blank"
           rel="noopener">
            IG
        </a>

        <a href="https://www.linkedin.com/company/mokfeh/"
           target="_blank"
           rel="noopener">
            in
        </a>

        <a href="https://www.tiktok.com/@muk.fh"
           target="_blank"
           rel="noopener">
            TT
        </a>

    </div>


    <div class="copyright">
        © 2026 MUKAFIH. All Rights Reserved.
    </div>

</footer>



<script>

/* =========================
   LOADER
========================= */

window.addEventListener("load",function(){

    setTimeout(function(){

        document
        .getElementById("loader")
        .classList.add("hide");

    },500);

});


/* =========================
   HEADER
========================= */

const header=document.getElementById("header");

window.addEventListener("scroll",function(){

    if(window.scrollY>40){
        header.classList.add("scrolled");
    }else{
        header.classList.remove("scrolled");
    }

});


/* =========================
   MOBILE MENU
========================= */

const menuBtn=document.getElementById("menuBtn");
const nav=document.getElementById("nav");

menuBtn.addEventListener("click",function(){

    nav.classList.toggle("open");

});

document.querySelectorAll("nav a").forEach(function(link){

    link.addEventListener("click",function(){

        nav.classList.remove("open");

    });

});


/* =========================
   LANGUAGE SWITCH
========================= */

let currentLanguage="ar";

const languageBtn=document.getElementById("languageBtn");

function changeLanguage(language){

    currentLanguage=language;

    document.documentElement.lang=language;

    document.documentElement.dir=
        language==="ar"
        ? "rtl"
        : "ltr";

    document.body.classList.toggle(
        "en",
        language==="en"
    );


    languageBtn.textContent=
        language==="ar"
        ? "EN"
        : "AR";


    document.querySelectorAll("[data-ar]").forEach(function(element){

        element.innerHTML=
            language==="ar"
            ? element.getAttribute("data-ar")
            : element.getAttribute("data-en");

    });


    document.querySelectorAll("input,textarea").forEach(function(element){

        if(element.hasAttribute("data-ar-placeholder")){

            element.placeholder=
                language==="ar"
                ? element.getAttribute("data-ar-placeholder")
                : element.getAttribute("data-en-placeholder");

        }

    });

}


languageBtn.addEventListener("click",function(){

    changeLanguage(
        currentLanguage==="ar"
        ? "en"
        : "ar"
    );

});


/* =========================
   SCROLL REVEAL
========================= */

const revealObserver=
new IntersectionObserver(
    function(entries){

        entries.forEach(function(entry){

            if(entry.isIntersecting){

                entry.target.classList.add("show");

            }

        });

    },
    {
        threshold:.12
    }
);


document
.querySelectorAll(".reveal")
.forEach(function(element){

    revealObserver.observe(element);

});


/* =========================
   CONTACT FORM
========================= */

const contactForm=
document.getElementById("contactForm");

contactForm.addEventListener("submit",function(event){

    event.preventDefault();

    const message=
        document.getElementById("formMessage");

    if(currentLanguage==="ar"){

        message.textContent=
        "تم استلام رسالتك. شكرًا لتواصلك مع مكافح.";

    }else{

        message.textContent=
        "Your message has been received. Thank you for contacting MUKAFIH.";

    }

    contactForm.reset();

});


/* =========================
   ACTIVE NAV
========================= */

const sections=
document.querySelectorAll("main section[id]");

const navLinks=
document.querySelectorAll("nav a");

window.addEventListener("scroll",function(){

    let current="";

    sections.forEach(function(section){

        const top=
            section.offsetTop-150;

        if(window.scrollY>=top){

            current=section.getAttribute("id");

        }

    });


    navLinks.forEach(function(link){

        link.classList.remove("active");

        if(
            link.getAttribute("href")
            ==="#"+current
        ){

            link.classList.add("active");

        }

    });

});

</script>

</body>
</html>
