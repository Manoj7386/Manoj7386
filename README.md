<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/bbc73c3225.js" crossorigin="anonymous"></script>
</head>
<body>
    <h2>My Portfolio</h2>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#contact">Contact</a></li>

            </ul>
        </nav>
    </header>
    <div class="header-text">
        <h1>Hi, I'm <span>Manoj Yeluru</span> <br>From Nellore</h1>
    </div>
    <main>
        <section id="home">
            <img src="images/img1.jpg" alt="Your Image" class="home-image">
        </section>
    </main>
<!--------about------------->
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="images/img2.jpg">    
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>Hello! I'm Manoj, a recent BE graduate in 
                        Computer Science-AI&ML from Audisankara College of Engineering & Technology. 
                        With a strong foundation in Python, Web-development, ML ,DL. I'm eager 
                        to apply my skills and knowledge in a real-world setting.
                        I'm excited to start my career as a Software Engineer and 
                        contribute to innovative projects. In my spare time, 
                        I love to express my creativity through photography,
                        enjoy listening to music,and exploring new technologies.   
                    </p>
                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('education')">Education</p>  
                    </div>
                    <div class="tab-contents active-tab" id="skills" >
                        <ul>
                            <li><span>Programming Languages</span><br>Python, JavaScript</li>
                            <li><span>Databases</span><br>MySQL, MongoDB</li>
                            <li><span>Web development tools</span><br>HTML, CSS</li>
                            <li><span>Data analysis and visualization tools</span><br>Excel, Power BI</li>
                        </ul>

                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>AP Model School: 2021</span><br>CGPA:9.3</li>
                            <li><span>AP Model Junior College: 2023</span><br>CGPA:8</li>
                            <li><span>Audisankara College of Engineering & Technology : 2023-2027(expected)</span><br>Bachelor of Engineering in Artificial Intelligence and Machine Learning</li>
                        </ul>  
                    </div>
                </div>
            </div>
        </div>
    </div>
 <!------------PROJECTS----------> 
<div id="projects">
    <div class="container">
        <h1 class="sub-title">My Projects</h1>
        <div class="projects-list">
            <div>
                <i class="fa-solid fa-user-secret"></i>
                <h2>Face Detection Using Deep Learning</h2>
                <p>This System Can detect face if it detects face
                     then it will say Yes if not No</p>
            </div>
            <div>
                <i class="fa-solid fa-circle-question"></i>
                <h2>QASystem (Information Retrieval)</h2>
                <p>It is a powerful Question Answering (QA) System using LlamaIndex and 
                    Google Gemini,integrated with a sleek Streamlit interface. </p>

            </div>
            <div>
                <i class="fa-solid fa-circle-info"></i>
                <h2>Information Retrieval System Using Langchain and OPENAI </h2>
                <p>It is a powerful Information Retrieval System Using Langchain FrameWork and OpenAI API 
                    Key Embedding with a sleek Streamlit Interface.</p>
            </div>


        </div>
    </div>
</div>

<div id="contact">
    <div class="container">
        <div class="row">
            <div class="contact-left">
                <h1 class="sub-title">Contact Me</h1>
                <p><i class="fa-solid fa-paper-plane"></i>manojchowdary@gmail.com</p>
                <p><i class="fa-solid fa-phone-volume"></i>7386249091</p>
                <div class="social-icons">
                    <a href="https://www.instagram.com/manoj_chowdar_y?igsh=dXZnY2p1N2VwbzMy"><i class="fa-brands fa-instagram"></i></a>
                   
                    <a href="https://www.facebook.com/share/si7cRnPr3DuXN12M/?mibextid=qi2Omg"><i class="fa-brands fa-facebook"></i></a>
                </div>
            </div>
                <div class="contact-right">
                    <form>
                        <input type="text" name="Name" placeholder="Your Name">
                        <input type="email" name="Email" placeholder="Your Email">
                        <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
                        <button type="submit" class="btn btn2">Submit</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
    <div class="copyright">
        <p> Copyright &copy; Manoj Yeluru<i class="fa-solid fa-heart"></i>. All rights reserved.</p>
    </div>
</div>

  <script>
    var tablinks = document.getElementsByClassName("tab-links");
    var tabcontents = document.getElementsByClassName("tab-contents");

    function opentab(tabname){
        for(tablink of tablinks){
            tablink.classList.remove("active-link");
        }
        for(tabcontent of tabcontents){
            tabcontent.classList.remove("active-tab");
        }
        event.currentTarget.classList.add("active-link");
        document.getElementById(tabname).classList.add("active-tab");
    }
  </script>

</body>
</html>
