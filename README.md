<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8">
        <meta name="viewport" content="width=device-width, initial-scale=1.0">
        <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
        <title>Document</title>
        <link rel="stylesheet" href="portifolio.css">
    </head>
    <body>

        <header id="header">
            <nav>
                <a href="#home">Bosh sahifa</a>
                <a href="#about">Biz haqimizda</a>
                <a href="#services">Xizmatlar</a>
                <a href="#contact">Bog‘lanish</a>
            </nav>
        </header>
        <br>
        <main>
            <section class="home_item" id="home">
                <div class="name_item">
                    <div class="text_item">
                        <h3>Hi,I am </h3>
                    <br>
                    <h1>Tohirov <br>Abdulloh</h1>
                    <br>
                    <p>Frontend and Mobile developer</p>
                    <br>
                    <br>
                    <button type="submit"><a href="#">Resume</a></button>
                    </div>
                    
                </div>
                <div class="name_item"><img src="canva.png" alt="" srcset=""></div>
                <button class="top"><a href="#home">Bosh sahifa</a></button>
            </section>,
            <section class="about_item" id="about">
                <h2>About me</h2>
                <div class="flex">
                    <div class="about-img_item">
                        <img src="inashu.png" alt="" srcset="">
                    </div>
                <div class="information">
                    <h3>I'm Abdulloh</h3>
                    <p>Hello! My name is Abdulloh, and I’m a passionate Front-End Developer who loves turning ideas into beautiful and functional websites. I enjoy creating clean, modern, and responsive designs that provide a great user experience.
                    <br>
                    I’m always learning new technologies to improve my skills — especially in HTML, CSS, JavaScript, and modern frameworks. Coding is not just my work; it’s something that inspires me to build and grow every single day.
                    <br>
                    In my free time, I like experimenting with new design styles, exploring UI/UX trends, and working on personal projects. My goal is to become a professional front-end engineer and build websites that make a real impact.</p>
                </div>
                </div>
                
            </section>
            <br>
            <section class="skills">
                <h2>Skills</h2>
                <div class="flex">
                    <div class="skills-statistics_item">
                        <p>HTML</p>
                        <div class="container">
                            <div class="skills html">90%</div>
                        </div>

                        <p>CSS</p>
                        <div class="container">
                            <div class="skills css">80%</div>
                        </div>

                        <p>Bootstrap</p>
                        <div class="container">
                            <div class="skills js">65%</div>
                        </div>

                        <p>Python</p>
                        <div class="container">
                            <div class="skills php">60%</div>
                        </div>
                    </div>
                <div class="skills-img_item"><img src="" alt="" srcset=""></div>
                </div>
            </section>
            <section class="contact" id="contact">
                <h2>Contact</h2>
                <form action="">
                    <input type="text" placeholder="Name" required >
                    <br>
                    <br>
                    <input type="email" required placeholder="Email">
                    <br>
                    <br>
                    <textarea placeholder="Extra information" name="" id="" required></textarea>
                    <br>
                    <br>
                    <button type="submit" class="submit">Yuborish</button>
                </form>
                
            </section>
            <br>
            <br>
        </main>
        
        <footer>
            <h1 style="text-align: center;font-size: 3em;">Abdulloh</h1>
            <p style="font-size: 1.4em;">©2025 Abdulloh Tohirov. Copyright all right reserved</p>
            <nav>
                <a href="#home" style="color: white;">Bosh sahifa</a>
                <a href="#about" style="color: white;">Biz haqimizda</a>
                <a href="#services" style="color: white;">Xizmatlar</a>
                <a href="#contact" style="color: white;">Bog‘lanish</a>
            </nav>
        </footer>
        <script>
            const items = document.querySelectorAll('.name_item');

window.addEventListener('scroll', checkItems);

function checkItems() {
  const triggerBottom = window.innerHeight * 0.8;

  items.forEach(item => {
    const itemTop = item.getBoundingClientRect().top;

    if (itemTop < triggerBottom) {
      item.classList.add('show');  // ekranga kirsa paydo bo‘ladi
    } else {
      item.classList.remove('show'); // yuqoriga chiqsa yo‘qoladi (ixtiyoriy)
    }
  });
}
        </script>
    </body>
</html>
