# Fx
The mujiib  trading hub academy 
<!Doctype html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#211710">
<title>MUJIIB TRADING HUB ACADEMIC</title>

<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700;800&family=Playfair+Display:wght@600;700;800&display=swap" rel="stylesheet">

<style>
:root {
 --dark:#211710;
 --brown:#39271c;
 --gold:#c49a68;
 --gold2:#e0bd91;
 --cream:#f6f0e7;
 --white:#fffdf9;
 --muted:#a99c90;
 --border:rgba(196,154,104,.23);
}

* {
 margin:0;
 padding:0;
 box-sizing:border-box;
}

html {scroll-behavior:smooth;}

body {
 font-family:'DM Sans',sans-serif;
 background:var(--cream);
 color:var(--dark);
 overflow-x:hidden;
}

a {text-decoration:none;color:inherit;}

button {font:inherit;}

.container {
 width:min(1160px,90%);
 margin:auto;
}

.topbar {
 background:#17100c;
 color:#d5c2ad;
 text-align:center;
 padding:9px 15px;
 font-size:11px;
 letter-spacing:1.5px;
}

.topbar span {color:var(--gold2);}

header {
 position:sticky;
 top:0;
 z-index:100;
 background:rgba(33,23,16,.96);
 backdrop-filter:blur(15px);
 border-bottom:1px solid var(--border);
}

.nav {
 min-height:82px;
 display:flex;
 align-items:center;
 justify-content:space-between;
}

.brand {
 display:flex;
 align-items:center;
 gap:12px;
 color:white;
}

.brand img {
 width:52px;
 height:52px;
 object-fit:contain;
 border-radius:50%;
 background:#f6f0e7;
}

.brand-name {
 font-weight:800;
 font-size:15px;
 letter-spacing:.6px;
}

.brand-name small {
 display:block;
 color:var(--gold2);
 font-size:9px;
 letter-spacing:2px;
 margin-top:4px;
}

.nav-links {
 display:flex;
 align-items:center;
 gap:29px;
 color:#e8dfd5;
 font-size:13px;
}

.nav-links a:hover {color:var(--gold2);}

.nav-cta,.primary-btn {
 display:inline-flex;
 align-items:center;
 justify-content:center;
 padding:13px 22px;
 background:var(--gold);
 color:#211710;
 border-radius:5px;
 font-weight:800;
 font-size:12px;
 transition:.3s;
}

.nav-cta:hover,.primary-btn:hover {
 background:var(--gold2);
 transform:translateY(-2px);
}

.menu-btn {
 display:none;
 background:none;
 border:1px solid var(--border);
 color:white;
 padding:9px 13px;
 border-radius:5px;
 font-size:20px;
}

.hero {
 background:
 linear-gradient(90deg,rgba(25,17,12,.98),rgba(35,24,17,.87)),
 url("logo.jpg") center/contain no-repeat,
 var(--dark);
 color:white;
 padding:115px 0 120px;
 position:relative;
 overflow:hidden;
}

.hero:after {
 content:"";
 position:absolute;
 width:430px;
 height:430px;
 border:1px solid rgba(196,154,104,.15);
 border-radius:50%;
 right:-130px;
 top:30px;
 box-shadow:0 0 0 55px rgba(196,154,104,.025),
 0 0 0 110px rgba(196,154,104,.02);
 pointer-events:none;
}

.hero-content {
 max-width:760px;
 position:relative;
 z-index:2;
}

.eyebrow {
 color:var(--gold2);
 font-size:11px;
 font-weight:700;
 letter-spacing:3px;
 text-transform:uppercase;
 margin-bottom:23px;
}

.hero h1 {
 font-family:'Playfair Display',serif;
 font-size:clamp(42px,7vw,75px);
 line-height:1.12;
 font-weight:700;
 margin-bottom:24px;
}

.hero h1 span {color:var(--gold2);}

