<!DOCTYPE html>
<html lang="en">

<head>

<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Happy Birthday 💜</title>

<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600&family=Great+Vibes&display=swap" rel="stylesheet">

<link rel="stylesheet"
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.1/css/all.min.css">

<style>

/* ===== YOUR CSS START ===== */

*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Poppins',sans-serif;
}

body{
background:#050510;
color:white;
overflow-x:hidden;
}

body::before{
content:'';
position:fixed;
width:100%;
height:100%;
top:0;
left:0;
background:
radial-gradient(circle at 20% 20%, #6a00ff22, transparent 30%),
radial-gradient(circle at 80% 20%, #ff00cc22, transparent 30%),
radial-gradient(circle at 50% 80%, #00d4ff22, transparent 30%);
z-index:-2;
animation:bgMove 12s infinite alternate;
}

@keyframes bgMove{
from{transform:scale(1);}
to{transform:scale(1.2);}
}

#particles{
position:fixed;
width:100%;
height:100%;
pointer-events:none;
z-index:-1;
}

#intro{
height:100vh;
display:flex;
justify-content:center;
align-items:center;
text-align:center;
}

.intro-card{
padding:40px;
border:2px solid #ff4df0;
border-radius:25px;
box-shadow:0 0 20px #ff4df0,0 0 50px #ff4df0;
background:rgba(255,255,255,0.03);
backdrop-filter:blur(10px);
}

.moon{
font-size:80px;
margin-bottom:15px;
animation:float 3s infinite;
}

@keyframes float{
50%{transform:translateY(-10px);}
}

.intro-card h1{
font-family:'Great Vibes',cursive;
font-size:60px;
margin-bottom:20px;
}

#countdown{
font-size:90px;
font-weight:bold;
color:#ff4df0;
text-shadow:0 0 20px #ff4df0,0 0 50px #ff4df0;
}

#website{display:none;}

.hero{
height:100vh;
display:flex;
flex-direction:column;
justify-content:center;
align-items:center;
text-align:center;
padding:20px;
position:relative;
}

.glow-circle{
position:absolute;
width:300px;
height:300px;
border-radius:50%;
background:#ff4df055;
filter:blur(80px);
}

.hero-title{
font-size:80px;
font-family:'Great Vibes',cursive;
z-index:1;
color:#ff73ff;
text-shadow:0 0 20px #ff73ff,0 0 60px #ff73ff;
}

.hero-subtitle{
max-width:700px;
margin-top:20px;
font-size:20px;
z-index:1;
}

.hero-buttons{
margin-top:30px;
display:flex;
gap:20px;
flex-wrap:wrap;
justify-content:center;
}

button{
padding:14px 30px;
border:none;
border-radius:40px;
cursor:pointer;
background:#ff4df0;
color:white;
font-size:17px;
transition:.4s;
box-shadow:0 0 20px #ff4df0;
}

button:hover{transform:scale(1.08);}

.message-section{
padding:100px 20px;
display:flex;
justify-content:center;
}

.message-card{
max-width:850px;
padding:40px;
border-radius:20px;
border:2px solid #ff4df0;
box-shadow:0 0 20px #ff4df0;
text-align:center;
}

.message-card h2{font-size:35px;margin-bottom:20px;}

.message-card p{
font-size:18px;
line-height:1.9;
}

.gallery-section{
padding:100px 20px;
text-align:center;
}

.gallery-section h2{
font-size:45px;
margin-bottom:40px;
}

.slider{
display:flex;
justify-content:center;
align-items:center;
gap:20px;
}

.slide-container{
width:250px;
height:250px;
overflow:hidden;
}

.slide{
display:none;
width:100%;
height:100%;
font-size:80px;
border:2px solid #ff4df0;
border-radius:25px;
justify-content:center;
align-items:center;
box-shadow:0 0 20px #ff4df0;
}

.slide.active{display:flex;}

.prev,.next{
font-size:30px;
background:none;
border:none;
color:white;
cursor:pointer;
}

.fun-section{
padding:100px 20px;
text-align:center;
}

.fun-grid{
margin-top:50px;
display:grid;
grid-template-columns:repeat(auto-fit,minmax(180px,1fr));
gap:25px;
}

.fun-box{
padding:40px;
font-size:50px;
border:2px solid #ff4df0;
border-radius:20px;
cursor:pointer;
transition:.4s;
box-shadow:0 0 15px #ff4df0;
}

.fun-box:hover{transform:translateY(-10px);}

.popup{
display:none;
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:rgba(0,0,0,.8);
justify-content:center;
align-items:center;
z-index:1000;
}

.popup-content{
background:#111;
padding:30px;
border-radius:20px;
max-width:500px;
text-align:center;
border:2px solid #ff4df0;
}

#closePopup{float:right;cursor:pointer;font-size:28px;}

.gift-section{
padding:100px 20px;
text-align:center;
}

.gift-box{
width:180px;
height:180px;
margin:40px auto;
position:relative;
}

