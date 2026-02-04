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
            <div class="overlay">
              <h3>{{ project.name }}</h3>
              <p>{{ project.description }}</p>

              <div class="actions">
                <a :href="project.github" target="_blank" class="action-btn">
                  <i class="fa-solid fa-code"></i>
                  Code
                </a>
                <a
                  :href="project.live"
                  target="_blank"
                  class="action-btn primary"
                >
                  <i class="fa-solid fa-globe"></i>
                  Live
                </a>
              </div>
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
          image: "https://i.postimg.cc/ryDQ8TgQ/calc.png",
          name: "Calculator",
          description: "A simple working mathematical JS calculator",
          github: "https://github.com/ASHTONMDB9/Mycalculator",
          live: "https://famous-cannoli-bd8b1e.netlify.app",
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
          image: "https://i.postimg.cc/mZFFd0nM/phantom.png",
          name: "PhantomRealm",
          description: "A project creating a company website",
          github:
            "https://github.com/ASHTONMDB9/CAPSTONE-PhantomRealm-Frontend",
          live: "https://capstone-79884.firebaseapp.com/",
        },
        {
          id: 7,
          image: "https://i.postimg.cc/c1tMpm4z/capecoast.png",
          name: "Cape Customs",
          description: "A website with a listing of cars that can be filtered",
          github: "https://github.com/ASHTONMDB9/WestCoastCustoms",
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
          image: "https://i.postimg.cc/c1Vk2GLN/ecom.png",
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
  padding-top: 90px;
  padding-bottom: 60px;
  color: #e5e7eb;
}

.section {
  max-width: 1400px;
  margin: 0 auto;
  padding: 0 24px;
}

.section-title {
  text-align: center;
  font-family: Space Grotesk, sans-serif;
  font-size: 2.6rem;
  margin-bottom: 50px;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
}

/* Grid */
.projects-grid {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 2rem;
  max-width: 1500px;
  width: 100%;
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(12px);
  border-radius: 18px;
  padding: 28px;
}

/* Card */
.project-card {
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(125, 211, 252, 0.25);
  border-radius: 18px;
  overflow: hidden;
  box-shadow: 0 14px 30px rgba(0, 0, 0, 0.45);
  transition: transform 0.35s ease, box-shadow 0.35s ease;
}

.project-card:hover {
  transform: translateY(-10px);
  box-shadow: 0 0 30px rgba(125, 211, 252, 0.45);
}

/* Image */
.image-wrapper {
  position: relative;
  height: 320px;
}

.image-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: filter 0.35s ease, transform 0.35s ease;
}

.project-card:hover img {
  filter: brightness(0.35);
  transform: scale(1.05);
}

/* Overlay */
.overlay {
  position: absolute;
  inset: 0;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  padding: 18px;
  opacity: 0;
  backdrop-filter: blur(4px);
  transition: opacity 0.35s ease;
}

.project-card:hover .overlay {
  opacity: 1;
}

.overlay h3 {
  color: #7dd3fc;
  margin-bottom: 6px;
}

.overlay p {
  font-size: 0.95rem;
  color: #cbd5f5;
  line-height: 1.5;
}

/* Buttons */
.actions {
  display: flex;
  gap: 10px;
  margin-top: 12px;
}

.action-btn {
  padding: 8px 14px;
  border-radius: 10px;
  border: 1px solid rgba(125, 211, 252, 0.4);
  color: #cbd5f5;
  font-size: 0.85rem;
  text-decoration: none;
  display: flex;
  align-items: center;
  gap: 6px;
  transition: background 0.25s ease, transform 0.25s ease;
}

.action-btn:hover {
  background: rgba(125, 211, 252, 0.2);
  transform: translateY(-2px);
}

.action-btn.primary {
  background: linear-gradient(90deg, #7dd3fc, #a78bfa);
  color: #020617;
  border: none;
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
  }
}
</style>
