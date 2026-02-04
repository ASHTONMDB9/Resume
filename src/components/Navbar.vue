<template>
  <nav id="nav" class="navbar navbar-expand-lg fixed-top custom-nav">
    <div class="container-fluid nav-inner">
      <router-link class="navbar-brand" to="/">
        <img
          src="https://i.postimg.cc/mZ7ptKGr/Ashton-Logo.png"
          alt="Ashton logo"
          class="logo"
        />
      </router-link>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#Toggler"
      >
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="Toggler">
        <ul class="navbar-nav ms-auto">
          <li class="nav-item">
            <router-link class="nav-link" to="/">Home</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/About">About</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/Projects">Projects</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/Resume">Resume</router-link>
          </li>
          <li class="nav-item">
            <router-link class="nav-link" to="/Contact">Contact</router-link>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  components: {},
  mounted() {
    const nav = document.getElementById("nav");

    const onScroll = () => {
      if (window.scrollY > 20) {
        nav.classList.add("nav-scrolled");
      } else {
        nav.classList.remove("nav-scrolled");
      }
    };

    window.addEventListener("scroll", onScroll);
  },
};
</script>

<style scoped>
/*Navbar*/
.custom-nav {
  background: transparent;
  padding: 0.8rem 1.6rem;
  transition: background 0.4s ease, backdrop-filter 0.4s ease,
    box-shadow 0.4s ease;
}
.nav-inner {
  display: flex;
  align-items: center;
}
.logo {
  height: 42px;
  opacity: 0.9;
  transition: opacity 0.3s ease, transform 0.3s ease;
}
.logo:hover {
  opacity: 1;
  transform: scale(1.03);
}
.nav-scrolled {
  background: rgba(5, 6, 10, 0.65);
  backdrop-filter: blur(12px);
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4),
    inset 0 0 0 1px rgba(255, 255, 255, 0.04);
}
.navbar-nav {
  gap: 1.6rem;
  align-items: center;
}
.nav-link {
  position: relative;
  font-family: Inter, sans-serif;
  font-size: 0.75rem;
  letter-spacing: 0.35em;
  text-transform: uppercase;
  color: #cbd5f5;
  padding: 0.3rem 0;
  transition: color 0.3s ease;
}
.nav-link:hover {
  color: #e0f2fe;
}
.nav-link::after {
  content: "";
  position: absolute;
  left: 50%;
  bottom: -6px;
  width: 0;
  height: 2px;
  background: linear-gradient(90deg, #7dd3fc, #a78bfa);
  transform: translateX(-50%);
  transition: width 0.3s ease;
}
.nav-link:hover::after {
  width: 60%;
}
a.router-link-exact-active {
  color: #7dd3fc;
}
a.router-link-exact-active::after {
  width: 70%;
}
.navbar-toggler {
  border: none;
}
.navbar-toggler-icon {
  filter: brightness(1.4);
}
</style>
