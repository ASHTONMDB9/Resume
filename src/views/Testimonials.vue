<template>
  <div class="testimonials-page">
    <!-- Tabs -->
    <div class="tabs">
      <ul class="nav nav-tabs">
        <li class="nav-item">
          <router-link class="nav-link" to="/Resume">
            <h6>Resume</h6>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link active" to="/Testimonials">
            <h6>Testimonials</h6>
          </router-link>
        </li>
      </ul>
    </div>

    <!-- Grid -->
    <section class="testimonials-grid">
      <article
        v-for="testimonial in testimonials"
        :key="testimonial.id"
        class="testimonial-card"
      >
        <img
          :src="testimonial.image"
          :alt="testimonial.name"
          class="profile-img"
        />

        <h3>{{ testimonial.name }}</h3>
        <span class="role">{{ testimonial.role }}</span>

        <p class="quote">“{{ testimonial.testimony }}”</p>
      </article>
    </section>
  </div>
</template>

<script>
export default {
  data() {
    return {
      testimonials: [
        {
          id: "1",
          image: "https://i.postimg.cc/L5vZ8fZJ/Carla-1-1-removebg-preview.png",
          name: "Carla Lawrence",
          testimony:
            "Ashton Abrahams is an excellent addition to any team. He is a without a doubt a very skilled web developer. Ashton's ability to integrate beautiful design and web functionality is outstanding. I count myself lucky to have had him as a colleague for his pleasant disposition and humorous character.",
          role: "Colleague",
        },
        {
          id: "2",
          image: "https://i.postimg.cc/QMCsT3QC/Ricardo-2.png",
          name: "Ricardo Moses",
          testimony:
            "Ashton is a diligent worker, always stays focused and works hard. He's kind and open-minded personality makes him a pleasure to be around in a work environment.",
          role: "Colleague",
        },
        {
          id: "3",
          image:
            "https://i.postimg.cc/5Nbk6MDv/T02-LW4-RMXJQ-U036-JA3-NVL5-45897a34dc43-512-removebg-preview.png",
          name: "Jason Wandrag",
          testimony:
            "I think Ashton Abrahams is a very consistent student. When he is confident about the answer, he loves participating in class. As long as he focuses in class, Ashton Abrahams will improve steadily.",
          role: "Lecturer",
        },
        {
          id: "4",
          image:
            "https://i.postimg.cc/j2tzjMWQ/Mika-Rinquest-removebg-preview.png",
          name: "Mika Rinquest",
          testimony:
            "Once Ashton starts working he does not allow for any distractions. He fits in well with others and has the potential to be a valuable member of any team.",
          role: "Colleague",
        },
        {
          id: "5",
          image: "https://i.postimg.cc/LsPbJkBQ/Zoe-3-1-removebg-preview.png",
          name: "Zoe Van Der Schyff",
          testimony:
            "Ashton is one of the smartest, hard-working people I know. He tries over and over until he gets it right. He will strive until he gets what he needs, and he will do what he needs to do to get things done.",
          role: "Colleague",
        },
        {
          id: "6",
          image:
            "https://i.postimg.cc/vmFMDHFM/Chanique-1-removebg-preview.png",
          name: "Chanique Mansoor",
          testimony:
            "Ashton is a true example of a leader and strives in everything he does, his personality and persona is something I could only aspire to have. Wishing him all the best with his future as a developer.",
          role: "Colleague",
        },
        {
          id: "7",
          image: "https://i.postimg.cc/k5p1hrk1/Jesse-2.png",
          name: "Jesse Spence",
          testimony:
            "Ashton is extremely creative, artistic and has a great eye for design. This combined with his friendly attitude and good communication makes him an incredible person to work with. I am extremely grateful to have worked and learned along side him.",
          role: "Colleague",
        },
        {
          id: "8",
          image: "https://i.postimg.cc/vmfgCfKj/Charles-2.png",
          name: "Abdus-Samad Charles",
          testimony:
            "Ashton is a trustworthy and hardworking individual who enjoys solving problems and helping others. He has a very calm demeaner and is easily approachable.",
          role: "Colleague",
        },
      ],
    };
  },
};
</script>
<style scoped>
.testimonials-page {
  padding-top: 90px;
  padding-bottom: 80px;
  color: #e5e7eb;
}

/* Tabs (reuse your existing language) */
.tabs {
  display: flex;
  justify-content: center;
  margin-top: 50px;
  margin-bottom: 50px;
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

/* Grid */
.testimonials-grid {
  max-width: 1500px;
  margin: 0 auto;
  padding: 0 32px;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
  gap: 2.4rem;
}

/* Card */
.testimonial-card {
  background: rgba(5, 6, 10, 0.55);
  border-radius: 20px;
  border: 1px solid rgba(125, 211, 252, 0.25);
  backdrop-filter: blur(14px);
  padding: 34px 28px;
  text-align: center;
  box-shadow: 0 14px 30px rgba(0, 0, 0, 0.45);
  transition: transform 0.35s ease, box-shadow 0.35s ease;
}

.testimonial-card:hover {
  transform: translateY(-8px);
  box-shadow: 0 0 22px rgba(125, 211, 252, 0.4),
    0 0 32px rgba(167, 139, 250, 0.35);
}

/* Image */
.profile-img {
  width: 110px;
  height: 110px;
  object-fit: contain;
  border-radius: 50%;
  border: 1px solid rgba(125, 211, 252, 0.35);
  padding: 10px;
  margin-bottom: 18px;
  background: rgba(5, 6, 10, 0.7);
}

/* Text */
.testimonial-card h3 {
  font-family: Space Grotesk, sans-serif;
  font-size: 1.4rem;
  margin-bottom: 6px;
  color: #ffffff;
}

.role {
  display: block;
  font-size: 0.75rem;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: #7dd3fc;
  margin-bottom: 16px;
}

.quote {
  font-size: 0.95rem;
  line-height: 1.65;
  color: #cbd5f5;
  font-style: italic;
}

/* Responsive polish */
@media (max-width: 560px) {
  .testimonial-card {
    padding: 28px 22px;
  }

  .profile-img {
    width: 95px;
    height: 95px;
  }
}
</style>
