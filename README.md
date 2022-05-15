# my-portfolio

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css">
    <link rel="stylesheet" media="screen and (max-width:530px)" href="phone.css">
</head>
<style>
    *{
        margin: 0;
        padding: 0;
        box-sizing: border-box;
    }
    html{
        scroll-behavior: smooth;
    }
    /*navbar */
    .navbar{
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: rgb(0, 0,0,0.5);
        position: sticky;
        top: 0;
    }
    .navbar ul{
        display: flex;
        list-style: none;
        margin: 20px 0px;
    }
    .navbar ui li{
        font-family: century;
        font-size: 1.1rem;
        font-weight: bold;
        font-size: x-large;
    }
    .navbar ul li a{
        text-decoration:rgb(150, 15, 15);
        color:black;
        padding: 8px 25px;
        transition: all .5s ease;
    }
    .navbar ul li a:hover{
        background-color: rgb(255, 255, 255);
        color: black;
        box-shadow: 0 0 10px white;
    }

    /* Home section */
    #home{
        display: flex;
        flex-direction: column;
        background-color: none;
        height: 1000PX;
        justify-content:center;
        align-items:center;
        color:maroon;
        font-size: x-large;
    }
    #home::before{
        content: "";
        position: absolute;
        top: 0;
        right: 0;
        background:url('https://res.cloudinary.com/dsd8yegd2/image/upload/v1648454033/WhatsApp_Image_2022-03-28_at_1.19.13_PM_afrusn.jpg') no-repeat center center/cover;
        height: 1000px;
        width: 100%;
        z-index: -1;
        opacity: .8;
    }
    .main{
        display: flex;
        flex-direction: column;
        border: 1px solid white;
        align-items: center;
        position: absolute;
        top: 30%;
        right: 10%;
    }
    .headings{
        font-family: century;
        font-size: 3rem;
        text-align:center;
        margin: 40px 0px;
    }
    .btn{
        padding: 10x 35px;
        background-color: transparent;
        border: 1px solid white;
        color:black;
        outline: none;
        transition: .6s ease;
    }
    .btn:hover{
        cursor: pointer;
        background-color: white;
        color: black;
        box-shadow: 0 0 5px white,0 0 10px white,0 0 15px white;
        font-weight: bold;
    }

    /*About Selection */
    about{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        padding: 20px;
        margin-bottom: 50px;
    }
    #pic{
        display: flex;
    }
    #pic img{
        width: 575px;
        height: 400px;
    }
    #intro{
        display: flex;
        flex-direction: column;
        text-align: justify;
        padding: 10px;
    }
    #intro h2{
        font-size: 2rem;
        margin-bottom: 20px;
    }

    /* Picture Section */
    #pictures{
        display: flex;
        flex-direction: column;
        background-color: rgba(0, 0, 0, 0.9);
        color: white;
        align-items: center;
        padding: 20px;

    }
    .gallery{
        display: flex;
        flex-wrap: wrap;
        justify-content: space-around;
        box-sizing: border-box;
    }
    .gallery img{
        width: 200px;
        height: 240px;
        margin: 10px;
    }

    /* Skills Section */
    #skills{
        display: flex;
        flex-direction: column-reverse;
        padding: 20px;
        align-items: center;
    }
    .row{
        display: flex;
    }
    .box{
        display: flex;
        flex-direction: column;
        width: 350px;
        height: 450px;
        border: 1px solid black;
        margin: 10px;
        align-items: center;
        text-align: justify;
        padding: 10px;
        border-radius: 15px;
        background: linear-gradient(to top, rgb(16, 15, 15) 50%, white 50%);
        background-size: 100% 200%;
        transition: all .8s;
    }
    .box:hover{
        background-position: left bottom;
        color: rgb(243, 243, 243);
        border: none;
        box-shadow: 0 0 20px rgb(3, 3, 3);
    }
    .box image{
        width: 80px;
        height: 80px;
        background-color: white;
        padding: 10px;
    }

    /* contact section */
    #contact{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        background-color:black;
        color: white;
    }
    .form{
        display: flex;
        flex-direction: column;
        box-sizing: border-box;
        align-items: center;
        margin: 20px 0px;
    }
    .input{
        padding: 12px;
        margin: 15px;
        width: 30%;
        border:none;
        outline: none;
    }
    footer p {
        text-align: center;
    }

    .experience-area h1 {
        padding: 5%;
    }

    .site-footer
    {
        background-color:black;
        padding:45px 0 20px;
        font-size:15px;
        line-height:24px;
        color:#737373;
    }
    .site-footer hr
    {
        border-top-color:#bbb;
        opacity:0.5
    }
    .site-footer hr.small
    {
        margin:20px 0
    }
    .site-footer h6
    {
        color:#fff;
        font-size:16px;
        text-transform:uppercase;
        margin-top:5px;
        letter-spacing:2px
    }
    .site-footer a
    {
        color:#737373;
    }
    .site-footer a:hover
    {
        color:#3366cc;
        text-decoration:none;
    }
    .footer-links
    {
        padding-left:0;
        list-style:none
    }
    .footer-links li
    {
        display:block
    }
    .footer-links a
    {
        color:#737373
    }
    .footer-links a:active,.footer-links a:focus,.footer-links a:hover
    {
        color:#3366cc;
        text-decoration:none;
    }
    .footer-links.inline li
    {
        display:inline-block
    }
    .site-footer .social-icons
    {
        text-align:center
    }
    .site-footer .social-icons a
    {
        width:60px;
        height:52px;
        line-height:40px;
        border-radius:100%;
        background-color:#33353d
    }
    .copyright-text
    {
        margin:0
    }
    @media (max-width:991px)
    {
        .site-footer [class^=col-]
        {
        margin-bottom:30px
        }
    }
    @media (max-width:767px)
    {
        .site-footer
        {
        padding-bottom:0
        }
        .site-footer .copyright-text,.site-footer .social-icons
        {
        text-align:center
        }
    }
    .social-icons
    {
        padding-left:0;
        margin-bottom:0;
        list-style:none
    }
    .social-icons li
    {
        display:inline-block;
        margin-bottom:5px
    }
    .social-icons li.title
    {
        margin-right:15px;
        text-transform:uppercase;
        color:#96a2b2;
        font-weight:700;
        font-size:13px
    }
    .social-icons a{
        position:relative;
        background-color:#eceeef;
        color:#818a91;
        font-size:30px;
        display:inline-block;
        bottom: 20px;
        line-height:44px;
        width:30px;
        height:34px;
        text-align:center;
        margin-right:8px;
        border-radius:100%;
        -webkit-transition:all .2s linear;
        -o-transition:all .2s linear;
        transition:all .2s linear
    }
    .social-icons a:active,.social-icons a:focus,.social-icons a:hover
    {
        color:#fff;
        background-color:#29aafe
    }
    .social-icons.size-sm a
    {
        line-height:34px;
        height:24px;
        width:24px;
        font-size:12px
    }
    .social-icons a.facebook:hover
    {
        background-color:#3b5998
    }
    .social-icons a.twitter:hover
    {
        background-color:#00aced
    }
    .social-icons a.linkedin:hover
    {
        background-color:#007bb6
    }
    .social-icons a.dribbble:hover
    {
        background-color:#5a5758
    }
    @media (max-width:767px)
    {
        .social-icons li.title
        {
        display:block;
        margin-right:0;
        font-weight:600
        }
    }
