<template>
<Navbar/>
  <router-view/>
  <Footer/>
</template>


<script>
import Navbar from "./components/Navbar.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    Navbar,
    Footer
  },
};
</script>


<style>
#app {
  overflow-x: hidden;
}
body {
  background-color: black;
  height: 100%;
  margin-top: 80px;
  margin-bottom: 100px;
}
::-webkit-scrollbar {
  width: 5px;
}
::-webkit-scrollbar-track {
  border-radius: 50px;
  background: black;
  border: 1px solid blue;
}
::-webkit-scrollbar-thumb {
  background: blue; 
  border-radius: 10px;
}
::-webkit-scrollbar-thumb:hover {
  background: blue; 
  border: 1px solid black;
}
</style>
 