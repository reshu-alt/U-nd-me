# U-nd-me
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Happy Birthday G 💙</title>

<style>
body {
    margin: 0;
    font-family: 'Poppins', sans-serif;
    background: linear-gradient(135deg,#cdb4db,#a2d2ff,#ffc8dd);
    color: white;
    text-align: center;
    overflow-x: hidden;
}

.page {
    display: none;
    padding: 40px 20px;
    min-height: 100vh;
}

.active {
    display: block;
}

h1, h2 {
    animation: fadeIn 2s ease-in-out;
}

button {
    padding: 12px 25px;
    margin: 10px;
    border: none;
    border-radius: 25px;
    font-size: 16px;
    cursor: pointer;
    background: linear-gradient(45deg,#89cff0,#ffafcc);
    color: white;
    transition: 0.3s;
}

button:hover {
    transform: scale(1.1);
}

img {
    width: 250px;
    border-radius: 20px;
    margin: 15px;
    box-shadow: 0 0 20px rgba(255,255,255,0.6);
}

.gallery {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

textarea {
    width: 80%;
    height: 100px;
    border-radius: 15px;
    border: none;
    padding: 10px;
}

.music-player {
    margin: 20px 0;
    background: rgba(255,255,255,0.2);
    padding: 15px;
    border-radius: 15px;
    backdrop-filter: blur(10px);
}

audio {
    width: 100%;
    max-width: 400px;
    margin: 10px auto;
}

@keyframes fadeIn {
    from {opacity: 0;}
    to {opacity: 1;}
}

#noBtn {
    position: absolute;
}
</style>
</head>

<body>

<!-- Background Music -->
<audio id="bgmusic" loop>
  <source src="music/mereyaara.mp3" type="audio/mpeg">
</audio>

<!-- PAGE 1 -->
<div class="page active" id="page1">
    <h1>Happy Birthday My G 💙</h1>
    <h2>Are you ready for your surprise, Bobo? 🐷</h2>
    <button onclick="startJourney()">💙 Yes obviously!</button>
    <button id="noBtn">🙄 No but okay</button>
</div>

<!-- PAGE 2 -->
<div class="page" id="page2">
    <h2>Our Story Begins 💫</h2>
    <p>You and me... the cutest chaos ever created 💙</p>
    <img src="data:image/jpeg;base64,/9j/..." alt="Memory 1">
    <img src="data:image/jpeg;base64,/9j/..." alt="Memory 2">
    <br>
    <button onclick="nextPage(3)">Wanna see something more crazy? 👀</button>
</div>

<!-- PAGE 3 -->
<div class="page" id="page3">
    <h2>Our Top Songs Era 🎵</h2>
    <div class="music-player">
        <p>🎵 Listen to our songs:</p>
        <audio controls>
            <source src="music/mereyaara.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <p>Mere Yaara 💿</p>
    </div>
    
    <div class="music-player">
        <audio controls>
            <source src="music/banarasiya.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <p>Banarasiya 💿</p>
    </div>
    
    <div class="music-player">
        <audio controls>
            <source src="music/tu-kisi-rail.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <p>Tu Kisi Rail Si Guzarti Hai 💿</p>
    </div>
    
    <div class="music-player">
        <audio controls>
            <source src="music/pehli-baar.mp3" type="audio/mpeg">
            Your browser does not support the audio element.
        </audio>
        <p>Pehli Baar 💿</p>
    </div>
    
    <button onclick="nextPage(4)">Play Mini Game 🎮</button>
</div>

<!-- PAGE 4 GAME -->
<div class="page" id="page4">
    <h2>Mini Game 😏</h2>
    <p>What is my nickname for you?</p>
    <button onclick="correctAnswer()">Bobo 🐷</button>
    <button onclick="wrongAnswer()">Golu</button>
</div>

<!-- PAGE 5 -->
<div class="page" id="page5">
    <h2>Memory Gallery 📸</h2>
    <div class="gallery">
        <img src="data:image/jpeg;base64,/9j/..." alt="Memory 3">
        <img src="data:image/webp;base64,/9j/..." alt="Memory 4">
        <img src="data:image/jpeg;base64,/9j/..." alt="Memory 5">
    </div>
    <button onclick="nextPage(6)">Open Secret Vault 🔐</button>
</div>

<!-- PAGE 6 -->
<div class="page" id="page6">
    <h2>10 Reasons I Love You 💌</h2>
    <p>1. You are my safe place 💙</p>
    <p>2. You tolerate my drama 😌</p>
    <p>3. Certified Bobo 🐷</p>
    <p>4. My human teddy bear</p>
    <p>5. You support my dreams</p>
    <p>6. Your laugh is contagious 😂</p>
    <p>7. You make ordinary moments special</p>
    <p>8. Your presence calms me</p>
    <p>9. You believe in me always</p>
    <p>10. Because you're you 💙</p>
    <button onclick="nextPage(7)">Next Surprise 🎁</button>
</div>

<!-- PAGE 7 -->
<div class="page" id="page7">
    <h2>Choose Our Next Date 🎮</h2>
    <button onclick="alert('Movie night it is 🎬💙')">Movie Night</button>
    <button onclick="alert('Long drive with songs 🚗💙')">Long Drive</button>
    <button onclick="alert('Annoying each other forever 😏')">Annoy Each Other</button>
    <button onclick="alert('Nice try 😂 No silent treatment allowed')">Silent Treatment</button>
    <br><br>
    <button onclick="nextPage(8)">Final Page 💖</button>
</div>

<!-- PAGE 8 -->
<div class="page" id="page8">
    <h2>Future With You 🌌</h2>
    <p>I want to grow with you, support you, and celebrate every birthday together 💙</p>
    <h3>Happy Birthday once again my forever person 💙</h3>
    <p>Yours forever (even when you're annoying),</p>
    <h2>Reshu 💌</h2>

    <h3>Write something for me Bobo 🐷</h3>
    <textarea placeholder="Type here..."></textarea>
</div>

<script>
function startJourney(){
    document.getElementById("bgmusic").play();
    nextPage(2);
}

function nextPage(pageNumber){
    document.querySelectorAll(".page").forEach(p => p.classList.remove("active"));
    document.getElementById("page"+pageNumber).classList.add("active");
}

function correctAnswer(){
    alert("Correct 😌 You know me well Bobo 🐷");
    nextPage(5);
}

function wrongAnswer(){
    alert("Wrong 😏 Try again!");
}

const noBtn = document.getElementById("noBtn");

noBtn.addEventListener("mouseover", function() {
    const x = Math.random() * (window.innerWidth - 150);
    const y = Math.random() * (window.innerHeight - 150);
    noBtn.style.left = x + "px";
    noBtn.style.top = y + "px";
});
</script>

</body>
</html>![IMG_20260201_160458_367](https://github.com/user-attachments/assets/3c09622e-299f-4548-b0bb-11eeebfd6e8c)
![IMG_20260219_191638_991](https://github.com/user-attachments/assets/c9114c87-eb6f-4071-9dfc-a47e53bc2f76)
