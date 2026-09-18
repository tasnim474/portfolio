<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">

    <meta name="viewport"
        content="width=device-width, initial-scale=1.0">

    <title>Tasnim Hasan Seyam | Personal Website</title>

    <meta name="description"
        content="Official personal website of Tasnim Hasan Seyam — profile, skills, projects, certificates, posts and contact information.">

    <meta name="author"
        content="Tasnim Hasan Seyam">

    <meta name="robots"
        content="index, follow">

    <meta property="og:title"
        content="Tasnim Hasan Seyam | Personal Website">

    <meta property="og:description"
        content="Personal website of Tasnim Hasan Seyam.">

    <meta property="og:type"
        content="website">

    <link rel="canonical"
        href="https://tasnim474.github.io/">

    <style>

        /* =========================
           BASIC SETTINGS
        ========================= */

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        html {
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            color: #f8fafc;
            line-height: 1.6;

            background:
                radial-gradient(
                    circle at 20% 10%,
                    rgba(110, 231, 255, 0.13),
                    transparent 30%
                ),

                radial-gradient(
                    circle at 80% 20%,
                    rgba(167, 139, 250, 0.14),
                    transparent 32%
                ),

                linear-gradient(
                    135deg,
                    #050816,
                    #0b1220 55%,
                    #080b15
                );

            min-height: 100vh;
        }

        body::before {

            content: "";

            position: fixed;

            inset: 0;

            pointer-events: none;

            background-image:
                linear-gradient(
                    rgba(255,255,255,0.025) 1px,
                    transparent 1px
                ),

                linear-gradient(
                    90deg,
                    rgba(255,255,255,0.025) 1px,
                    transparent 1px
                );

            background-size: 42px 42px;

            mask-image:
                linear-gradient(
                    to bottom,
                    black,
                    transparent 85%
                );
        }


        /* =========================
           NAVBAR
        ========================= */

        nav {

            position: sticky;

            top: 0;

            z-index: 100;

            background:
                rgba(5, 8, 22, 0.78);

            backdrop-filter: blur(15px);

            border-bottom:
                1px solid
                rgba(255,255,255,0.10);
        }

        .nav {

            max-width: 1100px;

            margin: auto;

            padding:
                15px 22px;

            display: flex;

            justify-content: space-between;

            align-items: center;

            gap: 15px;
        }

        .logo {

            font-weight: 800;

            letter-spacing: 0.3px;

            font-size: 18px;
        }

        .logo span {

            color: #6ee7ff;
        }

        .nav a {

            color: #dce5f5;

            text-decoration: none;

            margin-left: 18px;

            font-size: 14px;

            transition: 0.3s;
        }

        .nav a:hover {

            color: #6ee7ff;
        }


        /* =========================
           HERO
        ========================= */

        .hero {

            max-width: 1100px;

            margin: auto;

            padding:
                95px 22px 75px;

            display: grid;

            grid-template-columns:
                1.35fr 0.65fr;

            gap: 55px;

            align-items: center;
        }

        .badge {

            display: inline-block;

            border:
                1px solid
                rgba(110,231,255,0.30);

            background:
                rgba(110,231,255,0.06);

            color: #6ee7ff;

            padding:
                6px 12px;

            border-radius: 99px;

            font-size: 13px;

            margin-bottom: 18px;
        }

        h1 {

            font-size:
                clamp(42px, 7vw, 78px);

            line-height: 1.02;

            letter-spacing: -3px;
        }

        .gradient {

            background:
                linear-gradient(
                    90deg,
                    #6ee7ff,
                    #a78bfa
                );

            -webkit-background-clip: text;

            background-clip: text;

            color: transparent;
        }

        .hero p {

            color: #aab5c8;

            font-size: 18px;

            max-width: 650px;

            margin:
                22px 0;
        }


        /* =========================
           BUTTONS
        ========================= */

        .btns {

            display: flex;

            gap: 12px;

            flex-wrap: wrap;
        }

        .btn {

            padding:
                11px 18px;

            border-radius: 12px;

            text-decoration: none;

            border:
                1px solid
                rgba(255,255,255,0.11);

            color: white;

            background:
                rgba(255,255,255,0.04);

            transition: 0.3s;
        }

        .btn:hover {

            transform: translateY(-3px);

            border-color:
                rgba(110,231,255,0.5);
        }

        .btn.primary {

            background:
                linear-gradient(
                    90deg,
                    rgba(110,231,255,0.18),
                    rgba(167,139,250,0.18)
                );

            border-color:
                rgba(110,231,255,0.35);
        }


        /* =========================
           PROFILE PHOTO
        ========================= */

        .photo-wrap {

            display: flex;

            justify-content: center;
        }

        .photo {

            width: 270px;

            height: 270px;

            object-fit: cover;

            border-radius: 50%;

            border:
                5px solid
                rgba(255,255,255,0.10);

            box-shadow:
                0 0 70px
                rgba(110,231,255,0.15);

            transition: 0.4s;
        }

        .photo:hover {

            transform:
                scale(1.04);

            box-shadow:
                0 0 90px
                rgba(110,231,255,0.25);
        }


        /* =========================
           SECTIONS
        ========================= */

        section {

            max-width: 1100px;

            margin: auto;

            padding:
                55px 22px;
        }

        .section-title {

            font-size: 30px;

            margin-bottom: 22px;
        }

        .sub {

            color: #aab5c8;

            margin-bottom: 25px;
        }


        /* =========================
           CARDS
        ========================= */

        .grid {

            display: grid;

            grid-template-columns:
                repeat(3, 1fr);

            gap: 18px;
        }

        .card {

            background:
                rgba(15,23,42,0.72);

            border:
                1px solid
                rgba(255,255,255,0.11);

            border-radius: 18px;

            padding: 22px;

            backdrop-filter: blur(10px);

            transition: 0.3s;
        }

        .card:hover {

            transform:
                translateY(-5px);

            border-color:
                rgba(110,231,255,0.25);
        }

        .card h3 {

            margin-bottom: 8px;
        }

        .card p {

            color: #aab5c8;
        }


        /* =========================
           SKILL TAGS
        ========================= */

        .tags {

            display: flex;

            flex-wrap: wrap;

            gap: 9px;

            margin-top: 15px;
        }

        .tag {

            padding:
                6px 10px;

            border-radius: 9px;

            background:
                rgba(110,231,255,0.08);

            border:
                1px solid
                rgba(110,231,255,0.13);

            font-size: 13px;

            color: #d9faff;
        }


        /* =========================
           POSTS
        ========================= */

        .post {

            display: flex;

            flex-direction: column;

            gap: 10px;
        }

        .date {

            font-size: 12px;

            color: #7f8da5;
        }

        .post a {

            color: #6ee7ff;

            text-decoration: none;
        }


        /* =========================
           CONTACT
        ========================= */

        .contact {

            display: grid;

            grid-template-columns:
                1fr 1fr;

            gap: 18px;
        }

        .contact a {

            color: #6ee7ff;

            text-decoration: none;
        }


        /* =========================
           FOOTER
        ========================= */

        footer {

            text-align: center;

            color: #7f8da5;

            padding:
                35px 22px;

            border-top:
                1px solid
                rgba(255,255,255,0.10);

            margin-top: 30px;
        }


        /* =========================
           MOBILE
        ========================= */

        @media(max-width:760px) {

            .hero {

                grid-template-columns: 1fr;

                text-align: center;

                padding-top: 65px;
            }

            .hero p {

                margin-left: auto;

                margin-right: auto;
            }

            .btns {

                justify-content: center;
            }

            .grid {

                grid-template-columns: 1fr;
            }

            .contact {

                grid-template-columns: 1fr;
            }

            .nav {

                flex-direction: column;
            }

            .nav a {

                margin:
                    0 7px;
            }

            .photo {

                width: 220px;

                height: 220px;
            }

            h1 {

                letter-spacing: -2px;
            }
        }

    </style>


    <!-- =========================
         GOOGLE / SEARCH ENGINE DATA
    ========================= -->

    <script type="application/ld+json">

    {
        "@context": "https://schema.org",

        "@type": "Person",

        "name": "Tasnim Hasan Seyam",

        "url":
        "https://tasnim474.github.io/",

        "image":
        "https://tasnim474.github.io/profile.jpg",

        "description":
        "Personal website of Tasnim Hasan Seyam."
    }

    </script>

