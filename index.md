---
layout: default
title: "Nic Sawaya"
---


<!-- ============================================================
     HERO
     ============================================================ -->
## Hero {#hero}
<!-- Profile photo -->
<!-- Your name + tagline -->
<!-- 2 CTA buttons: Contact | View Projects -->
<!-- Quick stats row -->
<!--   - X years experience -->
<!--   - X projects shipped -->
<!--   - X engines used -->

<hr>

<!-- ============================================================
     PROJECTS SECTION
     ============================================================ -->

<section id="projects">
  <h2>Projects</h2>
  <p class="section-sub">A collection of games and prototypes I've built and iterated on.</p>

  <!-- Filter Tabs -->
  <div class="filter-tabs">
    <button class="filter-btn active" data-filter="all">All</button>
    <button class="filter-btn" data-filter="game">Games</button>
    <button class="filter-btn" data-filter="prototype">Prototypes</button>
  </div>

  <!-- Project Cards -->
  <div class="project-grid">

    <div class="project-card" data-category="game">
      <img src="assets/images/OrbitLogoV1.png" class="project-thumb" alt="Orbit Protocol">
      <div class="project-info">
        <div class="project-tags">
          <span class="tag">Unreal Engine</span>
          <span class="tag">FPS</span>
          <span class="tag">Roguelite</span>
        </div>
        <h3>Orbit Protocol</h3>
        <p>Rogue‑Lite Retro‑Futuristic FPS set aboard a collapsing 1970s space colony.</p>
        <a class="project-btn" href="/projects/orbit-protocol">View Project</a>
      </div>
    </div>

    <!-- Add more cards here. Use data-category="game" or data-category="prototype" -->

  </div>
</section>

<style>
  #projects {
    padding: 4rem 2rem;
    max-width: 1100px;
    margin: 0 auto;
  }

  #projects h2 {
    font-size: 2rem;
    margin-bottom: 0.4rem;
  }

  .section-sub {
    color: #888;
    margin-bottom: 2rem;
  }

  .filter-tabs {
    display: flex;
    gap: 0.75rem;
    margin-bottom: 2rem;
  }

  .filter-btn {
    padding: 0.45rem 1.2rem;
    border: 1px solid #444;
    border-radius: 999px;
    background: transparent;
    color: inherit;
    cursor: pointer;
    font-size: 0.9rem;
    transition: all 0.2s ease;
  }

  .filter-btn:hover {
    border-color: #fff;
  }

  .filter-btn.active {
    background: #fff;
    color: #000;
    border-color: #fff;
  }

  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 1.5rem;
  }

  .project-card {
    background: #111;
    border: 1px solid #222;
    border-radius: 12px;
    overflow: hidden;
    transition: transform 0.2s ease, border-color 0.2s ease;
  }

  .project-card:hover {
    transform: translateY(-4px);
    border-color: #555;
  }

  .project-card.hidden {
    display: none;
  }

  .project-thumb {
    width: 100%;
    height: 180px;
    object-fit: cover;
    display: block;
  }

  .project-info {
    padding: 1.2rem;
  }

  .project-tags {
    display: flex;
    flex-wrap: wrap;
    gap: 0.4rem;
    margin-bottom: 0.75rem;
  }

  .tag {
    font-size: 0.72rem;
    padding: 0.2rem 0.6rem;
    border-radius: 999px;
    border: 1px solid #444;
    color: #aaa;
  }

  .project-info h3 {
    margin: 0 0 0.4rem;
    font-size: 1.1rem;
  }

  .project-info p {
    font-size: 0.88rem;
    color: #aaa;
    margin-bottom: 1rem;
    line-height: 1.5;
  }

  .project-btn {
    display: inline-block;
    padding: 0.45rem 1.1rem;
    border: 1px solid #555;
    border-radius: 8px;
    font-size: 0.85rem;
    text-decoration: none;
    color: inherit;
    transition: all 0.2s ease;
  }

  .project-btn:hover {
    background: #fff;
    color: #000;
    border-color: #fff;
  }
</style>

<script>
  const filterBtns = document.querySelectorAll('.filter-btn');
  const cards = document.querySelectorAll('.project-card');

  filterBtns.forEach(btn => {
    btn.addEventListener('click', () => {
      filterBtns.forEach(b => b.classList.remove('active'));
      btn.classList.add('active');

      const filter = btn.dataset.filter;

      cards.forEach(card => {
        if (filter === 'all' || card.dataset.category === filter) {
          card.classList.remove('hidden');
        } else {
          card.classList.add('hidden');
        }
      });
    });
  });
</script>

<hr>

<!-- ============================================================
     SKILLS
     ============================================================ -->
## Skills {#skills}
<!-- Group 1: Engines & Tools -->
<!--   Unreal Engine, Unity, Rider, Perforce, Git -->

<!-- Group 2: Languages -->
<!--   Blueprint, C++, GDScript, etc. -->

<!-- Group 3: Specialties -->
<!--   FPS Mechanics, Weapon Systems, Ability Frameworks -->
<!--   UI/UX, Level Design, Worldbuilding -->

<!-- Group 4: Soft Skills -->
<!--   Iteration, Rapid Prototyping, Visual Identity -->

<hr>

<!-- ============================================================
     CONTACT
     ============================================================ -->
## Contact {#contact}
<!-- Email -->
<!-- GitHub link -->
<!-- Optional: Itch.io, LinkedIn, ArtStation -->
