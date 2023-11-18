<template>
  <div class="tabs">
    <ul class="nav nav-tabs">
      <li class="nav-item">
        <router-link class="nav-link" aria-current="page" to="/About"><h6>Bio</h6></router-link>
      </li>
      <li class="nav-item">
        <router-link class="nav-link active" to="/Skills"><h6>Skills</h6></router-link>
      </li>
    </ul>
  </div>
  
  <h1 class="softskills">Soft-Skills</h1>
  
  <div class="container mt-3">
    <div class="row">
      <div class="col-md">
      <div class="ui-widgets">
      <div class="ui-values">90%</div>
      <div class="ui-labels">Communication</div>
      </div>
  </div>
      <div class="col-md">
      <div class="ui-widgets">
      <div class="ui-values">75%</div>
      <div class="ui-labels">Problem-solving</div>
      </div>
  </div>
      <div class="col-md">
      <div class="ui-widgets">
      <div class="ui-values">80%</div>
      <div class="ui-labels">Creativity</div>
      </div>
  </div>
    <div class="col-md">
  <div class="ui-widgets">
      <div class="ui-values">85%</div>
      <div class="ui-labels">Teamwork</div>
    </div>
  </div>
    </div>
  </div>



  <h1 class="softskills">Technical Skills</h1>


  <div class="container">
    <div class="row">
      <div class="card text-light bg-black mb-4 mt-2">
        <div class="card-header text-center">HTML</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-html5"></i></h5>
    <p class="card-text text-center">HTML is the standard markup language for creating Web pages. 
       HTML describes the structure of a Web page.</p>
  </div>
</div>
    </div>
    <div class="row">
    <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">CSS</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-css3"></i></h5>
    <p class="card-text text-center">CSS is the language we use to style an HTML document. 
      CSS describes how HTML elements should be displayed.</p>
  </div>
</div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">BOOTSTRAP</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-bootstrap"></i></h5>
    <p class="card-text text-center">Bootstrap is a powerful, feature-packed frontend toolkit. 
      Build anything from prototype to production in minutes.</p>
  </div>
</div>
    </div>
  </div>
  
<div class="row">
  <div class="col-md">
      <div class="card text-light bg-black mb-2">
        <div class="card-header text-center">MySQL</div>
        <div class="card-body">
          <h5 class="card-title text-center"><i class="fa-solid fa-database"></i></h5>
          <p class="card-text text-center">MySQL is a relational database management system (RDBMS) developed by Oracle that is based on structured query language (SQL).</p>
        </div>
      </div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-2">
  <div class="card-header text-center">JAVASCRIPT</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-js"></i></h5>
    <p class="card-text text-center">Javascript is a scripting language, primarily used on the Web. 
      It is used to enhance HTML pages and is commonly found embedded in HTML code.</p>
  </div>
</div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-2">
  <div class="card-header text-center">VUE JS</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-vuejs"></i></h5>
    <p class="card-text text-center"> Vue is a JavaScript framework for building user interfaces. 
      It builds on top of standard HTML, CSS and JavaScript.</p>
  </div>
</div>
    </div>
</div>
<div class="row">
  <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">Node/ Node JS</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-node"></i>/<i class="fa-brands fa-node-js"></i></h5>
    <p class="card-text text-center">NodeJs is a runtime environment for executing JS code outside of the browser, 
      it is build upon Chrome v8 engine using c++.</p>
  </div>
</div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">WordPress</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-wordpress"></i></h5>
    <p class="card-text text-center">WordPress is the simplest, most popular way to create your own website or blog. 
      It makes building a website accessible to anyone, even people who aren't developers.</p>
  </div>
</div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">SEO</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-searchengin"></i></h5>
    <p class="card-text text-center">Search Engine Optimization (SEO) is the 
      process of getting traffic from free, organic, editorial, or natural search results in search engines.</p>
  </div>
</div>
    </div>
    <div class="col-md">
        <div class="card text-light bg-black mb-4 mt-2">
  <div class="card-header text-center">PHP</div>
  <div class="card-body">
    <h5 class="card-title text-center"><i class="fa-brands fa-php"></i></h5>
    <p class="card-text text-center">PHP is a server scripting language, and a powerful tool 
      for making dynamic and interactive Web pages.</p>
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
.card:hover {
  box-shadow: -5px -5px 10px 5px blue, 5px 5px 10px 5px blue;
  transform: scale(1.1);
  transition: all 0.5s linear;
  z-index: 20;
}
.card-header {
    font-size: 20px;
    text-decoration: underline 3px;
    text-decoration-color: blue;
    box-shadow: -5px -5px 10px 5px blue, 5px 5px 10px 5px blue;
}
.card h5 {
    font-size: 50px
}
h5 i {
  color: blue;
}
.softskills {
  display: flex;
  justify-content: center;
  margin-top: 20px;
  margin-bottom: 40px;
  color: white;
  text-decoration: underline 3px;
  text-decoration-color: blue;
}
.ui-widgets {
    position: relative;
    display: inline-block;
    width: 10rem;
    height: 10rem;
    border-radius: 9rem;
    margin-left: 70px;
    margin-bottom: 50px;
    border: 1.2rem solid blue;
    box-shadow: inset 0 0 7px white;
    border-left-color: darkblue;
    border-top-color: blue;
    border-right-color: darkblue;
    border-bottom-color: blue;
    text-align: center;
    box-sizing: border-box;
}
.ui-widgets:hover {
  box-shadow: -5px -5px 10px 5px white, 5px 5px 10px 5px white;
  transform: scale(1.1);
  transition: all 0.5s linear;
  z-index: 20;
}
.ui-widgets .ui-values {
    top: 30px;
    position: absolute;
    left: 10px;
    right: 0;
    color: white;
    font-weight: 700px;
    font-size: 2.0rem;
}
.ui-widgets .ui-labels {
    left: 0;
    bottom: 25px;
    text-shadow: 0 0 4px grey;
    color: white;
    position: absolute;
    width: 100%;
    font-size: 12px;
}
</style>