</style>
<body>
    <nav class="navbar">
        <ul>
            <li><a href="#home">home</a></li>
            <li><a href="#about">About me</a></li>
            <li><a href="#pictures">Pictures</a></li>
            <li><a href="#Skills">Skills</a></li>
            <li><a href="#contact">Contact Me</a></li>
        </ul>
    </nav>

    <section id="home">
            <div class="Main">
                 <h1 class="Headings">I AM <br>hara tej </h1>
                 <button class="btn">
                    LEARNER
              </button>
             </div>
         </section> 

        <section id="about">
            <h1 class="headings">ABOUT ME</h1>
            <div id="pic">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1652637918/s/21BME7026_Photo_g9upvy.jpg" alt="">
                <div id="intro">
                    <h2>HARATEJ DIVI</h2>
                    <P>My name is Hara Tej...... I am from vijayawada which is in Krishna district. Recently I got a seat in VIT-AP university through EAPCET. I am representing the Mechanical department. Recently I have joined SAE club and SPM club. Both clubs are playing a crucial role for me to built a good career.  I am very interested in coding so that SPM club is playing a major role to built my confidence. 
In free times I used to play cricket, kabaddi because it keeps me to feel free from any situation and it helps me to handle that situation in a quiet manner..............!                  

                    </P>
                </div>
            </div>
        </section>

        <section id="pictures">
            <h1 class="headings">PICTURES</h1>
            <div class="gallery">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1652610103/my%20library/download_py0wnf.jpg" alt="">
                <img src="https://res.cloudinary.com/du3iufefj/image/upload/v1652610151/my%20library/download_tpuwwc.jpg" alt="">

            </div>
        </section>

        <center><section id="Skills">
            <h1 class="headings">SKILLS</h1>
            <div class="row">
                <div class="box">
                    <h1 class="headings">MY SKILLS</h1>
                    <p>My skills are the back bone for me. I am quiet decent in communication skills.. I have some basic stuff regarding Autocad, Java, Python, Html and Css....!!</p>
                    </div>
        </section></center>

        <section id="contact">
            <center><h1 class="heading">CONTACT</h1></center>
            <form action=""class="form">
                <input type="text" name="name" class="input" placeholder="9347870667">
                <input type="email" name="email" class="input" placeholder="haratej2402@gmail.com">

            </form>
        </section>

        <footer>
            <!-- Add icon library -->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">

<!-- Add font awesome icons -->


            <p>HARA TEJ DIVI</p>


        <!-- Footer -->
  <section id="footer">
    <div class="footer container">
      <div class="brand">

      </div>

      <div class="social-icon">
        <div class="social-item">
          <a href="https://www.facebook.com/profile.php?id=100081020930976" target="_blank"><img src="data:image/png;base64,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" /></a>

          <a href="https://www.instagram.com/haratej_sgk/" target="_blank"><img src="data:image/png;base64,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
          " /></a>

          <a href="https://twitter.com/Dhtej_7" target="_blank"><img src="data:image/jpeg;base64,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" /></a>
        </div>
      </div>
      <p>Copyright © 2022 Hara Tej. All rights reserved</p>
    </div>
  </section>
  <!-- End Footer -->
  <script src="./app.js"></script>
</body>

</html>
