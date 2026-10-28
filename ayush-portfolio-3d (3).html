<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Ayush Vishwakarma — Backend &amp; AI/ML Engineer</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@400;500;600;700&family=Inter:wght@400;500;600&family=JetBrains+Mono:wght@400;500;700&display=swap" rel="stylesheet">
<style>
  :root{
    --bg:#060814;
    --bg-elevated:#0b0f1d;
    --bg-card:#0e1324;
    --border:#212a42;
    --border-soft:#1a2138;
    --text:#eef1f8;
    --muted:#8791ab;
    --violet:#8b5cf6;
    --cyan:#00e5ff;
    --violet-dim:rgba(139,92,246,0.18);
    --cyan-dim:rgba(0,229,255,0.18);
    --font-display:'Space Grotesk', sans-serif;
    --font-body:'Inter', sans-serif;
    --font-mono:'JetBrains Mono', monospace;
  }

  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    background:var(--bg);
    color:var(--text);
    font-family:var(--font-body);
    overflow-x:hidden;
    cursor:none;
    line-height:1.6;
  }
  @media (max-width:900px){ body{cursor:auto;} }
  ::selection{background:var(--violet-dim);color:var(--cyan);}
  ::-webkit-scrollbar{width:10px;}
  ::-webkit-scrollbar-track{background:var(--bg);}
  ::-webkit-scrollbar-thumb{background:var(--border);border-radius:6px;}

  /* ---------- loader ---------- */
  #loader{
    position:fixed;inset:0;z-index:9999;
    background:var(--bg);
    display:flex;flex-direction:column;align-items:center;justify-content:center;
    gap:18px;
    transition:opacity 0.7s ease, visibility 0.7s ease;
  }
  #loader.hidden{opacity:0;visibility:hidden;pointer-events:none;}
  .loader-cube-stage{perspective:400px;}
  .loader-cube{
    width:46px;height:46px;position:relative;
    transform-style:preserve-3d;
    animation:cubeSpin 2.2s linear infinite;
  }
  .loader-cube div{
    position:absolute;width:46px;height:46px;
    border:1px solid var(--cyan);
    background:rgba(0,229,255,0.05);
  }
  .loader-cube .f1{transform:translateZ(23px);}
  .loader-cube .f2{transform:rotateY(90deg) translateZ(23px);}
  .loader-cube .f3{transform:rotateY(180deg) translateZ(23px);}
  .loader-cube .f4{transform:rotateY(-90deg) translateZ(23px);}
  .loader-cube .f5{transform:rotateX(90deg) translateZ(23px);}
  .loader-cube .f6{transform:rotateX(-90deg) translateZ(23px);}
  @keyframes cubeSpin{
    0%{transform:rotateX(0) rotateY(0);}
    100%{transform:rotateX(360deg) rotateY(360deg);}
  }
  .loader-mark{font-family:var(--font-mono);font-size:13px;color:var(--muted);letter-spacing:2px;}

  /* ---------- custom cursor ---------- */
  .cursor-dot, .cursor-ring{
    position:fixed;top:0;left:0;pointer-events:none;z-index:9998;
    transform:translate(-50%,-50%);
  }
  .cursor-dot{
    width:6px;height:6px;border-radius:50%;
    background:var(--cyan);
    box-shadow:0 0 10px 3px var(--cyan-dim);
  }
  .cursor-ring{
    width:34px;height:34px;border-radius:50%;
    border:1px solid var(--violet);
    opacity:0.7;
    transition:width 0.2s ease, height 0.2s ease, border-color 0.2s ease;
  }
  .cursor-ring.active{width:56px;height:56px;border-color:var(--cyan);}
  @media (max-width:900px){ .cursor-dot,.cursor-ring{display:none;} }

  /* ---------- background layers ---------- */
  #network-canvas{position:fixed;inset:0;z-index:0;opacity:0.45;}
  .bg-orb{
    position:fixed;border-radius:50%;filter:blur(90px);z-index:0;pointer-events:none;
  }
  .orb-1{width:480px;height:480px;background:radial-gradient(circle, var(--violet-dim), transparent 70%);top:-120px;left:-100px;}
  .orb-2{width:520px;height:520px;background:radial-gradient(circle, var(--cyan-dim), transparent 70%);bottom:-160px;right:-140px;}

  .shape-field{position:fixed;inset:0;z-index:0;pointer-events:none;perspective:900px;overflow:hidden;}
  .drift-shape{
    position:absolute;
    border:1px solid var(--border-soft);
    transform-style:preserve-3d;
    opacity:0.5;
  }
  .drift-shape.cube{width:60px;height:60px;}
  .drift-shape.cube div{position:absolute;width:60px;height:60px;border:1px solid rgba(0,229,255,0.25);}
  .drift-shape.cube .a{transform:translateZ(30px);}
  .drift-shape.cube .b{transform:rotateY(90deg) translateZ(30px);}
  .drift-shape.cube .c{transform:rotateX(90deg) translateZ(30px);}
  .drift-shape.ring{
    width:90px;height:90px;border-radius:50%;
    border:1px solid rgba(139,92,246,0.3);
  }
  .d1{top:14%;left:8%;animation:driftA 22s ease-in-out infinite;}
  .d2{top:60%;left:85%;animation:driftB 26s ease-in-out infinite;}
  .d3{top:78%;left:12%;animation:driftA 30s ease-in-out infinite reverse;}
  .d4{top:22%;left:78%;animation:driftB 18s ease-in-out infinite;}
  @keyframes driftA{
    0%,100%{transform:translate(0,0) rotateX(10deg) rotateY(0deg);}
    50%{transform:translate(20px,-30px) rotateX(60deg) rotateY(180deg);}
  }
  @keyframes driftB{
    0%,100%{transform:translate(0,0) rotateX(0deg) rotateY(20deg);}
    50%{transform:translate(-25px,25px) rotateX(-180deg) rotateY(-40deg);}
  }
  @media (max-width:700px){ .shape-field{display:none;} }

  /* ---------- layout ---------- */
  .wrap{max-width:1120px;margin:0 auto;padding:0 32px;position:relative;z-index:2;}
  section{position:relative;z-index:2;padding:120px 0;}
  @media (max-width:700px){ section{padding:80px 0;} .wrap{padding:0 20px;} }

  .eyebrow{
    font-family:var(--font-mono);font-size:12px;letter-spacing:3px;text-transform:uppercase;
    color:var(--cyan);display:flex;align-items:center;gap:10px;margin-bottom:18px;
  }
  .eyebrow::before{content:'';width:22px;height:1px;background:var(--cyan);}

  h2.section-title{
    font-family:var(--font-display);font-size:clamp(28px,4vw,42px);font-weight:600;
    letter-spacing:-0.5px;margin-bottom:48px;
  }

  .reveal{opacity:0;transition:opacity 0.9s cubic-bezier(.2,.7,.2,1), transform 0.9s cubic-bezier(.2,.7,.2,1);}
  .reveal.up{transform:translateY(40px);}
  .reveal.left{transform:translateX(-50px);}
  .reveal.right{transform:translateX(50px);}
  .reveal.in{opacity:1;transform:translate(0,0);}

  /* ---------- nav ---------- */
  header{
    position:fixed;top:0;left:0;right:0;z-index:100;
    backdrop-filter:blur(12px);background:rgba(6,8,20,0.65);
    border-bottom:1px solid var(--border-soft);
  }
  nav{max-width:1120px;margin:0 auto;padding:18px 32px;display:flex;align-items:center;justify-content:space-between;}
  .logo{font-family:var(--font-mono);font-size:15px;letter-spacing:1px;}
  .logo span{color:var(--cyan);}
  .nav-links{display:flex;gap:32px;list-style:none;}
  .nav-links a{font-family:var(--font-mono);font-size:13px;color:var(--muted);text-decoration:none;letter-spacing:0.5px;transition:color 0.25s ease;}
  .nav-links a:hover{color:var(--cyan);}
  @media (max-width:700px){ .nav-links{display:none;} }

  /* ---------- hero ---------- */
  .hero{min-height:100vh;display:flex;align-items:center;padding-top:80px;}
  .hero-grid{display:grid;grid-template-columns:1.15fr 0.85fr;gap:40px;align-items:center;width:100%;}
  @media (max-width:900px){ .hero-grid{grid-template-columns:1fr;text-align:center;} }

  .hero-name{
    font-family:var(--font-display);font-size:clamp(38px,6.5vw,72px);font-weight:700;line-height:1.05;letter-spacing:-1.5px;
    background:linear-gradient(100deg,#eef1f8 15%, var(--cyan) 45%, var(--violet) 65%, #eef1f8 85%);
    background-size:250% auto;-webkit-background-clip:text;background-clip:text;color:transparent;
    animation:shimmer 6s linear infinite;
  }
  @keyframes shimmer{0%{background-position:0% 50%;}100%{background-position:250% 50%;}}

  .hero-role{font-family:var(--font-mono);color:var(--muted);font-size:clamp(14px,2vw,17px);margin-top:18px;min-height:24px;}
  .hero-role .caret{display:inline-block;width:8px;height:16px;background:var(--cyan);margin-left:2px;vertical-align:middle;animation:blink 1s step-start infinite;}
  @keyframes blink{50%{opacity:0;}}

  .hero-desc{margin-top:26px;max-width:520px;color:var(--muted);font-size:16px;}
  @media (max-width:900px){ .hero-desc{margin:26px auto 0;} }
  .hero-cta{margin-top:36px;display:flex;gap:16px;}
  @media (max-width:900px){ .hero-cta{justify-content:center;} }

  .btn{
    font-family:var(--font-mono);font-size:13px;letter-spacing:0.5px;padding:14px 26px;border-radius:6px;
    text-decoration:none;display:inline-flex;align-items:center;gap:8px;
    transition:transform 0.25s ease, box-shadow 0.25s ease;
  }
  .btn-primary{background:linear-gradient(120deg,var(--cyan),var(--violet));color:#04060f;font-weight:700;}
  .btn-primary:hover{transform:translateY(-3px);box-shadow:0 10px 34px -8px var(--cyan-dim);}
  .btn-outline{border:1px solid var(--border);color:var(--text);}
  .btn-outline:hover{border-color:var(--cyan);color:var(--cyan);transform:translateY(-3px);}

  /* ---------- 3D tilt ID badge ---------- */
  .badge-stage{perspective:1200px;display:flex;align-items:center;justify-content:center;height:380px;}
  .id-badge{
    width:270px;height:340px;border-radius:20px;position:relative;
    background:linear-gradient(160deg, rgba(139,92,246,0.14), rgba(0,229,255,0.08));
    border:1px solid var(--border);
    backdrop-filter:blur(6px);
    transform-style:preserve-3d;
    transition:transform 0.12s ease-out;
    box-shadow:0 40px 80px -30px rgba(0,0,0,0.7);
    padding:26px;
    display:flex;flex-direction:column;justify-content:space-between;
  }
  .id-badge::before{
    content:'';position:absolute;inset:0;border-radius:20px;
    background:linear-gradient(120deg, transparent 30%, rgba(255,255,255,0.06) 50%, transparent 70%);
    background-size:200% 200%;
    animation:sheen 5s ease-in-out infinite;
    pointer-events:none;
  }
  @keyframes sheen{
    0%,100%{background-position:200% 200%;}
    50%{background-position:0% 0%;}
  }
  .id-top{display:flex;justify-content:space-between;align-items:center;font-family:var(--font-mono);font-size:10px;color:var(--muted);letter-spacing:1.5px;}
  .id-dot{width:8px;height:8px;border-radius:50%;background:var(--cyan);box-shadow:0 0 10px 3px var(--cyan-dim);animation:pulseDot 2s ease-in-out infinite;}
  @keyframes pulseDot{0%,100%{opacity:1;}50%{opacity:0.4;}}
  .id-avatar{
    width:110px;height:110px;border-radius:50%;margin:14px auto;
    background:linear-gradient(145deg, var(--bg-card), var(--bg-elevated));
    border:1px solid var(--border);
    display:flex;align-items:center;justify-content:center;
    font-family:var(--font-display);font-size:36px;font-weight:700;color:var(--cyan);
    transform:translateZ(30px);
    box-shadow:0 0 40px -6px var(--cyan-dim);
  }
  .id-name{font-family:var(--font-display);font-size:19px;text-align:center;transform:translateZ(20px);}
  .id-role{font-family:var(--font-mono);font-size:11px;color:var(--muted);text-align:center;margin-top:4px;transform:translateZ(20px);}
  .id-bar{height:1px;background:var(--border-soft);margin:16px 0;}
  .id-stats{display:flex;justify-content:space-between;font-family:var(--font-mono);font-size:11px;color:var(--muted);transform:translateZ(15px);}
  .id-stats b{color:var(--cyan);display:block;font-size:15px;font-family:var(--font-display);}
  @media (max-width:900px){ .badge-stage{height:320px;} }

  /* ---------- about ---------- */
  .about-grid{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center;}
  @media (max-width:900px){ .about-grid{grid-template-columns:1fr;} }
  .about-text p{color:var(--muted);margin-bottom:16px;font-size:16px;}
  .about-text strong{color:var(--text);}

  .card-3d-stage{perspective:1000px;display:flex;justify-content:center;}
  .card-3d{
    width:280px;height:340px;
    background:linear-gradient(160deg, var(--bg-card), var(--bg-elevated));
    border:1px solid var(--border);border-radius:16px;padding:28px;
    display:flex;flex-direction:column;justify-content:space-between;
    box-shadow:0 30px 60px -20px rgba(0,0,0,0.6);
    animation:float3d 8s ease-in-out infinite;
    transform-style:preserve-3d;
  }
  @keyframes float3d{
    0%{transform:rotateX(6deg) rotateY(-8deg) translateY(0px);}
    25%{transform:rotateX(-4deg) rotateY(6deg) translateY(-10px);}
    50%{transform:rotateX(6deg) rotateY(10deg) translateY(0px);}
    75%{transform:rotateX(-6deg) rotateY(-6deg) translateY(10px);}
    100%{transform:rotateX(6deg) rotateY(-8deg) translateY(0px);}
  }
  .card-3d .tag{font-family:var(--font-mono);font-size:11px;color:var(--violet);letter-spacing:2px;}
  .card-3d .stat{font-family:var(--font-display);font-size:40px;font-weight:700;color:var(--text);}
  .card-3d .stat-label{color:var(--muted);font-size:13px;}
  .card-3d .row{display:flex;justify-content:space-between;font-family:var(--font-mono);font-size:12px;color:var(--muted);}
  .card-3d .row span:last-child{color:var(--cyan);}

  .extra-tags{display:flex;flex-wrap:wrap;gap:10px;margin-top:20px;}
  .extra-tags span{font-family:var(--font-mono);font-size:12px;color:var(--muted);border:1px solid var(--border);padding:6px 14px;border-radius:20px;}

  /* ---------- skills ---------- */
  .skills-list{display:flex;flex-direction:column;gap:22px;max-width:640px;}
  .skill-row .label{display:flex;justify-content:space-between;font-family:var(--font-mono);font-size:13px;margin-bottom:8px;color:var(--text);}
  .skill-row .label span:last-child{color:var(--muted);}
  .skill-track{height:6px;background:var(--border);border-radius:4px;overflow:hidden;}
  .skill-fill{height:100%;width:0%;border-radius:4px;background:linear-gradient(90deg, var(--cyan), var(--violet));transition:width 1.4s cubic-bezier(.2,.8,.2,1);}

  /* ---------- marquee ---------- */
  .marquee-section{padding:60px 0;border-top:1px solid var(--border-soft);border-bottom:1px solid var(--border-soft);background:var(--bg-elevated);overflow:hidden;}
  .marquee-track{display:flex;width:max-content;animation:marquee 22s linear infinite;}
  .marquee-track span{font-family:var(--font-display);font-size:28px;font-weight:600;color:var(--muted);padding:0 40px;white-space:nowrap;display:flex;align-items:center;gap:40px;}
  .marquee-track span::after{content:'◆';color:var(--cyan);font-size:14px;}
  @keyframes marquee{0%{transform:translateX(0);}100%{transform:translateX(-50%);}}

  /* ---------- projects — 3D flip cards ---------- */
  .projects-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(280px,1fr));gap:28px;}
  .flip-stage{perspective:1400px;height:300px;}
  .flip-card{
    position:relative;width:100%;height:100%;
    transform-style:preserve-3d;
    transition:transform 0.7s cubic-bezier(.2,.8,.2,1);
  }
  .flip-stage:hover .flip-card{transform:rotateY(180deg);}
  .flip-face{
    position:absolute;inset:0;backface-visibility:hidden;
    border-radius:14px;border:1px solid var(--border);
    padding:28px;overflow:hidden;
    display:flex;flex-direction:column;
  }
  .flip-front{
    background:var(--bg-card);justify-content:space-between;
  }
  .flip-front::before{
    content:'';position:absolute;top:0;left:-100%;right:-100%;height:3px;
    background:linear-gradient(90deg, transparent, var(--cyan), var(--violet), transparent);
    transition:left 0.6s ease;
  }
  .flip-stage:hover .flip-front::before{left:0;}
  .flip-back{
    background:linear-gradient(160deg, var(--bg-card), #12183080);
    transform:rotateY(180deg);
    justify-content:center;
  }
  .project-tag{font-family:var(--font-mono);font-size:11px;color:var(--violet);letter-spacing:1.5px;margin-bottom:14px;display:inline-block;}
  .flip-front h3{font-family:var(--font-display);font-size:22px;margin-bottom:auto;}
  .flip-hint{font-family:var(--font-mono);font-size:11px;color:var(--muted);letter-spacing:1px;}
  .flip-back p{color:var(--muted);font-size:14px;margin-bottom:14px;}
  .project-stack{display:flex;flex-wrap:wrap;gap:8px;margin-top:auto;}
  .project-stack span{font-family:var(--font-mono);font-size:11px;color:var(--cyan);border:1px solid var(--cyan-dim);padding:4px 10px;border-radius:20px;}
  @media (max-width:700px){
    .flip-stage{height:auto;perspective:none;}
    .flip-card{transform:none !important;transition:none;position:relative;height:auto;}
    .flip-face{position:relative;backface-visibility:visible;}
    .flip-back{transform:none;margin-top:16px;}
  }

  /* ---------- experience ---------- */
  .exp-item{border-left:2px solid var(--border);padding-left:28px;margin-bottom:36px;position:relative;}
  .exp-item::before{content:'';position:absolute;left:-6px;top:4px;width:10px;height:10px;border-radius:50%;background:var(--cyan);box-shadow:0 0 12px 2px var(--cyan-dim);}
  .exp-item .exp-meta{font-family:var(--font-mono);font-size:12px;color:var(--muted);margin-bottom:6px;}
  .exp-item h3{font-family:var(--font-display);font-size:19px;margin-bottom:8px;}
  .exp-item p{color:var(--muted);font-size:14.5px;}

  /* ---------- contact ---------- */
  .contact-section{text-align:center;}
  .contact-btn-wrap{position:relative;display:inline-flex;align-items:center;justify-content:center;margin-top:20px;}
  .contact-ripple{position:absolute;border-radius:50%;border:1px solid var(--cyan);width:100%;height:100%;opacity:0;animation:rippleGrow 2.4s ease-out infinite;}
  .contact-ripple:nth-child(2){animation-delay:0.8s;}
  .contact-ripple:nth-child(3){animation-delay:1.6s;}
  @keyframes rippleGrow{0%{transform:scale(1);opacity:0.7;}100%{transform:scale(2.4);opacity:0;}}
  .contact-btn{
    position:relative;z-index:2;font-family:var(--font-mono);font-size:15px;font-weight:700;
    background:linear-gradient(120deg,var(--cyan),var(--violet));color:#04060f;
    padding:20px 44px;border-radius:50px;text-decoration:none;
    box-shadow:0 20px 50px -15px var(--cyan-dim);transition:transform 0.3s ease;
  }
  .contact-btn:hover{transform:scale(1.06);}
  .contact-links{margin-top:36px;display:flex;gap:28px;justify-content:center;flex-wrap:wrap;font-family:var(--font-mono);font-size:13px;}
  .contact-links a{color:var(--muted);text-decoration:none;transition:color 0.25s;}
  .contact-links a:hover{color:var(--cyan);}

  footer{text-align:center;padding:36px 0;color:var(--muted);font-family:var(--font-mono);font-size:12px;border-top:1px solid var(--border-soft);}
</style>
</head>
<body>

<div id="loader">
  <div class="loader-cube-stage">
    <div class="loader-cube">
      <div class="f1"></div><div class="f2"></div><div class="f3"></div>
      <div class="f4"></div><div class="f5"></div><div class="f6"></div>
    </div>
  </div>
  <div class="loader-mark">INITIALIZING SYSTEM</div>
</div>

<div class="cursor-dot" id="cursorDot"></div>
<div class="cursor-ring" id="cursorRing"></div>

<canvas id="network-canvas"></canvas>
<div class="bg-orb orb-1"></div>
<div class="bg-orb orb-2"></div>
<div class="shape-field">
  <div class="drift-shape cube d1"><div class="a"></div><div class="b"></div><div class="c"></div></div>
  <div class="drift-shape ring d2"></div>
  <div class="drift-shape cube d3"><div class="a"></div><div class="b"></div><div class="c"></div></div>
  <div class="drift-shape ring d4"></div>
</div>

<header>
  <nav>
    <div class="logo">ayush<span>.dev</span></div>
    <ul class="nav-links">
      <li><a href="#about">about</a></li>
      <li><a href="#skills">skills</a></li>
      <li><a href="#projects">projects</a></li>
      <li><a href="#experience">experience</a></li>
      <li><a href="#contact">contact</a></li>
    </ul>
  </nav>
</header>

<section class="hero">
  <div class="wrap hero-grid">
    <div>
      <div class="eyebrow">AI/ML ENGINEERING STUDENT · BHOPAL, INDIA</div>
      <h1 class="hero-name">Ayush<br>Vishwakarma</h1>
      <div class="hero-role"><span id="typedRole"></span><span class="caret"></span></div>
      <p class="hero-desc">I design and ship backend systems end-to-end — from database schema to cloud deployment — and I'm currently applying that same ownership to AI/ML engineering. B.Tech CS (AI &amp; ML) student at LNCT, Bhopal.</p>
      <div class="hero-cta">
        <a href="#projects" class="btn btn-primary">View Projects</a>
        <a href="#contact" class="btn btn-outline">Get in Touch</a>
      </div>
    </div>
    <div class="badge-stage">
      <div class="id-badge" id="idBadge">
        <div class="id-top"><span>ID · AV-2026</span><span class="id-dot"></span></div>
        <div class="id-avatar">AV</div>
        <div class="id-name">Ayush Vishwakarma</div>
        <div class="id-role">Backend &amp; AI/ML Engineer</div>
        <div class="id-bar"></div>
        <div class="id-stats">
          <div><b>3</b>Projects</div>
          <div><b>2</b>Roles</div>
          <div><b>∞</b>Curiosity</div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="about">
  <div class="wrap about-grid">
    <div class="reveal left">
      <div class="eyebrow">ABOUT</div>
      <h2 class="section-title">Backend systems,<br>owned end to end.</h2>
      <div class="about-text">
        <p>I'm a <strong>Computer Science (AI &amp; ML) student at Lakshmi Narain College of Technology (LNCT), Bhopal</strong>, expected to graduate in 2029. Outside coursework, I run my own projects as a one-person team — architecture, implementation, deployment, and documentation.</p>
        <p>My focus is <strong>backend architecture and database schema design</strong>, built with Python and Node.js and shipped through Docker and CI/CD pipelines. I pair that with <strong>digital content creation</strong> on YouTube and Instagram, where I translate technical ideas into clear, accessible narratives.</p>
        <p>Comfortable working <strong>remote-first</strong>, with async communication and milestone-based delivery as default habits rather than adjustments.</p>
      </div>
      <div class="extra-tags">
        <span>Remote-first</span>
        <span>Async communication</span>
        <span>Full project ownership</span>
      </div>
    </div>
    <div class="reveal right">
      <div class="card-3d-stage">
        <div class="card-3d">
          <div class="tag">STATUS · ONLINE</div>
          <div>
            <div class="stat">3</div>
            <div class="stat-label">independent projects shipped</div>
          </div>
          <div class="row"><span>Runtime</span><span>Python / Node.js</span></div>
          <div class="row"><span>Infra</span><span>Docker · AWS</span></div>
          <div class="row"><span>Mode</span><span>Remote / Async</span></div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="skills">
  <div class="wrap">
    <div class="reveal up">
      <div class="eyebrow">SKILLS</div>
      <h2 class="section-title">What I build with</h2>
    </div>
    <div class="skills-list reveal up">
      <div class="skill-row">
        <div class="label"><span>Python</span><span>90%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="90"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>Node.js</span><span>82%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="82"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>Database Schema Design</span><span>80%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="80"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>Backend Architecture (REST APIs)</span><span>85%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="85"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>C</span><span>68%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="68"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>HTML / CSS</span><span>75%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="75"></div></div>
      </div>
      <div class="skill-row">
        <div class="label"><span>Digital Content Creation</span><span>78%</span></div>
        <div class="skill-track"><div class="skill-fill" data-width="78"></div></div>
      </div>
    </div>
  </div>
</section>

<div class="marquee-section">
  <div class="marquee-track" id="marqueeTrack">
    <span>Full-Stack Development</span>
    <span>Database Architecture</span>
    <span>Digital Content Creation</span>
    <span>Tech Storytelling</span>
    <span>AI/ML Research</span>
    <span>Full-Stack Development</span>
    <span>Database Architecture</span>
    <span>Digital Content Creation</span>
    <span>Tech Storytelling</span>
    <span>AI/ML Research</span>
  </div>
</div>

<section id="projects">
  <div class="wrap">
    <div class="reveal up">
      <div class="eyebrow">PROJECTS</div>
      <h2 class="section-title">Independent builds — hover to flip</h2>
    </div>
    <div class="projects-grid">
      <div class="flip-stage reveal up">
        <div class="flip-card">
          <div class="flip-face flip-front">
            <div>
              <span class="project-tag">INDEPENDENT PROJECT</span>
              <h3>Fleet Management System</h3>
            </div>
            <div class="flip-hint">hover for details →</div>
          </div>
          <div class="flip-face flip-back">
            <p>A Node.js backend and relational database schema managing documentation, fuel tracking, and scheduling for a real-world fleet of 6 vehicles and drivers. Greedy routing logic for driver assignment cut data-retrieval latency for maintenance and operational records.</p>
            <div class="project-stack"><span>Node.js</span><span>SQL</span><span>REST API</span></div>
          </div>
        </div>
      </div>
      <div class="flip-stage reveal up">
        <div class="flip-card">
          <div class="flip-face flip-front">
            <div>
              <span class="project-tag">CONCEPTUAL DESIGN</span>
              <h3>QR-Code Smart Ordering System</h3>
            </div>
            <div class="flip-hint">hover for details →</div>
          </div>
          <div class="flip-face flip-back">
            <p>A conceptual contactless self-ordering and inventory synchronization backend designed for retail shops, mapping QR-driven data flows end to end for real-time inventory updates and checkout accuracy.</p>
            <div class="project-stack"><span>System Design</span><span>REST API</span><span>Retail Tech</span></div>
          </div>
        </div>
      </div>
      <div class="flip-stage reveal up">
        <div class="flip-card">
          <div class="flip-face flip-front">
            <div>
              <span class="project-tag">INDEPENDENT PROJECT</span>
              <h3>AI-Powered Document Analyzer API</h3>
            </div>
            <div class="flip-hint">hover for details →</div>
          </div>
          <div class="flip-face flip-back">
            <p>A scalable RESTful API for document processing and NLP-based summarization, built with Python and FastAPI, containerized with Docker and deployed on AWS. CI/CD via GitHub Actions streamlined remote-first delivery.</p>
            <div class="project-stack"><span>Python</span><span>FastAPI</span><span>Docker</span><span>AWS</span></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>

<section id="experience">
  <div class="wrap">
    <div class="reveal up">
      <div class="eyebrow">EXPERIENCE</div>
      <h2 class="section-title">Where I've worked</h2>
    </div>
    <div class="reveal up">
      <div class="exp-item">
        <div class="exp-meta">NOV 2025 – PRESENT · REMOTE</div>
        <h3>Technical Project Lead — Self-Managed Ventures</h3>
        <p>Architected multiple web, backend, and AI application workflows end to end, including system design for fleet tracking and resource management applications, owning architecture, implementation, and deployment under fixed deadlines.</p>
      </div>
      <div class="exp-item">
        <div class="exp-meta">JAN 2026 – PRESENT · REMOTE</div>
        <h3>Digital Content Creator — YouTube &amp; Instagram</h3>
        <p>Produce technical and lifestyle content, translating complex ideas into accessible short-form narratives and growing engagement through structured scripting and consistent publishing.</p>
      </div>
    </div>
  </div>
</section>

<section id="contact" class="contact-section">
  <div class="wrap">
    <div class="reveal up">
      <div class="eyebrow" style="justify-content:center;">CONTACT</div>
      <h2 class="section-title">Let's build something.</h2>
      <p style="color:var(--muted);max-width:480px;margin:0 auto 10px;">Open to remote entry-level Backend or AI/ML Software Engineering roles and internships.</p>
      <div class="contact-btn-wrap">
        <div class="contact-ripple"></div>
        <div class="contact-ripple"></div>
        <div class="contact-ripple"></div>
        <a href="mailto:ayushvishwakarma192168@gmail.com" class="contact-btn">Say Hello →</a>
      </div>
      <div class="contact-links">
        <a href="mailto:ayushvishwakarma192168@gmail.com">ayushvishwakarma192168@gmail.com</a>
        <a href="tel:+919753622969">+91 9753622969</a>
        <a href="https://linkedin.com/in/ayushvishwakarma-tech" target="_blank" rel="noopener">linkedin.com/in/ayushvishwakarma-tech</a>
        <a href="https://github.com/ayushmrs" target="_blank" rel="noopener">github.com/ayushmrs</a>
      </div>
    </div>
  </div>
</section>

<footer>
  © 2026 Ayush Vishwakarma · Built with HTML, CSS &amp; vanilla JS
</footer>

<script>
window.addEventListener('load', () => {
  const loader = document.getElementById('loader');
  setTimeout(() => loader.classList.add('hidden'), 500);
});

const dot = document.getElementById('cursorDot');
const ring = document.getElementById('cursorRing');
let mouseX = 0, mouseY = 0, ringX = 0, ringY = 0;

if (window.matchMedia('(hover: hover)').matches) {
  document.addEventListener('mousemove', (e) => {
    mouseX = e.clientX; mouseY = e.clientY;
    dot.style.left = mouseX + 'px';
    dot.style.top = mouseY + 'px';
  });
  function animateRing(){
    ringX += (mouseX - ringX) * 0.18;
    ringY += (mouseY - ringY) * 0.18;
    ring.style.left = ringX + 'px';
    ring.style.top = ringY + 'px';
    requestAnimationFrame(animateRing);
  }
  animateRing();
  document.querySelectorAll('a, button, .flip-stage, .skill-row').forEach(el => {
    el.addEventListener('mouseenter', () => ring.classList.add('active'));
    el.addEventListener('mouseleave', () => ring.classList.remove('active'));
  });
}

// ---------- 3D tilt badge ----------
const badgeStage = document.querySelector('.badge-stage');
const idBadge = document.getElementById('idBadge');
if(badgeStage){
  badgeStage.addEventListener('mousemove', (e) => {
    const rect = badgeStage.getBoundingClientRect();
    const px = (e.clientX - rect.left) / rect.width - 0.5;
    const py = (e.clientY - rect.top) / rect.height - 0.5;
    idBadge.style.transform = `rotateY(${px*24}deg) rotateX(${-py*24}deg)`;
  });
  badgeStage.addEventListener('mouseleave', () => {
    idBadge.style.transform = 'rotateY(0deg) rotateX(0deg)';
  });
}

// ---------- typewriter roles ----------
const roles = ['Backend Engineer', 'AI/ML Student', 'Systems Architect', 'Full-Stack Developer'];
const typedEl = document.getElementById('typedRole');
let roleIndex = 0, charIndex = 0, deleting = false;
function typeLoop(){
  const current = roles[roleIndex];
  if(!deleting){
    charIndex++;
    typedEl.textContent = current.slice(0, charIndex);
    if(charIndex === current.length){ deleting = true; setTimeout(typeLoop, 1400); return; }
  } else {
    charIndex--;
    typedEl.textContent = current.slice(0, charIndex);
    if(charIndex === 0){ deleting = false; roleIndex = (roleIndex + 1) % roles.length; }
  }
  setTimeout(typeLoop, deleting ? 40 : 80);
}
typeLoop();

// ---------- particle network canvas ----------
const canvas = document.getElementById('network-canvas');
const ctx = canvas.getContext('2d');
let w, h, particles = [];
const PARTICLE_COUNT = 70;
let mouse = { x: null, y: null };
function resizeCanvas(){ w = canvas.width = window.innerWidth; h = canvas.height = window.innerHeight; }
resizeCanvas();
window.addEventListener('resize', resizeCanvas);
window.addEventListener('mousemove', (e) => { mouse.x = e.clientX; mouse.y = e.clientY; });
window.addEventListener('mouseout', () => { mouse.x = null; mouse.y = null; });
function initParticles(){
  particles = [];
  for(let i=0;i<PARTICLE_COUNT;i++){
    particles.push({ x: Math.random()*w, y: Math.random()*h, vx: (Math.random()-0.5)*0.35, vy: (Math.random()-0.5)*0.35, r: Math.random()*1.6+0.6 });
  }
}
initParticles();
function drawNetwork(){
  ctx.clearRect(0,0,w,h);
  for(let i=0;i<particles.length;i++){
    const p = particles[i];
    p.x += p.vx; p.y += p.vy;
    if(p.x < 0 || p.x > w) p.vx *= -1;
    if(p.y < 0 || p.y > h) p.vy *= -1;
    if(mouse.x !== null){
      const dx = p.x - mouse.x, dy = p.y - mouse.y;
      const dist = Math.sqrt(dx*dx+dy*dy);
      if(dist < 140){ p.x += dx/dist*0.6; p.y += dy/dist*0.6; }
    }
    ctx.beginPath();
    ctx.arc(p.x, p.y, p.r, 0, Math.PI*2);
    ctx.fillStyle = 'rgba(0,229,255,0.5)';
    ctx.fill();
  }
  for(let i=0;i<particles.length;i++){
    for(let j=i+1;j<particles.length;j++){
      const dx = particles[i].x - particles[j].x;
      const dy = particles[i].y - particles[j].y;
      const dist = Math.sqrt(dx*dx+dy*dy);
      if(dist < 130){
        ctx.beginPath();
        ctx.strokeStyle = 'rgba(135,145,171,' + (1 - dist/130)*0.3 + ')';
        ctx.lineWidth = 1;
        ctx.moveTo(particles[i].x, particles[i].y);
        ctx.lineTo(particles[j].x, particles[j].y);
        ctx.stroke();
      }
    }
  }
  requestAnimationFrame(drawNetwork);
}
drawNetwork();

// ---------- scroll reveal ----------
const revealEls = document.querySelectorAll('.reveal');
const io = new IntersectionObserver((entries) => {
  entries.forEach(entry => { if(entry.isIntersecting){ entry.target.classList.add('in'); } });
}, { threshold: 0.15 });
revealEls.forEach(el => io.observe(el));

// ---------- animated skill bars ----------
const skillFills = document.querySelectorAll('.skill-fill');
const skillIO = new IntersectionObserver((entries) => {
  entries.forEach(entry => {
    if(entry.isIntersecting){
      const el = entry.target;
      el.style.width = el.dataset.width + '%';
      skillIO.unobserve(el);
    }
  });
}, { threshold: 0.4 });
skillFills.forEach(el => skillIO.observe(el));
</script>

</body>
</html>
