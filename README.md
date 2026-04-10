<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>BAMA GO TO UGM</title>

<style>
body {
    margin: 0;
    height: 100vh;
    overflow: hidden;
    font-family: Arial, sans-serif;
}

/* BACKGROUND LANGIT */
.bg {
    position: absolute;
    width: 100%;
    height: 100%;
    background: url('https://i.imgur.com/6Iej2c3.jpg') no-repeat center;
    background-size: cover;
}

/* TEKS */
h1 {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    
    font-size: 50px;
    font-weight: bold;
    text-align: center;

    color: white;
    text-shadow: 0 0 20px rgba(0,0,0,0.5),
                 0 0 40px rgba(0,0,0,0.3);

    animation: float 3s ease-in-out infinite;
}

/* ANIMASI GERAK HALUS */
@keyframes float {
    0%   { transform: translate(-50%, -50%) translateY(0px); }
    50%  { transform: translate(-50%, -50%) translateY(-10px); }
    100% { transform: translate(-50%, -50%) translateY(0px); }
}
</style>
</head>

<body>

<div class="bg"></div>

<h1>BAMA GO TO UGM</h1>

</body>
</html>
