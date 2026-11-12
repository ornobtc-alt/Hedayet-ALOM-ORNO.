
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#050912">

<title>INFINIX IT | Official Website</title>

<meta name="description" content="INFINIX IT - Digital Technology, Social Media Solutions, Web Development, UI/UX Design and Cybersecurity. Founded by Hedayet Alom Orno.">

<style>
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800;900&display=swap');

:root {
    --bg: #050912;
    --panel: #0c1423;
    --cyan: #00e5ff;
    --blue: #3578ff;
    --white: #f5f9ff;
    --muted: #9baabd;
    --border: rgba(0,229,255,.17);
}

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background: var(--bg);
    color: var(--white);
    font-family: 'Inter', sans-serif;
    overflow-x: hidden;
}

a {
    text-decoration: none;
    color: inherit;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: auto;
}

/* BACKGROUND */

body::before {
    content: "";
    position: fixed;
    inset: 0;
    background-image:
    linear-gradient(rgba(0,229,255,.025) 1px, transparent 1px),
    linear-gradient(90deg, rgba(0,229,255,.025) 1px, transparent 1px);
    background-size: 45px 45px;
    pointer-events: none;
    z-index: -1;
}

/* NAVIGATION */

header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
    background: rgba(5,9,18,.88);
    backdrop-filter: blur(18px);
    border-bottom: 1px solid var(--border);
}

.navbar {
    height: 80px;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 25px;
    font-weight: 900;
    letter-spacing: 2px;
    color: var(--cyan);
}

.logo span {
    color: white;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 30px;
}

.nav-links a {
    font-size: 13px;
    color: #c4d1df;
    transition: .3s;
}

.nav-links a:hover {
    color: var(--cyan);
}

.nav-btn {
    border: 1px solid var(--cyan);
    padding: 10px 17px;
    border-radius: 6px;
    color: var(--cyan) !important;
}

.menu-btn {
    display: none;
    color: white;
    font-size: 25px;
    background: none;
    border: none;
}

/* HERO */

.hero {
    min-height: 100vh;
    display: flex;
    align-items: center;
    position: relative;
    padding-top: 80px;
}

.hero-content {
    max-width: 850px;
}

.status {
    display: inline-block;
    border: 1px solid var(--border);
    background: rgba(0,229,255,.06);
    color: var(--cyan);
    padding: 9px 17px;
    border-radius: 30px;
    font-size: 11px;
    letter-spacing: 2px;
    margin-bottom: 30px;
}

.hero h1 {
    font-size: clamp(45px, 8vw, 90px);
    font-weight: 900;
    line-height: 1.08;
    letter-spacing: -3px;
}

.gradient {
    background: linear-gradient(90deg, #00e5ff, #4988ff);
    -webkit-background-clip: text;
    color: transparent;
}

.hero p {
    max-width: 650px;
    margin-top: 25px;
    color: var(--muted);
    line-height: 1.9;
    font-size: 15px;
}

.buttons {
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    margin-top: 35px;
}

.btn {
    display: inline-block;
    padding: 15px 25px;
    border-radius: 7px;
    font-size: 13px;
    font-weight: 800;
    transition: .3s;
}

.btn-primary {
    background: var(--cyan);
    color: #03101a;
}

.btn-secondary {
    border: 1px solid var(--border);
    color: white;
}

.btn:hover {
    transform: translateY(-4px);
    box-shadow: 0 0 25px rgba(0,229,255,.22);
}

.hero-bottom {
    display: flex;
    gap: 45px;
    flex-wrap: wrap;
    margin-top: 65px;
}

.hero-bottom h3 {
    font-size: 16px;
    color: var(--cyan);
}

.hero-bottom p {
    margin-top: 5px;
    font-size: 11px;
}

/* GENERAL SECTIONS */

section {
    padding: 100px 0;
}

.section-title {
    text-align: center;
    margin-bottom: 55px;
}

.section-title small {
    color: var(--cyan);
    letter-spacing: 4px;
    font-size: 11px;
    font-weight: 800;
}

.section-title h2 {
    font-size: clamp(30px, 5vw, 48px);
    margin-top: 13px;
    font-weight: 900;
}

.section-title p {
    color: var(--muted);
    max-width: 650px;
    margin: 15px auto 0;
    line-height: 1.8;
    font-size: 14px;
}

/* ABOUT */

.about-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 55px;
    align-items: center;
}

.about-text h2 {
    font-size: 35px;
    margin-bottom: 12px;
}

.about-text h3 {
    color: var(--cyan);
    font-size: 15px;
    margin-bottom: 22px;
}

.about-text p {
    color: var(--muted);
    font-size: 14px;
    line-height: 2;
    margin-bottom: 15px;
}

