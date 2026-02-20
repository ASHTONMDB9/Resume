<template>
  <div class="certificates-page">
    <section class="section">
      <header class="certificates-header">
        <h3 class="certificates-title">Certificates</h3>
        <p class="subtitle">Courses • Achievements • Professional Growth</p>
      </header>

      <div class="certificates-grid">
        <article
          v-for="cert in certificates"
          :key="cert.id"
          class="certificate-card"
        >
          <div class="image-wrapper">
            <img :src="cert.image" :alt="cert.title" />
          </div>

          <div class="certificate-content">
            <h3 class="certificate-title">{{ cert.title }}</h3>

            <div class="actions">
              <a
                :href="cert.file"
                download
                target="_blank"
                class="action-btn primary"
              >
                <i class="fa-solid fa-download"></i> Download
              </a>
            </div>
          </div>
        </article>
      </div>

      <!-- Back Button -->
      <div class="back-section">
        <button class="back-btn" @click="$router.back()">
          <h6>Back</h6>
        </button>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      certificates: [
        {
          id: 1,
          title: "Full-Stack Web Development",
          image: "/certificates/fullstack.png",
          file: "/certificates/fullstack.pdf",
        },
        {
          id: 2,
          title: "SEO Training",
          image: "/certificates/seo.png",
          file: "/certificates/seo.pdf",
        },
        {
          id: 3,
          title: "Leadership Training",
          image: "/certificates/leadership.png",
          file: "/certificates/leadership.pdf",
        },
      ],
    };
  },
};
</script>

<style scoped>
.certificates-page {
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
/* Header */
.certificates-header {
  margin-bottom: 40px;
  text-align: center;
}

.certificates-title {
  font-family: Space Grotesk, sans-serif;
  font-size: 2.2rem;
  color: #fff;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
  margin-bottom: 15px;
}

.subtitle {
  font-family: Inter, sans-serif;
  letter-spacing: 0.3em;
  text-transform: uppercase;
  font-size: 0.85rem;
  color: #94a3b8;
}
/* Grid */
.certificates-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(320px, 320px));
  justify-content: center;
  gap: 2.4rem;
}

/* Card */
.certificate-card {
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(125, 211, 252, 0.22);
  border-radius: 18px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
  box-shadow: 0 10px 26px rgba(0, 0, 0, 0.45);
  transition: transform 0.35s ease, box-shadow 0.35s ease;
}

.certificate-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 0 20px rgba(125, 211, 252, 0.35),
    0 0 30px rgba(167, 139, 250, 0.25);
}

/* Image wrapper */
.image-wrapper {
  position: relative;
  aspect-ratio: 4 / 3;
  overflow: hidden;
}

.image-wrapper img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  transition: transform 0.35s ease, filter 0.35s ease;
}

.certificate-card:hover img {
  transform: scale(1.05);
  filter: brightness(0.85);
}

/* Content */
.certificate-content {
  padding: 20px 22px 24px;
}

.certificate-title {
  font-family: Space Grotesk, sans-serif;
  font-size: 1.25rem;
  margin-bottom: 16px;
  color: #7dd3fc;
}

/* Actions */
.actions {
  display: flex;
  gap: 12px;
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

.action-btn.primary {
  background: linear-gradient(90deg, #7dd3fc, #a78bfa);
  color: #020617;
  border: none;
  box-shadow: 0 0 14px rgba(125, 211, 252, 0.45);
}

.action-btn.primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 0 18px rgba(167, 139, 250, 0.65);
}

/* Back button */
.back-section {
  display: flex;
  justify-content: center;
  margin-top: 60px;
}

.back-btn {
  padding: 10px 24px;
  border-radius: 10px;
  background: transparent;
  border: 1px solid rgba(125, 211, 252, 0.65);
  color: #7dd3fc;
  font-family: Inter, sans-serif;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  transition: background 0.25s ease, color 0.25s ease, box-shadow 0.25s ease;
}

.back-btn h6 {
  margin: 5px;
}

.back-btn:hover {
  background: rgba(125, 211, 252, 0.12);
  color: #e0f2fe;
  box-shadow: 0 0 16px rgba(125, 211, 252, 0.35),
    0 0 26px rgba(167, 139, 250, 0.35);
}
</style>
