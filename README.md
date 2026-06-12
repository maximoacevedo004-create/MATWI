<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Base de Datos de Tornados F4 y F5</title>

<style>
body{
    font-family:Arial,Helvetica,sans-serif;
    margin:0;
    background:#111;
    color:white;
}

header{
    background:#003366;
    padding:20px;
    text-align:center;
}

input{
    width:80%;
    max-width:500px;
    padding:12px;
    border-radius:8px;
    border:none;
    margin-top:15px;
    font-size:16px;
}

.contenedor{
    display:flex;
    flex-wrap:wrap;
    justify-content:center;
    gap:20px;
    padding:20px;
}

.tarjeta{
    width:350px;
    background:#222;
    border-radius:10px;
    padding:20px;
    box-shadow:0 0 10px rgba(0,0,0,.5);
}

.tarjeta h2{
    color:#4fc3f7;
}

footer{
    background:#000;
    text-align:center;
    padding:20px;
}
</style>

</head>

<body>

<header>

<h1>🌪 Tornados F4 y F5</h1>

<p>Busca cualquier tornado por su nombre o ciudad.</p>

<input type="text" id="buscar" placeholder="Buscar tornado..." onkeyup="filtrar()">

</header>

<div class="contenedor" id="lista">

<div class="tarjeta">
<h2>El Reno (2011)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Oklahoma, Estados Unidos</p>
<p><b>Vientos:</b> 476 km/h</p>
<p><b>Ancho:</b> 2.4 km</p>
<p><b>Recorrido:</b> 101 km</p>
<p><b>Fallecidos:</b> 9</p>
<p><b>Heridos:</b> 181</p>
<p><b>Descripción:</b> Uno de los tornados más violentos registrados.</p>
</div>

<div class="tarjeta">
<h2>Joplin (2011)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Misuri</p>
<p><b>Vientos:</b> 320 km/h</p>
<p><b>Ancho:</b> 1.6 km</p>
<p><b>Recorrido:</b> 35 km</p>
<p><b>Fallecidos:</b> 158</p>
<p><b>Heridos:</b> Más de 1000</p>
</div>

<div class="tarjeta">
<h2>Moore (2013)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Oklahoma</p>
<p><b>Vientos:</b> 340 km/h</p>
<p><b>Ancho:</b> 2.1 km</p>
<p><b>Recorrido:</b> 27 km</p>
<p><b>Fallecidos:</b> 24</p>
</div>

<div class="tarjeta">
<h2>Hackleburg (2011)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Alabama</p>
<p><b>Vientos:</b> 340 km/h</p>
<p><b>Ancho:</b> 1.2 km</p>
<p><b>Recorrido:</b> 212 km</p>
<p><b>Fallecidos:</b> 72</p>
</div>

<div class="tarjeta">
<h2>Bridge Creek–Moore (1999)</h2>
<p><b>Categoría:</b> F5</p>
<p><b>Ubicación:</b> Oklahoma</p>
<p><b>Vientos:</b> 484 km/h</p>
<p><b>Ancho:</b> 1.6 km</p>
<p><b>Recorrido:</b> 61 km</p>
<p><b>Fallecidos:</b> 36</p>
</div>

<div class="tarjeta">
<h2>Greensburg (2007)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Kansas</p>
<p><b>Vientos:</b> 330 km/h</p>
<p><b>Ancho:</b> 2.7 km</p>
<p><b>Recorrido:</b> 45 km</p>
<p><b>Fallecidos:</b> 11</p>
</div>

<div class="tarjeta">
<h2>Parkersburg (2008)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Iowa</p>
<p><b>Vientos:</b> 330 km/h</p>
<p><b>Ancho:</b> 1.2 km</p>
<p><b>Recorrido:</b> 69 km</p>
<p><b>Fallecidos:</b> 9</p>
</div>

<div class="tarjeta">
<h2>Smithville (2011)</h2>
<p><b>Categoría:</b> EF5</p>
<p><b>Ubicación:</b> Misisipi</p>
<p><b>Vientos:</b> 330 km/h</p>
<p><b>Ancho:</b> 0.8 km</p>
<p><b>Recorrido:</b> 79 km</p>
<p><b>Fallecidos:</b> 23</p>
</div>