.about-panel {
    background: linear-gradient(145deg,#10243a,#09111e);
    border: 1px solid var(--border);
    padding: 40px;
    border-radius: 15px;
    text-align: center;
}

.about-panel .initial {
    font-size: 100px;
    font-weight: 900;
    color: var(--cyan);
    text-shadow: 0 0 35px #00e5ff55;
}

.about-panel h3 {
    font-size: 25px;
    letter-spacing: 3px;
}

.about-panel p {
    color: var(--muted);
    font-size: 12px;
    margin-top: 12px;
}

.skills {
    display: flex;
    flex-wrap: wrap;
    gap: 10px;
    margin-top: 22px;
}

.skill {
    border: 1px solid var(--border);
    background: rgba(0,229,255,.04);
    color: #c4e9f2;
    padding: 9px 13px;
    border-radius: 30px;
    font-size: 11px;
}

/* SERVICES */

.services-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.service-card {
    background: linear-gradient(145deg,#101d2d,#09111c);
    border: 1px solid var(--border);
    border-radius: 13px;
    padding: 30px;
    transition: .35s;
}

.service-card:hover {
    transform: translateY(-8px);
    border-color: var(--cyan);
    box-shadow: 0 10px 35px #00e5ff12;
}

.service-icon {
    font-size: 28px;
    color: var(--cyan);
    margin-bottom: 22px;
}

.service-card h3 {
    font-size: 17px;
    margin-bottom: 12px;
}

.service-card p {
    font-size: 13px;
    line-height: 1.9;
    color: var(--muted);
}

/* FOUNDER */

.founder-section {
    background: linear-gradient(120deg,#091321,#0c1d2c);
    border-top: 1px solid var(--border);
    border-bottom: 1px solid var(--border);
}

.founder-card {
    max-width: 850px;
    margin: auto;
    padding: 45px 30px;
    text-align: center;
    border: 1px solid var(--border);
    border-radius: 18px;
    background: #0a1422;
}

.founder-label {
    color: var(--cyan);
    letter-spacing: 4px;
    font-size: 11px;
    font-weight: 800;
}

.founder-card h2 {
    font-size: clamp(28px,5vw,45px);
    margin: 20px 0 10px;
}

.founder-card h3 {
    color: var(--cyan);
    font-size: 14px;
}

.founder-card p {
    max-width: 600px;
    margin: 20px auto 0;
    color: var(--muted);
    font-size: 14px;
    line-height: 1.9;
}

/* TEAM */

.team-grid {
    display: grid;
    grid-template-columns: repeat(3,1fr);
    gap: 20px;
}

.team-card {
    text-align: center;
    padding: 30px 20px;
    background: var(--panel);
    border: 1px solid var(--border);
    border-radius: 13px;
}

.avatar {
    width: 75px;
    height: 75px;
    display: grid;
    place-items: center;
    margin: 0 auto 20px;
    background: linear-gradient(135deg,#00dfff,#376bff);
    color: #06111c;
    font-size: 28px;
    font-weight: 900;
    border-radius: 50%;
}

.team-card h3 {
    font-size: 17px;
    margin-bottom: 8px;
}

.team-card p {
    color: var(--muted);
    font-size: 12px;
    line-height: 1.8;
}

/* CONTACT */

.contact-box {
    text-align: center;
    padding: 55px 25px;
    border: 1px solid var(--border);
    background: linear-gradient(135deg,#0d2437,#0b1320);
    border-radius: 18px;
}

.contact-box h2 {
    font-size: clamp(28px,5vw,45px);
}

.contact-box p {
    color: var(--muted);
    margin-top: 15px;
    font-size: 14px;
}

.email {
    display: inline-block;
    color: var(--cyan);
    margin-top: 20px;
    font-weight: 700;
    font-size: 16px;
}

/* FOOTER */

footer {
    background: #03060c;
    border-top: 1px solid var(--border);
    padding: 35px 0;
    text-align: center;
}

footer h2 {
    color: var(--cyan);
    letter-spacing: 3px;
    font-size: 20px;
}

footer p {
    color: #75869b;
    font-size: 11px;
    margin-top: 12px;
}

/* ANIMATION */

.reveal {
    animation: reveal 1s ease both;
}

@keyframes reveal {
    from {
        opacity: 0;
        transform: translateY(25px);
    }
    to {
        opacity: 1;
        transform: translateY(0);
    }
}

/* MOBILE */

@media(max-width:850px) {

    .menu-btn {
        display: block;
    }

    .nav-links {
        display: none;
        position: absolute;
        top: 80px;
        left: 0;
        width: 100%;
        background: #091321;
        padding: 25px;
        flex-direction: column;
        border-bottom: 1px solid var(--border);
    }

    .nav-links.active {
        display: flex;
    }

    .about-grid {
        grid-template-columns: 1fr;
    }

    .services-grid {
        grid-template-columns: repeat(2,1fr);
    }

    .team-grid {
        grid-template-columns: 1fr 1fr;
    }
}

@media(max-width:550px) {

    .services-grid,
    .team-grid {
        grid-template-columns: 1fr;
    }

    .hero h1 {
        letter-spacing: -2px;
    }

    .hero-bottom {
        gap: 22px;
    }

    section {
        padding: 70px 0;
    }

    .about-panel {
        padding: 25px;
    }
}

</style>
</head>

<body>

<!-- NAVBAR -->

<header>
<div class="container navbar">

    <a href="#home" class="logo">
        INFINIX <span>IT.</span>
    </a>

    <button class="menu-btn" id="menuBtn">☰</button>

    <nav class="nav-links" id="navLinks">
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#services">Services</a>
        <a href="#founder">Founder</a>
        <a href="#team">Team</a>
        <a href="#contact" class="nav-btn">Contact Us</a>
    </nav>

</div>
</header>

<!-- HERO SECTION -->

<section class="hero" id="home">

<div class="container hero-content reveal">

    <div class="status">
        ● DIGITAL TECHNOLOGY & INNOVATION
    </div>

    <h1>
        WELCOME TO<br>
        <span class="gradient">INFINIX IT.</span>
    </h1>

    <p>
        We create modern digital experiences through
        technology, creativity and innovation.

        From social media solutions to web development,
        UI/UX design and cybersecurity awareness,
        we focus on building a smarter digital future.
    </p>

    <div class="buttons">
        <a href="#services" class="btn btn-primary">
            EXPLORE SERVICES →
        </a>

        <a href="#contact" class="btn btn-secondary">
            CONTACT US
        </a>
    </div>

    <div class="hero-bottom">

        <div>
            <h3>INNOVATION</h3>
            <p>Creative Digital Ideas</p>
        </div>

        <div>
            <h3>TECHNOLOGY</h3>
            <p>Modern Tech Solutions</p>
        </div>

        <div>
            <h3>SECURITY</h3>
            <p>Responsible Digital Security</p>
        </div>

    </div>

</div>
</section>

<!-- ABOUT -->

<section id="about">

<div class="container">

    <div class="section-title">
        <small>WHO WE ARE</small>
        <h2>ABOUT <span class="gradient">ME</span></h2>
        <p>
            The person behind INFINIX IT and the vision
            that drives our digital journey.
        </p>
    </div>

    <div class="about-grid">

        <div class="about-text">

            <h2>Hedayet Alom Orno</h2>

            <h3>Founder & CEO — INFINIX IT</h3>

            <p>
                Hello! I am Hedayet Alom Orno,
                Founder and CEO of INFINIX IT.

                I am passionate about digital technology,
                online platforms, creative design,
                software development and cybersecurity.
            </p>

            <p>
                My work and professional interests include
                Facebook services, social media management,
                digital branding, website development,
                UI/UX design, software engineering,
                graphic design and technology projects.
            </p>

            <p>
                I believe in creativity, continuous learning,
                teamwork and responsible technology.
                My vision is to develop innovative digital
                solutions and build a strong technology identity.
            </p>

            <div class="skills">
                <span class="skill">Social Media</span>
                <span class="skill">Web Development</span>
                <span class="skill">UI/UX Design</span>
                <span class="skill">Software</span>
                <span class="skill">Cybersecurity</span>
                <span class="skill">Digital Branding</span>
            </div>

        </div>

        <div class="about-panel">

            <div class="initial">I</div>

            <h3>INFINIX IT</h3>

            <p>
                DIGITAL TECHNOLOGY • INNOVATION • CREATIVITY
            </p>

            <br>

            <h3 style="font-size:17px;color:#00e5ff;">
                FOUNDER & CEO
            </h3>

            <p>Hedayet Alom Orno</p>

        </div>

    </div>

</div>
</section>

<!-- SERVICES -->

<section id="services">

<div class="container">

    <div class="section-title">
        <small>WHAT WE DO</small>
        <h2>OUR <span class="gradient">SERVICES</span></h2>
        <p>
            Professional digital services and
            technology-focused solutions.
        </p>
    </div>

    <div class="services-grid">

        <div class="service-card">
            <div class="service-icon">◈</div>
            <h3>Facebook Services</h3>
            <p>
                Facebook page management, page setup,
                branding, content support and
                platform-related assistance.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">◎</div>
            <h3>Social Media Management</h3>
            <p>
                Social media management, profile
                optimization, digital presence and
                online brand development.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">⌘</div>
            <h3>Web Development</h3>
            <p>
                Modern responsive websites,
                landing pages, frontend development
                and website customization.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">◇</div>
            <h3>UI/UX Design</h3>
            <p>
                Clean interfaces, user experience
                design, website layouts and
                professional digital products.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">⌨</div>
            <h3>Software Engineering</h3>
            <p>
                Software concepts, programming,
                development workflows and
                digital project solutions.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">⌁</div>
            <h3>Cybersecurity</h3>
            <p>
                Cybersecurity awareness,
                ethical hacking education,
                defensive security and
                authorized security testing.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">✦</div>
            <h3>Graphic Design</h3>
            <p>
                Logo design, brand identity,
                social media graphics, banners
                and creative visual content.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">▣</div>
            <h3>Digital Branding</h3>
            <p>
                Online branding, business identity,
                digital marketing concepts
                and brand presentation.
            </p>
        </div>

        <div class="service-card">
            <div class="service-icon">⌬</div>
            <h3>Technology Solutions</h3>
            <p>
                Creative technology ideas,
                digital consultation and
                innovative project development.
            </p>
        </div>

    </div>

</div>
</section>

<!-- FOUNDER -->

<section class="founder-section" id="founder">

<div class="container">

    <div class="section-title">
        <small>LEADERSHIP</small>
        <h2>MEET THE <span class="gradient">FOUNDER</span></h2>
    </div>

    <div class="founder-card">

        <div class="founder-label">
            FOUNDER & CHIEF EXECUTIVE OFFICER
        </div>

        <h2>Hedayet Alom Orno</h2>

        <h3>FOUNDER & CEO OF INFINIX IT</h3>

        <p>
            The founder of INFINIX IT, driven by
            creativity, digital innovation and
            technology.

            Leading the vision of INFINIX IT with
            a focus on digital services, modern
            development, creative solutions and
            responsible technology.
        </p>

    </div>

</div>
</section>

<!-- TEAM -->

<section id="team">

<div class="container">

    <div class="section-title">
        <small>OUR PEOPLE</small>
        <h2>MEET OUR <span class="gradient">TEAM</span></h2>
        <p>
            A collaborative team working together
            towards digital innovation.
        </p>
    </div>

    <div class="team-grid">

        <div class="team-card">

            <div class="avatar">O</div>

            <h3>Hedayet Alom Orno</h3>

            <p>
                Founder & CEO
                <br>
                INFINIX IT
            </p>

        </div>

        <div class="team-card">

            <div class="avatar">02</div>

            <h3>Team Member 02</h3>

            <p>
                Team Member
                <br>
                INFINIX IT
            </p>

        </div>

        <div class="team-card">

            <div class="avatar">03</div>

            <h3>Team Member 03</h3>

            <p>
                Team Member
                <br>
                INFINIX IT
            </p>

        </div>

    </div>

</div>
</section>

<!-- CONTACT -->

<section id="contact">

<div class="container">

    <div class="contact-box">

        <div class="section-title" style="margin-bottom:20px;">

            <small>GET IN TOUCH</small>

            <h2>
                LET'S WORK <span class="gradient">TOGETHER</span>
            </h2>

        </div>

        <p>
            Have a project, business inquiry or collaboration idea?
            Contact INFINIX IT.
        </p>

        <a class="email" href="mailto:ornobtc@gmail.com">
            ornobtc@gmail.com
        </a>

        <br>

        <a href="mailto:ornobtc@gmail.com?subject=INFINIX%20IT%20Business%20Inquiry"
           class="btn btn-primary">
            SEND AN EMAIL →
        </a>

    </div>

</div>
</section>

<!-- FOOTER -->

<footer>

<div class="container">

    <h2>INFINIX IT</h2>

    <p>
        DIGITAL TECHNOLOGY • INNOVATION • SECURITY
    </p>

    <p>
        Founder & CEO: Hedayet Alom Orno
    </p>

    <p>
        Email: ornobtc@gmail.com
    </p>

    <p>
        © <span id="year"></span> INFINIX IT.
        All Rights Reserved.
    </p>

</div>

</footer>

<!-- JAVASCRIPT -->

<script>

const menuBtn = document.getElementById("menuBtn");
const navLinks = document.getElementById("navLinks");

menuBtn.addEventListener("click", function() {

    navLinks.classList.toggle("active");

});

document.querySelectorAll(".nav-links a").forEach(function(link) {

    link.addEventListener("click", function() {
        navLinks.classList.remove("active");
    });

});

document.getElementById("year").textContent =
new Date().getFullYear();

</script>

</body>
</html>
