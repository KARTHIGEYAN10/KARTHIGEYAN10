<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Your Name — Portfolio</title>
  <meta name="description" content="Your short bio — Fullstack dev | Java | Python | MERN" />

  <!-- Simple styling, self contained -->
  <style>
    :root{
      --bg:#0f1724; --card:#0b1220; --muted:#9aa4b2; --accent:#06b6d4; --glass: rgba(255,255,255,0.03);
      --radius:12px; --container:1100px;
      font-family: Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
    }
    *{box-sizing:border-box}
    body{
      margin:0; background:linear-gradient(180deg,var(--bg),#071124 85%);
      color:#e6eef6; -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
      padding:48px 16px;
      display:flex; justify-content:center;
    }
    .wrap{max-width:var(--container); width:100%}
    header{display:flex; gap:24px; align-items:center}
    .avatar{
      width:120px; height:120px; border-radius:18px; overflow:hidden;
      box-shadow:0 6px 30px rgba(2,6,23,0.6); border:1px solid rgba(255,255,255,0.04);
      flex:0 0 120px; background:linear-gradient(135deg,#0ea5a5,#6366f1);
      display:flex; align-items:center; justify-content:center; font-weight:700; font-size:28px;
    }
    h1{margin:0; font-size:28px}
    p.lead{margin:6px 0 12px; color:var(--muted)}
    .buttons{display:flex; gap:10px; flex-wrap:wrap}
    .btn{
      background:var(--glass); padding:8px 12px; border-radius:10px; color:inherit; border:1px solid rgba(255,255,255,0.04);
      text-decoration:none; font-weight:600; font-size:14px;
    }
    .grid{
      display:grid; grid-template-columns:1fr 320px; gap:20px; margin-top:28px;
    }
    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01)); padding:18px; border-radius:var(--radius); border:1px solid rgba(255,255,255,0.03)}
    .skills{display:flex; gap:8px; flex-wrap:wrap; margin-top:8px}
    .chip{background:rgba(255,255,255,0.03); padding:6px 10px; border-radius:999px; color:var(--muted); font-weight:600; font-size:13px}
    .projects{display:grid; grid-template-columns:repeat(2,1fr); gap:12px; margin-top:12px}
    .proj{padding:12px; border-radius:10px; background:rgba(255,255,255,0.015); border:1px solid rgba(255,255,255,0.03)}
    .contact{display:flex; gap:10px; margin-top:12px; flex-wrap:wrap}
    footer{margin-top:30px; color:var(--muted); font-size:13px; text-align:center}
    @media (max-width:900px){
      .grid{grid-template-columns:1fr; }
      .projects{grid-template-columns:1fr}
      header{flex-direction:row; gap:12px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="avatar">YK<!-- Replace with <img src="..." /> if you have avatar --></div>
      <div>
        <h1>Your Name <span style="color:var(--muted); font-size:14px; font-weight:600"> — Fullstack Developer</span></h1>
        <p class="lead">I build web apps with Java, Python and the MERN stack. Currently interning at StartupName. Open to internships & graduate roles.</p>
        <div class="buttons">
          <a class="btn" href="https://github.com/yourusername" target="_blank">GitHub</a>
          <a class="btn" href="https://linkedin.com/in/yourprofile" target="_blank">LinkedIn</a>
          <a class="btn" href="mailto:youremail@example.com">Email</a>
          <a class="btn" href="/resume.pdf" target="_blank">Resume</a>
        </div>
      </div>
    </header>

    <div class="grid">
      <!-- Left main column -->
      <div>
        <section class="card">
          <h3>About</h3>
          <p class="lead" style="margin-top:6px; color:var(--muted)">Short intro: 3–4 lines describing what you do, tech + domain interest (e.g., healthcare apps, ML pipelines).</p>
          <div style="margin-top:12px">
            <strong>Top skills</strong>
            <div class="skills">
              <span class="chip">Java</span>
              <span class="chip">Python</span>
              <span class="chip">React</span>
              <span class="chip">Node.js</span>
              <span class="chip">MongoDB</span>
              <span class="chip">SQL</span>
            </div>
          </div>
        </section>

        <section class="card" style="margin-top:12px">
          <h3>Highlighted projects</h3>
          <div class="projects">
            <div class="proj">
              <strong>Project A</strong>
              <p class="lead" style="margin:6px 0 0; color:var(--muted)">Short description (what it does). <a href="#" style="color:var(--accent)">View repo</a></p>
            </div>
            <div class="proj">
              <strong>Project B</strong>
              <p class="lead" style="margin:6px 0 0; color:var(--muted)">Short description. <a href="#" style="color:var(--accent)">View repo</a></p>
            </div>
            <div class="proj">
              <strong>Cloud Kitchen Project</strong>
              <p class="lead" style="margin:6px 0 0; color:var(--muted)">MERN app with cart & purchases. <a href="#" style="color:var(--accent)">Demo</a></p>
            </div>
            <div class="proj">
              <strong>Vehicle Monitor</strong>
              <p class="lead" style="margin:6px 0 0; color:var(--muted)">YOLO + OpenCV classification & counting. <a href="#" style="color:var(--accent)">Repo</a></p>
            </div>
          </div>
        </section>
      </div>

      <!-- Right column (widgets) -->
      <aside>
        <div class="card">
          <h4>GitHub</h4>
          <!-- Replace YOUR_USERNAME in image URLs if you want to show live stats -->
          <img src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=dark" alt="stats" style="width:100%; border-radius:8px; margin-top:8px" />
        </div>

        <div class="card" style="margin-top:12px">
          <h4>Contact</h4>
          <div class="contact">
            <a class="btn" href="mailto:youremail@example.com">Email</a>
            <a class="btn" href="tel:+911234567890">Call</a>
          </div>
          <p class="lead" style="margin-top:8px; color:var(--muted)">Open to internships, remote/joining roles. Preferred timezone: IST (Asia/Kolkata).</p>
        </div>
      </aside>
    </div>

    <footer>
      Built with ❤️ — <strong>Your Name</strong> • <span style="color:var(--muted)">Last updated: <!-- put date --> Sep 2025</span>
    </footer>
  </div>
</body>
</html>

