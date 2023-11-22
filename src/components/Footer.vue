<template>
      <footer>
          <div class="copyright-area">
            <div class="container">
                <div class="row">
                    <div class="col-xl-6 col-lg-6 text-center text-lg-left">
                        <div class="copyright-text">
                            <p>Ashton Abrahams Copyright &copy; 2022, All Right Reserved</p>
                        </div>
                    </div>
                    <div class="col-xl-6 col-lg-6 d-none d-lg-block text-right">
                        <div class="footer-menu">
                            <ul>
                                <li><router-link to="/">Home</router-link></li>
                                <li><router-link to="/Contact">Contact</router-link></li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
      </footer>
</template>
<script>
export default {
    components: {

 }
}
</script>
<style>
footer {
    margin-top: 30px;
}

.copyright-area{
  background: black;
  padding: 25px 0;
}
.copyright-text p {
  /* margin: 0; */
  font-size: 14px;
  color: #878787;
}
.footer-menu li {
  display: inline-block;
  margin-left: 20px;
}
.footer-menu li:hover a{
  color: blue;
}
.footer-menu li a {
  font-size: 14px;
  color: #878787;
}    
</style>