.gift-body{
width:180px;
height:120px;
background:#ff4df0;
position:absolute;
bottom:0;
border-radius:10px;
}

.gift-top{
width:180px;
height:50px;
background:#ff85f7;
position:absolute;
top:0;
border-radius:10px;
transition:1s;
}

.gift-open .gift-top{
transform:translateY(-90px) rotate(-10deg);
}

#giftMessage{
display:none;
font-size:28px;
margin-top:30px;
color:#ffd700;
}

.final-section{
padding:150px 20px;
text-align:center;
}

.sky-heart{
font-size:90px;
animation:pulse 2s infinite;
}

@keyframes pulse{
50%{transform:scale(1.2);}
}

.final-section h2{
font-size:55px;
margin-bottom:20px;
font-family:'Great Vibes',cursive;
color:#ff73ff;
}

.final-section p{
max-width:700px;
margin:auto;
line-height:2;
font-size:20px;
}

@media(max-width:768px){
.hero-title{font-size:55px;}
.intro-card h1{font-size:45px;}
#countdown{font-size:70px;}
.message-card{padding:25px;}
}

/* ===== YOUR CSS END ===== */

</style>

</head>

<body>

<div id="particles"></div>

<section id="intro">
<div class="intro-card">
<div class="moon">🌙</div>
<h1>A Surprise For You...</h1>
<div id="countdown">10</div>
<p>Something beautiful is loading ✨</p>
</div>
</section>

<div id="website">

<section class="hero">
<div class="glow-circle"></div>

<h1 class="hero-title">Happy Birthday Bestie 🎂</h1>

<p class="hero-subtitle">
Today is all about celebrating the amazing soul that makes every moment brighter 💜
</p>

<div class="hero-buttons">
<button id="celebrateBtn">Celebrate 🎉</button>
<button id="musicBtn">🎵 Music</button>
</div>
</section>

<section class="message-section">
<div class="message-card">
<h2>Dear Best Friend 💌</h2>
<p id="typing-text"></p>
</div>
</section>

<section class="gallery-section">
<h2>Memories 🌸</h2>

<div class="slider">
<button class="prev">❮</button>

<div class="slide-container">
<div class="slide active">👭💜✨</div>
<div class="slide">🌙🎂💖</div>
<div class="slide">🎁🌸⭐</div>
<div class="slide">💫🧸💕</div>
</div>

<button class="next">❯</button>
</div>
</section>

<section class="fun-section">
<h2>Choose Something Fun ✨</h2>

<div class="fun-grid">
<div class="fun-box" id="heartBtn">❤️<span>Open Heart</span></div>
<div class="fun-box" id="letterBtn">💌<span>Sweet Message</span></div>
<div class="fun-box" id="wishBtn">⭐<span>Make A Wish</span></div>
<div class="fun-box" id="giftOpenBtn">🎁<span>Special Gift</span></div>
</div>
</section>

<div class="popup" id="popup">
<div class="popup-content">
<span id="closePopup">×</span>
<p id="popupText"></p>
</div>
</div>

<section class="gift-section">
<h2>Your Surprise Gift 🎁</h2>

<div class="gift-box">
<div class="gift-top"></div>
<div class="gift-body"></div>
</div>

<button id="openGift">Open Gift 💖</button>

<div id="giftMessage">
You are one of the most precious people in my life 💜✨
</div>
</section>

<section class="final-section">
<div class="sky-heart">💖</div>

<h2>I'm Lucky To Have You</h2>

<p>
Thank you for being such an important part of my life.
May your smile always shine brighter than the stars.

Happy Birthday Once Again 🎂✨
</p>
</section>

</div>

<audio id="birthdayMusic" loop>
<source src="music.mp3" type="audio/mpeg">
</audio>

<script>
/* ===== YOUR JS (basic safe merge template) ===== */

const intro = document.getElementById("intro");
const website = document.getElementById("website");
const countdown = document.getElementById("countdown");

let time = 10;

let timer = setInterval(() => {
time--;
countdown.textContent = time;

if(time === 0){
clearInterval(timer);
intro.style.display = "none";
website.style.display = "block";
}
},1000);

/* buttons */
document.getElementById("celebrateBtn").onclick = () => {
alert("🎉 Happy Birthday!");
};

document.getElementById("musicBtn").onclick = () => {
const music = document.getElementById("birthdayMusic");
music.play();
};

/* gift */
document.getElementById("openGift").onclick = () => {
document.querySelector(".gift-box").classList.toggle("gift-open");
document.getElementById("giftMessage").style.display = "block";
};

/* slider */
let index = 0;
const slides = document.querySelectorAll(".slide");

document.querySelector(".next").onclick = () => {
slides[index].classList.remove("active");
index = (index + 1) % slides.length;
slides[index].classList.add("active");
};

document.querySelector(".prev").onclick = () => {
slides[index].classList.remove("active");
index = (index - 1 + slides.length) % slides.length;
slides[index].classList.add("active");
};

</script>

</body>
</html>
