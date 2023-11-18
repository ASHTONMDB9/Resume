<template>
    <nav class="navbar navbar-dark navbar-expand-lg bg-dark">
  <div class="container-fluid">
    <a class="navbar-brand">A.A
        <span> ASHTON ABRAHAMS</span>
    </a>
    <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#Toggler" aria-controls="Toggler" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="Toggler">
      <ul class="navbar-nav mb-1 mb-lg-0">
        <li class="nav-item">
          <router-link class="nav-link active" aria-current="page" to="/">Home</router-link>
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
</style>