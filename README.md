
<!DOCTYPE html>
<html lang="ar" dir="rtl">

<head>

    <meta charset="UTF-8">

    <meta name="viewport"
          content="width=device-width, initial-scale=1.0">

    <meta name="theme-color" content="#090909">

    <meta name="description"
          content="مكافح | حلول ذكية للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والطائرات المسيّرة.">

    <meta name="keywords"
          content="مكافح, مكافحة الحرائق, الذكاء الاصطناعي, الطائرات المسيّرة, FireTech, Saudi Arabia, MUKAFIH">

    <meta property="og:title"
          content="مكافح | MUKAFIH">

    <meta property="og:description"
          content="نبتكر اليوم لنحمي الغد. حلول ذكية للحماية من الحرائق.">

    <meta property="og:type"
          content="website">

    <meta property="og:url"
          content="https://malakalobidan.github.io/MUKKAFH/">

    <title>مكافح | MUKAFIH — Fire Protection Technology</title>

    <link rel="icon"
          href="assets/mukafih-logo.png">

    <style>

        /* =========================================================
           RESET
        ========================================================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family:
                "Segoe UI",
                Tahoma,
                Arial,
                sans-serif;

            background: #080808;
            color: #ffffff;

            overflow-x: hidden;

            line-height: 1.7;
        }

        body.light {
            background: #f5f5f5;
            color: #111;
        }

        img {
            max-width: 100%;
            display: block;
        }

        a {
            color: inherit;
            text-decoration: none;
        }

        button,
        input,
        textarea,
        select {
            font: inherit;
        }

        button {
            cursor: pointer;
        }

        ::selection {
            background: #e3262e;
            color: white;
        }


        /* =========================================================
           VARIABLES
        ========================================================= */

        :root {

            --red: #e3262e;
            --red-dark: #b71920;

            --black: #080808;
            --black-soft: #101010;
            --gray: #a4a4a4;
            --gray-dark: #1b1b1b;

            --border: rgba(255,255,255,.10);

            --max-width: 1250px;

            --transition:
                .35s cubic-bezier(.2,.8,.2,1);
        }


        /* =========================================================
           GLOBAL
        ========================================================= */

        .container {
            width: min(
                calc(100% - 40px),
                var(--max-width)
            );

            margin-inline: auto;
        }

        .section {
            padding: 120px 0;
            position: relative;
        }

        .eyebrow {

            display: inline-flex;

            align-items: center;

            gap: 10px;

            color: var(--red);

            font-size: 13px;

            font-weight: 800;

            letter-spacing: 2px;

            text-transform: uppercase;

            margin-bottom: 18px;
        }

        .eyebrow::before {

            content: "";

            width: 28px;

            height: 2px;

            background: var(--red);
        }

        .section-title {

            font-size:
                clamp(38px, 5vw, 72px);

            line-height: 1.05;

            letter-spacing: -2px;

            max-width: 850px;

            margin-bottom: 25px;

            font-weight: 800;
        }

        .section-description {

            color: var(--gray);

            max-width: 700px;

            font-size: 17px;

            line-height: 2;
        }


        /* =========================================================
           HEADER
        ========================================================= */

        header {

            position: fixed;

            top: 0;
            left: 0;
            right: 0;

            z-index: 1000;

            transition:
                var(--transition);

            background:
                linear-gradient(
                    to bottom,
                    rgba(0,0,0,.75),
                    transparent
                );
        }

        header.scrolled {

            background:
                rgba(8,8,8,.88);

            backdrop-filter:
                blur(18px);

            border-bottom:
                1px solid var(--border);
        }

        .nav {

            height: 84px;

            display: flex;

            align-items: center;

            justify-content: space-between;

            gap: 25px;
        }

        .logo {

            display: flex;

            align-items: center;

            gap: 12px;

            font-weight: 900;

            letter-spacing: 1px;
        }

        .logo img {

            width: 48px;
            height: 48px;

            object-fit: contain;
        }

        .logo-text {

            display: flex;

            flex-direction: column;

            line-height: 1.1;
        }

        .logo-ar {

            font-size: 18px;
        }

        .logo-en {

            color: var(--red);

            font-size: 10px;

            letter-spacing: 2px;
        }

        .nav-links {

            display: flex;

            align-items: center;

            gap: 28px;

            list-style: none;
        }

        .nav-links a {

            color: #ddd;

            font-size: 14px;

            transition: var(--transition);

            position: relative;
        }

        .nav-links a::after {

            content: "";

            position: absolute;

            bottom: -8px;

            right: 0;

            width: 0;

            height: 2px;

            background: var(--red);

            transition: var(--transition);
        }

        .nav-links a:hover {

            color: white;
        }

        .nav-links a:hover::after {

            width: 100%;
        }

        .nav-actions {

            display: flex;

            align-items: center;

            gap: 10px;
        }

        .lang-btn {

            background:
                transparent;

            border:
                1px solid var(--border);

            color: white;

            border-radius: 999px;

            padding: 9px 15px;

            font-weight: 700;

            transition: var(--transition);
        }

        .lang-btn:hover {

            background: white;

            color: black;
        }

        .menu-btn {

            display: none;

            background: transparent;

            border: none;

            color: white;

            font-size: 26px;
        }


        /* =========================================================
           HERO
        ========================================================= */

        .hero {

            min-height: 100vh;

            display: flex;

            align-items: center;

            position: relative;

            overflow: hidden;

            background: #050505;
        }

        .hero-bg {

            position: absolute;

            inset: 0;

            background:
                linear-gradient(
                    90deg,
                    rgba(0,0,0,.96) 0%,
                    rgba(0,0,0,.78) 40%,
                    rgba(0,0,0,.25) 100%
                );

            z-index: 1;
        }

        .hero-image {

            position: absolute;

            inset: 0;

            width: 100%;
            height: 100%;

            object-fit: cover;

            opacity: .48;

            z-index: 0;
        }

        .hero-content {

            position: relative;

            z-index: 2;

            padding-top: 80px;
        }

        .hero-kicker {

            color: var(--red);

            font-weight: 800;

            letter-spacing: 3px;

            font-size: 13px;

            margin-bottom: 20px;
        }

        .hero h1 {

            font-size:
                clamp(52px, 8vw, 110px);

            line-height: .95;

            letter-spacing: -5px;

            max-width: 900px;

            margin-bottom: 30px;

            font-weight: 900;
        }

        .hero h1 span {

            color: var(--red);
        }

        .hero-text {

            max-width: 650px;

            color: #d1d1d1;

            font-size: 18px;

            line-height: 2;

            margin-bottom: 35px;
        }

        .hero-buttons {

            display: flex;

            gap: 14px;

            flex-wrap: wrap;
        }

        .btn {

            display: inline-flex;

            align-items: center;

            justify-content: center;

            min-height: 52px;

            padding:
                0 25px;

            border-radius: 999px;

            border: 1px solid transparent;

            font-weight: 800;

            transition:
                var(--transition);
        }

        .btn-primary {

            background: var(--red);

            color: white;

            box-shadow:
                0 15px 40px
                rgba(227,38,46,.18);
        }

        .btn-primary:hover {

            background: #ff3038;

            transform:
                translateY(-3px);
        }

        .btn-outline {

            border-color:
                rgba(255,255,255,.25);

            color: white;

            background:
                rgba(255,255,255,.03);

            backdrop-filter:
                blur(8px);
        }

        .btn-outline:hover {

            border-color: white;

            background: white;

            color: black;

            transform:
                translateY(-3px);
        }

        .hero-stats {

            margin-top: 70px;

            display: flex;

            gap: 45px;

            flex-wrap: wrap;
        }

        .hero-stat {

            border-right:
                1px solid var(--border);

            padding-right: 25px;
        }

        [dir="ltr"] .hero-stat {

            border-right: none;

            border-left:
                1px solid var(--border);

            padding-right: 0;

            padding-left: 25px;
        }

        .hero-stat strong {

            display: block;

            font-size: 26px;
        }

        .hero-stat span {

            color: var(--gray);

            font-size: 12px;
        }


        /* =========================================================
           ABOUT
        ========================================================= */

        .about {

            background:
                linear-gradient(
                    180deg,
                    #080808,
                    #0d0d0d
                );
        }

        .about-grid {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 80px;

            align-items: center;
        }

        .about-image {

            position: relative;

            border-radius: 4px;

            overflow: hidden;

            min-height: 520px;

            background: #111;
        }

        .about-image img {

            width: 100%;
            height: 100%;

            min-height: 520px;

            object-fit: cover;

            transition:
                transform .8s ease;
        }

        .about-image:hover img {

            transform: scale(1.04);
        }

        .about-image::after {

            content: "";

            position: absolute;

            inset: 18px;

            border:
                1px solid
                rgba(255,255,255,.15);

            pointer-events: none;
        }

        .about-copy p {

            color: var(--gray);

            line-height: 2.1;

            margin-bottom: 25px;

            font-size: 17px;
        }

        .principles {

            display: grid;

            grid-template-columns:
                repeat(3,1fr);

            gap: 15px;

            margin-top: 35px;
        }

        .principle {

            padding: 20px;

            border:
                1px solid var(--border);

            background:
                rgba(255,255,255,.025);
        }

        .principle strong {

            color: var(--red);

            display: block;

            font-size: 12px;

            margin-bottom: 8px;

            letter-spacing: 1px;
        }

        .principle span {

            font-weight: 700;
        }


        /* =========================================================
           SERVICES
        ========================================================= */

        .services-grid {

            display: grid;

            grid-template-columns:
                repeat(2,1fr);

            gap: 16px;

            margin-top: 55px;
        }

        .service {

            position: relative;

            min-height: 330px;

            border:
                1px solid var(--border);

            background:
                linear-gradient(
                    145deg,
                    #151515,
                    #0c0c0c
                );

            padding: 35px;

            overflow: hidden;

            transition:
                var(--transition);
        }

        .service:hover {

            transform:
                translateY(-7px);

            border-color:
                rgba(227,38,46,.5);
        }

        .service-number {

            color: var(--red);

            font-size: 13px;

            font-weight: 900;

            letter-spacing: 2px;

            margin-bottom: 50px;
        }

        .service h3 {

            font-size: 27px;

            margin-bottom: 15px;
        }

        .service p {

            color: var(--gray);

            max-width: 500px;

            line-height: 1.9;
        }

        .service-icon {

            position: absolute;

            bottom: 25px;

            left: 30px;

            font-size: 70px;

            opacity: .06;

            font-weight: 900;
        }


        /* =========================================================
           TECHNOLOGY
        ========================================================= */

        .technology {

            background: #050505;
        }

        .tech-grid {

            display: grid;

            grid-template-columns:
                1.1fr .9fr;

            gap: 70px;

            align-items: center;
        }

        .tech-image {

            min-height: 600px;

            overflow: hidden;

            position: relative;
        }

        .tech-image img {

            width: 100%;
            height: 600px;

            object-fit: cover;
        }

        .tech-image::before {

            content: "";

            position: absolute;

            inset: 0;

            background:
                linear-gradient(
                    135deg,
                    rgba(227,38,46,.2),
                    transparent 45%
                );

            z-index: 1;
        }

        .tech-list {

            margin-top: 35px;

            display: grid;

            gap: 14px;
        }

        .tech-item {

            display: grid;

            grid-template-columns:
                50px 1fr;

            gap: 15px;

            padding: 20px 0;

            border-bottom:
                1px solid var(--border);
        }

        .tech-number {

            color: var(--red);

            font-weight: 900;
        }

        .tech-item h4 {

            margin-bottom: 5px;

            font-size: 17px;
        }

        .tech-item p {

            color: var(--gray);

            font-size: 14px;
        }


        /* =========================================================
           PROCESS
        ========================================================= */

        .process-grid {

            display: grid;

            grid-template-columns:
                repeat(5,1fr);

            margin-top: 60px;

            border-top:
                1px solid var(--border);

            border-bottom:
                1px solid var(--border);
        }

        .process-step {

            padding: 35px 22px;

            border-left:
                1px solid var(--border);

            min-height: 240px;
        }

        [dir="ltr"] .process-step {

            border-left: none;

            border-right:
                1px solid var(--border);
        }

        .process-step:last-child {

            border-left: none;
        }

        [dir="ltr"] .process-step:last-child {

            border-right: none;
        }

        .process-number {

            color: var(--red);

            font-size: 12px;

            font-weight: 900;

            margin-bottom: 45px;
        }

        .process-step h3 {

            margin-bottom: 10px;
        }

        .process-step p {

            color: var(--gray);

            font-size: 14px;
        }


        /* =========================================================
           SECTORS
        ========================================================= */

        .sectors-grid {

            display: grid;

            grid-template-columns:
                repeat(3,1fr);

            gap: 14px;

            margin-top: 55px;
        }

        .sector {

            min-height: 260px;

            position: relative;

            overflow: hidden;

            display: flex;

            align-items: flex-end;

            padding: 25px;

            background: #111;

            border:
                1px solid var(--border);
        }

        .sector img {

            position: absolute;

            inset: 0;

            width: 100%;
            height: 100%;

            object-fit: cover;

            opacity: .42;

            transition:
                transform .7s ease,
                opacity .5s ease;
        }

        .sector::after {

            content: "";

            position: absolute;

            inset: 0;

            background:
                linear-gradient(
                    to top,
                    rgba(0,0,0,.9),
                    rgba(0,0,0,.1)
                );
        }

        .sector:hover img {

            transform: scale(1.07);

            opacity: .65;
        }

        .sector-content {

            position: relative;

            z-index: 2;
        }

        .sector-number {

            color: var(--red);

            font-size: 12px;

            font-weight: 900;
        }

        .sector h3 {

            font-size: 23px;

            margin-top: 5px;
        }


        /* =========================================================
           ACHIEVEMENTS
        ========================================================= */

        .achievements {

            background:
                linear-gradient(
                    180deg,
                    #080808,
                    #111
                );
        }

        .geneva {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 45px;

            margin-top: 55px;

            border:
                1px solid
                rgba(227,38,46,.35);

            background:
                linear-gradient(
                    135deg,
                    rgba(227,38,46,.08),
                    rgba(255,255,255,.02)
                );
        }

        .geneva-image {

            min-height: 450px;

            overflow: hidden;
        }

        .geneva-image img {

            width: 100%;
            height: 100%;

            min-height: 450px;

            object-fit: cover;
        }

        .geneva-content {

            padding: 55px 45px;

            display: flex;

            flex-direction: column;

            justify-content: center;
        }

        .geneva-badge {

            color: var(--red);

            font-size: 12px;

            font-weight: 900;

            letter-spacing: 2px;

            margin-bottom: 20px;
        }

        .geneva-content h3 {

            font-size:
                clamp(35px,5vw,65px);

            line-height: 1;

            margin-bottom: 18px;
        }

        .geneva-content p {

            color: var(--gray);

            line-height: 1.9;
        }

        .awards-grid {

            display: grid;

            grid-template-columns:
                repeat(4,1fr);

            gap: 12px;

            margin-top: 14px;
        }

        .award-card {

            border:
                1px solid var(--border);

            background: #101010;

            overflow: hidden;

            transition:
                var(--transition);
        }

        .award-card:hover {

            transform:
                translateY(-5px);

            border-color:
                rgba(227,38,46,.45);
        }

        .award-image {

            height: 190px;

            overflow: hidden;

            background: #161616;
        }

        .award-image img {

            width: 100%;
            height: 100%;

            object-fit: cover;
        }

        .award-body {

            padding: 20px;

            min-height: 150px;
        }

        .award-body span {

            color: var(--red);

            font-size: 10px;

            font-weight: 900;

            letter-spacing: 1px;
        }

        .award-body h4 {

            font-size: 15px;

            line-height: 1.6;

            margin-top: 7px;
        }

        .timeline {

            margin-top: 70px;

            display: grid;

            gap: 0;
        }

        .timeline-item {

            display: grid;

            grid-template-columns:
                120px 1fr;

            gap: 30px;

            padding: 28px 0;

            border-top:
                1px solid var(--border);
        }

        .timeline-year {

            color: var(--red);

            font-weight: 900;

            font-size: 13px;

            letter-spacing: 1px;
        }

        .timeline-item h4 {

            margin-bottom: 5px;
        }

        .timeline-item p {

            color: var(--gray);

            font-size: 14px;

            max-width: 800px;
        }


        /* =========================================================
           MEDIA
        ========================================================= */

        .media {

            padding-top: 90px;
        }

        .media-layout {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 50px;

            align-items: center;
        }

        .media-image {

            min-height: 450px;

            overflow: hidden;
        }

        .media-image img {

            width: 100%;
            height: 450px;

            object-fit: cover;
        }

        .media-copy p {

            color: var(--gray);

            line-height: 2;

            margin-bottom: 20px;
        }

        .media-tags {

            display: flex;

            flex-wrap: wrap;

            gap: 10px;
        }

        .media-tag {

            border:
                1px solid var(--border);

            padding:
                9px 15px;

            font-size: 12px;

            color: #ccc;

            border-radius: 999px;
        }


        /* =========================================================
           CONTACT
        ========================================================= */

        .contact {

            background:
                #e3262e;

            color: white;
        }

        .contact .eyebrow {

            color: white;
        }

        .contact .eyebrow::before {

            background: white;
        }

        .contact-grid {

            display: grid;

            grid-template-columns:
                .8fr 1.2fr;

            gap: 80px;

            align-items: start;
        }

        .contact .section-title {

            max-width: 550px;
        }

        .contact-description {

            color:
                rgba(255,255,255,.8);

            line-height: 2;

            max-width: 500px;
        }

        .contact-form {

            background:
                #080808;

            padding: 35px;

            border:
                1px solid
                rgba(255,255,255,.15);

            border-radius: 3px;
        }

        .form-grid {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 14px;
        }

        .field {

            display: flex;

            flex-direction: column;

            gap: 8px;
        }

        .field.full {

            grid-column:
                1 / -1;
        }

        .field label {

            font-size: 12px;

            color: #aaa;

            font-weight: 700;
        }

        .field input,
        .field textarea,
        .field select {

            width: 100%;

            background: #111;

            border:
                1px solid
                rgba(255,255,255,.12);

            color: white;

            padding: 15px;

            outline: none;

            border-radius: 2px;

            transition:
                var(--transition);
        }

        .field textarea {

            min-height: 150px;

            resize: vertical;
        }

        .field input:focus,
        .field textarea:focus,
        .field select:focus {

            border-color:
                var(--red);
        }

        .field select option {

            background: #111;

            color: white;
        }

        .form-submit {

            margin-top: 18px;

            width: 100%;

            border: none;

            background: white;

            color: black;

            min-height: 55px;

            font-weight: 900;

            transition:
                var(--transition);
        }

        .form-submit:hover {

            background: #ddd;

            transform:
                translateY(-2px);
        }

        .form-submit:disabled {

            opacity: .5;

            cursor: wait;
        }

        .form-message {

            display: none;

            margin-top: 15px;

            padding: 14px;

            font-size: 13px;

            line-height: 1.7;

        }

        .form-message.success {

            display: block;

            background:
                rgba(50,200,100,.12);

            border:
                1px solid
                rgba(50,200,100,.35);

            color: #8ff0ae;
        }

        .form-message.error {

            display: block;

            background:
                rgba(227,38,46,.12);

            border:
                1px solid
                rgba(227,38,46,.35);

            color: #ff9ba0;
        }

        .honeypot {

            display: none !important;
        }


        /* =========================================================
           FOOTER
        ========================================================= */

        footer {

            background: #050505;

            border-top:
                1px solid var(--border);

            padding: 50px 0 25px;
        }

        .footer-top {

            display: flex;

            justify-content: space-between;

            align-items: center;

            gap: 30px;

            padding-bottom: 35px;

            border-bottom:
                1px solid var(--border);
        }

        .footer-brand {

            display: flex;

            align-items: center;

            gap: 12px;
        }

        .footer-brand img {

            width: 48px;
            height: 48px;

            object-fit: contain;
        }

        .footer-brand strong {

            display: block;
        }

        .footer-brand span {

            color: var(--red);

            font-size: 9px;

            letter-spacing: 2px;
        }

        .socials {

            display: flex;

            gap: 9px;

            flex-wrap: wrap;
        }

        .social {

            width: 42px;
            height: 42px;

            display: flex;

            align-items: center;

            justify-content: center;

            border:
                1px solid var(--border);

            border-radius: 50%;

            font-size: 11px;

            font-weight: 900;

            transition:
                var(--transition);
        }

        .social:hover {

            background: var(--red);

            border-color: var(--red);

            transform:
                translateY(-3px);
        }

        .footer-bottom {

            padding-top: 25px;

            color: #666;

            font-size: 11px;

            display: flex;

            justify-content: space-between;

            gap: 20px;
        }


        /* =========================================================
           REVEAL ANIMATION
        ========================================================= */

        .reveal {

            opacity: 0;

            transform:
                translateY(30px);

            transition:
                opacity .8s ease,
                transform .8s ease;
        }

        .reveal.visible {

            opacity: 1;

            transform:
                translateY(0);
        }


        /* =========================================================
           BACK TO TOP
        ========================================================= */

        .top-btn {

            position: fixed;

            bottom: 25px;

            left: 25px;

            width: 45px;
            height: 45px;

            border-radius: 50%;

            border:
                1px solid var(--border);

            background:
                rgba(10,10,10,.9);

            color: white;

            z-index: 999;

            opacity: 0;

            pointer-events: none;

            transition:
                var(--transition);
        }

        .top-btn.show {

            opacity: 1;

            pointer-events: auto;
        }


        /* =========================================================
           RESPONSIVE
        ========================================================= */

        @media (max-width: 1050px) {

            .nav-links {

                gap: 17px;
            }

            .about-grid,
            .tech-grid,
            .media-layout,
            .contact-grid,
            .geneva {

                grid-template-columns: 1fr;
            }

            .services-grid {

                grid-template-columns:
                    1fr 1fr;
            }

            .process-grid {

                grid-template-columns:
                    repeat(3,1fr);
            }

            .process-step:nth-child(4),
            .process-step:nth-child(5) {

                border-top:
                    1px solid var(--border);
            }

            .sectors-grid {

                grid-template-columns:
                    repeat(2,1fr);
            }

            .awards-grid {

                grid-template-columns:
                    repeat(2,1fr);
            }
        }


        @media (max-width: 800px) {

            .section {

                padding: 85px 0;
            }

            .nav {

                height: 72px;
            }

            .menu-btn {

                display: block;
            }

            .nav-links {

                position: absolute;

                top: 72px;

                right: 20px;
                left: 20px;

                display: none;

                flex-direction: column;

                align-items: stretch;

                gap: 0;

                background:
                    rgba(10,10,10,.98);

                border:
                    1px solid var(--border);

                padding: 10px;
            }

            .nav-links.active {

                display: flex;
            }

            .nav-links a {

                padding: 14px;

                border-bottom:
                    1px solid var(--border);
            }

            .nav-links li:last-child a {

                border-bottom: none;
            }

            .hero {

                min-height: 850px;
            }

            .hero h1 {

                letter-spacing: -3px;
            }

            .hero-stats {

                gap: 20px;
            }

            .hero-stat {

                padding-right: 15px;
            }

            .principles {

                grid-template-columns:
                    1fr;
            }

            .services-grid {

                grid-template-columns:
                    1fr;
            }

            .process-grid {

                grid-template-columns:
                    1fr;
            }

            .process-step {

                border-left: none;

                border-bottom:
                    1px solid var(--border);
            }

            [dir="ltr"] .process-step {

                border-right: none;
            }

            .process-step:last-child {

                border-bottom: none;
            }

            .sectors-grid {

                grid-template-columns:
                    1fr;
            }

            .awards-grid {

                grid-template-columns:
                    1fr;
            }

            .timeline-item {

                grid-template-columns:
                    1fr;

                gap: 5px;
            }

            .form-grid {

                grid-template-columns:
                    1fr;
            }

            .field.full {

                grid-column:
                    auto;
            }

            .footer-top,
            .footer-bottom {

                flex-direction: column;

                align-items: flex-start;
            }
        }


        @media (max-width: 500px) {

            .container {

                width:
                    min(
                        calc(100% - 28px),
                        var(--max-width)
                    );
            }

            .hero h1 {

                font-size: 52px;
            }

            .hero-text {

                font-size: 15px;
            }

            .geneva-content {

                padding: 35px 25px;
            }

            .contact-form {

                padding: 22px;
            }
        }

    </style>

