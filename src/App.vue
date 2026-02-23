<template>
  <div class="cursor">
    <span class="cursor-inner-ring"></span>
    <span class="cursor-dot"></span>
  </div>

  <Navbar />

  <main id="main-content">
    <router-view />
  </main>

  <Footer />
</template>

<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
export default {
  mounted() {
    const cursor = document.querySelector(".cursor");

    this.onMouseMove = (e) => {
      cursor.style.left = `${e.clientX}px`;
      cursor.style.top = `${e.clientY}px`;
    };

    this.onMouseOver = (e) => {
      if (e.target.closest("a, button, .impossible")) {
        cursor.style.transform = "translate(-50%, -50%) scale(1.4)";
      }
    };

    this.onMouseOut = (e) => {
      if (e.target.closest("a, button, .impossible")) {
        cursor.style.transform = "translate(-50%, -50%) scale(1)";
      }
    };

    window.addEventListener("mousemove", this.onMouseMove);
    document.addEventListener("mouseover", this.onMouseOver);
    document.addEventListener("mouseout", this.onMouseOut);
  },
  beforeUnmount() {
    window.removeEventListener("mousemove", this.onMouseMove);
    document.removeEventListener("mouseover", this.onMouseOver);
    document.removeEventListener("mouseout", this.onMouseOut);
  },
  components: {
    Navbar,
    Footer,
  },
};
</script>

<style>
* {
  cursor: none !important;
}

/* Main cursor container */
.cursor {
  position: fixed;
  top: 0;
  left: 0;
  width: 88px;
  height: 88px;
  pointer-events: none;
  z-index: 9999;
  transform: translate(-50%, -50%);
  transition: transform 0.18s cubic-bezier(0.4, 0, 0.2, 1), opacity 0.2s ease;
}

/* Solid outer ring */
.cursor::before {
  content: "";
  position: absolute;
  inset: 0;
  border-radius: 50%;
  border: 2px solid rgba(125, 211, 252, 0.85);
  box-shadow: 0 0 22px rgba(125, 211, 252, 0.35),
    inset 0 0 14px rgba(167, 139, 250, 0.35);
}

/* Inner ring */
.cursor-inner-ring {
  position: absolute;
  inset: 9px;
  border-radius: 50%;
  border: 1px solid rgba(167, 139, 250, 0.9);
  box-shadow: inset 0 0 10px rgba(167, 139, 250, 0.4);
}

/* Center dot (static relative to cursor) */
.cursor-dot {
  position: absolute;
  top: 50%;
  left: 50%;
  width: 8px;
  height: 8px;
  background: #7dd3fc;
  border-radius: 50%;
  transform: translate(-50%, -50%);
  box-shadow: 0 0 10px rgba(125, 211, 252, 0.8);
}
#app {
  overflow-x: hidden;
}
body {
  background-color: black;
  height: 100%;
  /* margin-top: 50px; */
  margin-bottom: 70px;
}
::-webkit-scrollbar {
  width: 5px;
}
::-webkit-scrollbar-track {
  border-radius: 50px;
  background: black;
  border: 1px solid rgba(167, 139, 250, 0.9);
}
::-webkit-scrollbar-thumb {
  background: #7dd3fc;
  border-radius: 10px;
}
::-webkit-scrollbar-thumb:hover {
  background: rgba(167, 139, 250, 0.4);
  border: 1px solid black;
}

/* Cursor responsive media queries */

/* Smaller desktops / tablets */
@media (max-width: 1024px) {
  .cursor {
    width: 60px;
    height: 60px;
  }

  .cursor::before {
    border-width: 1.5px;
    box-shadow: 0 0 16px rgba(125, 211, 252, 0.35),
      inset 0 0 10px rgba(167, 139, 250, 0.35);
  }

  .cursor-inner-ring {
    inset: 6px;
    border-width: 1px;
    box-shadow: inset 0 0 8px rgba(167, 139, 250, 0.4);
  }

  .cursor-dot {
    width: 6px;
    height: 6px;
    box-shadow: 0 0 8px rgba(125, 211, 252, 0.8);
  }
}

/* Small tablets / large phones */
@media (max-width: 768px) {
  .cursor {
    width: 48px;
    height: 48px;
  }

  .cursor::before {
    border-width: 1px;
    box-shadow: 0 0 12px rgba(125, 211, 252, 0.3),
      inset 0 0 6px rgba(167, 139, 250, 0.25);
  }

  .cursor-inner-ring {
    inset: 4px;
    border-width: 1px;
    box-shadow: inset 0 0 6px rgba(167, 139, 250, 0.3);
  }

  .cursor-dot {
    width: 5px;
    height: 5px;
    box-shadow: 0 0 6px rgba(125, 211, 252, 0.7);
  }
}

/* Phones / very small screens */
@media (max-width: 480px) {
  .cursor {
    display: none; /* hide cursor on touch devices */
  }
}
</style>
