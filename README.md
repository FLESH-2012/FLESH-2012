
<!DOCTYPE html>
<html lang="uz">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>SHAHRIYOR | Portfolio</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@500;700;800&family=Poppins:wght@400;500;600;700&display=swap');

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    scroll-behavior: smooth;
}

body {
    background: #070b16;
    color: white;
    font-family: Poppins, sans-serif;
}

:root {
    --neon: #00ffd5;
    --blue: #536dfe;
}

header {
    width: 100%;
    padding: 22px 8%;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: fixed;
    top: 0;
    background: rgba(7,11,22,.95);
    backdrop-filter: blur(15px);
    z-index: 100;
    border-bottom: 1px solid #26334b;
}

.logo {
    font-family: Orbitron;
    font-size: 22px;
    font-weight: 800;
    color: white;
    text-decoration: none;
}

.logo span {
    color: var(--neon);
}

nav {
    display: flex;
    gap: 25px;
}

nav a {
    text-decoration: none;
    color: #aaa;
    font-size: 13px;
    transition: .3s;
}

nav a:hover {
    color: var(--neon);
}

section {
    padding: 110px 8%;
    text-align: center;
}

.home {
    min-height: 100vh;
    display: flex;
    justify-content: space-between;
    align-items: center;
    text-align: left;
    gap: 40px;
    padding-top: 140px;
}

.welcome {
    color: var(--neon);
    letter-spacing: 5px;
}

.home h1 {
    font-family: Orbitron;
    font-size: clamp(35px, 6vw, 65px);
    margin: 20px 0;
}

.home h1 span {
    color: var(--neon);
    text-shadow: 0 0 25px #00ffd555;
}

.home h3 {
    color: #aab5c9;
    font-size: 23px;
}

.description {
    color: #aab5c9;
    max-width: 480px;
    line-height: 1.8;
    margin: 20px 0 30px;
}

.btn {
    display: inline-block;
    background: var(--neon);
    color: #071016;
    padding: 14px 25px;
    border: none;
    border-radius: 8px;
    font-weight: 700;
    text-decoration: none;
    cursor: pointer;
    transition: .3s;
}

.btn:hover {
    box-shadow: 0 0 30px var(--neon);
    transform: translateY(-4px);
}

.hero-icon {
    text-align: center;
}

.big-s {
    font-family: Orbitron;
    font-size: 230px;
    color: transparent;
    -webkit-text-stroke: 3px var(--neon);
    text-shadow: 0 0 40px #00ffd555;
    animation: float 3s infinite ease-in-out;
}

.hero-icon p {
    color: var(--neon);
    letter-spacing: 5px;
    font-size: 12px;
}

@keyframes float {
    50% { transform: translateY(-20px); }
}

h2 {
    font-family: Orbitron;
    font-size: clamp(25px, 4vw, 38px);
    margin-bottom: 40px;
}

h2 span {
    color: var(--neon);
}

.about-box, .skills-box, .game-box, .contact-box {
    max-width: 800px;
    margin: auto;
    padding: 35px;
    background: #10192b;
    border: 1px solid #263550;
    border-radius: 15px;
    box-shadow: 0 0 30px #00ffd510;
}

.about-box h3 {
    color: var(--neon);
    margin-bottom: 20px;
}

.about-box p {
    color: #abb9ce;
    line-height: 2;
}

.skill {
    margin: 25px 0;
    text-align: left;
}

.skill div {
    display: flex;
    justify-content: space-between;
    margin-bottom: 10px;
}

.skill b {
    color: var(--neon);
}

.bar {
    width: 100%;
    height: 9px;
    background: #26334b;
    border-radius: 20px;
    overflow: hidden;
}

.bar span {
    height: 100%;
    display: block;
    background: linear-gradient(90deg, var(--blue), var(--neon));
    border-radius: 20px;
}

.game-box canvas {
    display: block;
    width: 100%;
    max-width: 400px;
    height: auto;
    margin: 20px auto;
    background: #091321;
    border: 2px solid var(--neon);
    border-radius: 8px;
}

.score {
    font-family: Orbitron;
    color: var(--neon);
    font-size: 22px;
}

.game-box p {
    color: #9baac0;
    font-size: 12px;
    margin: 15px 0;
}

.contact-box {
    display: flex;
    flex-direction: column;
    gap: 20px;
}

