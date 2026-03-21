<<!DOCTYPE html>
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
      width: 200px;
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
  </style>
</head>

<body>

<header>
  <h1>Bienvenue à l’ICP ❤️</h1>
  <p>Accueil des étudiants IADE</p>
</header>

<!-- 🔐 ÉCRAN DE CONNEXION -->
<div id="loginPage" class="login">
  <h2>Accès réservé</h2>
  <input type="password" id="password" placeholder="Mot de passe">
  <button onclick="checkPassword()">Entrer</button>
  <p id="error" style="color:red;"></p>
</div>

<!-- CONTENU -->
<div id="content" class="hidden">

  <div class="container">

    <div class="card">
      <h2>👋 Bienvenue</h2>
      <p>
        Toute l’équipe est ravie de vous accueillir au bloc opératoire de l’ICP.
      </p>
    </div>

    <div class="card">
      <h2>📄 Documents</h2>
      <ul>
        <li><a href="docs/protocoles.pdf" target="_blank">Protocoles</a></li>
        <li><a href="docs/checklist.pdf" target="_blank">Check-list</a></li>
        <li><a href="docs/urgence.pdf" target="_blank">Urgences</a></li>
      </ul>
    </div>

  </div>

</div>

<script>
  function checkPassword() {
    const password = document.getElementById("password").value;
    
    // 🔑 MOT DE PASSE À MODIFIER ICI
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