# page-netlify<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Paiva Solutions</title>

  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;500;700&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      font-family: 'Inter', sans-serif;
      background: #0b0f19;
      color: #fff;
    }

    nav {
      position: fixed;
      width: 100%;
      background: #111827;
      padding: 15px;
      text-align: center;
      font-weight: bold;
      z-index: 1000;
    }

    .hero {
      padding: 120px 20px;
      text-align: center;
    }

    .hero h1 {
      font-size: 48px;
    }

    .hero p {
      color: #9ca3af;
      margin: 20px 0;
    }

    .btn {
      background: #3b82f6;
      border: none;
      padding: 15px 30px;
      border-radius: 10px;
      cursor: pointer;
      color: white;
      font-size: 16px;
    }

    .services {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      padding: 60px 20px;
    }

    .service {
      background: #1f2937;
      padding: 25px;
      border-radius: 15px;
      width: 280px;
      text-align: center;
    }

    .testimonials {
      padding: 60px 20px;
      background: #020617;
      text-align: center;
    }

    .testimonial {
      margin: 20px auto;
      max-width: 500px;
      font-style: italic;
      color: #cbd5f5;
    }

    .form {
      padding: 60px 20px;
      text-align: center;
    }

    input {
      display: block;
      width: 300px;
      margin: 10px auto;
      padding: 12px;
      border-radius: 8px;
      border: none;
    }

    footer {
      text-align: center;
      padding: 20px;
      color: #6b7280;
    }
  </style>
</head>

<body>

<nav>🚀 Paiva Solutions</nav>

<section class="hero">
  <h1>Soluções inteligentes em tecnologia</h1>
  <p>Automatize, escale e cresça com sistemas modernos</p>
  <button class="btn" onclick="scrollForm()">Começar agora</button>
</section>

<section class="services">
  <div class="service">
    <h3>💻 Desenvolvimento</h3>
    <p>Sistemas web modernos e escaláveis</p>
  </div>

  <div class="service">
    <h3>☁️ Cloud AWS</h3>
    <p>Infraestrutura segura e performática</p>
  </div>

  <div class="service">
    <h3>📊 Automação</h3>
    <p>Processos inteligentes e eficientes</p>
  </div>
</section>

<section class="testimonials">
  <h2>O que dizem nossos clientes</h2>

  <div class="testimonial">
    "Aumentamos nossa produtividade em 300%!"
  </div>

  <div class="testimonial">
    "Equipe extremamente profissional!"
  </div>
</section>

<section class="form" id="form">
  <h2>Fale com a gente</h2>

  <form onsubmit="sendLead(event)">
    <input type="text" placeholder="Nome" required>
    <input type="email" placeholder="Email" required>
    <button class="btn">Enviar</button>
  </form>
</section>

<footer>
  © 2026 Paiva Solutions
</footer>

<script>
  function scrollForm() {
    document.getElementById("form").scrollIntoView({ behavior: "smooth" });
  }

  function sendLead(e) {
    e.preventDefault();
    alert("Lead enviado 🚀");
  }
</script>

</body>
</html>