</head>


<body>

<!-- =========================================================
     HEADER
========================================================= -->

<header id="header">

    <div class="container">

        <nav class="nav">

            <a href="#home"
               class="logo">

                <img
                    src="assets/mukafih-logo.png"
                    alt="MUKAFIH Logo">

                <span class="logo-text">

                    <span class="logo-ar">
                        مكافح
                    </span>

                    <span class="logo-en">
                        MUKAFIH
                    </span>

                </span>

            </a>


            <ul class="nav-links"
                id="navLinks">

                <li>
                    <a href="#home"
                       data-ar="الرئيسية"
                       data-en="Home">
                        الرئيسية
                    </a>
                </li>

                <li>
                    <a href="#about"
                       data-ar="من نحن"
                       data-en="About">
                        من نحن
                    </a>
                </li>

                <li>
                    <a href="#solutions"
                       data-ar="الحلول"
                       data-en="Solutions">
                        الحلول
                    </a>
                </li>

                <li>
                    <a href="#technology"
                       data-ar="التقنية"
                       data-en="Technology">
                        التقنية
                    </a>
                </li>

                <li>
                    <a href="#sectors"
                       data-ar="القطاعات"
                       data-en="Sectors">
                        القطاعات
                    </a>
                </li>

                <li>
                    <a href="#achievements"
                       data-ar="الإنجازات"
                       data-en="Achievements">
                        الإنجازات
                    </a>
                </li>

                <li>
                    <a href="#contact"
                       data-ar="تواصل معنا"
                       data-en="Contact">
                        تواصل معنا
                    </a>
                </li>

            </ul>


            <div class="nav-actions">

                <button
                    class="lang-btn"
                    id="languageButton"
                    type="button">
                    EN
                </button>

                <button
                    class="menu-btn"
                    id="menuButton"
                    type="button"
                    aria-label="Menu">
                    ☰
                </button>

            </div>

        </nav>

    </div>

