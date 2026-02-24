<template>
  <section class="gallery">
    <h1 id="Art">Gallery</h1>
    <p v-if="windowWidth <= 996" class="hint">Scroll to view each image</p>
    <p v-else class="hint">Use the arrows to view each image</p>
    
    <!-- Mobile/Tablet grid -->
    <div v-if="windowWidth <= 996" class="mobile-gallery-grid">
      <div v-for="(item, index) in gallery" :key="index" class="mobile-box">
        <img :src="item.img" :alt="item.title" />
        <div class="label">{{ item.title }}</div>
      </div>
    </div>
    
    <div v-else class="gallery-wrap">
      <button class="side-btn left" @click="prev">←</button>
      
      <div class="container-fluid">
        <div class="container" :style="gridStyle">
          <div
            v-for="(item, index) in gallery"
            :key="index"
            class="box"
            :style="{ '--img': `url(${item.img})` }"
          >
            <div class="label" v-if="activeIndex === index">
              {{ item.title }}
            </div>
          </div>
        </div>
      </div>

      <button class="side-btn right" @click="next">→</button>
    </div>
    
    <router-link to="/About">
      <button class="work w-100"><h6>Back</h6></button>
    </router-link>
  </section>
</template>

<script>
export default {
  data() {
    return {
      activeIndex: 0,
      windowWidth: window.innerWidth,
      gallery: [
        {
          img: "https://i.postimg.cc/BQ9qkJ7s/Itachi.jpg",
          title: "Itachi of the Sharingan",
        },
        {
          img: "https://i.postimg.cc/Ls1cS1bs/Androids.jpg",
          title: "The Terrifying Androids",
        },
        {
          img: "https://i.postimg.cc/d3HHrsxX/Victoria.jpg",
          title: "The Victoria",
        },
        {
          img: "https://i.postimg.cc/KzxWBsJ6/Pan.jpg",
          title: "Pan, Daughter of Gohan",
        },
        { img: "https://i.postimg.cc/nLv5stYK/Muminah.jpg", title: "Sunshine" },
        {
          img: "https://i.postimg.cc/tJCvsZ2W/Vegito.jpg",
          title: "Rivals Unite",
        },
        {
          img: "https://i.postimg.cc/HW2fTHBb/Levi.jpg",
          title: "I Heart Eren Jaeger",
        },
        {
          img: "https://i.postimg.cc/NF0PP2hb/Trunks.jpg",
          title: "The warrior of Hope",
        },
        {
          img: "https://i.postimg.cc/pTQ3htxb/Issues.jpg",
          title: "Summertime Sadness",
        },
        {
          img: "https://i.postimg.cc/YChcXVNY/Dreams.jpg",
          title: "The Hopes and Dreams of One Sir Alex",
        },
        {
          img: "https://i.postimg.cc/yxFzsSpK/vegeta.jpg",
          title: "The Almighty Prince Vegeta",
        },
        {
          img: "https://i.postimg.cc/cLjpPmTj/Alex.jpg",
          title: "He Who Once Was",
        },
        {
          img: "https://i.postimg.cc/FHfqbSmx/Marshmellow.jpg",
          title: "What Is That Mellow-dy?",
        },
        {
          img: "https://i.postimg.cc/d1FxKSCW/Obtio.jpg",
          title: "I Don't Need The Blood Stains To Match My Eyes",
        },
        {
          img: "https://i.postimg.cc/W38Hn6yh/Gogeta.jpg",
          title: "The Angel Born In Hell",
        },
        {
          img: "https://i.postimg.cc/1zwj2Z8n/Meliodas.jpg",
          title: "The Dragon Sin of Wrath",
        },
        {
          img: "https://i.postimg.cc/0QCH5dd9/Skyline.jpg",
          title: "The Japanese Dream",
        },
        {
          img: "https://i.postimg.cc/YCJPdSCB/Mini.jpg",
          title: "Miniature Victory",
        },
        {
          img: "https://i.postimg.cc/gJbf22CH/Gohan.jpg",
          title: "Fight you? No, I wanna kill you",
        },
        {
          img: "https://i.postimg.cc/Fz980nsf/Kirito.jpg",
          title: "Alex Goes Down The Rabbit Hole",
        },
        {
          img: "https://i.postimg.cc/ZnVgHFCw/Land-Rover.jpg",
          title: "Classy and Comfortable",
        },
        {
          img: "https://i.postimg.cc/Kv8CzVHw/Love.jpg",
          title: "Love Is Blind, Deaf and Dumb",
        },
      ],
    };
  },
  computed: {
    gridStyle() {
      const cols = this.gallery
        .map((_, i) => (i === this.activeIndex ? "220fr" : "10fr"))
        .join(" ");

      return {
        gridTemplateColumns: cols,
      };
    },
  },
  mounted() {
    window.addEventListener("resize", this.handleResize);
  },
  beforeUnmount() {
    window.removeEventListener("resize", this.handleResize);
  },
  methods: {
    handleResize() {
      this.windowWidth = window.innerWidth;
    },
    next() {
      this.activeIndex = (this.activeIndex + 1) % this.gallery.length;
    },
    prev() {
      this.activeIndex =
        (this.activeIndex - 1 + this.gallery.length) % this.gallery.length;
    },
  },
};
</script>

<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.gallery {
  padding-top: 50px;
  text-align: center;
}

#Art {
  color: #f3f4f6;
  margin-top: 40px;
  text-decoration: underline 3px;
  text-decoration-color: #60a5fa;
}

.hint {
  color: #a7a7b3;
  margin-top: 10px;
}

.gallery-wrap {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
  margin-top: 30px;
}

.side-btn {
  border: 1px solid #60a5fa;
  background: rgba(0, 0, 0, 0.6);
  color: #60a5fa;
  padding: 14px 18px;
  border-radius: 999px;
  cursor: pointer;
  transition: all 0.3s ease;
}

.side-btn:hover {
  background: rgba(96, 165, 250, 0.18);
}

.container-fluid {
  flex: 1;
  display: flex;
  justify-content: center;
}

.container {
  display: grid;
  gap: 10px;
  width: 900px;
  height: 520px;
  transition: all 400ms;
}

.box {
  position: relative;
  background: var(--img) center center no-repeat;
  background-size: cover;
  border-radius: 6px;
  overflow: hidden;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.35);
  margin-bottom: 20px;
}

.label {
  position: absolute;
  bottom: 18px;
  left: 5px;
  background: rgba(0, 0, 0, 0.7);
  color: #60a5fa;
  padding: 10px 12px;
  letter-spacing: 2px;
  text-transform: uppercase;
  border-radius: 6px;
}

.box:nth-child(odd) {
  transform: translateY(-16px);
}

.box:nth-child(even) {
  transform: translateY(16px);
}

.work {
  margin-bottom: 20px;
  margin-top: 20px;
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

@media (max-width: 996px) {
  /* --- Mobile/Tablet grid --- */
  .mobile-gallery-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 12px;
    width: 95%;
    margin: 0 auto;
    margin-top: 20px;
  }

  .mobile-box {
    position: relative;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 6px 20px rgba(0, 0, 0, 0.25);
  }

  .mobile-box img {
    width: 100%;
    height: auto;
    display: block;
  }

  .mobile-box .label {
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    padding: 8px 12px;
    background: rgba(0, 0, 0, 0.65);
    color: #60a5fa;
    text-align: left;
    text-transform: uppercase;
    font-size: 0.85rem;
    border-top-right-radius: 6px;
  }

  /* --- Back button --- */
  .work {
    margin-top: 20px;
    margin-bottom: 100px;
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
}
</style>