</head>


<body>


    <!-- =========================
         NAVIGATION
    ========================= -->

    <nav>

        <div class="nav">

            <div class="logo">

                Tasnim
                <span>Hasan Seyam</span>

            </div>


            <div>

                <a href="#about">
                    About
                </a>

                <a href="#skills">
                    Skills
                </a>

                <a href="#projects">
                    Projects
                </a>

                <a href="#posts">
                    Posts
                </a>

                <a href="#contact">
                    Contact
                </a>

            </div>

        </div>

    </nav>



    <!-- =========================
         HERO
    ========================= -->

    <header class="hero">


        <div>

            <div class="badge">

                PERSONAL WEBSITE

            </div>


            <h1>

                Tasnim Hasan

                <br>

                <span class="gradient">
                    Seyam
                </span>

            </h1>


            <p>

                Welcome to my personal space on the web.
                Explore my profile, skills, projects,
                achievements and latest posts.

            </p>


            <div class="btns">

                <a
                    class="btn primary"
                    href="#projects">

                    View My Work

                </a>


                <a
                    class="btn"
                    href="#contact">

                    Contact Me

                </a>

            </div>

        </div>



        <div class="photo-wrap">

            <img
                class="photo"
                src="profile.jpg"
                alt="Tasnim Hasan Seyam">

        </div>


    </header>



    <!-- =========================
         ABOUT
    ========================= -->

    <section id="about">

        <h2 class="section-title">

            About Me

        </h2>


        <p class="sub">

            Welcome to my personal website.

        </p>


        <div class="card">

            <h3>
                Tasnim Hasan Seyam
            </h3>


            <p>

                I am a BSc student interested in
                technology, programming, web development
                and creative digital work.

                This website is my personal portfolio
                and online identity.

            </p>

        </div>

    </section>



    <!-- =========================
         SKILLS
    ========================= -->

    <section id="skills">

        <h2 class="section-title">

            Skills

        </h2>


        <div class="grid">


            <div class="card">

                <h3>
                    Programming
                </h3>

                <p>

                    Learning and practicing programming
                    fundamentals and Java.

                </p>


                <div class="tags">

                    <span class="tag">
                        C/C++
                    </span>

                    <span class="tag">
                        Java
                    </span>

                </div>

            </div>



            <div class="card">

                <h3>
                    Office & Productivity
                </h3>

                <p>

                    Document creation, presentations
                    and everyday productivity work.

                </p>


                <div class="tags">

                    <span class="tag">
                        MS Word
                    </span>

                    <span class="tag">
                        MS Office
                    </span>

                </div>

            </div>



            <div class="card">

                <h3>
                    Web & Creative
                </h3>

                <p>

                    Building personal websites
                    and working on digital content.

                </p>


                <div class="tags">

                    <span class="tag">
                        HTML
                    </span>

                    <span class="tag">
                        CSS
                    </span>

                    <span class="tag">
                        Web Design
                    </span>

                </div>

            </div>


        </div>

    </section>



    <!-- =========================
         PROJECTS
    ========================= -->

    <section id="projects">

        <h2 class="section-title">

            Projects & Achievements

        </h2>


        <p class="sub">

            Add your real projects, certificates
            and achievements here.

        </p>


        <div class="grid">


            <div class="card">

                <h3>
                    Project 01
                </h3>

                <p>

                    Write your project title,
                    description and link here.

                </p>

            </div>



            <div class="card">

                <h3>
                    Certificate 01
                </h3>

                <p>

                    Add certificate name,
                    issuing organization
                    and verification link.

                </p>

            </div>



            <div class="card">

                <h3>
                    Achievement 01
                </h3>

                <p>

                    Add an achievement,
                    competition, event
                    or other work.

                </p>

            </div>


        </div>

    </section>



    <!-- =========================
         POSTS
    ========================= -->

    <section id="posts">

        <h2 class="section-title">

            Latest Posts

        </h2>


        <div class="grid">


            <div class="card post">

                <span class="date">

                    September 2026

                </span>


                <h3>

                    Welcome to my website

                </h3>


                <p>

                    This is my personal website.
                    I will share my work, projects
                    and updates here.

                </p>

            </div>



            <div class="card post">

                <span class="date">

                    Add Date

                </span>


                <h3>

                    Your next post

                </h3>


                <p>

                    Replace this text with your
                    own update, story or
                    project announcement.

                </p>

            </div>


        </div>

    </section>



    <!-- =========================
         CONTACT
    ========================= -->

    <section id="contact">

        <h2 class="section-title">

            Contact

        </h2>


        <div class="contact">


            <div class="card">

                <h3>
                    Email
                </h3>


                <p>

                    <a href="mailto:YOUR_EMAIL@example.com">

                        YOUR_EMAIL@example.com

                    </a>

                </p>

            </div>



            <div class="card">

                <h3>
                    Social
                </h3>


                <p>

                    <a href="#">

                        Facebook

                    </a>

                    &nbsp; · &nbsp;

                    <a href="#">

                        Instagram

                    </a>

                </p>

            </div>


        </div>

    </section>



    <!-- =========================
         FOOTER
    ========================= -->

    <footer>

        © 2026 Tasnim Hasan Seyam
        · Personal Website

    </footer>


</body>

</html>