</header>


<!-- =========================================================
     HERO
========================================================= -->

<main>

<section
    class="hero"
    id="home">

    <img
        class="hero-image"
        src="assets/hero-drone-truck.jpg"
        alt="MUKAFIH Smart Fire Protection"
        loading="eager">

    <div class="hero-bg"></div>


    <div class="container">

        <div class="hero-content reveal">

            <div class="hero-kicker"
                 data-ar="FIRE PROTECTION • AI • AUTONOMOUS TECHNOLOGY"
                 data-en="FIRE PROTECTION • AI • AUTONOMOUS TECHNOLOGY">

                FIRE PROTECTION • AI • AUTONOMOUS TECHNOLOGY

            </div>


            <h1
                data-ar="نبتكر اليوم<br>لنحمي <span>الغد.</span>"
                data-en="Innovate Today.<br>Protect <span>Tomorrow.</span>">

                نبتكر اليوم<br>
                لنحمي <span>الغد.</span>

            </h1>


            <p
                class="hero-text"
                data-ar="نطور حلولًا متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والطائرات المسيّرة والأتمتة، لمساعدة المنشآت على الرصد المبكر واتخاذ القرار والاستجابة بذكاء."
                data-en="We develop advanced fire protection solutions that combine engineering, artificial intelligence, drones and automation to help facilities detect risks early, make smarter decisions and respond faster.">

                نطور حلولًا متقدمة للحماية من الحرائق تجمع بين الهندسة والذكاء الاصطناعي والطائرات المسيّرة والأتمتة، لمساعدة المنشآت على الرصد المبكر واتخاذ القرار والاستجابة بذكاء.

            </p>


            <div class="hero-buttons">

                <a
                    href="#solutions"
                    class="btn btn-primary"
                    data-ar="اكتشف حلولنا"
                    data-en="Explore Solutions">

                    اكتشف حلولنا

                </a>

                <a
                    href="#contact"
                    class="btn btn-outline"
                    data-ar="تواصل مع مكافح"
                    data-en="Contact MUKAFIH">

                    تواصل مع مكافح

                </a>

            </div>


            <div class="hero-stats">

                <div class="hero-stat">

                    <strong>AI</strong>

                    <span
                        data-ar="ذكاء اصطناعي"
                        data-en="Artificial Intelligence">
                        ذكاء اصطناعي
                    </span>

                </div>


                <div class="hero-stat">

                    <strong>3D</strong>

                    <span
                        data-ar="خرائط ثلاثية الأبعاد"
                        data-en="3D Mapping">
                        خرائط ثلاثية الأبعاد
                    </span>

                </div>


                <div class="hero-stat">

                    <strong>24/7</strong>

                    <span
                        data-ar="رصد واستجابة"
                        data-en="Monitoring & Response">
                        رصد واستجابة
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     ABOUT
========================================================= -->

