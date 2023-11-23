<template>
      <footer class="footer fixed-bottom">
        <!-- <div class="copyright-area">
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
                                <li><router-link class="nav-link" to="/">Home</router-link></li>
                                <li><router-link class="nav-link" to="/Contact">Contact</router-link></li>
                            <div class="footer-social-icon">
                                <h4>Follow Me:</h4>
                                <li><a href="https://www.facebook.com/profile.php?id=100085302518838" target="_blank"><i class="fab fa-facebook-f facebook-bg"></i></a></li>
                                <li><a href="https://twitter.com/ASHTON_M_DB9" target="_blank"><i class="fab fa-twitter twitter-bg"></i></a></li>
                                <li><a href="https://www.instagram.com/ashton.m_db9/" target="_blank"><i class="fa-brands fa-instagram"></i></a></li>
                                <li><a href="https://github.com/ASHTONMDB9" target="_blank"><i class="fa-brands fa-github"></i></a></li>
                                <li><a href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/" target="_blank"><i class="fa-brands fa-linkedin"></i></a></li>
                            </div>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div> -->


<div class="copyright-area">
            <div class="container">
                <div class="row">
                    <div class="col-xl-6 col-lg-6 text-center text-lg-left">
                        <div class="copyright-text">
                            <p>Ashton Abrahams Copyright &copy; 2021, All Right Reserved</p>
                        </div>
                    </div>
                    <div class="col-xl-6 col-lg-6 d-none d-lg-block text-right">
                        <div class="footer-menu">
                            <ul>
                                <li><router-link class="nav-link" to="/">Home</router-link></li>
                                <li><router-link class="nav-link" to="/Contact">Contact</router-link></li>

                                <li><p>Follow Me:</p></li>
                                <li><a href="https://www.facebook.com/profile.php?id=100085302518838" target="_blank"><i class="fab fa-facebook-f facebook-bg"></i></a></li>
                                <li><a href="https://twitter.com/ASHTON_M_DB9" target="_blank"><i class="fab fa-twitter twitter-bg"></i></a></li>
                                <li><a href="https://www.instagram.com/ashton.m_db9/" target="_blank"><i class="fa-brands fa-instagram"></i></a></li>
                                <li><a href="https://github.com/ASHTONMDB9" target="_blank"><i class="fa-brands fa-github"></i></a></li>
                                <li><a href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/" target="_blank"><i class="fa-brands fa-linkedin"></i></a></li>
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
<style scoped>

ul {
    margin: 0px;
    padding: 0px;
    /* top: 0px;
    bottom: 0px; */
}
.footer-section {
  background-attachment: fixed;
}
.copyright-area{
  background: #202020;
  padding-top: 25px;
  padding-bottom: 20px;
}
.copyright-text p {
  margin: 0;
  font-size: 14px;
  color: #878787;
}
.copyright-text p a{
  color: #ff5e14;
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
p {
  color: white;
  display: inline-block;
  font-size: 14px;
}
.footer-social-icon a {
  color: white;
  font-size: 16px;
}
.footer-social-icon i {
  height: 100px;
  width: 40px;
  font-size: 25px;
  text-align: center;
  line-height: 38px;
  border-radius: 50%;
}
.footer-social-icon i:hover {
  transform: scale(1.2);
  transition: all 1.5 linear smooth;
}

</style>