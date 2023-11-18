<template>
<div class="tabs">
<ul class="nav nav-tabs">
  <li class="nav-item">
    <router-link class="nav-link active" aria-current="page" to="/About"><h6>Bio</h6></router-link>
  </li>
  <li class="nav-item">
    <router-link class="nav-link" to="/Skills"><h6>Skills</h6></router-link>
  </li>
</ul>
</div>

<div class="container">
  <div class="row">
    <div class="col-md-3">
      <img class="img" id="ash2" src="https://i.postimg.cc/1ztMx7TZ/ash2-removebg-preview.png">
    </div>
    <div class="col-md-9 ps-5 text-light">
      <h3 class="about">About Me</h3>
      <span class="details">
      <h4 class="fw-bold">Full name: Ashton Abrahams</h4>
      <h4 class="fw-bold">Date of birth: 07/07/2004</h4>
      <h4 class="fw-bold">Gender: Male</h4>
      </span>
      <p class="lead">Hi there! I'm Ashton. I am consistent and committed. An optimistic and artistic minded person, who has been intrigued and enthusiastic about technology ever since I was six years old.</p>
      <p class="lead">I became interested in everything gaming and everything computers. I am friendly and confident, so working with others won't be a problem. I am always up for a challenge and will work diligently to achieve the goal.</p>
      <p class="lead">I have many hobbies that I enjoy e.g Gaming, Art: drawing/sketching, Making music, Watching anime, Hiking, Being outdoors, Go-karting, Cars, Socialising, Reading, Chess and Paintball</p>
      <p class="share fw-bold">Socials:</p>
    <span class="socials">
       <a href="https://www.facebook.com/profile.php?id=100083321873494" target="_blank"><i class="fa-brands fa-facebook"></i></a>
       <a href="https://www.instagram.com/ashton.m_db9/" target="_blank"><i class="fa-brands fa-instagram"></i></a>
       <a href="https://github.com/ASHTONMDB9" target="_blank"><i class="fa-brands fa-github me-1 ms-1"></i></a>
       <a href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/" target="_blank"><i class="fa-brands fa-linkedin"></i></a>
      </span>
    </div>
    <router-link to="/Gallery"><button class="work w-100"><h6>My Gallery</h6></button></router-link>
  </div>
</div>
</template>

<script>

</script>

<style scoped>
.tabs {
  display: flex;
  justify-content: center;
  margin-top: 50px;
  margin-bottom: 35px;
  color: white;
}
.container {
  margin-top: 100px;
}
#ash2 {
  margin-top: -100px;
}
.about {
  color: white;
  text-decoration: underline;
  text-decoration-color: blue;
  font-size: 40px;
  display: flex;
  flex-direction: column;
}
.details h4 {
  margin-top: 30px;
  margin-bottom: 30px;
}
.share {
  font-size: 20px;
}
.socials i {
  font-size: 30px;
  color: blue;
}
.socials i:hover {
  transform: scale(1.5);
  transition: all 1.5 linear;
}
.socials a {
  margin-right: 10px;
}
.work {
  color: blue;
  height: 40px;
  background-color: black;
  border: 1px solid blue;
}
.work:hover {
  color: black;
  background-color: white;
  border: 1px solid black;
}
</style>
 