<section
    class="section about"
    id="about">

    <div class="container">

        <div class="about-grid">

            <div class="about-image reveal">

                <img
                    src="assets/drone.jpg"
                    alt="MUKAFIH Drone"
                    loading="lazy">

            </div>


            <div class="about-copy reveal">

                <div
                    class="eyebrow"
                    data-ar="من نحن"
                    data-en="ABOUT US">
                    من نحن
                </div>


                <h2
                    class="section-title"
                    data-ar="الحماية لم تعد تنتظر وقوع الحريق."
                    data-en="Protection should not wait for the fire.">

                    الحماية لم تعد
                    تنتظر وقوع الحريق.

                </h2>


                <p
                    data-ar="نحن في مكافح نؤمن بقوة الابتكار والتقنية في تطوير مستقبل أكثر أمانًا. نعمل على تقديم حلول متقدمة للحماية من الحرائق مصممة للبيئات التي تتطلب سرعة الاستجابة وذكاء القرار."
                    data-en="At MUKAFIH, we believe in the power of innovation and technology to build a safer future. We develop advanced fire protection solutions for environments where fast response and intelligent decision-making matter.">

                    نحن في مكافح نؤمن بقوة الابتكار والتقنية في تطوير مستقبل أكثر أمانًا. نعمل على تقديم حلول متقدمة للحماية من الحرائق مصممة للبيئات التي تتطلب سرعة الاستجابة وذكاء القرار.

                </p>


                <p
                    data-ar="نمـزج بين الأنظمة الهندسية والتقنيات الذكية لنمنح المنشآت مستوى أعلى من الرصد والتحليل والاستجابة."
                    data-en="We combine engineering systems with intelligent technologies to provide facilities with a higher level of monitoring, analysis and response.">

                    نمـزج بين الأنظمة الهندسية والتقنيات الذكية لنمنح المنشآت مستوى أعلى من الرصد والتحليل والاستجابة.

                </p>


                <div class="principles">

                    <div class="principle">

                        <strong>01</strong>

                        <span
                            data-ar="الابتكار"
                            data-en="Innovation">
                            الابتكار
                        </span>

                    </div>


                    <div class="principle">

                        <strong>02</strong>

                        <span
                            data-ar="السلامة"
                            data-en="Safety">
                            السلامة
                        </span>

                    </div>


                    <div class="principle">

                        <strong>03</strong>

                        <span
                            data-ar="الاستجابة الذكية"
                            data-en="Smart Response">
                            الاستجابة الذكية
                        </span>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     SOLUTIONS
========================================================= -->

<section
    class="section"
    id="solutions">

    <div class="container">

        <div class="eyebrow"
             data-ar="حلول مكافح"
             data-en="MUKAFIH SOLUTIONS">

            حلول مكافح

        </div>


        <h2
            class="section-title reveal"
            data-ar="حلول مصممة<br>للخطر الحقيقي."
            data-en="Solutions designed<br>for real-world risk.">

            حلول مصممة
            <br>
            للخطر الحقيقي.

        </h2>


        <p
            class="section-description reveal"
            data-ar="من الكشف المبكر إلى الاستجابة، نطور منظومة حماية تتناسب مع طبيعة المنشأة ودرجة المخاطر فيها."
            data-en="From early detection to response, we develop protection systems tailored to the facility, its environment and its risk profile.">

            من الكشف المبكر إلى الاستجابة، نطور منظومة حماية تتناسب مع طبيعة المنشأة ودرجة المخاطر فيها.

        </p>


        <div class="services-grid">

            <article class="service reveal">

                <div class="service-number">
                    01
                </div>

                <h3
                    data-ar="الحماية الذكية بالطائرات المسيّرة"
                    data-en="Smart Drone Fire Protection">

                    الحماية الذكية بالطائرات المسيّرة

                </h3>

                <p
                    data-ar="حلول جوية ذكية للعمل داخل البيئات الصناعية والمنشآت المغلقة، للمساعدة في اكتشاف الحريق والتحقق منه والاستجابة المبكرة."
                    data-en="Smart aerial solutions designed for industrial and enclosed environments to support fire detection, verification and early response.">

                    حلول جوية ذكية للعمل داخل البيئات الصناعية والمنشآت المغلقة، للمساعدة في اكتشاف الحريق والتحقق منه والاستجابة المبكرة.

                </p>

                <div class="service-icon">
                    DRONE
                </div>

            </article>


            <article class="service reveal">

                <div class="service-number">
                    02
                </div>

                <h3
                    data-ar="أنظمة مكافحة الحرائق"
                    data-en="Fire Protection Systems">

                    أنظمة مكافحة الحرائق

                </h3>

                <p
                    data-ar="حلول حماية متقدمة مصممة وفق طبيعة كل منشأة واحتياجاتها التشغيلية."
                    data-en="Advanced protection solutions designed around the specific nature and operational requirements of each facility.">

                    حلول حماية متقدمة مصممة وفق طبيعة كل منشأة واحتياجاتها التشغيلية.

                </p>

                <div class="service-icon">
                    FIRE
                </div>

            </article>


            <article class="service reveal">

                <div class="service-number">
                    03
                </div>

                <h3
                    data-ar="الذكاء الاصطناعي والكشف المبكر"
                    data-en="AI & Early Detection">

                    الذكاء الاصطناعي والكشف المبكر

                </h3>

                <p
                    data-ar="توظيف الرؤية الحاسوبية والذكاء الاصطناعي لتحليل البيئة واكتشاف مؤشرات الخطر."
                    data-en="Using computer vision and artificial intelligence to analyze environments and identify potential risk indicators.">

                    توظيف الرؤية الحاسوبية والذكاء الاصطناعي لتحليل البيئة واكتشاف مؤشرات الخطر.

                </p>

                <div class="service-icon">
                    AI
                </div>

            </article>


            <article class="service reveal">

                <div class="service-number">
                    04
                </div>

                <h3
                    data-ar="حلول المنشآت الصناعية"
                    data-en="Industrial Facility Solutions">

                    حلول المنشآت الصناعية

                </h3>

                <p
                    data-ar="منظومات حماية للبيئات التي تتطلب مستويات عالية من المراقبة والاستجابة والسلامة."
                    data-en="Protection solutions for environments requiring advanced levels of monitoring, response and safety.">

                    منظومات حماية للبيئات التي تتطلب مستويات عالية من المراقبة والاستجابة والسلامة.

                </p>

                <div class="service-icon">
                    3D
                </div>

            </article>

        </div>

    </div>

