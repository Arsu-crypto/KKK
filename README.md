<html>
<head>
  <title>Happy Birthday Samra 🎉</title>
  <style>
    body {
      margin: 0;
      padding: 0;
      font-family: 'Times New Roman', Times, serif; /* Roman font */
      overflow: hidden;
      text-align: center;
      background: url('https://i.pinimg.com/736x/b6/8c/d2/b68cd2c21df95e1f2d445c0d2f997e8b.jpg') no-repeat center center fixed;
      background-size: cover;
      color: #fff;
    }

    #intro {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
    }

    #intro button {
      padding: 20px 40px;
      font-size: 30px;
      font-weight: bold;
      background: #ff69b4;
      color: white;
      border: none;
      border-radius: 15px;
      cursor: pointer;
      box-shadow: 2px 2px 10px rgba(0,0,0,0.5);
      transition: 0.3s;
    }

    #intro button:hover {
      transform: scale(1.1);
      box-shadow: 2px 2px 20px rgba(0,0,0,0.7);
    }

    #birthday {
      display: none;
      width: 100%;
      height: 100vh;
      position: relative;
    }

    h1 {
      margin-top: 12%;
      font-size: 90px; /* big heading */
      font-weight: bold;
      color: #ff69b4;
      text-shadow: 2px 2px 12px #fff, 0 0 25px #ff69b4;
      animation: fadeIn 3s ease-in-out;
    }

    p {
      font-size: 24px; /* smaller dua/message */
      margin-top: 20px;
      text-shadow: 1px 1px 5px rgba(0,0,0,0.5);
      animation: fadeIn 4s ease-in-out;
    }

    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }

    .flower {
      position: absolute;
      animation: fall linear infinite;
      opacity: 0.9;
      pointer-events: none;
    }

    @keyframes fall {
      0% {top: -10%; transform: rotate(0deg);}
      100% {top: 110%; transform: rotate(360deg);}
    }
  </style>
</head>
<body>

<div id="intro">
  <button onclick="showBirthday()">Open your surprise 🎉</button>
</div>

<div id="birthday">
  <h1>Happy Birthday Samra</h1>
  <p>May Allah keep you happy and bless you with a long, peaceful life. Happy Birthday, Sister!</p> 

  <audio autoplay loop>
    <source src="https://www.bensound.com/bensound-music/bensound-buddy.mp3" type="audio/mpeg">
  </audio>
</div>

<script>
function showBirthday() {
  document.getElementById('intro').style.display = 'none';
  document.getElementById('birthday').style.display = 'block';
}

// Attractive pink & white flowers (same method as pehle)
const flowerImages = [
  "https://i.ibb.co/qC9dQYf/pink-flower.png",
  "https://i.ibb.co/7JcDgHf/white-flower.png",
  "https://i.ibb.co/8mZ7V1M/pink2-flower.png"
];

for(let i=0; i<50; i++){
  let flower = document.createElement("img");
  flower.src = flowerImages[Math.floor(Math.random()*flowerImages.length)];
  flower.className = "flower";
  flower.style.left = Math.random()*100 + "vw";
  flower.style.width = (30 + Math.random()*50) + "px";
  flower.style.animationDuration = (Math.random()*5 + 5) + "s";
  document.getElementById('birthday').appendChild(flower);
}
</script>

</body>
</html>
