<!DOCTYPE html>
<html lang="fr">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>ICP IADE</title>

<style>
body {
  font-family: 'Segoe UI', Arial, sans-serif;
  margin: 0;
  padding: 10px;
  background: linear-gradient(135deg,#eaf2f8,#d6eaf8);
}

.hidden { display:none; }

header {
  background: rgba(93,173,226,0.6);
  backdrop-filter: blur(12px);
  color:white;
  padding:25px;
  text-align:center;
  border-radius:20px;
}

.card {
  background: rgba(255,255,255,0.7);
  backdrop-filter: blur(10px);
  border-radius:20px;
  padding:18px;
  margin-bottom:15px;
  box-shadow:0 8px 25px rgba(0,0,0,0.08);
  animation: fadeUp 0.6s ease forwards;
}

@keyframes fadeUp {
  from {opacity:0; transform:translateY(20px);} 
  to {opacity:1; transform:translateY(0);} 
}

.btn {
  display:block;
  padding:16px;
  border-radius:14px;
  text-align:center;
  font-weight:bold;
  background: linear-gradient(135deg,#3498db,#5dade2);
  color:white;
  margin-bottom:10px;
}

.bottom-menu {
  position:fixed;
  bottom:0;
  width:100%;
  backdrop-filter: blur(12px);
  background: rgba(255,255,255,0.8);
  display:flex;
  justify-content:space-around;
  padding:10px;
}

.login {
  display:flex;
  flex-direction:column;
  align-items:center;
  justify-content:center;
  height:80vh;
}

input { padding:12px; margin:10px; border-radius:8px; }

.disclaimer-overlay {
  position:fixed;
  top:0;left:0;width:100%;height:100%;
  background:rgba(0,0,0,0.85);
  display:flex;justify-content:center;align-items:center;
  z-index:9999;
}

.disclaimer-box {
  background:white;
  padding:25px;
  border-radius:20px;
  text-align:center;
}

#splash {
  position:fixed;
  width:100%;height:100%;
  background: linear-gradient(135deg,#5dade2,#48c9b0);
  color:white;
  display:flex;
  justify-content:center;
  align-items:center;
  font-size:30px;
  z-index:99999;
  animation: fadeOut 1s ease 2s forwards;
}

@keyframes fadeOut { to {opacity:0; visibility:hidden;} }

</style>
</head>

<body>

<div id="splash">🫀 ICP</div>

<header>
<h1>Bienvenue à l’ICP</h1>
<p>Bloc opératoire – IADE</p>
</header>

<div id="loginPage" class="login">
<h2>Accès réservé</h2>
<input type="password" id="password" placeholder="Mot de passe">
<button onclick="checkPassword()">Entrer</button>
<p id="error" style="color:red"></p>
</div>

<div id="disclaimer" class="disclaimer-overlay hidden">
<div class="disclaimer-box">
<h2>⚠️ Avertissement</h2>
<p>Support pédagogique non officiel</p>
<p>Ne remplace pas les protocoles</p>
<button onclick="acceptDisclaimer()">Continuer</button>
</div>
</div>

<div id="content" style="display:none;">

<div class="card">
<h2>Bienvenue</h2>
<p>Bienvenue au bloc ICP</p>
</div>

<div class="card">
<h2>Accès documents</h2>
<div class="btn" onclick="toggleMenu()">Protocoles</div>
<div id="menu" class="hidden">
<a class="btn" href="#">PDF 1</a>
<a class="btn" href="#">PDF 2</a>
</div>
</div>

</div>

<div class="bottom-menu">
<a href="#">📑</a>
<a href="#">🗺</a>
<a href="#">🎥</a>
</div>

<script>
function checkPassword(){
const password=document.getElementById("password").value;
if(password==="iadeicp543"){
 document.getElementById("loginPage").style.display="none";
 document.getElementById("disclaimer").classList.remove("hidden");
}else{
 document.getElementById("error").innerText="Incorrect";
}}

function acceptDisclaimer(){
 document.getElementById("disclaimer").style.display="none";
 document.getElementById("content").style.display="block";
}

function toggleMenu(){
 document.getElementById("menu").classList.toggle("hidden");
}
</script>

</body>
</html>
