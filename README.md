# portfolio.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.1/css/all.min.css">
    <title>Amrit Portfolio</title>
    <link rel="stylesheet" href="prtfolio.css">
    <link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
</head>
<body>
    <nav>
        <div class="nav-container">
            <div class="logo" data-aos="zoom-in" data-aos-duration="1000">
                <span> <b> <b> AMRIT PRITAM MOHANTY</b></b></span>
            </div>
            <div class="links">
                <div class="link" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="100"><a href="#">Home</a></div>
                <div class="link" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="200"><a href="#">About</a></div>
                <div class="link" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="300"><a href="#">Skills</a></div>
                <div class="link" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="400"><a href="#">Services</a></div>
                <div class="link" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="500"><a href="#">Blogs</a></div>
                <div class="link contact-btn" data-aos="fade-up" data-aos-duration="1000" data-aos-delay="600"><a href="#" >Contact Us</a></div>
            </div>
            <i class="fa-solid fa-bars hamburg" onclick="hamburg()"></i>
        </div>
        <div class="dropdown">
            <div class="links">
                <a href="">Home</a>
                <a href="">About</a>
                <a href="">Skills</a>
                <a href="">Services</a>
                <a href="">Blogs</a>
                <a href="">Contact Us</a>
                <i class="fa-solid fa-xmark cancel" onclick="cancel()"></i>
            </div>
        </div>
    </nav> <br> 
        <section>
            <div class="main-container">
                <div class="image" data-aos="zoom-in-right" data-aos-duration="2500">
                    <img src="IMG_4863.JPG" alt="">
                </div> 
                <div class="content">
                    <h1 data-aos="fade-left" data-aos-duration="1000" data-aos-delay="800">Hey This is  <span>Amrit Pritam Mohanty</span></h1>
                    <div class="typewriter" data-aos="fade-right" data-aos-duration="1000" data-aos-delay="900"> <small>I'm Passionate about</small> <span></span></div>
                    <p data-aos="flip-up" data-aos-duration="1000" data-aos-delay="1000">Hello, This is <b>Amrit Pritam Mohanty</b>, a passionate and detail-oriented B.Tech student from ITER (Institute of Technical Education and Research) with a strong interest in web development and software engineering.

                        With expertise in HTML, CSS, jQuery, Bootstrap, Java, and JavaScript, I specialize in creating responsive and dynamic web applications. I enjoy building clean, user-friendly interfaces and interactive websites that enhance user experiences. My proficiency in Java and JavaScript allows me to develop both frontend and backend functionalities efficiently.
                        
                        Beyond coding, I am always eager to learn new technologies, stay updated with industry trends, and work on innovative projects. My goal is to become a skilled full-stack developer and contribute to impactful software solutions.
                        
                        <br> Let's connect and collaborate! 🚀 </br></p>
                    <div class="social-links" data-aos="flip-down" data-aos-duration="1000" data-aos-delay="1200">
                        <a href="https://github.com/amritpritam05" ><i class="fa-brands fa-github"></i></a>
                        <a href="https://www.facebook.com/albus.dombledore.77/"><i class="fa-brands fa-facebook"></i></a>
                        <a href="https://www.linkedin.com/in/amrit-pritam-mohanty-9a49262b7?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app"><i class="fa-brands fa-linkedin"></i></a>
                        <a href="#"><i class="fa-brands fa-x-twitter"></i></a>
                    </div>
                    <div class="btn" data-aos="zoom-out-left" data-aos-duration="1000" data-aos-delay="1300">
                        <button>Download CV</button> 
                    </div>
                </div>
            </div>
        </section> 
        <script src="https://unpkg.com/aos@next/dist/aos.js"></script>
        <script>
          AOS.init({offset:0});
        </script>
        <script>
            function hamburg(){
                const navbar = document.querySelector(".dropdown")
                navbar.style.transform = "translateY(0px)"
            }
            function cancel(){
                const navbar = document.querySelector(".dropdown")
                navbar.style.transform = "translateY(-500px)"
            }
        </script> 
</body>
</html>

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@100;200;300;400;500;600&display=swap');
*{
    padding: 0;
    margin: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}
