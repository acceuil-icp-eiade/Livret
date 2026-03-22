<!DOCTYPE html>
<html lang="fr">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Accueil IADE - ICP</title>

  <style>
    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: 'Segoe UI', Arial, sans-serif;
      background-color: #f4f6f8;
      color: #2c3e50;
    }

    header {
      background: linear-gradient(135deg, #5dade2, #48c9b0);
      color: white;
      padding: 20px;
      text-align: center;
    }

    h1 {
      margin: 0;
      font-size: 22px;
    }

    .login {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 80vh;
      padding: 20px;
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
      cursor: pointer;
    }

    .hidden {
      display: none;
    }

    .nav {
      display: flex;
      overflow-x: auto;
      background: white;
      padding: 10px;
      gap: 10px;
      border-bottom: 1px solid #ddd;
    }

    .nav a {
      flex: 0 0 auto;
      background: #3498db;
      color: white;
      padding: 10px 14px;
      border-radius: 20px;
      text-decoration: none;
      font-size: 14px;
      white-space: nowrap;
    }

    .container {
      padding: 15px;
    }

    .card {
      background: white;
      border-radius: 15px;
      padding: 18px;
      margin-bottom: 15px;
      box-shadow: 0 4px 10px rgba(0,0,0,0.08);
    }

    h2 { color: #3498db; }

    .btn {
      display: block;
      background: #3498db;
      color: white;
      text-decoration: none;
      padding: 14px;
      margin-bottom: 10px;
      border-radius: 12px;
      text-align: center;
      font-weight: bold;
    }

    footer {
      text-align: center;
      font-size: 12px;
      color: #7f8c8d;
      padding: 15px;
    }
  </style>
</head>

<body>

<header>
  <h1>Bienvenue à l’ICP ❤️</h1>
  <p>Accueil des étudiants IADE</p>
</header>

<!-- 🔐 LOGIN -->
<div id="loginPage" class="login">
  <h2>Accès réservé</h2>
  <input type="password" id="password" placeholder="Mot de passe">
  <button onclick="checkPassword()">Entrer</button>
  <p id="error" style="color:red;"></p>
</div>

<!-- CONTENU COMPLET -->
<div id="content" class="hidden">

  <!-- NAV -->
  <div class="nav">
    <a href="#bienvenue">👋 Accueil</a>
    <a href="#jour1">📍 Jour 1</a>
    <a href="#docs">📄 Docs</a>
    <a href="#contacts">📞 Contacts</a>
  </div>

  <div class="container">

    <div class="card" id="bienvenue">
      <h2>👋 Bienvenue</h2>
      <p>
        Toute l’équipe du bloc opératoire de l’ICP est ravie de vous accueillir.  
        Vous êtes ici pour apprendre, progresser et poser toutes vos questions.
      </p>
    </div>

    <div class="card" id="jour1">
      <h2>📍 Premier jour</h2>
      <ul>
        <li>🕢 7h30 – Salle de repos</li>
        <li>👕 Tenue de bloc obligatoire</li>
        <li>🪪 Badge + carnet de stage</li>
      </ul>
    </div>

    <div class="card" id="docs">
      <h2>📄 Accès rapide aux documents</h2>

      <a class="btn" href="docs/protocoles.pdf" target="_blank">📘 Protocoles anesthésie</a>
      <a class="btn" href="docs/checklist.pdf" target="_blank">✅ Check-list sécurité</a>
      <a class="btn" href="docs/urgence.pdf" target="_blank">🚨 Urgences anesthésie</a>

    </div>

    <div class="card" id="contacts">
      <h2>📞 Contacts</h2>
      <p><strong>Cadre :</strong> (à compléter)</p>
      <p><strong>Référent IADE :</strong> (à compléter)</p>
    </div>

    <div class="card">
      <h2>💬 Message</h2>
      <p>
        Le bloc est un environnement exigeant mais formateur.  
        Prenez le temps, observez, et faites-vous confiance 🤝
      </p>
    </div>

  </div>

  <footer>
    Institut Cœur Poumon – Bloc opératoire
  </footer>

</div>

<script>
  function checkPassword() {
    const password = document.getElementById("password").value;

    // 🔑 Mot de passe
    const correctPassword = "iade543";

    if (password === correctPassword) {
      document.getElementById("loginPage").classList.add("hidden");
      document.getElementById("content").classList.remove("hidden");
    } else {
      document.getElementById("error").innerText = "Mot de passe incorrect";
    }
  }
</script>

</body>
</html>
