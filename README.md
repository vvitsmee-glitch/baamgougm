<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1.0" />
<title>Bama Go To UGM</title>

<style>
@import url('https://fonts.googleapis.com/css2?family=Creepster&display=swap');

body {
    margin: 0;
    height: 100vh;
    overflow: hidden;
    font-family: "Creepster", cursive;
    background: linear-gradient(to top, #020111, #191970);
}

/* LANGIT */
.sky {
    position: absolute;
    width: 100%;
    height: 100%;
}

/* AWAN */
.cloud {
    position: absolute;
    background: #fff;
    border-radius: 50%;
    opacity: 0.8;
}

.cloud::before,
.cloud::after {
    content: "";
    position: absolute;
    background: #fff;
    border-radius: 50%;
}

.cloud1 {
    width: 120px;
    height: 60px;
    top: 20%;
    left: -150px;
    animation: moveCloud 30s linear infinite;
}

.cloud1::before {
    width: 60px;
    height: 60px;
    top: -20px;
    left: 10px;
}

.cloud1::after {
    width: 80px;
    height: 80px;
    top: -30px;
    left: 40px;
}

.cloud2 {
    width: 150px;
    height: 70px;
    top: 40%;
    left: -200px;
    animation: moveCloud 45s linear infinite;
}

@keyframes moveCloud {
    from { transform: translateX(0); }
    to { transform: translateX(120vw); }
}

/* BINTANG */
.star {
    position: absolute;
    width: 2px;
    height: 2px;
    background: white;
    animation: twinkle 2s infinite alternate;
}

@keyframes twinkle {
    from { opacity: 0.2; }
    to { opacity: 1; }
}

/* TEKS */
h1 {
    position: absolute;
    color: transparent;
    font-size: 80px;
    text-align: center;
    background: linear-gradient(90deg, red, orange, yellow, cyan, blue, purple);
    -webkit-background-clip: text;
    animation: glow 2s ease-in-out infinite alternate;
}

@keyframes glow {
    from {
        text-shadow: 0 0 10px red, 0 0 20px orange;
    }
    to {
        text-shadow: 0 0 20px cyan, 0 0 40px blue;
    }
}
</style>
</head>

<body>

<div class="sky">
    <!-- AWAN -->
    <div class="cloud cloud1"></div>
    <div class="cloud cloud2"></div>     
    <!-- BINTANG RANDOM -->
    <script>
        for(let i=0;i<100;i++){
            let star = document.createElement("div");
            star.className = "star";
            star.style.top = Math.random()*100 + "vh";
            star.style.left = Math.random()*100 + "vw";
            star.style.animationDuration = (Math.random()*2+1)+"s";
            document.body.appendChild(star);
        }
    </script>
</div>

<h1>BAMA GO TO UGM</h1>

</body>
</html>