.contact-box a {
    color: var(--neon);
    background: #19253a;
    padding: 17px;
    border-radius: 8px;
    text-decoration: none;
    overflow-wrap: anywhere;
    transition: .3s;
}

.contact-box a:hover {
    background: var(--neon);
    color: #071016;
    transform: scale(1.02);
}

footer {
    padding: 25px;
    text-align: center;
    border-top: 1px solid #263550;
    color: #8794a9;
    font-size: 12px;
}

/* TELEFON UCHUN */
@media(max-width: 750px) {
    header {
        flex-direction: column;
        gap: 15px;
        padding: 15px;
    }

    nav {
        justify-content: center;
        flex-wrap: wrap;
        gap: 13px;
    }

    nav a {
        font-size: 11px;
    }

    .home {
        flex-direction: column;
        text-align: center;
        justify-content: center;
        padding-top: 160px;
    }

    .description {
        margin: 20px auto 30px;
    }

    .big-s {
        font-size: 130px;
    }

    section {
        padding: 80px 5%;
    }

    .about-box, .skills-box, .game-box, .contact-box {
        padding: 20px;
    }
}
</style>
</head>

<body>

<header>
    <a href="#home" class="logo">SHAHRIYOR<span>.</span></a>

    <nav>
        <a href="#home">Home</a>
        <a href="#about">About</a>
        <a href="#skills">Skills</a>
        <a href="#game">Snake</a>
        <a href="#contact">Contact</a>
    </nav>
</header>

<!-- HOME -->

<section class="home" id="home">

    <div>
        <p class="welcome">SALOM, MEN</p>

        <h1>
            SHAHRIYOR<br>
            <span>AMINBOYEV</span>
        </h1>

        <h3>Frontend Developer</h3>

        <p class="description">
            Men HTML, CSS va JavaScript yordamida
            zamonaviy va chiroyli web saytlar yarataman.
            Xush kelibsiz mening portfolio saytimga!
        </p>

        <a href="#contact" class="btn">
            MEN BILAN BOG‘LANISH →
        </a>
    </div>

    <div class="hero-icon">
        <div class="big-s">S</div>
        <p>CREATIVE DEVELOPER</p>
    </div>

</section>

<!-- ABOUT -->

<section id="about">

    <h2>MEN <span>HAQIMDA</span></h2>

    <div class="about-box">
        <h3>SHAHRIYOR AMINBOYEV</h3>

        <p>
            Salom! Men Shahriyor Aminboyevman.
            Dasturlashga juda qiziqaman.
            HTML, CSS va JavaScript yordamida
            turli xil loyihalar yarataman.
            Kelajakda professional dasturchi bo‘lishni
            maqsad qilganman.
        </p>
    </div>

</section>

<!-- SKILLS -->

<section id="skills">

    <h2>MY <span>SKILLS</span></h2>

    <div class="skills-box">

        <div class="skill">
            <div><span>HTML</span><b>90%</b></div>
            <div class="bar"><span style="width:90%"></span></div>
        </div>

        <div class="skill">
            <div><span>CSS</span><b>85%</b></div>
            <div class="bar"><span style="width:85%"></span></div>
        </div>

        <div class="skill">
            <div><span>JAVASCRIPT</span><b>70%</b></div>
            <div class="bar"><span style="width:70%"></span></div>
        </div>

    </div>

</section>

<!-- SNAKE GAME -->

<section id="game">

    <h2>SNAKE <span>GAME</span></h2>

    <div class="game-box">

        <div class="score">
            SCORE: <span id="score">0</span>
        </div>

        <canvas id="snake" width="400" height="400"></canvas>

        <button class="btn" onclick="startGame()">
            START GAME ▶
        </button>

        <p>
            ⬆ ⬇ ⬅ ➡ yoki W A S D tugmalari bilan boshqar!
        </p>

    </div>

</section>

<!-- CONTACT -->

<section id="contact">

    <h2>CONTACT <span>ME</span></h2>

    <div class="contact-box">

        <a href="tel:770437788">
            📞 TELEFON: 770437788
        </a>

        <a href="mailto:shahriyoraminboyev002@gmail.com">
            📧 GMAIL: shahriyoraminboyev002@gmail.com
        </a>

        <a href="https://www.instagram.com/shahriyor_225_/"
           target="_blank">
            📸 INSTAGRAM: @shahriyor_225_
        </a>

    </div>

</section>