.hero p {
 max-width:580px;
 color:#d4c9bd;
 line-height:1.9;
 font-size:15px;
 margin-bottom:32px;
}

.hero-buttons {
 display:flex;
 gap:13px;
 flex-wrap:wrap;
}

.secondary-btn {
 padding:13px 22px;
 border:1px solid rgba(255,255,255,.35);
 border-radius:5px;
 font-size:12px;
 font-weight:700;
 color:white;
 transition:.3s;
}

.secondary-btn:hover {
 border-color:var(--gold);
 color:var(--gold2);
}

.hero-note {
 margin-top:35px;
 color:#b6a99d;
 font-size:11px;
 letter-spacing:1px;
}

.hero-note span {color:var(--gold2);}

.stats {
 background:#302117;
 color:white;
}

.stats-grid {
 display:grid;
 grid-template-columns:repeat(3,1fr);
}

.stat {
 padding:27px 15px;
 text-align:center;
 border-right:1px solid var(--border);
}

.stat:last-child {border:0;}

.stat strong {
 display:block;
 color:var(--gold2);
 font-size:20px;
 margin-bottom:5px;
}

.stat small {
 color:#c1b3a6;
 font-size:11px;
 letter-spacing:1px;
}

.section {
 padding:95px 0;
}

.section-heading {
 max-width:650px;
 margin:0 auto 45px;
 text-align:center;
}

.section-heading .eyebrow {
 color:#a57b4e;
}

.section-heading h2 {
 font-family:'Playfair Display',serif;
 font-size:clamp(30px,5vw,43px);
 margin-bottom:13px;
}

.section-heading p {
 color:#817469;
 font-size:14px;
 line-height:1.8;
}

.about-grid {
 display:grid;
 grid-template-columns:1fr 1fr;
 gap:65px;
 align-items:center;
}

.about-visual {
 min-height:350px;
 background:
 linear-gradient(rgba(33,23,16,.73),rgba(33,23,16,.83)),
 url("logo.jpg") center/contain no-repeat,
 #38271d;
 border:1px solid var(--gold);
 border-radius:12px;
 display:flex;
 justify-content:center;
 align-items:center;
 padding:30px;
}

.about-visual img {
 width:180px;
 height:180px;
 object-fit:contain;
 border-radius:50%;
}

.about-text h2 {
 font-family:'Playfair Display',serif;
 font-size:39px;
 margin-bottom:20px;
}

.about-text p {
 color:#75695e;
 line-height:2;
 font-size:14px;
 margin-bottom:15px;
}

.features {
 display:grid;
 grid-template-columns:1fr 1fr;
 gap:15px;
 margin-top:28px;
}

.feature {
 padding:15px;
 background:white;
 border:1px solid #e7dbce;
 border-radius:7px;
 font-size:12px;
 font-weight:700;
}

.feature span {
 color:#a57b4e;
 margin-right:8px;
}

.courses-section {
 background:#eee5d9;
}

.course-grid {
 display:grid;
 grid-template-columns:repeat(2,1fr);
 gap:22px;
}

.course-card {
 background:var(--white);
 border:1px solid #e1d4c5;
 border-radius:10px;
 padding:30px;
 position:relative;
 transition:.3s;
}

.course-card:hover {
 transform:translateY(-6px);
 box-shadow:0 18px 35px rgba(43,28,18,.09);
 border-color:var(--gold);
}

.course-number {
 font-size:11px;
 color:#a17a50;
 font-weight:800;
 letter-spacing:2px;
}

.course-card h3 {
 font-family:'Playfair Display',serif;
 font-size:25px;
 margin:15px 0 10px;
}

.course-card p {
 font-size:13px;
 color:#817469;
 line-height:1.8;
 min-height:48px;
}

.price {
 font-size:34px;
 font-weight:800;
 color:#8c6038;
 margin:22px 0;
}

.price small {
 font-size:12px;
 color:#95887b;
 font-weight:500;
}

.course-card ul {
 list-style:none;
 border-top:1px solid #eee5da;
 padding-top:18px;
 margin-bottom:24px;
}

