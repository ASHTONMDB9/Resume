<template>
<h1 id="project">Projects</h1>

<div class="container-fluid mt-5">
<div v-for="project of projects" :key="project.id">
<div id="list" class="card text-light mt-3 mb-2 ms-2 me-2" style="width: 22rem; height: 25rem;">
    <img id="propic" v-bind:src="project.image" class="card-img" style="height: 23rem; object-fit: cover;">
    <div class="card-img-overlay">
    <h2 class="card-title">{{ project.name }}</h2>
    <p>{{ project.description }}</p>
    <div class="card-footer d-flex mt-3">
    <a :href="project.github" target="_blank" class="card-link"><i class="fa-solid fa-code"> View Code</i></a>
    <a :href="project.live" target="_blank" class="card-link"><i class="fa-solid fa-globe"> View Project</i></a>
  </div>
    </div>
    </div>
</div>
</div>
</template>
<script>
export default {
    data() {
    return {
       projects : [
      {
        id: "1",
        image: "https://i.postimg.cc/d1pR77nn/portfolio.png",
        name: "Mock Portfolio",
        description: "First attemp at making a simple personal portfolio",
        github: "https://github.com/ASHTONMDB9/Realportfolio",
        live: "https://ashtonaflsdev.netlify.app"
      },
      {
        id: "2",
        image: "https://i.postimg.cc/TwpqYjjp/temp.png",
        name: "Temp Converter",
        description: "A temperature converter for converting °C to °F",
        github: "https://github.com/ASHTONMDB9/Temp-calculator",
        live: "https://temp-calculator.netlify.app"
      },      
      {
        id: "3",
        image: "https://i.postimg.cc/ryDQ8TgQ/calc.png",
        name: "Calculator",
        description: "A simple working mathematical JS calculator",
        github: "https://github.com/ASHTONMDB9/Mycalculator",
        live: "https://famous-cannoli-bd8b1e.netlify.app"
      },
      {
        id: "4",
        image: "https://i.postimg.cc/qvxGmvMM/BMI.png",
        name: "BMI Calculator",
        description: "A calculator that calculates you body mass index",
        github: "https://github.com/ASHTONMDB9/BMI-Calculator",
        live: "https://aacalcbmi.netlify.app",
      },
      {
        id: "5",
        image: "https://i.postimg.cc/66FzqPmw/to-do.png",
        name: "To-do List",
        description: "A simple to-do list app for completing tasks",
        github: "https://github.com/ASHTONMDB9/js-todo-list",
        live: "https://magenta-meringue-b58be7.netlify.app",
      },
      {
        id: "6",
        image: "https://i.postimg.cc/mZFFd0nM/phantom.png",
        name: "PhantomRealm",
        description: "A project creating a company website",
        github: "https://github.com/ASHTONMDB9/CAPSTONE-PhantomRealm-Frontend",
        live: "https://capstone-79884.firebaseapp.com/"
      },
      {
        id: "7",
        image: "https://i.postimg.cc/c1tMpm4z/capecoast.png",
        name: "Cape Customs",
        description: "A website with a listing of cars that can be filtered ",
        github: "https://github.com/ASHTONMDB9/WestCoastCustoms",
        live: "https://capecoastcustoms.netlify.app",
      },
      {
        id: "8",
        image: "https://i.postimg.cc/zXmS8gyG/holiday.png",
        name: "Tokyo",
        description: "My favourite holiday destination with a contact page",
        github: "https://github.com/ASHTONMDB9/Holiday-Destination",
        live: "https://my-holiday-destination-tokyo.netlify.app",
      },
      {
        id: "9",
        image: "https://i.postimg.cc/c1Vk2GLN/ecom.png",
        name: "XYZ Tech",
        description: "A team project creating a company website",
        github: "https://github.com/ASHTONMDB9/EOMP",
        live: "https://ecommerce-a994b.firebaseapp.com/#/",
      },
      {
        id: "10",
        image: "https://i.postimg.cc/BnzsYqjK/deliciuous.png",
        name: "Restaurant",
        description: "An online restaurant website made using Bootstrap",
        github: "https://github.com/ASHTONMDB9/delicious",
        live: "https://clever-figolla-e35c78.netlify.app",
      }
    ] 
}
    }
}
</script>
<style scoped>
#project {
    color: white;
    margin-top: 80px;
    text-align: center;
    text-decoration: underline 3px;
    text-decoration-color: blue;
}
.container-fluid {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}
#list{
  background-color: black;
  display: block;
  margin: auto;
}
#list:hover {
  box-shadow: -5px -5px 10px 5px blue, 5px 5px 10px 5px blue;
  transform: scale(1.1);
  transition: all 0.5s linear;
  z-index: 20;
}
#list:hover .card-img {
  filter: opacity(0.2);
}
.card-title {
  text-decoration: underline 3px;
  text-decoration-color: blue;
}
.card-img-overlay {
  opacity: 0;
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
}
.card-img-overlay:hover {
  opacity: 1;
}
</style> 