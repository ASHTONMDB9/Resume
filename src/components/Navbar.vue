<template>
    <nav id="nav" class="navbar navbar-dark navbar-expand-lg fixed-top">
  <div class="container-fluid">
    <a class="navbar-brand w-100"><img style="height: 80px; width: 100;"  src="https://i.postimg.cc/mZ7ptKGr/Ashton-Logo.png">
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Toggler" aria-controls="Toggler" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="Toggler">
      <ul class="navbar-nav mb-1 mb-lg-0">
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
    components: {

    },
    mounted() {
    window.addEventListener('scroll',changeBackground);

function changeBackground(){
  let navbar = document.getElementById("nav");
  let scrollValue = window.scrollY;
  if(scrollValue <10){
    navbar.style.background = "transparent";
    navbar.style.transition = "all 0.5s linear"

    
}else{
    navbar.style.background = "#202020";
}
}
  }
}
</script>

<style>
/*Navbar*/

.navbar-nav {
display: flex;
flex-direction: column;
justify-content: center;
transition: smooth;
align-items: center;
}
.navbar-nav li {
  justify-content: center;
}
.nav-link:hover {
  color: blue;
}
.navbar a.router-link-exact-active {
  color: blue;
  text-decoration: underline overline;
  text-decoration-thickness: 2px;
  text-decoration-color: blue;
}
</style>