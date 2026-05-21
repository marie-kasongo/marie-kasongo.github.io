
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Marie Kasongo Portfolio</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, sans-serif;
      background: linear-gradient(to bottom, #fff7fa, #ffffff);
      color: #333;
    }

    nav {
      position: sticky;
      top: 0;
      background: rgba(255,255,255,0.9);
      backdrop-filter: blur(10px);
      border-bottom: 1px solid #ffd6e5;
      padding: 20px 8%;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 100;
    }

    nav h1 {
      color: #ec4899;
      font-size: 28px;
    }

    nav ul {
      display: flex;
      gap: 30px;
      list-style: none;
    }

    nav a {
      text-decoration: none;
      color: #ec4899;
      font-weight: 600;
    }

    .hero {
      padding: 80px 8%;
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 60px;
      align-items: center;
    }

    .hero h2 {
      font-size: 32px;
      margin-bottom: 10px;
    }

    .hero h1 {
      font-size: 72px;
      color: #ec4899;
      margin-bottom: 20px;
      line-height: 1;
    }

    .hero p {
      font-size: 20px;
      color: #666;
      line-height: 1.6;
      margin-bottom: 35px;
    }

    .buttons {
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
    }

    .btn {
      padding: 16px 30px;
      border-radius: 18px;
      border: none;
      font-size: 18px;
      cursor: pointer;
      transition: 0.3s;
    }

    .pink-btn {
      background: #ec4899;
      color: white;
      box-shadow: 0 10px 20px rgba(236,72,153,0.2);
    }

    .pink-btn:hover {
      background: #db2777;
    }

    .outline-btn {
      border: 2px solid #f9a8d4;
      background: white;
      color: #ec4899;
    }

    .outline-btn:hover {
      border-color: #ec4899;
    }

    .hero img {
      width: 100%;
      max-width: 420px;
      border-radius: 35px;
      box-shadow: 0 20px 40px rgba(236,72,153,0.2);
    }

    .sections {
      width: 85%;
      margin: auto;
      padding-bottom: 80px;
    }

    details {
      background: white;
      border-radius: 28px;
      margin-bottom: 25px;
      border: 1px solid #ffe4ef;
      overflow: hidden;
      box-shadow: 0 5px 20px rgba(0,0,0,0.03);
    }

    summary {
      padding: 30px;
      font-size: 30px;
      font-weight: bold;
      color: #ec4899;
      cursor: pointer;
      list-style: none;
    }

    details p,
    details ul,
    .card-container {
      padding: 0 30px 30px 30px;
      color: #666;
      line-height: 1.8;
      font-size: 18px;
    }

    .card-container {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px;
    }

    .card {
      background: #fff0f6;
      padding: 25px;
      border-radius: 22px;
    }

    .card h3 {
      color: #ec4899;
      margin-bottom: 10px;
    }

    .skills {
      display: flex;
      flex-wrap: wrap;
      gap: 15px;
      padding: 0 30px 30px;
    }

    .skill {
      background: #ffe4ef;
      color: #ec4899;
      padding: 12px 18px;
      border-radius: 999px;
      font-weight: 600;
    }

    footer {
      text-align: center;
      padding: 40px;
      border-top: 1px solid #ffd6e5;
      color: #777;
    }

    @media(max-width: 900px) {
      .hero {
        grid-template-columns: 1fr;
        text-align: center;
      }

      .hero h1 {
        font-size: 54px;
      }

      .buttons {
        justify-content: center;
      }

      .hero img {
        margin: auto;
      }

      .card-container {
        grid-template-columns: 1fr;
      }

      nav ul {
        display: none;
      }
    }
  </style>
</head>

<body>

  <nav>
    <h1>Marie Kasongo ✨</h1>

    <ul>
      <li><a href="#about">About</a></li>
      <li><a href="#research">Research</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#resume">Resume</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>

  <section class="hero">

    <div>
      <h2>Hi, I'm</h2>

      <h1>Marie Kasongo</h1>

      <p>
        Biomedical Engineering student at Brown University interested in biomedical imaging, AI in healthcare, computational biology, and translational research.
      </p>

      <div class="buttons">
        <button class="btn pink-btn">View My Work ↓</button>

        <button class="btn outline-btn">
          Download Resume
        </button>
      </div>
    </div>

    <div>
      <img src="https://images.unsplash.com/photo-1494790108377-be9c29b29330?q=80&w=1200&auto=format&fit=crop" />
    </div>

  </section>

  <section class="sections">

    <details id="about">
      <summary>💗 About Me</summary>

      <p>
        I am a Biomedical Engineering student passionate about biomedical imaging, cancer research, computational biology, and AI applications in healthcare.
      </p>
    </details>

    <details id="research">
      <summary>🧪 Research Experience</summary>

      <p>
        Research involving circulating tumor cell morphology analysis using CellProfiler, Cellpose, PCA analysis, and fluorescence imaging workflows.
      </p>
    </details>

    <details id="projects">
      <summary>💻 Featured Projects</summary>

      <div class="card-container">

        <div class="card">
          <h3>CTC Morphology Analysis</h3>

          <p>
            Research project investigating how extracellular matrix stiffness affects circulating tumor cell morphology.
          </p>
        </div>

        <div class="card">
          <h3>MATLAB Mass Launcher</h3>

          <p>
            Engineering simulation project involving ODE solving and projectile motion modeling.
          </p>
        </div>

      </div>
    </details>

    <details id="skills">
      <summary>✨ Technical Skills</summary>

      <div class="skills">
        <div class="skill">Python</div>
        <div class="skill">MATLAB</div>
        <div class="skill">CellProfiler</div>
        <div class="skill">Cellpose</div>
        <div class="skill">Microscopy Analysis</div>
        <div class="skill">PCA Analysis</div>
      </div>
    </details>

    <details id="resume">
      <summary>📄 Resume</summary>

      <p>
        Resume coming soon.
      </p>
    </details>

    <details id="contact">
      <summary>💌 Contact</summary>

      <p>
        LinkedIn: coming soon <br><br>
        Email: coming soon
      </p>
    </details>

  </section>

  <footer>
    © 2026 Marie Kasongo • Built with 💗 and GitHub Pages
  </footer>

</body>
</html>