.course-card li {
 font-size:12px;
 color:#62564b;
 padding:7px 0;
}

.course-card li:before {
 content:"✓";
 color:#a57b4e;
 font-weight:900;
 margin-right:10px;
}

.course-btn {
 display:block;
 text-align:center;
 padding:13px;
 border:1px solid var(--gold);
 border-radius:5px;
 color:#74502f;
 font-size:12px;
 font-weight:800;
 transition:.3s;
}

.course-btn:hover {
 background:var(--brown);
 color:white;
}

.mentor {
 background:var(--dark);
 color:white;
}

.mentor-grid {
 display:grid;
 grid-template-columns:1fr 1fr;
 gap:55px;
 align-items:center;
}

.mentor-image {
 min-height:300px;
 border:1px solid var(--border);
 border-radius:10px;
 display:flex;
 justify-content:center;
 align-items:center;
 background:
 linear-gradient(rgba(33,23,16,.75),rgba(33,23,16,.8)),
 url("logo.jpg") center/contain no-repeat;
}

.mentor-image img {
 width:170px;
 height:170px;
 object-fit:contain;
 background:var(--cream);
 border-radius:50%;
}

.mentor-text h2 {
 font-family:'Playfair Display',serif;
 font-size:40px;
 margin-bottom:18px;
}

.mentor-text p {
 color:#c5b9ad;
 font-size:14px;
 line-height:2;
 margin-bottom:20px;
}

.mentor-label {
 color:var(--gold2);
 font-size:11px;
 letter-spacing:2px;
 text-transform:uppercase;
 margin-bottom:12px;
}

.location {
 background:#eee5d9;
 text-align:center;
}

.location-box {
 max-width:750px;
 margin:auto;
 padding:35px;
 border:1px solid #dfcbb5;
 background:var(--white);
 border-radius:10px;
}

.location-box h3 {
 font-family:'Playfair Display',serif;
 font-size:28px;
 margin-bottom:12px;
}

.location-box p {
 color:#817469;
 font-size:14px;
}

.faq-list {
 max-width:750px;
 margin:auto;
}

details {
 background:white;
 padding:20px 22px;
 margin-bottom:12px;
 border:1px solid #e5d8ca;
 border-radius:7px;
}

summary {
 cursor:pointer;
 font-size:14px;
 font-weight:700;
}

details p {
 color:#817469;
 font-size:13px;
 line-height:1.8;
 padding-top:15px;
}

.contact-section {
 background:var(--brown);
 color:white;
 text-align:center;
 padding:80px 20px;
}

.contact-section h2 {
 font-family:'Playfair Display',serif;
 font-size:clamp(32px,5vw,48px);
 margin-bottom:16px;
}

.contact-section p {
 color:#d3c4b6;
 font-size:14px;
 line-height:1.9;
 max-width:600px;
 margin:0 auto 28px;
}

.contact-info {
 display:flex;
 justify-content:center;
 gap:30px;
 flex-wrap:wrap;
 margin-top:30px;
}

.contact-info a {
 color:var(--gold2);
 font-size:13px;
}

footer {
 background:#17100c;
 color:#b9a99b;
 padding:40px 0 25px;
}

.footer-content {
 display:flex;
 justify-content:space-between;
 gap:30px;
 flex-wrap:wrap;
}

.footer-brand {
 color:white;
 font-weight:800;
 font-size:15px;
}

.footer-brand p {
 color:#9c8c7e;
 font-weight:400;
 font-size:12px;
 margin-top:10px;
}

.footer-links {
 display:flex;
 gap:20px;
 flex-wrap:wrap;
 font-size:12px;
}

.footer-links a:hover {color:var(--gold2);}

.copyright {
 border-top:1px solid var(--border);
 margin-top:30px;
 padding-top:20px;
 text-align:center;
 font-size:11px;
 line-height:1.8;
}

