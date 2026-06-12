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
</html># MATWI