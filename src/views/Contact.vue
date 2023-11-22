<template>
    <!-- <div class="container-fluid">
        <div class="row">
        <div class="col-md">
            <h1 id="contact">Contact Me</h1>
            <img id="avatar" class="img-fluid" src="https://i.postimg.cc/3xxzjYqM/ash2-removebg-preview-contact.png">
            <div class="social">
                        <a href="https://www.facebook.com/profile.php?id=100083321873494" target="_blank"><i class="fa fa-facebook"></i></a>
                        <a href="https://www.instagram.com/ashton.m_db9/" target="_blank"><i class="fa fa-instagram"></i></a>
                        <a href="https://github.com/ASHTONMDB9" target="_blank"><i class="fa fa-github"></i></a>
                        <a href="https://www.linkedin.com/in/ashton-abrahams-0bb921237/" target="_blank"><i class="fa fa-linkedin"></i></a>
                    </div>
                    <p class="text text-light mt-4">If you have something you want to discuss, contact me or leave your details.</p>
                    <form action="https://formspree.io/f/mzboygza" method="POST">
                        <input type="text" name="Name" required placeholder=" your name">
                        <input type="email" name="Email" required placeholder="your email">
                        <input type="tel" name="Phone" placeholder="your phone">
                        <input type="text" name="Subject" required placeholder="subject">
                        <textarea type="text" name="Message" placeholder="your message"></textarea>
                        <button>send</button>
                    </form>
                </div>
                <div class="col-md-5">
                    <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3308.2675928504113!2d18.490509915821583!3d-33.985659832565865!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x1dcc433bedd50e81%3A0x9c746d268c8e0ad9!2sLife%20Choices!5e0!3m2!1sen!2sza!4v1658296857775!5m2!1sen!2sza" width="700" height="780" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>
                </div>
                </div>
    </div> -->






<div class="container">
                <div class="contact-parent">
                    <div class="contact-child child1">
                        <p>
                            <i class="fas fa-map-marker-alt"></i> Address <br />
                            <span> Lukas Street 08
                                <br />
                                Cape Town, SA
                            </span>
                        </p>

                        <p>
                            <i class="fas fa-phone-alt"></i> Let's Talk <br />
                            <span> 068 196 6648</span>
                        </p>

                        <p>
                            <i class=" far fa-envelope"></i> Queries <br />
                            <span>ashtonabrahams563@gmail.com</span>
                        </p>
                    </div>

                    <div class="contact-child child2">
                        <div class="inside-contact">
                            <h2>Contact Me</h2>
                            <h3>
                               <span id="confirm"></span>
                            </h3>
                         <form action="https://formspree.io/f/mzboygza" method="POST">
                            <p>Name *</p>
                            <input type="text" name="Name" required placeholder=" your name">

                            <p>Email *</p>
                            <input type="email" name="Email" required placeholder="your email">

                            <p>Phone *</p>
                            <input type="tel" name="Phone" placeholder="your phone">

                            <p>Subject *</p>
                            <input type="text" name="Subject" required placeholder="subject">

                            <p>Message *</p>
                            <textarea type="text" name="Message" placeholder="your message"></textarea>
                            
                            <button>send</button>
                            </form>
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

.contact-parent{
    display:flex;
    margin:80px 0;
}

.contact-child{
    display:flex;
    flex:1;
    box-shadow:0px 0px 10px -2px rgba(0,0,0,0.75);
}

.child1{
    background:linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url("https://cdn.pixabay.com/photo/2019/06/28/00/17/architecture-4303279_1280.jpg");
    background-size:cover;
    display:flex;
    flex-direction:column;
    justify-content:space-around;
    color:#fff;
    padding:100px 0;
}

.child1 p{
    padding-left:20%;
    font-size:20px;
    text-shadow:0px 0px 2px #000;
}

.child1 p span{
    font-size:16px;
    color:#9df2fd;
}

.child2{
    flex-direction:column;
    justify-content:space-around;
    align-items:center;
    background-color: gray;
}

.inside-contact{
    width:90%;
    margin:0 auto;
}

.inside-contact h2{
    text-transform:uppercase;
    text-align:center;
    margin-top:50px;
}

.inside-contact h3{
    text-align:center;
    font-size:16px;
    color:#0085e2;
}

.inside-contact input, .inside-contact textarea{
    width:100%;
    background-color:#eee;
    border:1px solid rgba(0,0,0,0.48);
    padding:5px 10px;
    margin-bottom:20px;
}

.inside-contact input[type=submit]{
    background-color:#000;
    color:#fff;
    transition:0.2s;
    border:2px solid #000;
    margin:30px 0;
}

.inside-contact input[type=submit]:hover{
    background-color:#fff;
    color:#000;
    transition:0.2s;
}

@media screen and (max-width:991px){
    .contact-parent{
        display:block;
        width:100%;
    }

    .child1{
        display:none;
    }

    .child2{
        background-image:linear-gradient(rgba(255,255,255,0.7),rgba(255,255,255,0.7)), url("https://cdn.pixabay.com/photo/2019/06/28/00/17/architecture-4303279_1280.jpg");
        background-size:cover;
    }

    .inside-contact input, .inside-contact textarea{
        background-color:#fff;
    }
}





/* .container-fluid {
    text-align: center;
    display: flex;
    flex-direction: column;
}
#contact {
    color: white;
    margin-top: 150px;
    text-decoration: underline 3px;
    text-decoration-color: blue;
}
.container-fluid .social {
    margin-top: 40px;
    display: flex;
    justify-content: center; 
}
.container-fluid .social i {
    width: 55px;
    color: blue;
    height: 55px;
    border-radius: 50%;
    border: 1px solid blue;
    line-height: 55px;
    font-size: 25px;
    transition: .5s ease;
    margin-right: 20px;
}
.container-fluid .social a {
    margin-right: 20px;
}
.container-fluid .social i:last-child {
    margin-right: 0;
}
.container-fluid .social i:hover {
    border-color: blue;
    box-shadow: 0 0 20px blue;
    transform: scale(1.2)
}
.container-fluid form {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}
.container-fluid form input {
    height: 40px;
    background-color: transparent;
    padding: 5px 0px;
    border: 0;
    border-bottom: 1px solid blue;
    margin-bottom: 30px;
    color: white;
}
.container-fluid form textarea {
    background-color: transparent;
    padding: 5px 0px;
    border: 0;
    border: 1px solid black;
    margin-bottom: 30px;
    height: 187px;
    width: 100%;
    color: white;
}
.container-fluid form input::-webkit-input-placeholder,
.container-fluid form textarea::-webkit-input-placeholder {
    color: blue;
    text-transform: capitalize;
}
.container-fluid form [name="name"],
.container-fluid form [name="email"],
.container-fluid form [name="phone"] {
    width: 31%;
}
.container-fluid form [name="subject"] {
    width: 100%;
    margin-bottom: 80px;
}
.container-fluid form input,textarea:focus {
    outline: none;
}
.container-fluid form button {
    background-color: transparent;
    padding: 10px 0;
    width: 100%;
    border: 1px solid blue;
    color: blue;
    text-transform: uppercase;
    overflow: hidden;
}
.container-fluid form button:hover {
    color: blue;
    border-color: blue;
    box-shadow: 0 0 20px blue;
} */
/* iframe {
    padding-right: 10px;
    margin-top: 120px;
    filter: invert(100%);
} */
</style>