.whatsapp {
 position:fixed;
 bottom:22px;
 right:20px;
 z-index:90;
 background:#247d49;
 color:white;
 padding:14px 19px;
 border-radius:50px;
 font-size:12px;
 font-weight:800;
 box-shadow:0 7px 20px #0003;
}

@media(max-width:850px) {
 .nav-links {
  display:none;
  position:absolute;
  top:82px;
  left:0;
  width:100%;
  background:#211710;
  padding:25px 6%;
  flex-direction:column;
  align-items:flex-start;
  border-top:1px solid var(--border);
 }
 .nav-links.active {display:flex;}
 .menu-btn {display:block;}
 .nav-cta {display:none;}
 .about-grid,.mentor-grid {grid-template-columns:1fr;gap:35px;}
}

@media(max-width:600px) {
 .hero {padding:85px 0;}
 .hero h1 {font-size:43px;}
 .section {padding:70px 0;}
 .course-grid {grid-template-columns:1fr;}
 .stats-grid {grid-template-columns:1fr;}
 .stat {border-right:0;border-bottom:1px solid var(--border);}
 .about-text h2,.mentor-text h2 {font-size:32px;}
 .features {grid-template-columns:1fr;}
 .footer-content {flex-direction:column;}
 .hero-buttons {flex-direction:column;align-items:flex-start;}
 .hero-buttons a {width:100%;text-align:center;}
}
</style>
</head>

<body>

<div class="topbar">
 WELCOME TO <span>MUJIIB TRADING HUB ACADEMIC</span> · ZARIA, NIGERIA
</div>

<header>
<div class="container nav">

<a class="brand" href="#home">
<img src="logo.jpg" alt="MUJIIB Academy logo">
<div class="brand-name">
MUJIIB TRADING HUB
<small>ACADEMIC</small>
</div>
</a>

<nav class="nav-links" id="navLinks">
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#courses">Courses</a>
<a href="#mentor">Mentor</a>
<a href="#contact">Contact</a>
</nav>

<a class="nav-cta" href="#courses">EXPLORE CLASSES ↗</a>

<button class="menu-btn" id="menuBtn" aria-label="Open navigation" aria-expanded="false">☰</button>

</div>
</header>

<main>

<section class="hero" id="home">
<div class="container">
<div class="hero-content">

<div class="eyebrow">WELCOME TO OUR ACADEMY</div>

<h1>
Build Your Knowledge.<br>
Understand The <span>Markets.</span>
</h1>

<p>
Welcome to MUJIIB TRADING HUB ACADEMIC, a trading education academy offering ICT and Smart Money Concepts learning programmes.
Explore our courses and discover the programme that matches your learning goals.
</p>

<div class="hero-buttons">
<a class="primary-btn" href="#courses">EXPLORE OUR COURSES ↗</a>
<a class="secondary-btn" href="#about">DISCOVER OUR ACADEMY</a>
</div>

<div class="hero-note">
<span>ICT EDUCATION</span> &nbsp; · &nbsp;
<span>SMART MONEY CONCEPTS</span> &nbsp; · &nbsp;
<span>ZARIA, NIGERIA</span>
</div>

</div>
</div>
</section>

<div class="stats">
<div class="container stats-grid">
<div class="stat">
<strong>ICT</strong>
<small>TRADING EDUCATION</small>
</div>
<div class="stat">
<strong>SMC</strong>
<small>SMART MONEY CONCEPTS</small>
</div>
<div class="stat">
<strong>bigginer class</strong>
<small>introduction to market</small></div>
  <div class="stat">
    <strong>📍location</strong>
    <small>ZARIA,KADUNA STATE,NIGERIA</small>
  </div>
</div>
</div>
</div>

<section class="section" id="about">
<div class="container about-grid">

<div class="about-visual">
<img src="logo.jpg" alt="MUJIIB Trading Hub official logo">
</div>

<div class="about-text">
<div class="eyebrow">WHO WE ARE</div>
<h2>About Our Academy</h2>

