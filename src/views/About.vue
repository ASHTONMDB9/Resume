<template>
  <div class="about-page">
    <div class="tabs">
      <ul class="nav nav-tabs">
        <li class="nav-item">
          <router-link class="nav-link active" to="/About">
            <h6>Bio</h6>
          </router-link>
        </li>
        <li class="nav-item">
          <router-link class="nav-link" to="/Skills">
            <h6>Skills</h6>
          </router-link>
        </li>
      </ul>
    </div>

    <div class="about-container">
      <div class="about-card">
        <div class="about-left">
          <img
            id="ash2"
            src="https://i.postimg.cc/1ztMx7TZ/ash2-removebg-preview.png"
            alt="Ashton"
          />
        </div>

        <div class="about-right">
          <h3 class="about-title">About Me</h3>

          <div class="details">
            <p><span>Full name:</span> Ashton Abrahams</p>
            <p><span>Date of birth:</span> 07/07/2004</p>
            <p><span>Gender:</span> Male</p>
          </div>

          <div class="bio">
            <p>
              Hi there! I'm Ashton — a consistent and committed developer with
              an optimistic and artistic mind. I’ve been fascinated with
              technology and computers since I was six.
            </p>
            <p>
              I love gaming, computers, and creative problem solving. I’m
              confident and I always welcome challenges — I’m a hard worker who
              finishes what I start and enjoy working with others so getting
              along with others comes naturally to me.
            </p>
            <p>
              Coding is one of my many passions and would love to pursue that
              further as it stimulates my creative mind and creating a working
              project/website excites me.
            </p>
            <p>
              An organized and dependable candidate successful at managing
              multiple priorities with a positive attitude and willingness to
              take on added responsibilities to meet team goals.
            </p>
            <div class="details">
              <p><span>Some of my hobbies include:</span></p>
            </div>
            <p>
              Gaming, Art: drawing/sketching/painting, Making music, Watching
              anime, Hiking, Being outdoors, Go-karting, Cars, Socialising,
              Reading, Chess, Coding
            </p>
          </div>

          <div class="socials-section">
            <span class="share">Socials</span>
            <div class="social-icons">
              <a
                href="https://www.facebook.com/profile.php?id=100083321873494"
                target="_blank"
                class="social-icon"
              >
                <i class="fa-brands fa-facebook"></i>
              </a>
              <a
                href="https://www.instagram.com/ashton.m_db9/"
                target="_blank"
                class="social-icon"
              >
                <i class="fa-brands fa-instagram"></i>
              </a>
              <a
                href="https://github.com/ASHTONMDB9"
                target="_blank"
                class="social-icon"
              >
                <i class="fa-brands fa-github"></i>
              </a>
              <a
                href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/"
                target="_blank"
                class="social-icon"
              >
                <i class="fa-brands fa-linkedin"></i>
              </a>
            </div>
          </div>

          <router-link to="/Gallery">
            <button class="work">
              <h6>My Gallery</h6>
            </button>
          </router-link>
        </div>
      </div>
    </div>
  </div>
</template>

<script></script>

<style scoped>
.about-page {
  padding-top: 110px;
  color: #e5e7eb;
}

.tabs {
  display: flex;
  justify-content: center;
  margin-top: 20px;
  margin-bottom: 30px;
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

.about-container {
  display: flex;
  justify-content: center;
  padding: 40px 60px;
}

.about-card {
  display: grid;
  grid-template-columns: 1fr 2fr;
  gap: 2rem;
  max-width: 1500px;
  width: 100%;
  background: rgba(5, 6, 10, 0.55);
  border: 1px solid rgba(255, 255, 255, 0.08);
  backdrop-filter: blur(12px);
  border-radius: 18px;
  padding: 8px;
}

.about-left {
  display: flex;
  justify-content: center;
  align-items: center;
}

#ash2 {
  width: 100%;
  max-width: 260px;
  height: auto;
  transform: translateY(-20px);
}

.about-title {
  font-family: Space Grotesk, sans-serif;
  font-size: 2.2rem;
  margin-bottom: 1rem;
  margin-top: 80px;
  color: #fff;
  text-decoration: underline;
  text-decoration-color: #7dd3fc;
}

.details p {
  margin: 8px 0;
  font-size: 1rem;
  color: #cbd5f5;
}

.details span {
  color: #7dd3fc;
  font-weight: 600;
}

.bio p {
  margin: 12px 0;
  font-size: 1rem;
  line-height: 1.6;
  color: #d1d5db;
}

.socials-section {
  margin-top: 18px;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.share {
  font-family: Inter, sans-serif;
  font-size: 0.85rem;
  letter-spacing: 0.25em;
  text-transform: uppercase;
  color: #94a3b8;
}

.social-icons {
  display: flex;
  gap: 0.7rem;
}

.social-icon {
  width: 40px;
  height: 40px;
  display: grid;
  place-items: center;
  border-radius: 50%;
  border: 1px solid rgba(125, 211, 252, 0.35);
  color: #cbd5f5;
  transition: transform 0.25s ease, box-shadow 0.25s ease;
}

.social-icon:hover {
  transform: scale(1.15);
  box-shadow: 0 0 16px rgba(125, 211, 252, 0.35),
    0 0 26px rgba(167, 139, 250, 0.35);
  color: #e0f2fe;
}

.work {
  margin-top: 22px;
  padding: 10px 20px;
  border-radius: 10px;
  background: transparent;
  border: 1px solid rgba(125, 211, 252, 0.65);
  color: #7dd3fc;
  font-family: Inter, sans-serif;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  transition: background 0.25s ease, color 0.25s ease;
}

.work:hover {
  background: rgba(125, 211, 252, 0.12);
  color: #e0f2fe;
}

@media (min-width: 1200px) {
  .about-card {
    padding: 34px;
    gap: 2.5rem;
  }
}

@media (max-width: 900px) {
  .about-card {
    grid-template-columns: 1fr;
    text-align: center;
  }

  .about-left {
    order: 1;
  }

  .about-right {
    order: 2;
  }
}
</style>
