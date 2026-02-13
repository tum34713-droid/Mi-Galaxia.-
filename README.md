# Mi-Galaxia.-
<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Te Amo 💜</title>
<style>
body{
  margin:0;
  overflow:hidden;
  background: radial-gradient(circle, #3b0066, #12001f);
  font-family: Arial;
  color:white;
  text-align:center;
}

h1{
  position:absolute;
  top:20px;
  width:100%;
}

.palabra{
  position:absolute;
  font-size:14px;
  animation: flotar 6s linear infinite;
}

@keyframes flotar{
  from{ transform: translateY(100vh); opacity:1;}
  to{ transform: translateY(-10vh); opacity:0;}
}
</style>
</head>

<body>

<h1>Te Amo Muchote 💛</h1>

<script>
const palabras = [
"Mi Reina 👑","Mi Amor","Mi Vida","Mi Tesoro",
"Mi Mundo","Mi Niña","Mi Paz","Mi Luz"
];

function crearPalabra(){
  const span = document.createElement("span");
  span.className="palabra";
  span.innerText = palabras[Math.floor(Math.random()*palabras.length)];
  span.style.left = Math.random()*100 + "vw";
  span.style.fontSize = (Math.random()*20+10)+"px";
  document.body.appendChild(span);

  setTimeout(()=>{ span.remove(); },6000);
}

setInterval(crearPalabra,300);
</script>

</body>
</html>
