<template>
  <div class="hero">
    <video autoplay loop muted playsinline id="land">
      <source src="../images/land.mp4" type="video/mp4" />
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
  margin-top: 300px;
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
</style>
