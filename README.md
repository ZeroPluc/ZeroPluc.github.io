/* RESET */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

/* VARIABLES */
:root {
  --bg: #0e0e0e;
  --fg: #f2f2f2;
  --muted: #9a9a9a;
  --accent: #e63946;
}

/* BASE */
body {
  font-family: Inter, Helvetica, Arial, sans-serif;
  background: var(--bg);
  color: var(--fg);
  line-height: 1.65;
  -webkit-font-smoothing: antialiased;
}

a {
  color: var(--fg);
  text-decoration: none;
  position: relative;
}

a::after {
  content: "";
  position: absolute;
  left: 0;
  bottom: -3px;
  width: 100%;
  height: 1px;
  background: var(--fg);
  transform: scaleX(0);
  transform-origin: left;
  transition: transform 0.3s ease;
}

a:hover::after {
  transform: scaleX(1);
}

/* NAV */
nav {
  position: fixed;
  top: 2rem;
  right: 2rem;
  display: flex;
  gap: 2rem;
  font-size: 0.85rem;
  letter-spacing: 0.05em;
  text-transform: uppercase;
  z-index: 10;
}

/* HEADER */
header {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 4rem;
}

header h1 {
  font-size: clamp(3rem, 9vw, 6.5rem);
  font-weight: 800;
  letter-spacing: -0.05em;
}

header p {
  max-width: 620px;
  margin-top: 2rem;
  color: var(--muted);
  font-size: 1.05rem;
}

/* SECTIONS */
section {
  padding: 7rem 4rem;
}

section h2 {
  font-size: 1.9rem;
  margin-bottom: 3rem;
  letter-spacing: -0.02em;
}

/* GRID */
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 2.5rem;
}

/* WORK ITEMS */
.work {
  aspect-ratio: 4 / 5;
  background: #141414;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--muted);
  font-size: 0.85rem;
  letter-spacing: 0.08em;
  text-transform: uppercase;
  transition: transform 0.4s ease, background 0.4s ease;
}

.work:hover {
  transform: translateY(-6px);
  background: #1f1f1f;
}

/* ABOUT */
.about {
  max-width: 720px;
  color: var(--muted);
  font-size: 1rem;
}

/* FOOTER */
footer {
  padding: 4rem;
  border-top: 1px solid #1f1f1f;
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  gap: 2rem;
  font-size: 0.85rem;
  color: var(--muted);
}

footer a {
  color: var(--fg);
}

/* MOBILE */
@media (max-width: 768px) {
  header,
  section,
  footer {
    padding: 3rem 2rem;
  }

  nav {
    right: 1.5rem;
    top: 1.5rem;
    gap: 1.2rem;
  }
}