</div>

<footer>

<p>Base de datos de tornados F4 y F5.</p>

</footer>

<script>
function filtrar(){

let texto=document.getElementById("buscar").value.toLowerCase();

let tarjetas=document.getElementsByClassName("tarjeta");

for(let i=0;i<tarjetas.length;i++){

let contenido=tarjetas[i].innerText.toLowerCase();

if(contenido.indexOf(texto)>-1){
tarjetas[i].style.display="block";
}else{
tarjetas[i].style.display="none";
}

}

}
</script>

</body>
</html># <!-- =========================
     CARRUSEL DE IMÁGENES
========================= -->
<div class="slider">
    <img id="foto"
    src="https://upload.wikimedia.org/wikipedia/commons/5/56/Tornado_Elie_Manitoba_2007.jpg">
</div>
<style>
.slider{
    width:95%;
    max-width:1000px;
    margin:auto;
    overflow:hidden;
    border-radius:15px;
    box-shadow:0 0 20px #00bfff;
}
.slider img{
    width:100%;
    height:450px;
    object-fit:cover;
}
</style>
<script>
let imagenes=[
"https://upload.wikimedia.org/wikipedia/commons/5/56/Tornado_Elie_Manitoba_2007.jpg",
"https://upload.wikimedia.org/wikipedia/commons/4/4b/Supercell_thunderstorm.jpg",
"https://upload.wikimedia.org/wikipedia/commons/f/f4/Tornado_near_Elie_Manitoba.jpg"
];
let numero=0;
setInterval(function(){
numero++;
if(numero>=imagenes.length){
numero=0;
}
document.getElementById("foto").src=imagenes[numero];
},4000);
</script>
<!-- =========================
     MAPA
========================= -->
<h2>🗺️ Mapa Mundial de Tornados</h2>
<iframe
src="https://www.google.com/maps/embed?pb=!1m18"
width="100%"
height="450"
style="border:0;border-radius:15px;"
loading="lazy">
</iframe>
<!-- =========================
     EFECTO LLUVIA
========================= -->
<style>
body::before{
content:"";
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background-image:
linear-gradient(
transparent 70%,
rgba(255,255,255,.15)
);
background-size:3px 30px;
animation:lluvia .3s linear infinite;
pointer-events:none;
}
@keyframes lluvia{
from{
transform:translateY(-30px);
}
to{
transform:translateY(30px);
}
}
</style>
<!-- =========================
     RAYOS
========================= -->
<style>
@keyframes relampago{
0%{opacity:0;}
5%{opacity:.9;}
10%{opacity:0;}
100%{opacity:0;}
}
.flash{
position:fixed;
top:0;
left:0;
width:100%;
height:100%;
background:white;
opacity:0;
animation:relampago 8s infinite;
pointer-events:none;
}
</style>
<div class="flash"></div>
<!-- =========================
     BOTÓN MODO OSCURO
========================= -->
<button onclick="modo()" id="boton">
🌙 Cambiar tema
</button>
<style>
#boton{
position:fixed;
bottom:20px;
right:20px;
padding:15px;
border:none;
border-radius:30px;
font-size:18px;
cursor:pointer;
background:#2196f3;
color:white;
}
</style>
<script>
function modo(){
document.body.classList.toggle("claro");
}
</script>
<style>
.claro{
background:#f2f2f2;
color:black;
}
.claro .tarjeta{
background:white;
color:black;
}
</style>
<!-- =========================
     CONTADOR
========================= -->
<h2 style="text-align:center;">
🌪 Tornados registrados:
<span id="contador">8</span>
</h2>
<!-- =========================
     REPRODUCTOR DE SONIDO
========================= -->
<audio controls style="width:100%;margin-top:20px;">
<source src="sonidos/trueno.mp3" type="audio/mpeg">
</audio>
<!-- =========================
     BOTÓN SUBIR
========================= -->
<button onclick="window.scrollTo({top:0,behavior:'smooth'})"
style="
position:fixed;
left:20px;
bottom:20px;
padding:15px;
border:none;
border-radius:50%;
font-size:25px;
cursor:pointer;
">
⬆
</button>