</section>


<!-- =========================================================
     TECHNOLOGY
========================================================= -->

<section
    class="section technology"
    id="technology">

    <div class="container">

        <div class="tech-grid">

            <div class="tech-image reveal">

                <img
                    src="assets/technology.jpg"
                    alt="MUKAFIH Technology"
                    loading="lazy">

            </div>


            <div class="reveal">

                <div class="eyebrow"
                     data-ar="التقنية"
                     data-en="TECHNOLOGY">

                    التقنية

                </div>


                <h2
                    class="section-title"
                    data-ar="عندما تصبح كل ثانية مهمة."
                    data-en="When every second matters.">

                    عندما تصبح
                    <br>
                    كل ثانية مهمة.

                </h2>


                <p
                    class="section-description"
                    data-ar="صممت منظومة مكافح لتعمل في البيئات التي قد تكون فيها الاستجابة البشرية صعبة أو محفوفة بالمخاطر."
                    data-en="MUKAFIH is designed for environments where human intervention can be difficult, dangerous or too slow.">

                    صممت منظومة مكافح لتعمل في البيئات التي قد تكون فيها الاستجابة البشرية صعبة أو محفوفة بالمخاطر.

                </p>


                <div class="tech-list">

                    <div class="tech-item">

                        <div class="tech-number">
                            01
                        </div>

                        <div>

                            <h4
                                data-ar="رصد وتحليل ذكي"
                                data-en="Intelligent Monitoring & Analysis">
                                رصد وتحليل ذكي
                            </h4>

                            <p
                                data-ar="مراقبة البيئة وتحليل البيانات لاكتشاف مؤشرات الخطر."
                                data-en="Monitoring environments and analyzing data to identify risk indicators.">
                                مراقبة البيئة وتحليل البيانات لاكتشاف مؤشرات الخطر.
                            </p>

                        </div>

                    </div>


                    <div class="tech-item">

                        <div class="tech-number">
                            02
                        </div>

                        <div>

                            <h4
                                data-ar="خرائط ثلاثية الأبعاد"
                                data-en="3D Indoor Mapping">
                                خرائط ثلاثية الأبعاد
                            </h4>

                            <p
                                data-ar="بناء تصور ثلاثي الأبعاد للبيئات الداخلية لدعم تحديد موقع الخطر."
                                data-en="Creating 3D representations of indoor environments to support precise risk localization.">
                                بناء تصور ثلاثي الأبعاد للبيئات الداخلية لدعم تحديد موقع الخطر.
                            </p>

                        </div>

                    </div>


                    <div class="tech-item">

                        <div class="tech-number">
                            03
                        </div>

                        <div>

                            <h4
                                data-ar="الرؤية الحاسوبية"
                                data-en="Computer Vision">
                                الرؤية الحاسوبية
                            </h4>

                            <p
                                data-ar="تحليل بصري ذكي لدعم اكتشاف الأحداث ومؤشرات الخطر."
                                data-en="Intelligent visual analysis to support event and risk detection.">
                                تحليل بصري ذكي لدعم اكتشاف الأحداث ومؤشرات الخطر.
                            </p>

                        </div>

                    </div>


                    <div class="tech-item">

                        <div class="tech-number">
                            04
                        </div>

                        <div>

                            <h4
                                data-ar="ملاحة في البيئات المغلقة"
                                data-en="Indoor Navigation">
                                ملاحة في البيئات المغلقة
                            </h4>

                            <p
                                data-ar="تقنيات تساعد على الحركة داخل البيئات التي لا يتوفر فيها GPS."
                                data-en="Navigation technologies designed for environments where GPS may not be available.">
                                تقنيات تساعد على الحركة داخل البيئات التي لا يتوفر فيها GPS.
                            </p>

                        </div>

                    </div>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     PROCESS
========================================================= -->

<section
    class="section"
    id="process">

    <div class="container">

        <div class="eyebrow"
             data-ar="كيف تعمل مكافح؟"
             data-en="HOW MUKAFIH WORKS?">

            كيف تعمل مكافح؟

        </div>


        <h2
            class="section-title reveal"
            data-ar="من الرصد إلى الاستجابة."
            data-en="From detection to response.">

            من الرصد
            <br>
            إلى الاستجابة.

        </h2>


        <div class="process-grid">

            <div class="process-step reveal">

                <div class="process-number">
                    01
                </div>

                <h3
                    data-ar="الرصد"
                    data-en="Detection">
                    الرصد
                </h3>

                <p
                    data-ar="مراقبة البيئة واكتشاف مؤشرات الخطر."
                    data-en="Monitoring the environment and identifying risk indicators.">
                    مراقبة البيئة واكتشاف مؤشرات الخطر.
                </p>

            </div>


            <div class="process-step reveal">

                <div class="process-number">
                    02
                </div>

                <h3
                    data-ar="التحليل"
                    data-en="Analysis">
                    التحليل
                </h3>

                <p
                    data-ar="تحليل البيانات وتحديد طبيعة الحدث."
                    data-en="Analyzing data and determining the nature of the event.">
                    تحليل البيانات وتحديد طبيعة الحدث.
                </p>

            </div>


            <div class="process-step reveal">

                <div class="process-number">
                    03
                </div>

                <h3
                    data-ar="تحديد الموقع"
                    data-en="Localization">
                    تحديد الموقع
                </h3>

                <p
                    data-ar="تحديد موقع الخطر داخل المنشأة."
                    data-en="Locating the risk within the facility.">
                    تحديد موقع الخطر داخل المنشأة.
                </p>

            </div>


            <div class="process-step reveal">

                <div class="process-number">
                    04
                </div>

                <h3
                    data-ar="الاستجابة"
                    data-en="Response">
                    الاستجابة
                </h3>

                <p
                    data-ar="تفعيل منظومة الاستجابة المناسبة."
                    data-en="Activating the appropriate response system.">
                    تفعيل منظومة الاستجابة المناسبة.
                </p>

            </div>


            <div class="process-step reveal">

                <div class="process-number">
                    05
                </div>

                <h3
                    data-ar="الحماية"
                    data-en="Protection">
                    الحماية
                </h3>

                <p
                    data-ar="المساعدة في الحد من انتشار الخطر وتقليل المخاطر."
                    data-en="Helping limit risk escalation and reduce potential damage.">
                    المساعدة في الحد من انتشار الخطر وتقليل المخاطر.
                </p>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     SECTORS
========================================================= -->

