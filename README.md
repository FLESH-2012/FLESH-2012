
<!DOCTYPE html>
<html lang="uz">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SHAHRIYOR | Portfolio</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<header>
    <a href="#" class="logo">SHAHRIYOR<span>.</span></a>

    <nav>
        <a href="#home">Bosh sahifa</a>
        <a href="#about">Men haqimda</a>
        <a href="#skills">Skills</a>
        <a href="#game">Snake</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<section class="home" id="home">
    <div class="home-content">
        <p class="welcome">SALOM, MEN</p>
        <h1>SHAHRIYOR<br><span>AMINBOYEV</span></h1>
        <h3>Frontend Developer</h3>
        <p class="description">
            Men HTML, CSS va JavaScript yordamida
            zamonaviy va chiroyli web saytlar yarataman.
        </p>
        <a href="#contact" class="btn">Men bilan bog‘lanish</a>
    </div>

    <div class="hero-icon">
        <div class="big-s">S</div>
        <p>CREATIVE DEVELOPER</p>
    </div>
</section>

<section id="about">
    <h2>MEN <span>HAQIMDA</span></h2>
    <div class="about-box">
        <h3>Shahriyor Aminboyev</h3>
        <p>
            Men dasturlashga qiziquvchi yosh dasturchiman.
            HTML, CSS va JavaScript tillarini o‘rganaman.
            Yangi loyihalar yaratishni va texnologiyalarni
            o‘rganishni yaxshi ko‘raman.
        </p>
    </div>
</section>

<section id="skills">
    <h2>MY <span>SKILLS</span></h2>

    <div class="skills">
        <div class="skill">HTML <b>90%</b></div>
        <div class="skill">CSS <b>85%</b></div>
        <div class="skill">JAVASCRIPT <b>70%</b></div>
    </div>
</section>

<section id="game">
    <h2>SNAKE <span>GAME</span></h2>
    <div class="game-box">
        <div class="score">SCORE: <span id="score">0</span></div>
        <canvas id="snake" width="400" height="400"></canvas>
        <button class="btn" onclick="startGame()">START GAME</button>
        <p>⬆ ⬇ ⬅ ➡ tugmalari bilan boshqar!</p>
    </div>
</section>

<section id="contact">
    <h2>CONTACT <span>ME</span></h2>

    <div class="contact-box">
        <a href="tel:770437788">📞 770437788</a>
        <a href="mailto:shahriyoraminboyev002@gmail.com">
            📧 shahriyoraminboyev002@gmail.com
        </a>
        <a href="https://www.instagram.com/shahriyor_225_/"
           target="_blank">📸 Instagram</a>
    </div>
</section>

<footer>
    <p>© 2026 SHAHRIYOR AMINBOYEV | ALL RIGHTS RESERVED</p>
</footer>

<script src="script.js"></script>
</body>
</html>
