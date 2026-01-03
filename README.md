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
