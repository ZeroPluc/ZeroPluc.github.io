# ZeroPluc.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>SECOND LAYER — Contemporary Art</title>
  <meta name="description" content="Contemporary artist portfolio — photography, painting, murals, digital art." />
  <style>
    :root {
      --bg: #0e0e0e;
      --fg: #f2f2f2;
      --muted: #9a9a9a;
      --accent: #e63946;
    }

    * { box-sizing: border-box; margin: 0; padding: 0; }

    body {
      font-family: Inter, Helvetica, Arial, sans-serif;
      background: var(--bg);
      color: var(--fg);
      line-height: 1.6;
    }

    a { color: var(--fg); text-decoration: none; }

    header {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      padding: 4rem;
    }

    header h1 {
      font-size: clamp(3rem, 8vw, 6rem);
      font-weight: 800;
      letter-spacing: -0.04em;
    }

    header p {
      max-width: 600px;
      margin-top: 1.5rem;
      color: var(--muted);
      font-size: 1.1rem;
    }

    nav {
      position: fixed;
      top: 2rem;
      right: 2rem;
      display: flex;
      gap: 2rem;
      font-size: 0.9rem;
    }

    section {
      padding: 6rem 4rem;
    }

    section h2 {
      font-size: 2rem;
      margin-bottom: 2rem;
    }

    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .work {
      aspect-ratio: 4 / 5;
      background: #1a1a1a;
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--muted);
      font-size: 0.9rem;
    }

    .about {
      max-width: 700px;
      color: var(--muted);
    }

    footer {
      padding: 4rem;
      border-top: 1px solid #1f1f1f;
      display: flex;
      justify-content: space-between;
      flex-wrap: wrap;
      gap: 2rem;
      font-size: 0.9rem;
      color: var(--muted);
    }

    footer a { color: var(--fg); }

    @media (max-width: 768px) {
      header, section, footer { padding: 3rem 2rem; }
      nav { right: 1.5rem; top: 1.5rem; }
    }
  </style>
</head>
<body>

  <nav>
    <a href="#work">Work</a>
    <a href="#about">About</a>
    <a href="#contact">Contact</a>
  </nav>

  <header>
    <h1>SECOND LAYER</h1>
    <p>
      Contemporary artist from Poland working across photography, painting, murals, and digital media.
      Rooted in graffiti, focused on transformation, surface, and modern visual language.
    </p>
  </header>

  <section id="work">
    <h2>Selected Work</h2>
    <div class="grid">
      <div class="work">Project 01</div>
      <div class="work">Project 02</div>
      <div class="work">Project 03</div>
      <div class="work">Project 04</div>
      <div class="work">Project 05</div>
      <div class="work">Project 06</div>
    </div>
  </section>

  <section id="about">
    <h2>About</h2>
    <div class="about">
      <p>
        I am a 25-year-old contemporary artist based in Poland, with a background in graffiti and a Bachelor’s degree in Fine Arts.
        My work explores the relationship between public space and the gallery, combining classical painting techniques
        with photography, murals, and digital processes.
      </p>
    </div>
  </section>

  <section id="contact">
    <h2>Contact</h2>
    <p class="about">
      For collaborations, commissions, or exhibitions:<br />
      <a href="mailto:hello@secondlayer.art">hello@secondlayer.art</a>
    </p>
  </section>

  <footer>
    <div>© 2026 SECOND LAYER</div>
    <div>
      <a href="#">Instagram</a> ·
      <a href="#">Behance</a> ·
      <a href="#">PDF Portfolio</a>
    </div>
  </footer>

</body>
</html>
