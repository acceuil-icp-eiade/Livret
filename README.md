
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

    header {
      background: linear-gradient(135deg, #5dade2, #48c9b0);
      color: white;
      padding: 20px;
      text-align: center;
      border-radius: 10px;
    }

    h1 {
      margin: 0;
      font-size: 22px;
    }

    /* 🔐 LOGIN */
    .login {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 80vh;
    }

    input {
      padding: 12px;
      margin: 10px;
      border-radius: 8px;
      border: 1px solid #ccc;
      width: 220px;
      text-align: center;
    }

    button {
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      background: #3498db;
      color: white;
      font-weight: bold;
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

body {
  padding-bottom: 70px;
}
.fiche:last-child {
  margin-bottom: 25px;
}

</style>

</head>
<div>
<div class="bottom-menu">
  <a href="#documents">📑</a>
  <a href="#pratique">🏥</a>
  <a href="#visite">🎥</a>
  <a href="#retour">📝</a>
  <a href="téléphone">☎️</a>
</div>

<body>

<header>
  <h1>Bienvenue à l’ICP 🫀🫁</h1>
  <p>Bloc opératoire – Accueil des étudiants IADE</p>
</header>

<!-- 🔐 PAGE DE CONNEXION -->
<div id="loginPage" class="login">
  <h2>Accès réservé</h2>
  <input type="password" id="password" placeholder="Mot de passe">
  <button onclick="checkPassword()">Entrer</button>
  <p id="error" style="color:red;"></p>
</div>

<!-- 🔓 CONTENU -->
<div id="content" class="hidden">

<div class="container">

  <div class="card">
    <h2>👋 Message de bienvenue</h2>
    <p>
      Toute l’équipe du bloc opératoire de l’Institut Cœur Poumon est ravie de vous accueillir.  
      Nous savons que les débuts peuvent être impressionnants — ici, vous êtes là pour apprendre, progresser et poser toutes vos questions.
    </p>
    <p><strong>👉 Il n’y a pas de "mauvaises questions".</strong></p>
  </div>

  <div class="card">
    <h2>📍 Votre premier jour</h2>
    <ul>
      <li><strong>Heure :</strong> 8h</li>
      <li><strong>Lieu :</strong> Salle de réveil du bloc</li>
      <li><strong>Tenue :</strong> Pyjama de bloc, calot, masque, chaussures dédiées</li>
      <li><strong>À prévoir :</strong> Badge, feuilles d'évaluation de stage</li>
    </ul>
  </div>

  <div class="card" id="pratique">
  <h2>🏥 Vie pratique</h2>
  <div class="info">
    <h3>👕 Vestiaires</h3>
    <p>Les vestiaires sont situés (à compléter).</p>
    <p>👉 Pensez à prévoir un cadenas pour votre casier.</p>
  </div>
  <div class="info">
    <h3>🧥 Casiers</h3>
    <p>Des casiers sont à votre disposition dans les vestiaires.</p>
    <p>👉 Merci de ne pas laisser d’objets de valeur.</p>
  </div>
  <div class="info">
    <h3>☕ Salle de pause</h3>
    <p>La salle de pause se trouve (à compléter).</p>
    <p>👉 Espace de repos réservé à l’équipe.</p>
  </div>
  <div class="info">
    <h3>🍽️ Salle à manger, restauration</h3>
    <p>La salle à manger est située (à compléter).</p>
    <p>👉 Possibilité de réchauffer vos repas sur place.
    </p>
    
  </div>
  
<div class="card" id="visite">
  <h2>🎥 Visite du service</h2>

  <button id="videoBtn" class="video-btn" onclick="toggleVideo()">
    ▶️ Voir la visite du bloc
  </button>

  <div id="videoContainer" class="video hidden">
    <iframe 
  id="videoFrame"
  src="https://www.youtube.com/embed/TON_ID_VIDEO?autoplay=1"
  frameborder="0"
  allow="fullscreen; autoplay"
  allowfullscreen>
</iframe>
    
  </div>
  
</div>
  <div class="card" id="organisation">
    <h2>🏥 Organisation du service</h2>
    <ul>
      <li>Bloc opératoire</li>
      <li>SSPI</li>
      <li>PTI</li>
    </ul>
    <p>
      Vous serez encadré(e)s par une équipe d’IADE, de médecins anesthésistes et d’IDE expérimentés.
    </p>

<a class="btn" href="docs/telephones.pdf" target="_blank">
  ☎️ Telephones 
</a>
  </div>

  <div class="card" id="documents">
    <h2>📄 Accès rapide aux documents</h2>

    

    <a class="btn" href="docs/chirurgies.pdf" target="_blank">
      ✅ les chirurgies 
    </a>
    
    <h2>Fiches par spécialité</h2>

<div class="fiche-container">

  <div class="fiche">
    <a href="pdf/chirurgie_cardiaque.pdf" target="_blank">
      <strong>Chirurgie cardiaque</strong><br>
      📄 Télécharger la fiche
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/chirurgie_thoracique.pdf" target="_blank">
      <strong>Chirurgie thoracique</strong><br>
      📄 Télécharger la fiche
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/chirurgie_vasculaire.pdf" target="_blank">
      <strong>Chirurgie vasculaire</strong><br>
      📄 Télécharger la fiche
    </a>
  </div>

  <div class="fiche">
    <a href="pdf/cardiologie_interventionnelle.pdf" target="_blank">
      <strong>Cardiologie interventionnelle</strong><br>
      📄 Télécharger la fiche
    </a>
  </div>
  
</div>

<style>
.fiche-container {
  display: grid;
  grid-template-columns: 1fr;
  gap: 15px;
  margin-top: 20px;
}

.fiche {
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
</style>

    <a class="btn" href="docs/urgences.pdf" target="_blank">
      🚨 Urgences anesthésie
    </a>
    
<a class="btn" href="docs/bilan_de_demi_stage.pdf" target="_blank">
      📘 bilan de demi-stage
    </a>
  </div>

  <div class="card">
    <h2>📞 Contacts</h2>
    <p><strong>Cadre :</strong> Mme Hennache Audrey</p>
    <p><strong>Référents IADE :</strong> Tosolini Karen, Carrier Sabah, Lavergne Sebastien, Molinaro Camille</p>
  </div>

  <div class="card">
    <h2>💬 Petit mot pour vous</h2>
    <p>
      Le bloc est un environnement exigeant, mais aussi passionnant.  
      Prenez le temps d’observer, de comprendre… et surtout de vous faire confiance.
    </p>
    <p><strong>On est là pour vous accompagner 🤝</strong></p>
  </div>

</div>

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

  // 🔑 CHANGE TON MOT DE PASSE ICI
  const correctPassword = "iadeicp543";

  if (password === correctPassword) {
    document.getElementById("loginPage").classList.add("hidden");
    document.getElementById("content").classList.remove("hidden");
  } else {
    document.getElementById("error").innerText = "Mot de passe incorrect";
  }
}
</script>

  <script>
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
</script>

