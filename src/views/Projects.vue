<template>
  <div class="projects-page">
    <section class="section">
      <h1 class="section-title">Projects</h1>

      <div class="projects-grid">
        <article
          v-for="project in projects"
          :key="project.id"
          class="project-card"
        >
          <div class="image-wrapper">
            <img :src="project.image" :alt="project.name" />
          </div>

          <div class="project-content">
            <h3 class="project-title">{{ project.name }}</h3>
            <p class="project-desc">{{ project.description }}</p>

            <div class="actions">
              <a :href="project.github" target="_blank" class="action-btn">
                <i class="fa-solid fa-code"></i> Code
              </a>
              <a
                :href="project.live"
                target="_blank"
                class="action-btn primary"
              >
                <i class="fa-solid fa-globe"></i> Live
              </a>
            </div>
          </div>
        </article>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      projects: [
        {
          id: 1,
          image: "https://i.postimg.cc/TwpqYjjp/temp.png",
          name: "Temp Converter",
          description: "A temperature converter for converting °C to °F",
          github: "https://github.com/ASHTONMDB9/Temp-calculator",
          live: "https://temp-calculator.netlify.app",
        },
        {
          id: 3,
          image: "https://i.postimg.cc/WpQvq4rf/DB9-calculator.png",
          name: "Calculator",
          description: "A simple working mathematical JS calculator",
          github: "https://github.com/ASHTONMDB9/Mycalculator",
          live: "https://db9calculator.netlify.app",
        },
        {
          id: 4,
          image: "https://i.postimg.cc/qvxGmvMM/BMI.png",
          name: "BMI Calculator",
          description: "A calculator that calculates your body mass index",
          github: "https://github.com/ASHTONMDB9/BMI-Calculator",
          live: "https://aacalcbmi.netlify.app",
        },
        {
          id: 5,
          image: "https://i.postimg.cc/66FzqPmw/to-do.png",
          name: "To-do List",
          description: "A simple to-do list app for completing tasks",
          github: "https://github.com/ASHTONMDB9/js-todo-list",
          live: "https://magenta-meringue-b58be7.netlify.app",
        },
        {
          id: 6,
          image: "https://i.postimg.cc/Pxp6LV98/2026-02-05-18-13-47-phantomrealm-Opera.png",
          name: "PhantomRealm",
          description: "A project creating a company website",
          github:
            "https://github.com/ASHTONMDB9/CAPSTONE-PhantomRealm-Frontend",
          live: "https://phantomrealm.netlify.app/",
        },
        {
          id: 7,
          image: "https://i.postimg.cc/c1tMpm4z/capecoast.png",
          name: "Cape Customs",
          description: "A website with a listing of cars that can be filtered",
          github: "https://github.com/ASHTONMDB9/CapeCoastCustoms",
          live: "https://capecoastcustoms.netlify.app",
        },
        {
          id: 8,
          image: "https://i.postimg.cc/zXmS8gyG/holiday.png",
          name: "Tokyo",
          description: "My favourite holiday destination with a contact page",
          github: "https://github.com/ASHTONMDB9/Holiday-Destination",
          live: "https://my-holiday-destination-tokyo.netlify.app",
        },
        {
          id: 9,
          image: "https://i.postimg.cc/gJXMwtQL/2026-02-05-18-14-24-XYZtech-Opera.png",
          name: "XYZ Tech",
          description: "A team project creating a company website",
          github: "https://github.com/ASHTONMDB9/EOMP",
          live: "https://ecommerce-a994b.firebaseapp.com/#/",
        },
      ],
    };
  },
};
</script>

<style scoped>
.projects-page {
  padding-top: 110px;
  padding-bottom: 80px;
  color: #e5e7eb;
}

.section {
  max-width: 1800px;
  margin: 0 auto;
  padding: 0 48px;
}

.section-title {
  text-align: center;
  font-family: Space Grotesk, sans-serif;
  font-size: 2.6rem;
  margin-bottom: 50px;
  color: #ffffff;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
}

.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
  gap: 2.4rem;
}

.project-card {
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(125, 211, 252, 0.22);
  border-radius: 18px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.45);
  transition: transform 0.35s ease, box-shadow 0.35s ease;
}

.project-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 0 20px rgba(125, 211, 252, 0.35),
    0 0 30px rgba(167, 139, 250, 0.25);
}

.image-wrapper {
  position: relative;
  aspect-ratio: 16 / 10;
  overflow: hidden;
}

.image-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease, filter 0.35s ease;
}

.project-card:hover img {
  transform: scale(1.05);
  filter: brightness(0.85);
}

.overlay {
  position: absolute;
  inset: 0;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 22px;
  background: linear-gradient(
    to top,
    rgba(5, 6, 10, 0.85),
    rgba(5, 6, 10, 0.35)
  );
  opacity: 0;
  transition: opacity 0.35s ease;
}

.project-card:hover .overlay {
  opacity: 1;
}

.project-content {
  padding: 20px 22px 24px;
}

.project-title {
  font-family: Space Grotesk, sans-serif;
  font-size: 1.35rem;
  margin-bottom: 6px;
  color: #7dd3fc;
}

.project-desc {
  font-size: 0.9rem;
  line-height: 1.55;
  color: #cbd5f5;
  margin-bottom: 16px;
}

/* Actions */
.actions {
  display: flex;
  gap: 12px;
  margin-top: 14px;
}

.action-btn {
  display: flex;
  align-items: center;
  gap: 6px;
  padding: 8px 16px;
  border-radius: 999px;
  border: 1px solid rgba(125, 211, 252, 0.45);
  color: #cbd5f5;
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.15em;
  text-transform: uppercase;
  text-decoration: none;
  transition: background 0.25s ease, transform 0.25s ease, box-shadow 0.25s ease;
}

.action-btn:hover {
  background: rgba(125, 211, 252, 0.18);
  transform: translateY(-2px);
}

.action-btn.primary {
  background: linear-gradient(90deg, #7dd3fc, #a78bfa);
  color: #020617;
  border: none;
  box-shadow: 0 0 14px rgba(125, 211, 252, 0.45);
}

.action-btn.primary:hover {
  box-shadow: 0 0 18px rgba(167, 139, 250, 0.65);
}

/* Responsive */
@media (max-width: 1200px) {
  .projects-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}

@media (max-width: 900px) {
  .projects-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (max-width: 560px) {
  .projects-grid {
    grid-template-columns: 1fr;
    padding: 22px;
  }
}
</style>
