<!DOCTYPE html>  
<html lang="tr">  
<head>  
<meta charset="UTF-8">  
<meta name="viewport" content="width=device-width, initial-scale=1.0">  
<title>Sevgililer Günü Sürprizi</title>  
  
<style>  
body {  
    margin: 0;  
    height: 100vh;  
    display: flex;  
    justify-content: center;  
    align-items: center;  
    background: linear-gradient(135deg, #ff9a9e, #fad0c4);  
    font-family: Arial, sans-serif;  
    overflow: hidden;  
}  
  
.envelope {  
    position: relative;  
    width: 300px;  
    height: 200px;  
    background: #e63946;  
    cursor: pointer;  
    transition: 0.5s;  
}  
  
.flap {  
    position: absolute;  
    top: 0;  
    left: 0;  
    width: 100%;  
    height: 100%;  
    background: #d62828;  
    clip-path: polygon(0 0, 50% 50%, 100% 0);  
    transform-origin: top;  
    transition: 0.6s;  
}  
  
.letter {  
    position: absolute;  
    width: 90%;  
    height: 90%;  
    background: white;  
    top: 5%;  
    left: 5%;  
    display: flex;  
    justify-content: center;  
    align-items: center;  
    text-align: center;  
    padding: 10px;  
    box-sizing: border-box;  
    transform: translateY(100%);  
    transition: 0.6s;  
    font-size: 18px;  
    color: #e63946;  
    border-radius: 10px;  
}  
  
.envelope.open .flap {  
    transform: rotateX(180deg);  
}  
  
.envelope.open .letter {  
    transform: translateY(0);  
}  
</style>  
</head>  
  
<body>  
  
<div class="envelope" onclick="openEnvelope(this)">  
    <div class="flap"></div>  
    <div class="letter">  
        ❤️ Sevgililer Günümüz Kutlu Olsun ❤️<br><br>  
        Seni her şeyden çok seviyorum 💕  
    </div>  
</div>  
  
<script>  
function openEnvelope(el) {  
    el.classList.toggle("open");  
}  
</script>  
  
</body>  
</html>  
