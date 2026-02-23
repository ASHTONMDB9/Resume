<template>
  <div class="hero">
    <video autoplay loop muted playsinline id="land">
      <source src="../images/land.mp4" type="video/mp4" loading="lazy" />
    </video>

    <div class="overlay"></div>

    <div class="content">
      <h1 class="intro">Hi, my name is</h1>
      <h1 class="name">Ashton Abrahams</h1>

      <h2 class="role">Aspiring Full-Stack Developer</h2>

      <h3 class="quote">
        Nothing is
        <span class="impossible">
          <span class="shine">'I</span>M<span class="shine">POSSIBLE'</span>
        </span>
      </h3>

      <p class="hint">Hover between quotes</p>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
/* Layout */
.hero {
  width: 100%;
  overflow: hidden;
  display: flex;
  justify-content: center;
  align-items: center;
}
#land {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -2;
  filter: saturate(1.1) contrast(1.05);
}
.overlay {
  position: absolute;
  inset: 0;
  background: linear-gradient(
    to bottom,
    rgba(8, 10, 20, 0.6),
    rgba(8, 10, 20, 0.9)
  );
  backdrop-filter: blur(2px);
  z-index: -1;
  justify-content: center;
  align-items: center;
}
.content {
  text-align: center;
  justify-content: center;
  align-items: center;
  padding: 1.5rem;
  animation: fadeUp 1.2s ease forwards;
}
.intro {
  color: white;
  font-weight: 500;
  font-size: 1.3rem;
  letter-spacing: 0.15em;
  margin-bottom: 0.4rem;
  white-space: nowrap;
  overflow: hidden;
  width: 240px;
  animation: type 2s steps(30, end) forwards;
}
.name {
  font-size: clamp(3rem, 6vw, 4.5rem);
  font-weight: 900;
  background: linear-gradient(90deg, #7dd3fc, #a78bfa, #22d3ee);
  background-size: 200%;
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  text-shadow: 0 6px 30px rgba(0, 0, 0, 0.6);
  opacity: 0;
  animation: nameReveal 2.2s ease forwards 2s;
}
.role {
  margin-top: 1rem;
  font-size: 0.95rem;
  color: #9aa4c7;
  letter-spacing: 0.25em;
  text-transform: uppercase;
}
.quote {
  margin-top: 1.8rem;
  font-family: monospace;
  font-size: 1.05rem;
  letter-spacing: 0.35em;
  color: red;
}
.impossible {
  position: relative;
  display: inline-flex;
  gap: 0.15em;
  transition: all 0.3s ease;
}
/* Impossible hover */
.quote span {
  transition: all 0.3s ease;
}
.quote:hover span:nth-child(1) {
  margin-right: 8px;
}
.quote:hover span:nth-child(2) {
  margin-left: 22px;
}
.impossible:hover {
  color: #e0f2fe;
  text-shadow: 0 0 8px white, 0 0 18px white, 0 0 32px white;
  transition: transform 0.3s ease;
}
.impossible:hover span {
  transform: translateY(-1px);
}
/* Hint */
.hint {
  margin-top: 0.8rem;
  font-size: 0.7rem;
  color: white;
  opacity: 0.8;
}
@keyframes shine {
  from {
    transform: translateX(-120%);
  }
  to {
    transform: translateX(120%);
  }
}
@keyframes type {
  from {
    width: 0;
  }
  to {
    width: 240px;
  }
}
@keyframes nameReveal {
  from {
    opacity: 0;
    transform: translateY(14px);
    background-position: 0%;
  }
  to {
    opacity: 1;
    transform: translateY(0);
    background-position: 100%;
  }
}
@keyframes fadeUp {
  from {
    opacity: 0;
    transform: translateY(24px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Media Queries */

/* Fluid scaling below 1920px */
@media (max-width: 1919px) {
  .hero {
    margin-top: clamp(150px, 15vw, 300px);
  }
  #land {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -2;
    filter: saturate(1.1) contrast(1.05);
  }
  .content {
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
    animation: fadeUp 1.2s ease forwards;
  }
  .intro {
    font-size: clamp(1rem, 1.2vw, 1.3rem);
    width: clamp(180px, 20vw, 240px);
  }

  .role {
    font-size: clamp(0.8rem, 0.9vw, 0.95rem);
  }

  .quote {
    font-size: clamp(0.9rem, 1vw, 1.05rem);
    letter-spacing: clamp(0.25em, 0.3vw, 0.35em);
  }

  .hint {
    font-size: clamp(0.6rem, 0.7vw, 0.7rem);
  }
}
@media (max-width: 1024px) {
  .content {
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
    animation: fadeUp 1.2s ease forwards;
    margin-top: 125px;
  }
  #land {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -2;
    filter: saturate(1.1) contrast(1.05);
  }
}
/* Tablets / medium devices */
@media (max-width: 992px) {
  .hero {
    margin-top: 180px;
    padding: 0 1rem;
  }
  #land {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -2;
    filter: saturate(1.1) contrast(1.05);
  }
  .intro {
    width: 180px;
    font-size: 1.1rem;
  }

  .name {
    font-size: clamp(2.2rem, 8vw, 3.5rem);
  }

  .role {
    font-size: 0.85rem;
    letter-spacing: 0.2em;
  }
  .content {
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
    animation: fadeUp 1.2s ease forwards;
    margin-top: 80px;
  }
  .quote {
    font-size: 0.95rem;
    letter-spacing: 0.3em;
  }

  .hint {
    font-size: 0.65rem;
  }
}

/* Small laptops / large phones */
@media (max-width: 768px) {
  .hero {
    margin-top: 140px;
    padding: 0 0.8rem;
  }
  .content {
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
    animation: fadeUp 1.2s ease forwards;
    margin-top: 120px;
  }
  .intro {
    width: 160px;
    font-size: 1rem;
  }
  #land {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -2;
    filter: saturate(1.1) contrast(1.05);
  }
  .name {
    font-size: clamp(1.8rem, 9vw, 3rem);
  }

  .role {
    font-size: 0.8rem;
  }

  .quote {
    font-size: 0.9rem;
  }

  .hint {
    font-size: 0.6rem;
  }
}

/* Mobile phones */
@media (max-width: 576px) {
  .hero {
    margin-top: 100px;
    padding: 0 0.5rem;
  }
  #land {
    position: absolute;
    inset: 0;
    width: 100%;
    height: 100%;
    object-fit: cover;
    z-index: -2;
    filter: saturate(1.1) contrast(1.05);
  }
  .intro {
    width: 140px;
    font-size: 0.9rem;
  }
  .content {
    text-align: center;
    justify-content: center;
    align-items: center;
    padding: 1.5rem;
    animation: fadeUp 1.2s ease forwards;
    margin-top: 180px;
  }
  .name {
    font-size: clamp(1.5rem, 10vw, 2.5rem);
  }

  .role {
    font-size: 0.75rem;
    letter-spacing: 0.15em;
  }

  .quote {
    font-size: 0.8rem;
    letter-spacing: 0.2em;
  }

  .hint {
    font-size: 0.55rem;
  }
}
</style>