<p>
MUJIIB TRADING HUB ACADEMIC is an educational platform focused on ICT and Smart Money Concepts (SMC).
</p>

<p>
We provide structured learning programmes for students interested in understanding financial markets, trading terminology and market analysis concepts.
</p>

<div class="features">
<div class="feature"><span>✦</span> ICT Classes</div>
<div class="feature"><span>✦</span> SMC Classes</div>
<div class="feature"><span>✦</span> bigginer Classes</div>
<div class="feature"><span>✦</span> Course Enquiries</div>
</div>

</div>
</div>
</section>

<section class="section courses-section" id="courses">
<div class="container">

<div class="section-heading">
<div class="eyebrow">OUR PROGRAMMES</div>
<h2>Explore Our Classes</h2>
<p>Explore the available educational programmes and their respective fees.</p>
</div>

<div class="course-grid">

<div class="course-card">
<div class="course-number">PROGRAMME 01 · ICT</div>
<h3>ICT Trading Class</h3>
<p>An educational programme focused on ICT trading concepts.</p>
<div class="price">₦60,000 <small>/ course</small></div>
<ul>
<li>ICT learning programme</li>
<li>Structured course education</li>
<li>Course registration enquiry</li>
</ul>
<a class="course-btn" href="https://wa.me/2349049959760?text=Hello%2C%20I%20want%20information%20about%20the%20ICT%20class.">ENQUIRE ABOUT ICT ↗</a>
</div>

<div class="course-card">
<div class="course-number">PROGRAMME 02 · bigginers</div>
<h3>Beginners Class</h3>
<p>An introductory learning programme for beginners.</p>
<div class="price">₦20,000 <small>/ course</small></div>
<ul>
<li>Introduction to market</li>
<li>Beginner learning programme</li>
<li>Course registration enquiry</li>
</ul>
<a class="course-btn" href="https://wa.me/2349049959760?text=Hello%2C%20I%20want%20information%20about%20the%20SMC%20Beginners%20class.">ENQUIRE ABOUT COURSE ↗</a>
</div>

<div class="course-card">
<div class="course-number">PROGRAMME 03 · SMC</div>
<h3>Advanced SMC Class</h3>
<p>An advanced educational programme in Smart Money Concepts.</p>
<div class="price">₦30,000 <small>/ course</small></div>
<ul>
<li>Advanced SMC education</li>
<li>Structured learning programme</li>
<li>Course registration enquiry</li>
</ul>
<a class="course-btn" href="https://wa.me/2349049959760?text=Hello%2C%20I%20want%20information%20about%20the%20Advanced%20SMC%20class.">ENQUIRE ABOUT COURSE ↗</a>
</div>

<div class="course-card">
<div class="course-number">PROGRAMME 04 · SMC</div>
<h3>SMC Master Class</h3>
<p>A higher-level SMC educational programme.</p>
<div class="price">₦50,000 <small>/ course</small></div>
<ul>
<li>Master-level SMC education</li>
<li>Structured learning programme</li>
<li>Course registration enquiry</li>
</ul>
<a class="course-btn" href="https://wa.me/2349049959760?text=Hello%2C%20I%20want%20information%20about%20the%20SMC%20Master%20class.">ENQUIRE ABOUT COURSE ↗</a>
</div>
  <div class="course-card">
<div class="course-number">PROGRAMME 02 · 1 in 1</div>
<h3>one in one class</h3>
<p>An introductory learning programme one in one,combine all programmes.</p>
<div class="price">₦70,000 <small>/ course</small></div>
<ul>
<li>Introduction to market</li>
<li>all learning programme</li>
<li>Course registration enquiry</li>
</ul>
<a class="course-btn" href="https://wa.me/2349049959760?text=Hello%2C%20I%20want%20information%20about%20the%20SMC%20Beginners%20class.">ENQUIRE ABOUT COURSE ↗</a>
</div>

</div>
</div>
</section>

