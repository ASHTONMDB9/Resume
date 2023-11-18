<template>
<div class="tabs">
<ul class="nav nav-tabs">
  <li class="nav-item">
    <router-link class="nav-link" aria-current="page" to="/Resume"><h6>Resume</h6></router-link>
  </li>
  <li class="nav-item">
    <router-link class="nav-link  active" to="/Testimonials"><h6>Testimonials</h6></router-link>
  </li>
</ul>

</div>

<div class="container-fluid">
<div id="tests" class="" v-for="testimonial of testimonials" :key="testimonial.id">
<div id="list" class="card text-light mt-3 ms-2 me-2" style="width: 22rem; height: 25rem;">
    <img id="propic" v-bind:src="testimonial.image" class="face face--front card-img" style="height: 25rem; object-fit: cover;">
    <div class="card-body">
    <h2 class="face face--back card-title mt-5">{{ testimonial.name }}</h2>
    <p class="face face--back">{{ testimonial.testimony }}</p>
    </div>
    </div>
</div>
</div>
</template>
<script>
export default {
  data() {
    return {
    testimonials : [
      {
        id: "1",
        image: "https://i.postimg.cc/L5vZ8fZJ/Carla-1-1-removebg-preview.png",
        name: "Carla Lawrence",
        testimony: "Ashton Abrahams is an excellent addition to any team. He is a without a doubt a very skilled web developer. Ashton's ability to integrate beautiful design and web functionality is outstanding. I count myself lucky to have had him as a colleague for his pleasant disposition and humorous character.",
        role: "Colleague"

      },
      {
        id: "2",
        image: "https://i.postimg.cc/Hsq7spr4/Ricardo-1-removebg-preview.png",
        name: "Ricardo Moses",
        testimony: "Ashton is a diligent worker, always stays focused and works hard. He's kind and open-minded personality makes him a pleasure to be around in a work environment.",
        role: "Colleague",

      },      
      {
        id: "3",
        image: "https://i.postimg.cc/5Nbk6MDv/T02-LW4-RMXJQ-U036-JA3-NVL5-45897a34dc43-512-removebg-preview.png",
        name: "Jason Wandrag",
        testimony: "I think Ashton Abrahams is a very consistent student. When he is confident about the answer, he loves participating in class. As long as he focuses in class, Ashton Abrahams will improve steadily.",
        role: "Lecturer",

      },
      {
        id: "4",
        image: "https://i.postimg.cc/j2tzjMWQ/Mika-Rinquest-removebg-preview.png",
        name: "Mika Rinquest",
        testimony: "Once Ashton starts working he does not allow for any distractions. He fits in well with others and has the potential to be a valuable member of any team.",
        role: "Colleague",

      },
      {
        id: "5",
        image: "https://i.postimg.cc/LsPbJkBQ/Zoe-3-1-removebg-preview.png",
        name: "Zoe Van Der Schyff",
        testimony: "Ashton is one of the smartest, hard-working people I know. He tries over and over until he gets it right. He will strive until he gets what he needs, and he will do what he needs to do to get things done.",
        role: "Colleague",
      },      
      {
        id: "6",
        image: "https://i.postimg.cc/vmFMDHFM/Chanique-1-removebg-preview.png",
        name: "Chanique Mansoor",
        testimony: "Ashton is a true example of a leader and strives in everything he does, his personality and persona is something I could only aspire to have. Wishing him all the best with his future as a developer.",
        role: "Colleague",
      },
      {
        id: "7",
        image: "https://i.postimg.cc/bvwmFpzV/1663691506237-removebg-preview.png",
        name: "Jesse Spence",
        testimony: "Ashton is extremely creative, artistic and has a great eye for design. This combined with his friendly attitude and good communication makes him an incredible person to work with. I am extremely grateful to have worked and learned along side him.",
        role: "Colleague",
      },
      {
        id: "8",
        image: "https://i.postimg.cc/jqXpph9g/Charles4-removebg-preview.png",
        name: "Abdus-Samad Charles",
        testimony: "Ashton is a trustworthy and hardworking individual who enjoys solving problems and helping others. He has a very calm demeaner and is easily approachable.",
        role: "Colleague",
      },
    ]
    }
  }
}
</script>
<style scoped>
.tabs {
  display: flex;
  justify-content: center;
  margin-top: 50px;
  margin-bottom: 35px;
  color: white;
}
.container-fluid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
  gap: 80px;
}
#list{
  position: relative;
  margin: 0.5rem;
  border-radius: 0.8rem;
  background-color: black;
}
#list:hover {
  box-shadow: -5px -5px 10px 5px blue, 5px 5px 10px 5px blue;
  transition: all 0.5s linear;
  z-index: 20;
}
.card-title {
  text-decoration: underline 3px;
  text-decoration-color: blue;
}

.face {
  display: block;
  position: absolute;
  top: 0;
  left: 0;
  border-radius: 0.8rem;
  background-size: cover;
  -webkit-backface-visibility: hidden;
          backface-visibility: hidden;
  transition: transform 0.5s ease-in-out;
}

.face--front {
  background-color: transparent;
}

.face--back {
  margin-top: 150px;
  background-color: black;
  transform: rotateY(180deg);
}

.card:hover .face--front {
  transform: rotateY(-180deg);
}

.card:hover .face--back {
  transform: rotateY(0deg);
}

</style>