<section
    class="section"
    id="sectors">

    <div class="container">

        <div class="eyebrow"
             data-ar="القطاعات"
             data-en="SECTORS">

            القطاعات

        </div>


        <h2
            class="section-title reveal"
            data-ar="حماية تتكيف مع بيئتك."
            data-en="Protection adapted to your environment.">

            حماية تتكيف
            <br>
            مع بيئتك.

        </h2>


        <p
            class="section-description reveal"
            data-ar="حلول موجهة للبيئات التي تتطلب مستويات متقدمة من المراقبة والاستجابة."
            data-en="Solutions for environments that require advanced monitoring and response capabilities.">

            حلول موجهة للبيئات التي تتطلب مستويات متقدمة من المراقبة والاستجابة.

        </p>


        <div class="sectors-grid">

            <article class="sector reveal">

                <img
                    src="assets/factory.jpg"
                    alt="Factories"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        01
                    </div>

                    <h3
                        data-ar="المصانع"
                        data-en="Factories">
                        المصانع
                    </h3>

                </div>

            </article>


            <article class="sector reveal">

                <img
                    src="assets/warehouse.jpg"
                    alt="Warehouses"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        02
                    </div>

                    <h3
                        data-ar="المستودعات"
                        data-en="Warehouses">
                        المستودعات
                    </h3>

                </div>

            </article>


            <article class="sector reveal">

                <img
                    src="assets/electrical-room.jpg"
                    alt="Electrical Facilities"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        03
                    </div>

                    <h3
                        data-ar="غرف الكهرباء والمحطات"
                        data-en="Electrical Facilities">
                        غرف الكهرباء والمحطات
                    </h3>

                </div>

            </article>


            <article class="sector reveal">

                <img
                    src="assets/data-center.jpg"
                    alt="Data Centers"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        04
                    </div>

                    <h3
                        data-ar="مراكز البيانات"
                        data-en="Data Centers">
                        مراكز البيانات
                    </h3>

                </div>

            </article>


            <article class="sector reveal">

                <img
                    src="assets/tunnel.jpg"
                    alt="Tunnels"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        05
                    </div>

                    <h3
                        data-ar="الأنفاق والمرافق المغلقة"
                        data-en="Tunnels & Enclosed Facilities">
                        الأنفاق والمرافق المغلقة
                    </h3>

                </div>

            </article>


            <article class="sector reveal">

                <img
                    src="assets/industrial-facility.jpg"
                    alt="High Risk Facilities"
                    loading="lazy">

                <div class="sector-content">

                    <div class="sector-number">
                        06
                    </div>

                    <h3
                        data-ar="المنشآت عالية الخطورة"
                        data-en="High-Risk Facilities">
                        المنشآت عالية الخطورة
                    </h3>

                </div>

            </article>

        </div>

    </div>

</section>


<!-- =========================================================
     ACHIEVEMENTS
========================================================= -->

<section
    class="section achievements"
    id="achievements">

    <div class="container">

        <div class="eyebrow"
             data-ar="الإنجازات والتكريمات"
             data-en="ACHIEVEMENTS & RECOGNITION">

            الإنجازات والتكريمات

        </div>


        <h2
            class="section-title reveal"
            data-ar="إنجازات تصنع الثقة."
            data-en="Achievements that build trust.">

            إنجازات
            <br>
            تصنع الثقة.

        </h2>


        <p
            class="section-description reveal"
            data-ar="من الاحتضان والتأهل إلى التقدير الدولي، نواصل بناء رحلة مكافح بخطوات موثقة."
            data-en="From incubation and national competitions to international recognition, MUKAFIH continues to build its journey through documented milestones.">

            من الاحتضان والتأهل إلى التقدير الدولي، نواصل بناء رحلة مكافح بخطوات موثقة.

        </p>


        <!-- GENEVA -->

        <div class="geneva reveal">

            <div class="geneva-image">

                <img
                    src="assets/award-geneva.jpg"
                    alt="Geneva Gold Medal"
                    loading="lazy">

            </div>


            <div class="geneva-content">

                <div class="geneva-badge">

                    51ST GENEVA INTERNATIONAL EXHIBITION OF INVENTIONS

                </div>


                <h3
                    data-ar="الميدالية الذهبية"
                    data-en="Gold Medal">

                    الميدالية الذهبية

                </h3>


                <p
                    data-ar="مع مرتبة الشرف — تكريم دولي يبرز قيمة الابتكار الذي تقدمه مكافح."
                    data-en="With Honors — an international recognition highlighting the innovation developed by MUKAFIH.">

                    مع مرتبة الشرف — تكريم دولي يبرز قيمة الابتكار الذي تقدمه مكافح.

                </p>

            </div>

        </div>


        <!-- SPECIAL AWARDS -->

        <div class="awards-grid">

            <article class="award-card reveal">

                <div class="award-image">

                    <img
                        src="assets/award-hkust.jpg"
                        alt="HKUST Award"
                        loading="lazy">

                </div>

                <div class="award-body">

                    <span>
                        SPECIAL AWARD
                    </span>

                    <h4>
                        THE HONG KONG UNIVERSITY OF SCIENCE AND TECHNOLOGY
                    </h4>

                </div>

            </article>


            <article class="award-card reveal">

                <div class="award-image">

                    <img
                        src="assets/award-french.jpg"
                        alt="French Inventors Federation"
                        loading="lazy">

                </div>

                <div class="award-body">

                    <span>
                        SPECIAL RECOGNITION
                    </span>

                    <h4
                        data-ar="شهادة وميدالية — الاتحاد الفرنسي للمخترعين"
                        data-en="Certificate & Medal — French Inventors Federation">

                        شهادة وميدالية — الاتحاد الفرنسي للمخترعين

                    </h4>

                </div>

            </article>


            <article class="award-card reveal">

                <div class="award-image">

                    <img
                        src="assets/award-malaysia.jpg"
                        alt="Malaysia Delegation Award"
                        loading="lazy">

                </div>

                <div class="award-body">

                    <span>
                        SPECIAL AWARD
                    </span>

                    <h4
                        data-ar="الجائزة الخاصة — وفد ماليزيا"
                        data-en="Special Award — Malaysia Delegation">

                        الجائزة الخاصة — وفد ماليزيا

                    </h4>

                </div>

            </article>


            <article class="award-card reveal">

                <div class="award-image">

                    <img
                        src="assets/award-qassim.jpg"
                        alt="Qassim University Award"
                        loading="lazy">

                </div>

                <div class="award-body">

                    <span>
                        SPECIAL AWARD
                    </span>

                    <h4
                        data-ar="جائزة خاصة — جامعة القصيم"
                        data-en="Special Award — Qassim University">

                        جائزة خاصة — جامعة القصيم

                    </h4>

                </div>

            </article>

        </div>


        <!-- TIMELINE -->

        <div class="timeline">

            <div class="timeline-item reveal">

                <div class="timeline-year">
                    2025
                </div>

                <div>

                    <h4
                        data-ar="برنامج الاحتضان — CEIES"
                        data-en="Incubation Program — CEIES">

                        برنامج الاحتضان — CEIES

                    </h4>

                    <p
                        data-ar="برنامج الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز، خلال الفترة من يناير إلى ديسمبر 2025."
                        data-en="Incubation at the Center of Excellence for Engineering Systems and Electrical Engineering at King Abdulaziz University from January to December 2025.">

                        برنامج الاحتضان في مركز التميز البحثي للأنظمة الهندسية والكهربائية بجامعة الملك عبدالعزيز، خلال الفترة من يناير إلى ديسمبر 2025.

                    </p>

                </div>

            </div>


            <div class="timeline-item reveal">

                <div class="timeline-year">
                    2026
                </div>

                <div>

                    <h4
                        data-ar="إنجاز السعودية — التأهل للنهائيات"
                        data-en="Enjaz Saudi Arabia — Finalist">

                        إنجاز السعودية — التأهل للنهائيات

                    </h4>

                    <p
                        data-ar="التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية 2026."
                        data-en="Qualified for the finals of the Idea Competition by Enjaz Saudi Arabia 2026.">

                        التأهل إلى نهائيات مسابقة فكرة التابعة لإنجاز السعودية 2026.

                    </p>

                </div>

            </div>


            <div class="timeline-item reveal">

                <div class="timeline-year">
                    2026
                </div>

                <div>

                    <h4
                        data-ar="أفضل 20 مشروعًا رياديًا"
                        data-en="Top 20 Entrepreneurial Projects">

                        أفضل 20 مشروعًا رياديًا

                    </h4>

                    <p
                        data-ar="كنا ضمن أفضل 20 مشروعًا رياديًا مشاركًا في المؤتمر الأول للابتكار وريادة الأعمال بجامعة الملك عبدالعزيز."
                        data-en="Selected among the Top 20 entrepreneurial projects participating in the First Innovation & Entrepreneurship Conference at King Abdulaziz University.">

                        كنا ضمن أفضل 20 مشروعًا رياديًا مشاركًا في المؤتمر الأول للابتكار وريادة الأعمال بجامعة الملك عبدالعزيز.

                    </p>

                </div>

            </div>


            <div class="timeline-item reveal">

                <div class="timeline-year">
                    MILESTONE
                </div>

                <div>

                    <h4
                        data-ar="غرفة جدة — أسبوع ريادة الأعمال"
                        data-en="Jeddah Chamber — Entrepreneurship Week">

                        غرفة جدة — أسبوع ريادة الأعمال

                    </h4>

                    <p
                        data-ar="المشاركة ضمن فعاليات أسبوع ريادة الأعمال في غرفة جدة."
                        data-en="Participation in Entrepreneurship Week activities at Jeddah Chamber.">

                        المشاركة ضمن فعاليات أسبوع ريادة الأعمال في غرفة جدة.

                    </p>

                </div>

            </div>


            <div class="timeline-item reveal">

                <div class="timeline-year">
                    MILESTONE
                </div>

                <div>

                    <h4
                        data-ar="معرض رواد الأعمال — كلية العلوم"
                        data-en="Entrepreneurs Exhibition — College of Science">

                        معرض رواد الأعمال — كلية العلوم

                    </h4>

                    <p
                        data-ar="المشاركة في معرض رواد الأعمال بكلية العلوم."
                        data-en="Participation in the Entrepreneurs Exhibition at the College of Science.">

                        المشاركة في معرض رواد الأعمال بكلية العلوم.

                    </p>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     MEDIA / OFFICIAL PRESENCE