<footer>
    © 2026 SHAHRIYOR AMINBOYEV | ALL RIGHTS RESERVED
</footer>

<script>

// SNAKE GAME

const canvas = document.getElementById("snake");
const ctx = canvas.getContext("2d");

const size = 20;
const cells = 20;

let snake = [];
let food = {};
let dx = 1;
let dy = 0;
let score = 0;
let game;
let running = false;

function createFood() {
    food = {
        x: Math.floor(Math.random() * cells),
        y: Math.floor(Math.random() * cells)
    };

    if (snake.some(p => p.x === food.x && p.y === food.y)) {
        createFood();
    }
}

function startGame() {
    clearInterval(game);

    snake = [
        {x: 10, y: 10},
        {x: 9, y: 10},
        {x: 8, y: 10}
    ];

    dx = 1;
    dy = 0;
    score = 0;

    document.getElementById("score").textContent = score;

    createFood();

    running = true;

    draw();

    game = setInterval(update, 120);
}

function update() {

    const head = {
        x: snake[0].x + dx,
        y: snake[0].y + dy
    };

    const ate = head.x === food.x && head.y === food.y;
    const body = ate ? snake : snake.slice(0, -1);

    if (
        head.x < 0 ||
        head.y < 0 ||
        head.x >= cells ||
        head.y >= cells ||
        body.some(p => p.x === head.x && p.y === head.y)
    ) {
        endGame();
        return;
    }

    snake.unshift(head);

    if (ate) {
        score += 10;

        document.getElementById("score").textContent = score;

        createFood();
    } else {
        snake.pop();
    }

    draw();
}

function draw() {

    ctx.clearRect(0, 0, 400, 400);

    // GRID

    ctx.strokeStyle = "#17283d";

    for (let i = 0; i <= cells; i++) {
        ctx.beginPath();
        ctx.moveTo(i * size, 0);
        ctx.lineTo(i * size, 400);
        ctx.stroke();

        ctx.beginPath();
        ctx.moveTo(0, i * size);
        ctx.lineTo(400, i * size);
        ctx.stroke();
    }

    // FOOD

    ctx.fillStyle = "#ff477e";
    ctx.shadowColor = "#ff477e";
    ctx.shadowBlur = 15;

    ctx.beginPath();
    ctx.arc(
        food.x * size + 10,
        food.y * size + 10,
        7, 0, Math.PI * 2
    );
    ctx.fill();

    ctx.shadowBlur = 0;

    // SNAKE

    snake.forEach((p, i) => {

        ctx.fillStyle = i === 0 ? "#ffffff" : "#00ffd5";

        ctx.shadowColor = "#00ffd5";
        ctx.shadowBlur = 10;

        ctx.beginPath();

        ctx.roundRect(
            p.x * size + 2,
            p.y * size + 2,
            size - 4,
            size - 4,
            5
        );

        ctx.fill();

    });

    ctx.shadowBlur = 0;
}

function endGame() {

    clearInterval(game);
    running = false;

    draw();

    ctx.fillStyle = "rgba(0,0,0,.8)";
    ctx.fillRect(0, 0, 400, 400);

    ctx.textAlign = "center";
    ctx.fillStyle = "#00ffd5";
    ctx.font = "bold 28px Arial";

    ctx.fillText("GAME OVER", 200, 180);

    ctx.fillStyle = "white";
    ctx.font = "16px Arial";

    ctx.fillText("SCORE: " + score, 200, 220);
}

// KEYBOARD

document.addEventListener("keydown", function(e) {

    if (!running) return;

    const key = e.key.toLowerCase();

    if (key.startsWith("arrow")) {
        e.preventDefault();
    }

    if ((key === "arrowup" || key === "w") && dy !== 1) {
        dx = 0;
        dy = -1;
    }

    else if ((key === "arrowdown" || key === "s") && dy !== -1) {
        dx = 0;
        dy = 1;
    }

    else if ((key === "arrowleft" || key === "a") && dx !== 1) {
        dx = -1;
        dy = 0;
    }

    else if ((key === "arrowright" || key === "d") && dx !== -1) {
        dx = 1;
        dy = 0;
    }

});

// INITIAL SCREEN

snake = [
    {x: 10, y: 10},
    {x: 9, y: 10},
    {x: 8, y: 10}
];

food = {x: 15, y: 8};

draw();

</script>

</body>
</html>
