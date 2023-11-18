<template>
<div class="tabs">
<ul class="nav nav-tabs">
  <li class="nav-item">
    <router-link class="nav-link active" aria-current="page" to="/Resume"><h6>Resume</h6></router-link>
  </li>
  <li class="nav-item">
    <router-link class="nav-link" to="/Testimonials"><h6>Testimonials</h6></router-link>
  </li>
</ul>
</div>


    <div class="resume text-light">
  <header class="text-center">
      <h1>Ashton Abrahams</h1>
      <h2 class="head">Aspiring Full-Stack Developer</h2>
  </header>

  <div class="container mt-4">
  <div class="row">
        <div class="col-md-6">
      <h2 class="head"><i class="fa-solid fa-briefcase"></i> Work Experience</h2>
      <section>
          <h3 class="info">Full-Stack Developer <span class="time">
            <time datetime="2022-03-28" class="start">2022</time>
            &#8211; Present
            </span></h3>
        <p><strong>Life Choices </strong><b>314 Imam Haron Rd, Lansdowne, Cape Town, 7780</b></p>
        <ul>
          <li>Started the Life Choices Academy Coding Course in 2022, class<br/>
             1 of Cohort 10.</li>
          <li>Learnt the basis of coding languages and frameworks such as<br/>
             HTML, CSS, Bootstrap, MySQL, JavaScript, Vue and Node JS.</li>
          <li>Spent 12 months in the course, divided by six months of training<br/> 
          and six months internship.</li>
          <li>Finished a complete 4 month internship/ SEO course with<br/> Grizzly New Marketing.</li>
        </ul>
      </section>
      <h2 class="head"><i class="fa-solid fa-flag"></i> Other Ventures</h2>
      <section>
          <h3 class="info">Leader's Quest <span class="time">
            <time datetime="2020-05-29" class="start">2020</time> &#8211; 
            <time datetime="2020-05-14" class="end">2021</time>
            </span></h3>
        <p><strong>Life Choices </strong><b>314 Imam Haron Rd, Lansdowne, Cape Town, 7780</b></p>
        <ul>
          <li>I was a part of Life Choices' Leader's Quest in<br/>
           2020.</li>
          <li>During the course we were given leadership<br/>
           training and participated in various exercises<br/>
            and activities.</li>
        </ul>
      </section>
      </div>

      <div class="col-md-6">
      <section>
          <h2 class="head"><i class="fa-solid fa-handshake-simple"></i> Volunteer Work</h2>
        <h3 class="info">Volunteered at XO Africa Travel Agency<span class="time">
          <time datetime="2003-07-04">2019</time>
          </span></h3>
        <p><strong>XO Africa </strong><b>9 Somerset Rd, Green Point, Cape Town, 8001</b></p>
        <ul>
            <li>As part of job shadowing, I volunteered at XO Africa who deals with the<br/>
             planning and organisation of events and travelling such as business trips <br/>
             and tours or personal vacations and holidays.</li>
        </ul>
        <h3 class="info">Volunteered at Valhalla Park Public Library <span class="time">
          <time datetime="2002-06-03">2018</time>
          </span></h3>
        <p><strong>Valhalla Park Public Library </strong><b>4 Angela St, Valhalla Park, Cape Town, 7490</b></p>
        <ul>
            <li>I volunteered at my local library and helped pack the shelves and sort through<br/>
             inventory, I served as an assistant assisting the staff with tasks.</li>
        </ul>
      </section>
  
  <div class="resume_skills">
    <aside>
      <section>
        <h2 class="head"><i class="fa-solid fa-graduation-cap"></i> Education</h2>
        <ul>
        <li>Matriculated at Alexander Sinton High School, <span class="time">
          <time datetime="2021-10-16">2016-2021</time>
          </span></li>
        <li>Silverlea Primary School, <span class="time">
          <time datetime="2015-12-14">2009-2015</time>
          </span></li>
        </ul>
      </section>
    </aside>
  </div>
      </div>
  </div>
  </div>
    </div>
</template>

<script>
export default {
    
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
.head {
    color: blue;
}
.info {
    text-decoration: underline;
    text-decoration-color: blue;
    padding-top: 10px;
}
</style>