html{
    overflow-x: hidden;
}
body{
    width: 100%;
    height: 100vh;
    overflow: hidden;
    background: linear-gradient(to right, rgb(255,255,255), rgb(163, 206, 252));
}
nav{
    width: 100%;
    height: 10vh;
    position: sticky;
}
.nav-container{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-around;
    align-items: center;
}
.logo{
    color: black;
    font-size: 2rem;
    font-weight: bolder;
}
.logo span{
    color: rgb(8, 8, 8);
    text-shadow: 0 0 10px rgb(96, 101, 93);
}
.hamburg, .cancel{
    cursor: pointer;
    position: absolute;
    right: 15px;
    top: 10px;
    color: black;
    font-size: 2rem;
    display: none;
}
.nav-container .links {
    display: flex;
    gap: 3rem;
    align-items: center;
}
.nav-container .links a{
    position: relative;
    font-size: 1.2rem;
    color: black;
    text-decoration: none;
    font-weight: 500;
    transform: 0.3s linear;
}
.nav-container .links a::before{
    position: absolute;
    content: "";
    bottom: -3px;
    left: 0;
    width: 0%;
    height: 3px;
    background-color: rgb(6, 105, 219);
    transition: 0.2s linear;
}
.nav-container .links a:hover::before{
    width: 100%;
}
.nav-container .contact-btn{
    background-color: transparent;
    padding: 5px 20px;
    border-radius: 20px;
    border: 2px solid rgb(6, 105, 219);
    transition: 0.2s linear;
}
.nav-container .contact-btn a{
    color: white;
    transition: 0.3s linear;
}
.nav-container .contact-btn:hover, .nav-container .contact-btn:hover a{
    background-color: rgb(6, 105, 219);
    color: white;
}
.nav-container .links a:hover{
    color:rgb(6, 105, 219);
}
.dropdown{
    z-index: 100;
    position: absolute;
    top: 0;
    transform: translateY(-500px);
    width: 100%;
    height: auto;
    backdrop-filter: brightness(40%) blur(3px);
    box-shadow: 0 0 20px black;
    transition: 0.2s linear;
}
.dropdown .links a{
    color: white;
    display: flex;
    text-decoration: none;
    justify-content: center;
    padding: 15px 0;
    align-items: center;
    transition: 0.2s linear;
}
.dropdown .links a:hover{
    background-color: rgb(6, 105, 219);
}
section{
    width: 100%;
    height: 90vh;
}
.main-container{
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: space-evenly;
    align-items: center;
}
.main-container .image{
    z-index: -1;
    width: 50%;
}
.main-container .image img{
    width: 100%;
}
.main-container .content{
    color: black;
    width: 40%;
    min-height: 100px;
}
.content h1{
    font-size: clamp(1rem, 2rem + 5vw, 3rem);
}
.content h1 span{
    color: rgb(6, 105, 219);
    text-shadow: 0 0 10px rgb(135, 189, 249);
}
.content .typewriter{
    font-weight: 600;
    font-size: clamp(1rem, 1rem + 5vw, 2rem);
}
.content .typewriter span{
    color:rgb(6, 105, 219);
    font-size: 2.5rem;
    text-shadow: 0 0 5px rgb(137, 188, 246);
    position: relative;
    transition: 0.3s linear;
}
.typewriter span::before{
    content: "Developer";
    animation: words 15s infinite;
}
.typewriter span::after{
    content: "";
    position: absolute;
    width: calc(100% + 8px);
    height: 100%;
    border-left: 3px solid black;
    animation:  cursor 0.6s linear infinite;
}
@keyframes cursor {
    to{
        border-left: 2px solid #3360f2;
    }
}
@keyframes words {
    0%, 33%{
        content: "Web Developing";
    }
    34%, 66%{
        content: "Designing";
    }
    67%, 85%{
        content: "Problem Solving";
    }
    86%, 100%{
        content: "Generative A.I.";
    }
}
.content p{
    font-size: clamp(0.4rem, 0.2rem + 9vw, 1rem);
    margin: 10px 0;
}
.social-links i{
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 3rem;
    height: 3rem;
    background-color:transparent;
    border: 0.2rem solid rgb(6, 105, 219);
    border-radius: 50%;
    color:rgb(6, 105, 219);
    margin: 5px 10px;
    font-size: 1.5rem;
    transition: 0.2s linear;
}
.social-links i:hover{
    scale: 1.3;
    color: white;
    background-color: rgb(6, 105, 219);
    filter: drop-shadow(0 0 10px rgb(6, 105, 219));
}
.content button{
    width: 40%;
    height: 6vh;
    margin: 30px;
    background-color: rgb(6, 105, 219);
    color: white;
    border: none;
    outline: none;
    font-size: 100%;
    font-weight: 700;
    border-radius: 5px;
    transition: 0.2s linear;
}
.content button:hover{
 scale: 1.1;
 color: rgb(27, 119, 223);
 border: 2px solid rgb(6, 105, 219);
 background-color: transparent;
 font-weight: 700;
 box-shadow: 0 0 40px rgb(6, 105, 219);
}
@media (max-width:884px) {
    body{
        overflow-y: visible;
    }
    nav .logo{
        position: absolute;
        top: 16px;
        left: 15px;
        font-size: 1.5rem;
    }
    .main-container{
        display: flex;
        flex-direction: column;
    }
    .nav-container .links{
        display: none;
    }
    .hamburg,.cancel{
        display: block;
    }
    .main-container .content{
        width: 80%;
    }
    .social-links i{
        width: 2.5rem;
        height: 2.5rem;
        font-size: 1.5rem;
    }
    .cancel{
        color: white;
    }
    .main-container .image{
        width: 80%;
        margin-bottom: 0px;
    }
}