<section class="section mentor" id="mentor">
<div class="container mentor-grid">

<div class="mentor-image">
<img src="logo.jpg" alt="Academy logo">
</div>

<div class="mentor-text">
<div class="mentor-label">ACADEMY INSTRUCTOR</div>
<h2>Learn With Sadiq</h2>
<p>
Meet Sadiq, the academy contact and mentor behind MUJIIB TRADING HUB ACADEMIC. Explore the academy's available educational programmes and contact the team for more information about course registration.
</p>
<a class="primary-btn" href="https://www.tiktok.com/@fx_sadeeq_ah">VISIT TIKTOK PROFILE ↗</a>
</div>

</div>
</section>

<section class="section location">
<div class="container">
<div class="location-box">
<div class="eyebrow">FIND OUR ACADEMY</div>
<h3>Zaria, Kaduna State</h3>
<p>Nigeria 🇳🇬</p>
</div>
</div>
</section>

<section class="section">
<div class="container">
<div class="section-heading">
<div class="eyebrow">NEED MORE INFORMATION?</div>
<h2>Frequently Asked Questions</h2>
<p>Some useful information about our educational programmes.</p>
</div>

<div class="faq-list">

<details>
<summary>What courses are available?</summary>
<p>We offer ICT Trading Class and three SMC programmes: Beginners, Advanced and Master Class.</p>
</details>

<details>
<summary>How much does the ICT class cost?</summary>
<p>The listed ICT class fee is ₦60,000.</p>
</details>

<details>
<summary>What are the SMC course fees?</summary>
<p>Beginners: ₦20,000. Advanced: ₦30,000. Master: ₦50,000.</p>
</details>

<details>
<summary>How can I contact the academy?</summary>
<p>You can contact the academy through WhatsApp, phone, email or TikTok.</p>
</details>

</div>
</div>
</section>

<section class="contact-section" id="contact">
<div class="container">

<div class="eyebrow">GET IN TOUCH</div>

<h2>Let's Connect.</h2>

<p>
For course enquiries and further information, contact MUJIIB TRADING HUB ACADEMIC through any of our official communication channels.
</p>

<a class="primary-btn" href="https://wa.me/2349049959760">CONTACT US ON WHATSAPP ↗</a>

<div class="contact-info">
<a href="tel:09049959760">☎ 09049959760</a>
<a href="mailto:Sadiqauwal4537@gmail.com">✉ SEND EMAIL</a>
<a href="https://www.tiktok.com/@fx_sadeeq_ah">♪ TIKTOK PROFILE</a>
</div>

</div>
</section>

</main>

<footer>
<div class="container">

<div class="footer-content">
<div class="footer-brand">
MUJIIB TRADING HUB ACADEMIC
<p>ICT & SMC Trading Education</p>
</div>

<div class="footer-links">
<a href="#home">Home</a>
<a href="#about">About</a>
<a href="#courses">Courses</a>
<a href="#contact">Contact</a>
</div>
</div>

<div class="copyright">
© 2026 MUJIIB TRADING HUB ACADEMIC. All Rights Reserved.
<br>
Educational content only. Trading involves financial risk and no profits are guaranteed.
</div>

</div>
</footer>

<a class="whatsapp" href="https://wa.me/2349049959760">
WhatsApp ↗
</a>

<script>
const menuBtn = document.getElementById("menuBtn");
const navLinks = document.getElementById("navLinks");

menuBtn.addEventListener("click", function(){
 navLinks.classList.toggle("active");
 const opened = navLinks.classList.contains("active");
 menuBtn.setAttribute("aria-expanded", opened);
 menuBtn.textContent = opened ? "✕" : "☰";
});

document.querySelectorAll(".nav-links a").forEach(link=>{
 link.addEventListener("click",()=>{
  navLinks.classList.remove("active");
  menuBtn.setAttribute("aria-expanded","false");
  menuBtn.textContent="☰";
 });
});
</script>

</body>
</html>
