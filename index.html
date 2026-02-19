<!doctype html>
<html lang="es">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1">
<title>La Tierra y la Biosfera · Evaluación</title>

<style>
body{
  margin:0;
  font-family: Arial, sans-serif;
  background: linear-gradient(135deg,#0b1320,#0e3a3a);
  color:white;
  padding:20px;
}

.wrap{
  max-width:1100px;
  margin:auto;
}

header{
  background:rgba(255,255,255,0.08);
  padding:20px;
  border-radius:15px;
  margin-bottom:20px;
}

h1{margin:0;}

input{
  margin-top:15px;
  padding:10px;
  width:100%;
  max-width:400px;
  border-radius:8px;
  border:none;
  font-size:14px;
}

.grid{
  display:grid;
  grid-template-columns:1fr;
  gap:20px;
}

@media(min-width:900px){
  .grid{
    grid-template-columns:1fr 1fr;
  }
}

.panel{
  background:white;
  color:#333;
  padding:15px;
  border-radius:15px;
}

.chips{
  display:flex;
  flex-wrap:wrap;
  gap:10px;
}

.chip{
  padding:8px 12px;
  border-radius:20px;
  background:#f1f5f9;
  cursor:grab;
  font-weight:bold;
}

.target{
  border:1px solid #ddd;
  padding:10px;
  border-radius:10px;
  margin-bottom:10px;
}

.dropzone{
  border:2px dashed #aaa;
  padding:10px;
  text-align:center;
  border-radius:8px;
  margin-top:8px;
}

.correct{
  background:#d1fae5;
  border-color:#16a34a;
}

.wrong{
  background:#fee2e2;
  border-color:#dc2626;
}

button{
  margin-top:15px;
  padding:10px 15px;
  border:none;
  border-radius:8px;
  background:#2563eb;
  color:white;
  font-weight:bold;
  cursor:pointer;
}

button.secondary{
  background:gray;
}

.toast{
  margin-top:15px;
  padding:15px;
  background:#0f172a;
  border-radius:10px;
}
</style>
</head>

<body>

<div class="wrap">

<header>
<h1>🌍 La Tierra y la Biosfera · Evaluación</h1>
<p>Arrastra cada concepto a su definición correcta y presiona Calificar.</p>

<input type="text" id="studentName" placeholder="Escribe tu nombre completo">

<br>
<button class="secondary" onclick="init()">Reiniciar</button>
<button onclick="grade()">Calificar</button>

<div id="result"></div>

</header>

<div class="grid">

<div class="panel">
<h2>Conceptos</h2>
<div class="chips" id="chips"></div>
</div>

<div class="panel">
<h2>Definiciones</h2>
<div id="targets"></div>
</div>

</div>

</div>

<script>
const BANK = [
{key:"Atmósfera", def:"Capa de gases que rodea la Tierra y regula el clima."},
{key:"Hidrosfera", def:"Conjunto de todas las aguas del planeta."},
{key:"Litosfera", def:"Capa sólida externa de la Tierra."},
{key:"Biosfera", def:"Zona donde existe vida en el planeta."},
{key:"Ecosistema", def:"Interacción entre seres vivos y su ambiente."},
{key:"Biodiversidad", def:"Variedad de especies, genes y ecosistemas."},
{key:"Ciclo del agua", def:"Movimiento del agua entre evaporación y precipitación."},
{key:"Ciclo del carbono", def:"Circulación del carbono entre atmósfera y seres vivos."},
{key:"Cadenas tróficas", def:"Relaciones alimentarias entre organismos."},
{key:"Servicios ecosistémicos", def:"Beneficios que la naturaleza brinda al ser humano."}
];

let placements = {};
let graded = false;

function shuffle(arr){
return arr.sort(()=>Math.random()-0.5);
}

function init(){
placements = {};
graded = false;

document.getElementById("result").innerHTML="";

const chipsDiv = document.getElementById("chips");
chipsDiv.innerHTML="";

shuffle([...BANK]).forEach(item=>{
const chip = document.createElement("div");
chip.className="chip";
chip.textContent=item.key;
chip.draggable=true;
chip.dataset.key=item.key;

chip.addEventListener("dragstart", e=>{
e.dataTransfer.setData("text", item.key);
});

chipsDiv.appendChild(chip);
});

const targetsDiv=document.getElementById("targets");
targetsDiv.innerHTML="";

shuffle([...BANK]).forEach((item,i)=>{
const div=document.createElement("div");
div.className="target";

div.innerHTML=`<strong>${item.def}</strong>
<div class="dropzone" data-correct="${item.key}">Suelta aquí</div>`;

const zone=div.querySelector(".dropzone");

zone.addEventListener("dragover", e=>e.preventDefault());

zone.addEventListener("drop", e=>{
e.preventDefault();
if(graded) return;
const key=e.dataTransfer.getData("text");
zone.textContent=key;
placements[i]=key;
});

targetsDiv.appendChild(div);
});
}

function grade(){

const name=document.getElementById("studentName").value.trim();

if(name===""){
alert("Por favor escribe tu nombre antes de calificar.");
return;
}

if(graded) return;

let correct=0;
const zones=document.querySelectorAll(".dropzone");

zones.forEach((zone,i)=>{
const expected=zone.dataset.correct;
const placed=placements[i];

zone.classList.remove("correct","wrong");

if(placed===expected){
zone.classList.add("correct");
correct++;
}else{
zone.classList.add("wrong");
}
});

graded=true;

const total=BANK.length;
const percent=Math.round((correct/total)*100);

let mensaje="";
if(percent>=90) mensaje="Excelente dominio 👏";
else if(percent>=70) mensaje="Buen trabajo ✅";
else if(percent>=50) mensaje="Vas avanzando ⚠️";
else mensaje="Necesitas repasar 💪";

document.getElementById("result").innerHTML=
`<div class="toast">
<strong>Alumno:</strong> ${name}<br>
<strong>Resultado:</strong> ${correct} / ${total} (${percent}%)<br>
${mensaje}<br><br>
Toma captura de pantalla y súbela a Classroom.
</div>`;
}

init();
</script>

</body>
</html>