========================================================= -->

<section
    class="section media">

    <div class="container">

        <div class="media-layout">

            <div class="media-image reveal">

                <img
                    src="assets/achievement-prince-saud.jpg"
                    alt="MUKAFIH Official Meeting"
                    loading="lazy">

            </div>


            <div class="media-copy reveal">

                <div class="eyebrow"
                     data-ar="حضور رسمي وإعلامي"
                     data-en="OFFICIAL & MEDIA PRESENCE">

                    حضور رسمي وإعلامي

                </div>


                <h2
                    class="section-title"
                    data-ar="من الابتكار إلى الحضور."
                    data-en="From innovation to impact.">

                    من الابتكار
                    <br>
                    إلى الحضور.

                </h2>


                <p
                    data-ar="حظيت مكافح بحضور وتمثيل في مناسبات وبرامج تعكس رحلتها في الابتكار وريادة الأعمال، من بينها لقاء صاحب السمو الأمير سعود بن جلوي محافظ جدة عقب الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز د. طريف الأعمى."
                    data-en="MUKAFIH has been represented across events and programs reflecting its innovation and entrepreneurship journey, including a meeting with His Highness Prince Saud bin Jalawi, Governor of Jeddah, following the Geneva International Exhibition of Inventions, in the presence of the President of King Abdulaziz University, Dr. Tareef Al-Aama.">

                    حظيت مكافح بحضور وتمثيل في مناسبات وبرامج تعكس رحلتها في الابتكار وريادة الأعمال، من بينها لقاء صاحب السمو الأمير سعود بن جلوي محافظ جدة عقب الفوز في معرض جنيف الدولي للاختراعات، بحضور رئيس جامعة الملك عبدالعزيز د. طريف الأعمى.

                </p>


                <div class="media-tags">

                    <span class="media-tag"
                          data-ar="ملتقى تمكين المستقبل"
                          data-en="Future Empowerment Forum">
                        ملتقى تمكين المستقبل
                    </span>

                    <span class="media-tag"
                          data-ar="إذاعة الرياض"
                          data-en="Riyadh Radio">
                        إذاعة الرياض
                    </span>

                    <span class="media-tag"
                          data-ar="Hack4Earth"
                          data-en="Hack4Earth">
                        Hack4Earth
                    </span>

                    <span class="media-tag"
                          data-ar="غرفة جدة"
                          data-en="Jeddah Chamber">
                        غرفة جدة
                    </span>

                </div>

            </div>

        </div>

    </div>

</section>


<!-- =========================================================
     CONTACT
========================================================= -->

<section
    class="section contact"
    id="contact">

    <div class="container">

        <div class="contact-grid">

            <div class="reveal">

                <div class="eyebrow"
                     data-ar="تواصل معنا"
                     data-en="CONTACT US">

                    تواصل معنا

                </div>


                <h2
                    class="section-title"
                    data-ar="هل منشأتك مستعدة للخطر قبل وقوعه؟"
                    data-en="Is your facility ready before risk occurs?">

                    هل منشأتك مستعدة
                    <br>
                    للخطر قبل وقوعه؟

                </h2>


                <p
                    class="contact-description"
                    data-ar="نحن هنا لمناقشة احتياجات منشأتك وفرص التعاون وبناء مستوى حماية أكثر ذكاءً."
                    data-en="We are here to discuss your facility's needs, explore collaboration opportunities and build a smarter level of protection.">

                    نحن هنا لمناقشة احتياجات منشأتك وفرص التعاون وبناء مستوى حماية أكثر ذكاءً.

                </p>

            </div>


            <!-- REAL CONTACT FORM -->

            <form
                id="contactForm"
                class="contact-form reveal"
                action="https://formsubmit.co/ajax/mkafh2024@gmail.com"
                method="POST">

                <!-- Email subject -->

                <input
                    type="hidden"
                    name="_subject"
                    value="رسالة جديدة من موقع مكافح | New MUKAFIH Website Inquiry">


                <!-- Email template -->

                <input
                    type="hidden"
                    name="_template"
                    value="table">


                <!-- Reply-To -->

                <input
                    type="hidden"
                    name="_replyto"
                    value="">


                <!-- Anti-spam honeypot -->

                <input
                    type="text"
                    name="_honey"
                    class="honeypot"
                    tabindex="-1"
                    autocomplete="off">


                <div class="form-grid">


                    <div class="field">

                        <label
                            for="name"
                            data-ar="الاسم الكامل"
                            data-en="Full Name">

                            الاسم الكامل

                        </label>

                        <input
                            id="name"
                            type="text"
                            name="name"
                            required
                            autocomplete="name"
                            placeholder="الاسم الكامل">

                    </div>


                    <div class="field">

                        <label
                            for="email"
                            data-ar="البريد الإلكتروني"
                            data-en="Email Address">

                            البريد الإلكتروني

                        </label>

                        <input
                            id="email"
                            type="email"
                            name="email"
                            required
                            autocomplete="email"
                            placeholder="name@example.com">

                    </div>


                    <div class="field">

                        <label
                            for="company"
                            data-ar="الشركة / المنشأة"
                            data-en="Company / Facility">

                            الشركة / المنشأة

                        </label>

                        <input
                            id="company"
                            type="text"
                            name="company"
                            autocomplete="organization"
                            placeholder="اسم الشركة">

                    </div>


                    <div class="field">

                        <label
                            for="sector"
                            data-ar="القطاع"
                            data-en="Sector">

                            القطاع

                        </label>

                        <select
                            id="sector"
                            name="sector">

                            <option
                                value=""
                                data-ar="اختر القطاع"
                                data-en="Select sector">
                                اختر القطاع
                            </option>

                            <option
                                value="Factories"
                                data-ar="المصانع"
                                data-en="Factories">
                                المصانع
                            </option>

                            <option
                                value="Warehouses"
                                data-ar="المستودعات"
                                data-en="Warehouses">
                                المستودعات
                            </option>

                            <option
                                value="Data Centers"
                                data-ar="مراكز البيانات"
                                data-en="Data Centers">
                                مراكز البيانات
                            </option>

                            <option
                                value="Electrical Facilities"
                                data-ar="الكهرباء والمحطات"
                                data-en="Electrical Facilities">
                                الكهرباء والمحطات
                            </option>

                            <option
                                value="Other"
                                data-ar="أخرى"
                                data-en="Other">
                                أخرى
                            </option>

                        </select>

                    </div>


                    <div class="field full">

                        <label
                            for="message"
                            data-ar="الرسالة"
                            data-en="Message">

                            الرسالة

                        </label>

                        <textarea
                            id="message"
                            name="message"
                            required
                            placeholder="اكتب رسالتك هنا..."></textarea>

                    </div>

                </div>


                <button
                    id="submitButton"
                    class="form-submit"
                    type="submit"
                    data-ar="إرسال الرسالة"
                    data-en="Send Message">

                    إرسال الرسالة

                </button>


                <div
                    id="formMessage"
                    class="form-message"
                    role="status"
                    aria-live="polite">
                </div>

            </form>

        </div>

    </div>

