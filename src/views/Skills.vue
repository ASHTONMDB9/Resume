<template>
  <div class="skills-page">
    <div class="tabs">
      <ul class="nav nav-tabs">
        <li class="nav-item">
          <router-link class="nav-link" to="/About">
            <h6>Bio</h6>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link active" to="/Skills">
            <h6>Skills</h6>
          </router-link>
        </li>
      </ul>
    </div>

    <section class="section">
      <h1 class="section-title">Soft Skills</h1>

      <div class="soft-grid">
        <div class="soft-card">
          <div class="ring ring-comm" data-value="90"></div>
          <div class="soft-label">Communication</div>
        </div>

        <div class="soft-card">
          <div class="ring ring-prob" data-value="75"></div>
          <div class="soft-label">Problem Solving</div>
        </div>

        <div class="soft-card">
          <div class="ring ring-creative" data-value="80"></div>
          <div class="soft-label">Creativity</div>
        </div>

        <div class="soft-card">
          <div class="ring ring-team" data-value="85"></div>
          <div class="soft-label">Teamwork</div>
        </div>
      </div>
    </section>

    <section class="section">
      <h1 class="section-title">Technical Skills</h1>

      <div class="tech-grid">
        <div class="tech-card">
          <div class="tech-header">HTML</div>
          <div class="tech-icon"><i class="fa-brands fa-html5"></i></div>
          <p class="tech-desc">
            HTML is the standard markup language for creating Web pages.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">CSS</div>
          <div class="tech-icon"><i class="fa-brands fa-css3"></i></div>
          <p class="tech-desc">
            CSS styles HTML documents and controls how elements are displayed.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">Bootstrap</div>
          <div class="tech-icon"><i class="fa-brands fa-bootstrap"></i></div>
          <p class="tech-desc">
            Bootstrap is a frontend toolkit for building responsive UIs fast.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">MySQL</div>
          <div class="tech-icon"><i class="fa-solid fa-database"></i></div>
          <p class="tech-desc">
            MySQL is a relational database system using SQL.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">JavaScript</div>
          <div class="tech-icon"><i class="fa-brands fa-js"></i></div>
          <p class="tech-desc">
            JavaScript is used to create interactive and dynamic web pages.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">Vue JS</div>
          <div class="tech-icon"><i class="fa-brands fa-vuejs"></i></div>
          <p class="tech-desc">
            Vue is a JS framework for building modern user interfaces.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">Node.js</div>
          <div class="tech-icon"><i class="fa-brands fa-node-js"></i></div>
          <p class="tech-desc">
            Node is a runtime for executing JS outside the browser.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">WordPress</div>
          <div class="tech-icon"><i class="fa-brands fa-wordpress"></i></div>
          <p class="tech-desc">
            WordPress makes building websites accessible to anyone.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">SEO</div>
          <div class="tech-icon"><i class="fa-brands fa-searchengin"></i></div>
          <p class="tech-desc">
            SEO improves visibility in organic search results.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">PHP</div>
          <div class="tech-icon"><i class="fa-brands fa-php"></i></div>
          <p class="tech-desc">
            PHP is a server-side language for dynamic web pages.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">Python</div>
          <div class="tech-icon"><i class="fa-brands fa-python"></i></div>
          <p class="tech-desc">
            Python is an interpreted, object-oriented, high-level programming
            language with dynamic semantics.
          </p>
        </div>

        <div class="tech-card">
          <div class="tech-header">Git</div>
          <div class="tech-icon"><i class="fa-brands fa-github"></i></div>
          <p class="tech-desc">
            Git is a version control system that intelligently tracks changes in
            files.
          </p>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.skills-page {
  padding-top: 90px;
  padding-bottom: 60px;
  color: #e5e7eb;
}

/* Tabs */
.tabs {
  display: flex;
  justify-content: center;
  margin: 20px 0;
}

.nav-tabs .nav-link {
  font-family: Inter, sans-serif;
  font-size: 0.85rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: #cbd5f5;
  border: none;
  padding: 10px 22px;
}

.nav-tabs .nav-link.active {
  color: #7dd3fc;
  border-bottom: 2px solid #7dd3fc;
}

/* Sections */
.section {
  max-width: 1200px;
  margin: 0 auto 50px;
  padding: 0 20px;
}

.section-title {
  text-align: center;
  font-family: Space Grotesk, sans-serif;
  font-size: 2.4rem;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
  margin-bottom: 30px;
}

/* Soft Skills Grid */
.soft-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.5rem;
  justify-items: center;
}

.soft-card {
  width: 160px;
  text-align: center;
}

.soft-label {
  margin-top: 12px;
  font-family: Inter, sans-serif;
  font-size: 0.95rem;
  letter-spacing: 0.1em;
  color: #cbd5f5;
}

/* Circular progress ring */
.ring {
  width: 160px;
  height: 160px;
  border-radius: 50%;
  background: conic-gradient(
    #7dd3fc 0deg,
    #7dd3fc calc(var(--value) * 1deg),
    rgba(255, 255, 255, 0.08) 0deg
  );
  position: relative;
  display: grid;
  place-items: center;
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.5);
}

.ring::before {
  content: attr(data-value) "%";
  font-family: Space Grotesk, sans-serif;
  font-size: 1.3rem;
  font-weight: 700;
  color: #e0f2fe;
}

.ring::after {
  content: "";
  width: 120px;
  height: 120px;
  border-radius: 50%;
  background: rgba(5, 6, 10, 0.6);
  border: 1px solid rgba(255, 255, 255, 0.08);
  background-size: cover;
  background-position: center;
  box-shadow: inset 0 0 15px rgba(0, 0, 0, 0.6);
}

/* IMAGE FOR EACH SKILL */
.ring-comm::after {
  background-image: url("../images/comm.jpg");
}

.ring-prob::after {
  background-image: url("../images/prob.jpg");
}

.ring-creative::after {
  background-image: url("../images/create.jpg");
}

.ring-team::after {
  background-image: url("../images/team.jpg");
}

/* Tech Grid */
.tech-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1.2rem;
}

.tech-card {
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(255, 255, 255, 0.08);
  border-radius: 16px;
  padding: 18px;
  text-align: center;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.tech-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 14px 30px rgba(0, 0, 0, 0.45),
    0 0 18px rgba(125, 211, 252, 0.25);
}

.tech-header {
  font-family: Space Grotesk, sans-serif;
  font-size: 1.1rem;
  margin-bottom: 12px;
  color: #7dd3fc;
}

.tech-icon {
  font-size: 2.5rem;
  margin-bottom: 12px;
  color: #cbd5f5;
}

.tech-desc {
  font-family: Inter, sans-serif;
  font-size: 0.95rem;
  color: #cbd5f5;
  line-height: 1.5;
}

/* Responsive */
@media (max-width: 992px) {
  .soft-grid,
  .tech-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 576px) {
  .soft-grid,
  .tech-grid {
    grid-template-columns: 1fr;
  }
}
</style>
