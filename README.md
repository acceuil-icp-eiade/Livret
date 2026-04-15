
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Accueil IADE - ICP</title>

  <style>
    * { box-sizing: border-box; }

    body {
      font-family: 'Segoe UI', Arial, sans-serif;
      margin: 0;
      padding: 10px;
      background-color: #f7f9fb;
      color: #2c3e50;
    }
    body {
  max-width: 500px;
  margin: auto;
    }
header {
  background: linear-gradient(135deg, #5dade2, #48c9b0);
  color: white;
  padding: 15px 10px;
  text-align: center;
  border-radius: 16px;
  margin-bottom: 10px;
}

header h1 {
  font-size: 20px;
  margin-bottom: 5px;
}

header p {
  font-size: 13px;
  opacity: 0.9;
}
    header {
  animation: fadeInHeader 0.8s ease;
}

@keyframes fadeInHeader {
  from {
    opacity: 0;
    transform: translateY(-15px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
    .title {
  opacity: 0;
  transform: translateY(-10px);
  animation: fadeTitle 0.6s ease forwards;
}

@keyframes fadeTitle {
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
    .icons {
  font-size: 28px;
  margin-top: 5px;

  opacity: 0;
  transform: scale(0.8);

  animation: popIcons 0.5s ease forwards;
  animation-delay: 0.4s;
}

/* quand JS ajoute show → on change juste l’état, pas l’animation */
.icons.show {
  opacity: 1;
  transform: scale(1);
  animation: float 2s ease-in-out infinite;
}

@keyframes popIcons {
  to {
    opacity: 1;
    transform: scale(1);
  }
}

@keyframes float {
  0% { transform: translateY(0); }
  50% { transform: translateY(-4px); }
  100% { transform: translateY(0); }
}

.icons {
  will-change: transform, opacity;
}

    /* 🔐 LOGIN */
    .login {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 10px;
  animation: fadeIn 0.6s ease;
}

.login h2 {
  margin-bottom: 10px;
}

input {
  padding: 14px;
  margin: 8px;
  border-radius: 12px;
  border: none;
  width: 240px;
  text-align: center;
  font-size: 16px;
  background: #eef2f7;
  box-shadow: inset 2px 2px 5px rgba(0,0,0,0.05);
}

button {
  padding: 14px 20px;
  border: none;
  border-radius: 12px;
  background: linear-gradient(135deg, #3498db, #5dade2);
  color: white;
  font-weight: bold;
  font-size: 16px;
  margin-top: 10px;
  transition: 0.2s;
  box-shadow: 0 4px 10px rgba(0,0,0,0.15);
}

button:active {
  transform: scale(0.97);
}
    button:hover {
  filter: brightness(1.1);
    }
    
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(15px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
    .card {
      background: white;
      padding: 15px;
      margin-bottom: 15px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }
.card {
  padding: 20px; /* au lieu de 40px ou plus */
  margin-bottom: 20px; /* réduit l’espace en dessous */
}
    h2 {
      color: #3498db;
      font-size: 18px;
    }
    .card {
  transition: transform 0.2s ease, box-shadow 0.2s ease;
}

.card:active {
  transform: scale(0.98);
}

.card:hover {
  transform: translateY(-2px);
  box-shadow: 0 6px 15px rgba(0,0,0,0.12);
}

    button {
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      background: #3498db;
      color: white;
      font-weight: bold;
    }
   button {
  background: linear-gradient(135deg, #3498db, #5dade2);
  box-shadow: 0 4px 10px rgba(0,0,0,0.15);
  transition: 0.2s;
}

button:active {
  transform: scale(0.97);
}
    .hidden {
      display: none;
    }

    .container {
      padding: 10px;
      width: 100%;
      max-width: 100%;
    }

    .card {
      background: white;
      padding: 15px;
      margin-bottom: 15px;
      border-radius: 12px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }
.card {
  padding: 20px; /* au lieu de 40px ou plus */
  margin-bottom: 20px; /* réduit l’espace en dessous */
}
    h2 {
      color: #3498db;
      font-size: 18px;
    }

    /* 🔥 BOUTONS PDF */
    .btn {
      display: block;
      background: #3498db;
      color: white;
      text-decoration: none;
      padding: 16px;
      margin-bottom: 10px;
      border-radius: 12px;
      text-align: center;
      font-size: 16px;
      font-weight: bold;
    }

    .btn:active {
      background: #2c80b4;
    }

    footer {
      text-align: center;
      padding: 15px;
      color: #7f8c8d;
      font-size: 12px;
    }
    .info {
  background: #f9fbfc;
  padding: 12px;
  border-radius: 10px;
  margin-bottom: 10px;
  border-left: 5px solid #48c9b0;
}

.info h3 {
  margin: 0 0 5px 0;
  font-size: 16px;
}
    .info {
  background: #f9fbfc;
  padding: 12px;
  border-radius: 10px;
  margin-bottom: 10px;
  border-left: 5px solid #48c9b0;
}

.info h3 {
  margin: 0 0 5px 0;
  font-size: 16px;
}
    .video-btn {
  width: 100%;
  padding: 14px;
  border: none;
  border-radius: 12px;
  background: linear-gradient(135deg, #48c9b0, #5dade2);
  color: white;
  font-size: 16px;
  font-weight: bold;
  transition: 0.3s;
}

.video-btn:active {
  transform: scale(0.98);
}

.video {
  margin-top: 15px;
  position: relative;
  padding-bottom: 56.25%;
  height: 0;
  overflow: hidden;
  opacity: 0;
  transition: opacity 0.4s ease;
}

.video iframe {
  position: absolute;
  width: 100%;
  height: 100%;
  border-radius: 12px;
}

.video.show {
  opacity: 1;
}
.btn-pdf {
  display: inline-block;
  margin-top: 10px;
  padding: 10px 15px;
  background-color: #2c7be5;
  color: white;
  text-decoration: none;
  border-radius: 8px;
  font-weight: 500;
  transition: 0.2s;
}

.btn-pdf:hover {
  background-color: #1a5fd0;
}

.bottom-menu {
  position: fixed;
  bottom: 0;
  left: 0;
  width: 100%;
  background: white;
  display: flex;
  justify-content: space-around;
  padding: 10px 0;
  box-shadow: 0 -2px 10px rgba(0,0,0,0.1);
  z-index: 1000;
}

.bottom-menu a {
  text-decoration: none;
  font-size: 22px;
}
.fiche {
  background: #ffffff;
  padding: 18px;
  border-radius: 12px;
  box-shadow: 0 3px 10px rgba(0,0,0,0.06);
  margin-bottom: 15px;
}
    .icons {
  font-size: 28px;
  margin-top: 5px;
    }
    .icons {
  font-size: 28px;
  margin-top: 5px;
  animation: float 2s infinite ease-in-out;
}

@keyframes float {
  0% { transform: translateY(0); }
  50% { transform: translateY(-3px); }
  100% { transform: translateY(0); }
}
body {
  padding-bottom: 70px;
}
.fiche:last-child {
  margin-bottom: 25px;
}
 ul {
  padding-left: 18px;
}

li {
  margin-bottom: 6px;
}

.card ul {
  margin-top: 10px;
}
    #chirMenu {
  background-color: #ff4fa3;
  color: white;
    }
    .btn.chirurgie {
  background: linear-gradient(135deg, #ff4fa3, #ff7ac3);
  color: white;
  border-radius: 12px;
  padding: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.15);
    }
#chirMenu {
  background-color: #ff4fa3; /* rose */
  color: white;
  padding: 10px;
  border-radius: 8px;
  }
    .disclaimer-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;

  /* 🔥 effet flou */
  background: rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);

  /* 🎬 animation */
  opacity: 0;
  pointer-events: none;
  transition: opacity 0.4s ease;
}

.disclaimer-overlay.show {
  opacity: 1;
  pointer-events: all;
}
.disclaimer-overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;

  display: flex;
  justify-content: center;
  align-items: center;
  z-index: 9999;

  background: rgba(0, 0, 0, 0.4);
  backdrop-filter: blur(8px);
  -webkit-backdrop-filter: blur(8px);

  opacity: 0;
  pointer-events: none;
  transition: opacity 0.4s ease;
}

.disclaimer-overlay.show {
  opacity: 1;
  pointer-events: all;
}
    .disclaimer-box {
  background: rgba(255,255,255,0.9);
  backdrop-filter: blur(6px);
  border-radius: 16px;
  padding: 30px;
  max-width: 500px;
  text-align: center;

  box-shadow: 0 10px 40px rgba(0,0,0,0.3);

  /* 👇 animation */
  transform: scale(0.9);
  opacity: 0;
  transition: all 0.4s ease;
}

.disclaimer-overlay.show .disclaimer-box {
  transform: scale(1);
  opacity: 1;
}
.disclaimer-box {
  background: rgba(255,255,255,0.85);
backdrop-filter: blur(6px);
border-radius: 16px;
  color: #000;
  padding: 30px;
  max-width: 500px;
  border-radius: 12px;
  text-align: center;
  box-shadow: 0 10px 30px rgba(0,0,0,0.3);
}

.disclaimer-box h2 {
  margin-bottom: 15px;
}

.disclaimer-box p {
  font-size: 14px;
  margin-bottom: 10px;
}

.disclaimer-box button {
  margin-top: 15px;
  padding: 10px 20px;
  border: none;
  background: #28a745;
  color: white;
  border-radius: 8px;
  cursor: pointer;
  font-size: 16px;
}

.disclaimer-box button:hover {
  background: #218838;
}
    .hidden {
  display: none !important;
    }
    .clickable {
  cursor: pointer;
  transition: 0.3s;
}

.clickable:hover {
  background-color: #f5f5f5;
  transform: scale(1.01);
}

.content {
  margin-top: 15px;
}

.hidden {
  display: none;
}
    #loginPage {
  opacity: 1;
  transition: opacity 0.4s ease;
}

#loginPage.hide {
  opacity: 0;
  pointer-events: none;
}
    .menu-item {
  width: 100%;
  padding: 15px;
  background: #fff;
  border-radius: 10px;
  margin-bottom: 10px;
    }
</style>

</head>

<body>

<header>
  <h1 class="title">Bienvenue</h1>
  <div class="icons">❤️ 🫁</div>
<script src="script.js"></script>
  <p>Bloc opératoire – Accueil des étudiants IADE</p>
</header>

<!-- 🔐 PAGE DE CONNEXION -->
<div id="loginPage" class="login">
  <h2>Accès réservé</h2>
  <input type="password" id="password" placeholder="Mot de passe">
  <button onclick="checkPassword()">Entrer</button>
  <p id="error" style="color:red;"></p>
</div>

<!-- DISCLAIMER -->
<div id="disclaimer" class="disclaimer-overlay">
  <div class="disclaimer-box">
    <h2>⚠️ Avertissement</h2>
    
    <p>
      Ce site est un support pédagogique personnel destiné aux étudiants IADE.
      Il ne remplace en aucun cas les protocoles officiels de notre établissement.
    </p>

    <p>
      Les informations présentées sont générales et doivent être adaptées
      aux pratiques locales et aux recommandations en vigueur.
    </p>

    <p>
      Ce site est non officiel et n’engage pas le CHU de Lille.</p>
      <p>
      En cliquant sur Continuer, vous reconnaissez avoir pris connaissance de cet avertissement.
    </p>

    <button onclick="acceptDisclaimer()">✅ Continuer</button>
  </div>
</div>

<!-- 🔓 CONTENU -->

<div class="bottom-menu">
  <a href="#documents">📑</a>
  <a href="#plan">🗺</a>
  <a href="#visite">🎥</a>
  <a href="#retour">📝</a>
  <a href="pdf/telephones.pdf">☎️</a>
</div>

<div id="content" class="hidden">

<div class="container">

  <div class="card">
    <h2>👋 Message de bienvenue</h2>
    <p>
      Toute l’équipe du bloc opératoire de l’Institut Cœur Poumon est ravie de vous accueillir.  
    </p>
    <p>
      Nous savons que les débuts peuvent être impressionnants — ici, vous êtes là pour apprendre, progresser et poser toutes vos questions...
    </p>
    <p>
      votre bien être, votre épanouissement professionnel et votre autonomisation sont au cœur de notre accompagnement.
    </p>
    <p><strong>👉 Il n’y a pas de "mauvaises questions".</strong></p>
  </div>
  
  <div class="card clickable" onclick="toggleItem(this)">
  <h2>📍 Votre premier jour</h2>

  <div class="content hidden">
    <ul>
      <li><strong>Heure :</strong> 8h</li>
      <li><strong>Lieu :</strong> Salle de réveil du bloc</li>
      <li><strong>Tenue :</strong> Pyjama de bloc, calot, masque, chaussures dédiées</li>
      <li><strong>À prévoir :</strong> Badge, feuilles d'évaluation de stage</li>
      <li>une bannette <strong>"étudiants IADE "</strong> vous permettra de déposer vos fiches d'horaire ainsi que vos rapports de stage</li>
      <li>vous y trouverez une <strong>fiche de suivi</strong> à remplir tout au long du stage</li>
    </ul>
  </div>
</div>
  
<div class="card clickable" onclick="toggleItem(this)">
    <h2>🏥 Vie pratique</h2>
  
  <div class="content hidden">
    <ul>
    <li> à votre disposition</li>
    <h3>👕 Vestiaires</h3>
    <li>👉 Pensez à prévoir un cadenas pour votre casier.</li>
    <li>👉 Merci de ne pas y laisser d’objets de valeur.</li>
    <h3>🧥 Casiers</h3>
    <li>Des casiers sont à votre disposition en SSPI.</li>
     <h3>☕ Salle de pause</h3>
    <li>Une salle de pause est à votre disposition.</li>
    <li>👉 Espace de repos réservé au café.</li>
    <h3>🍽️ restauration</h3>
    <li>La salle à manger est située au sein du bloc.</li>
    <li>le self est situé au niveau-2.</li>  
    <li>le relais H est situé au niveau 0.</li>
    <li>👉 Possibilité de réchauffer vos repas sur place.
    </li>
    </ul>
</div>
</div>

<div class="fiche fiche-plan" id="plan">
  
  <h3>🗺️ Plan du bloc opératoire</h3>
  <p>Consultez le plan pour vous repérer facilement dans le service.</p>

  <a href="pdf/plan2.pdf" target="_blank" class="btn-pdf">
    📄 Télécharger le plan
  </a>
</div>
<div class="card" id="visite">
  <h2>🎥 Visite du service</h2>

  <button id="videoBtn" class="video-btn" onclick="toggleVideo()">
    ▶️ Voir la visite du bloc
  </button>
  <div id="videoContainer" class="video hidden">
  
  <iframe id="videoFrame"
  src="https://www.youtube.com/embed/TON_ID_VIDEO?autoplay=1"
  frameborder="0"
  allow="fullscreen; autoplay"
  allowfullscreen>
</iframe>
  </div>
  
  
  <div class="card clickable" onclick="toggleItem(this)">
    <h2>🏥 Organigramme du service</h2>

      <div class="content hidden">
    <ul>
      <li><strong>bloc opératoire :</strong></li>
      <li>Chirurgie cardiaque: Professeur Vincentelli </li>
      <li>Chirurgie thoracique: Professeur Venissac</li>      
      <li><strong>PTI:</strong></li>
      <LI>Cardiologie: Professeur Lemesle</LI>
      <li><strong>Anesthésie:</strong></li>
      <li>Chef de service:Dr Desbordes</li>
  
    <li> Vous serez encadré(e)s par une équipe d’IADE, de médecins anesthésistes et d’IDE expérimenté(e)s. </li>
    </ul>
  </div>
  </div>

  <div class="card clickable" onclick="toggleItem(this)">
    <h2> ♻️ Référents</h2>
    
    <div class="content hidden">
    <ul>
      <li><strong>cadre sup:</strong> Mme Reumaux Laurence </li>
    <li><strong>IADE Référente de soins:</strong> Mme Hennache Audrey </li>
    <li><strong>Référents IADE :</strong> Tosolini Karen, Carrier Sabah, Lavergne Sebastien, Molinaro Camille</li>
      <li><strong>Référent SSPI:</strong> Bichelberger Eve</li>
      </ul>
  </div>
  </div>
  </div>
  
<div>
<a class="btn" href="pdf/telephones.pdf" target="_blank">
  ☎️ Telephones 
</a>
  </div>
  
    <div class="card" id="documents">
  <h2>📄 Accès rapide aux documents</h2>

  <div class="btn" onclick="toggleChir()">
    
    ✅ présentation des chirurgies
  </div>

  <div id="chirMenu" class="hidden">  
    <a class="btn" href="pdf/COEUR.pdf" target="_blank"> 🫀 À cœur ouvert</a> 
    <a class="btn" href="pdf/CEC.pdf" target="_blank"> 🔧 ⚙️La CEC</a>
    <a class="btn" href="pdf/CARDIOLOGIE1.pdf" target="_blank">❤️ interventionnelle</a> 
    <a class="btn"
href="pdf/VASCULAIRE.pdf" target="_blank">
📕 vasculaire</a>    
    <a class="btn"
href="pdf/POUMON.pdf" target="_blank">
🩻 thoracique</a>
      
  </div>

    <style>
.hidden {
  display: none;
}
</style>

<script>
function toggleChir() {
  var menu = document.getElementById("chirMenu");
  menu.classList.toggle("hidden");
}
</script>
</div>
    
  <div class="btn" onclick="toggleSpecialites()">
  📂 Anesthésie par spécialité
</div>

<div id="specialitesMenu" class="hidden">

  <div class="fiche">
    <a href="pdf/CHIRURGIE_CARDIAQUE.pdf" target="_blank">
      ❤️ Chirurgie cardiaque
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/CHIRURGIE_THORACIQUE.pdf" target="_blank">
      🫁 Chirurgie thoracique
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/CHIRURGIE_VASCULAIRE.pdf" target="_blank">
      🩸 Chirurgie vasculaire
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/TAVI.pdf" target="_blank">
      💉 Cardiologie interventionnelle
    </a>
  </div>

</div>
  
</div>
<script>
function toggleSpecialites() {
  const menu = document.getElementById("specialitesMenu");
  menu.classList.toggle("hidden");
}
</script>
<style>
.fiche-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 15px;
  margin-top: 20px;
}
  
.fiche-container .fiche {
  background: #f5f5f5;
  padding: 15px;
  border-radius: 12px;
  transition: 0.3s;
}

.fiche a {
  text-decoration: none;
  color: #333;
  display: block;
}

.fiche:hover {
  background: #e6f2ff;
  transform: translateY(-2px);
}
  .fiche-plan {
  background: white;
  }
  .btn.urgence {
  background: linear-gradient(135deg, #ff3b3b, #b30000);
  color: white;
  animation: pulseUrgence 1.8s infinite;
  box-shadow: 0 0 0 rgba(255, 0, 0, 0.7);
}

@keyframes pulseUrgence {
  0% {
    transform: scale(1);
    box-shadow: 0 0 0 0 rgba(255, 0, 0, 0.7);
  }
  50% {
    transform: scale(1.05);
    box-shadow: 0 0 15px 5px rgba(255, 0, 0, 0.5);
  }
  100% {
    transform: scale(1);
    box-shadow: 0 0 0 0 rgba(255, 0, 0, 0.7);
  }
}

.btn.urgence:hover {
  background: linear-gradient(135deg, #ff1a1a, #800000);
  transform: scale(1.08);
}
.btn.bilan {
  background: linear-gradient(135deg, #28a745, #1e7e34);
  color: white;
}

.btn.bilan:hover {
  background: linear-gradient(135deg, #34d058, #19692c);
  transform: scale(1.05);
}
</style>

  <div class="btn urgence" onclick="toggleUrgences()">
  🚨 Protocoles d'urgence
</div>

<div id="urgencesMenu" class="hidden">

  <div class="fiche">
    <a href="pdf/hemorragie.pdf" target="_blank">
      🩸 Hémorragie
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/arret.pdf" target="_blank">
      ❤️ Arrêt cardiaque
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/choc_anaphylactique.pdf" target="_blank">
      ⚠️ Choc anaphylactique
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/detresse_respiratoire.pdf" target="_blank">
      🫁 Détresse respiratoire
    </a>
  </div>
  
  <div class="fiche">
    <a 
      href="pdf/hyperthermie_maligne.pdf" target="_blank">
      🌡hyperthermie maligne 
    </a>
  </div>
  
  <script>
function toggleUrgences() {
  const menu = document.getElementById("urgencesMenu");
  menu.classList.toggle("hidden");
}
</script>
</div>
<a class="btn"
  href="pdf/Antibioprophylaxie_ICP.pdf"
  target="_blank">
      💊 Antibioprophylaxie
</a>
<a class="btn bilan" href="docs/bilan_de_demi_stage.pdf" target="_blank">
      📘 bilan de demi-stage
    </a>
  <div class="card">
    <h2>💬 Petit mot pour vous</h2>
    <p>
      Le bloc est un environnement exigeant, mais aussi passionnant.  
      Prenez le temps d’observer, de comprendre… et surtout de vous faire confiance.
    </p>
    <p><strong>On est là pour vous accompagner 🤝</strong></p>
  </div>

<div class="card" id="retour">
  <h2>📝 Retour de stage</h2>

  <p>
    Votre avis est essentiel pour améliorer l’accueil des étudiants.
  </p>

  <a class="btn" href="https://forms.gle/4ATLvfYK83cmkXiN7" target="_blank">
    📝 Donner mon avis
  </a>
</div>
<footer>
  Institut Cœur Poumon – Bloc opératoire
</footer>

<script>
  function checkPassword() {
  const password = document.getElementById("password").value;

  if (password === "iadeicp543") {
    
    const login = document.getElementById("loginPage");
    const disclaimer = document.getElementById("disclaimer");

    // 🔥 fade out login
    login.classList.add("hide");

    // attendre la fin de l'animation
    setTimeout(() => {
      login.classList.add("hidden");

      // 🔥 afficher disclaimer avec animation
      disclaimer.classList.add("show");
    }, 400);

  } else {
    document.getElementById("error").innerText = "Mot de passe incorrect";
  }
  }
window.addEventListener("load", () => {
  setTimeout(() => {
    document.querySelector(".icons").classList.add("show");
  }, 800);
});

function toggleVideo() {
  const video = document.getElementById("videoContainer");
  const iframe = document.getElementById("videoFrame");
  const button = document.getElementById("videoBtn");

  if (video.classList.contains("show")) {
    video.classList.remove("show");
    setTimeout(() => video.classList.add("hidden"), 400);
    button.innerHTML = "▶️ Voir la visite du bloc";
  } else {
    video.classList.remove("hidden");
    setTimeout(() => video.classList.add("show"), 10);
    button.innerHTML = "❌ Fermer la vidéo";

    setTimeout(() => {
      if (iframe.requestFullscreen) {
        iframe.requestFullscreen();
      } else if (iframe.webkitRequestFullscreen) {
        iframe.webkitRequestFullscreen();
      } else if (iframe.msRequestFullscreen) {
        iframe.msRequestFullscreen();
      }
    }, 500);
  }
}
    
function showDisclaimer() {
  document.getElementById("disclaimer").classList.add("show");
}
function acceptDisclaimer() {
  const disclaimer = document.getElementById("disclaimer");
  const content = document.getElementById("content");

  // fade out disclaimer
  disclaimer.classList.remove("show");

  setTimeout(() => {
    content.classList.remove("hidden");
  }, 300);
}
  function acceptDisclaimer() {
  const disclaimer = document.getElementById("disclaimer");
  const content = document.getElementById("content");
disclaimer.classList.remove("show");
  content.classList.remove("hidden");
  }
function toggleItem(element) {
  const content = element.querySelector(".content");
  content.classList.toggle("hidden");
}window.addEventListener("load", () => {
  setTimeout(() => {
    document.querySelector(".icons")?.classList.add("show");
  }, 800);
});
  window.addEventListener("load", () => {
  setTimeout(() => {
    const icons = document.querySelector(".icons");
    if (icons) {
      icons.classList.add("show");
    }
  }, 800);
});
</script>