</section>

</main>


<!-- =========================================================
     FOOTER
========================================================= -->

<footer>

    <div class="container">

        <div class="footer-top">

            <div class="footer-brand">

                <img
                    src="assets/mukafih-logo.png"
                    alt="MUKAFIH">

                <div>

                    <strong>
                        مكافح MUKAFIH
                    </strong>

                    <span>
                        FIRE PROTECTION TECHNOLOGY
                    </span>

                </div>

            </div>


            <div class="socials">

                <a
                    class="social"
                    href="https://x.com/muk_fh?s=21"
                    target="_blank"
                    rel="noopener noreferrer"
                    aria-label="X">
                    X
                </a>

                <a
                    class="social"
                    href="https://www.instagram.com/muk.fh/"
                    target="_blank"
                    rel="noopener noreferrer"
                    aria-label="Instagram">
                    IG
                </a>

                <a
                    class="social"
                    href="https://www.linkedin.com/company/mokfeh/"
                    target="_blank"
                    rel="noopener noreferrer"
                    aria-label="LinkedIn">
                    in
                </a>

                <a
                    class="social"
                    href="https://www.tiktok.com/@muk.fh"
                    target="_blank"
                    rel="noopener noreferrer"
                    aria-label="TikTok">
                    TT
                </a>

            </div>

        </div>


        <div class="footer-bottom">

            <span
                data-ar="© 2026 مكافح. جميع الحقوق محفوظة."
                data-en="© 2026 MUKAFIH. All Rights Reserved.">

                © 2026 مكافح. جميع الحقوق محفوظة.

            </span>


            <span>
                Saudi Arabia
            </span>

        </div>

    </div>

</footer>


<!-- BACK TO TOP -->

<button
    class="top-btn"
    id="topButton"
    type="button"
    aria-label="Back to top">

    ↑

</button>


<script>

    /* =========================================================
       LANGUAGE SYSTEM
    ========================================================= */

    let currentLanguage = "ar";

    const languageButton =
        document.getElementById("languageButton");


    function updateLanguage(language) {

        currentLanguage = language;

        document.documentElement.lang =
            language;

        document.documentElement.dir =
            language === "ar"
                ? "rtl"
                : "ltr";


        document
            .querySelectorAll("[data-ar]")
            .forEach(element => {

                const text =
                    element.getAttribute(
                        `data-${language}`
                    );

                if (!text) return;


                if (
                    element.tagName === "INPUT" ||
                    element.tagName === "TEXTAREA"
                ) {

                    element.placeholder =
                        text;

                } else if (
                    element.tagName === "OPTION"
                ) {

                    element.textContent =
                        text;

                } else {

                    element.innerHTML =
                        text;
                }

            });


        languageButton.textContent =
            language === "ar"
                ? "EN"
                : "ع";


        /* Form placeholders */

        const message =
            document.getElementById("message");

        if (message) {

            message.placeholder =
                language === "ar"
                    ? "اكتب رسالتك هنا..."
                    : "Write your message here...";
        }

        const name =
            document.getElementById("name");

        if (name) {

            name.placeholder =
                language === "ar"
                    ? "الاسم الكامل"
                    : "Full name";
        }

        const email =
            document.getElementById("email");

        if (email) {

            email.placeholder =
                "name@example.com";
        }

        const company =
            document.getElementById("company");

        if (company) {

            company.placeholder =
                language === "ar"
                    ? "اسم الشركة"
                    : "Company name";
        }

    }


    languageButton.addEventListener(
        "click",
        () => {

            updateLanguage(
                currentLanguage === "ar"
                    ? "en"
                    : "ar"
            );

        }
    );


    /* =========================================================
       MOBILE MENU
    ========================================================= */

    const menuButton =
        document.getElementById("menuButton");

    const navLinks =
        document.getElementById("navLinks");


    menuButton.addEventListener(
        "click",
        () => {

            navLinks.classList.toggle(
                "active"
            );

        }
    );


    document
        .querySelectorAll(".nav-links a")
        .forEach(link => {

            link.addEventListener(
                "click",
                () => {

                    navLinks.classList.remove(
                        "active"
                    );

                }
            );

        });


    /* =========================================================
       HEADER SCROLL
    ========================================================= */

    const header =
        document.getElementById("header");

    const topButton =
        document.getElementById("topButton");


    window.addEventListener(
        "scroll",
        () => {

            if (window.scrollY > 50) {

                header.classList.add(
                    "scrolled"
                );

            } else {

                header.classList.remove(
                    "scrolled"
                );

            }


            if (window.scrollY > 500) {

                topButton.classList.add(
                    "show"
                );

            } else {

                topButton.classList.remove(
                    "show"
                );

            }

        }
    );


    topButton.addEventListener(
        "click",
        () => {

            window.scrollTo({
                top: 0,
                behavior: "smooth"
            });

        }
    );


    /* =========================================================
       SCROLL REVEAL
    ========================================================= */

    const observer =
        new IntersectionObserver(
            entries => {

                entries.forEach(entry => {

                    if (
                        entry.isIntersecting
                    ) {

                        entry.target.classList.add(
                            "visible"
                        );

                        observer.unobserve(
                            entry.target
                        );

                    }

                });

            },
            {
                threshold: .12
            }
        );


    document
        .querySelectorAll(".reveal")
        .forEach(element => {

            observer.observe(element);

        });


    /* =========================================================
       CONTACT FORM — REAL EMAIL
    ========================================================= */

    const contactForm =
        document.getElementById(
            "contactForm"
        );

    const submitButton =
        document.getElementById(
            "submitButton"
        );

    const formMessage =
        document.getElementById(
            "formMessage"
        );


    contactForm.addEventListener(
        "submit",
        async function(event) {

            event.preventDefault();


            /* Honeypot */

            const honey =
                contactForm.querySelector(
                    '[name="_honey"]'
                );

            if (honey.value) {

                return;
            }


            const email =
                document.getElementById(
                    "email"
                ).value.trim();


            const emailPattern =
                /^[^\s@]+@[^\s@]+\.[^\s@]+$/;


            if (!emailPattern.test(email)) {

                showFormMessage(
                    currentLanguage === "ar"
                        ? "فضلاً أدخل بريدًا إلكترونيًا صحيحًا."
                        : "Please enter a valid email address.",
                    "error"
                );

                return;
            }


            submitButton.disabled =
                true;


            submitButton.textContent =
                currentLanguage === "ar"
                    ? "جاري الإرسال..."
                    : "Sending...";


            formMessage.className =
                "form-message";


            const formData =
                new FormData(
                    contactForm
                );


            /*
             * FormSubmit uses the user's email
             * as Reply-To.
             */

            formData.set(
                "_replyto",
                email
            );


            try {

                const response =
                    await fetch(
                        "https://formsubmit.co/ajax/mkafh2024@gmail.com",
                        {
                            method: "POST",

                            headers: {
                                "Accept":
                                    "application/json"
                            },

                            body: formData
                        }
                    );


                const data =
                    await response.json();


                if (
                    response.ok &&
                    (
                        data.success === true ||
                        data.success === "true"
                    )
                ) {

                    showFormMessage(
                        currentLanguage === "ar"
                            ? "تم إرسال رسالتك بنجاح. شكرًا لتواصلك مع مكافح."
                            : "Your message has been sent successfully. Thank you for contacting MUKAFIH.",
                        "success"
                    );


                    contactForm.reset();


                } else {

                    throw new Error(
                        "Form submission failed"
                    );

                }


            } catch (error) {

                console.error(
                    "Form Error:",
                    error
                );


                showFormMessage(
                    currentLanguage === "ar"
                        ? "تعذر إرسال الرسالة حاليًا. فضلاً حاول مرة أخرى."
                        : "We could not send your message right now. Please try again.",
                    "error"
                );


            } finally {

                submitButton.disabled =
                    false;


                submitButton.textContent =
                    currentLanguage === "ar"
                        ? "إرسال الرسالة"
                        : "Send Message";

            }

        }
    );


    function showFormMessage(
        message,
        type
    ) {

        formMessage.textContent =
            message;

        formMessage.className =
            `form-message ${type}`;

    }


    /* =========================================================
       START IN ARABIC
    ========================================================= */

    updateLanguage("ar");

</script>


</body>

</html>
