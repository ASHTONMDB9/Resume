<template>
<div class="container">
  <video autoplay muted loop id="land">
  <source src="../images/Landing.mp4" type="video/mp4">
</video>
    <div><h1>Hi, my name is</h1>
    <h1>Ashton Abrahams</h1></div>
    <h2 class="text text-center mt-1">Aspiring Full-Stack Developer</h2>
    <h3 class="text text-center mt-1">Nothing is <span class="impossible"><span>'I</span>M<span>POSSIBLE'</span></span></h3>
    <p class="text-white text-center">Hover between quotes for animation</p>
    </div>
</template>


<script>
export default {
  
}
</script>
<style scoped>
#land {
  position: fixed;
  z-index: -5;
  right: 0;
  bottom: 0;
  min-width: 100%;
  min-height: 100%;
}
.container {
  margin-top: 285px;

}
.container h1:nth-child(1) {
  color: white;
  font-weight: 800;
  font-size: 30px;
  margin: 0 auto auto auto;
  white-space: nowrap;
  overflow: hidden;
  width: 230px;
  animation: type 2s steps(40,end) forwards;
}
.container h1:nth-child(2) {
  display: flex;
  justify-content: center;
  opacity: 0;
  font-family: sans-serif;
  margin: 0 auto auto auto;
  background: linear-gradient( black, blue, black);
  font-weight: 800;
  font-size: 50px;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  overflow: hidden;
  animation: move-animation 2.2s steps(40,end) 2s forwards, blink .5s step-end infinite alternate;
}
@keyframes move-animation {
  0% {
    background-position: 0 0;
    opacity: 0;
    width: 0;
  }
  1% {
    background-position: 0 0;
    opacity: 1;
    border-right: 1px solid black;
  }
  50% {
    background-position: 150px 0;
    opacity: 1;
    border-right: 1px solid black;
  }
  100% {
    background-position: 500px 0;
    opacity: 1;
    border-right: 1px solid black;
  }
}
@keyframes type {
  0% {
    width: 0;
  }
  1%, 99%{
    border-right: 1px solid black;
  }
  100%{
    border-right: none;
  }
}

@keyframes blink {
  50% {
    border-color: transparent;
  }
}
h2 {
  color: grey;
  text-shadow: 0 0 10px blue, 0 0 20px blue, 0 0 40px blue;
}
h3{
  color: red;
  padding-top: 20px;
  font-weight: bold;
  font-family: monospace;
  letter-spacing: 7px;
}
h3 span{
  transition: .5s linear
}
h3:hover span:nth-child(1){
  margin-right: 5px
}
h3:hover span:nth-child(2){
  margin-left: 30px
}
.impossible:hover {
  color: #fff;
  text-shadow: 0 0 10px #fff, 0 0 20px #fff, 0 0 40px #fff;
}
</style>
