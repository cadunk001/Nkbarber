# Nkbarber 
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>NK Barbershop - Estilo em Alta</title>
  <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@700&family=Montserrat&display=swap" rel="stylesheet">
  <style>
    body {
      background: #0A0A0A;
      color: #FFFFFF;
      font-family: 'Montserrat', sans-serif;
      margin: 0;
      padding: 0;
      line-height: 1.6;
    }
    .hero {
      padding: 60px 20px;
      text-align: center;
      background: linear-gradient(135deg, #00FFCC, #FF007A);
      border-bottom: 5px solid #FFD700;
      clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
    }
    .hero h1 {
      font-family: 'Orbitron', sans-serif;
      font-size: 4em;
      color: #FFD700;
      text-shadow: 2px 2px 6px #000000, 0 0 10px #FF007A;
      margin: 0;
    }
    .hero p {
      font-size: 1.2em;
      color: #FFFFFF;
      text-shadow: 1px 1px 3px #000000;
    }
    .hero a {
      display: inline-block;
      background: #FF007A;
      color: #FFFFFF;
      padding: 15px 30px;
      border-radius: 10px;
      text-decoration: none;
      margin-top: 20px;
      font-family: 'Orbitron', sans-serif;
      border: 2px solid #FFD700;
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      overflow: hidden;
    }
    .hero a::before {
      content: '';
      position: absolute;
      top: 50%;
      left: 50%;
      width: 0;
      height: 0;
      background: rgba(255, 215, 0, 0.3);
      border-radius: 50%;
      transform: translate(-50%, -50%);
      transition: width 0.6s, height 0.6s;
    }
    .hero a:hover::before {
      width: 200%;
      height: 200%;
    }
    .hero a:hover {
      transform: scale(1.1);
      box-shadow: 0 0 20px #00FFCC;
    }
    .services-section {
      padding: 50px 20px;
      text-align: center;
      background: linear-gradient(45deg, #0A0A0A, #1A1A1A);
    }
    .services-section h2 {
      font-family: 'Orbitron', sans-serif;
      font-size: 2.5em;
      color: #00FFCC;
      text-shadow: 1px 1px 5px #FF007A, 0 0 15px #FFD700;
      margin-bottom: 30px;
      position: relative;
    }
    .services-section h2::after {
      content: '';
      position: absolute;
      bottom: -5px;
      left: 50%;
      transform: translateX(-50%);
      width: 50px;
      height: 3px;
      background: #FFD700;
      border-radius: 2px;
    }
    .services-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 20px;
    }
    .service-card {
      background: linear-gradient(45deg, #1A1A1A, #2A2A2A);
      border-radius: 15px;
      padding: 20px;
      border: 2px solid #FFD700;
      transition: transform 0.3s, box-shadow 0.3s;
      position: relative;
      overflow: hidden;
    }
    .service-card::before {
      content: '';
      position: absolute;
      top: -50%;
      left: -50%;
      width: 200%;
      height: 200%;
      background: radial-gradient(circle, rgba(0, 255, 204, 0.1) 0%, transparent 70%);
      animation: rotate 10s linear infinite;
    }
    @keyframes rotate {
      0% { transform: rotate(0deg); }
      100% { transform: rotate(360deg); }
    }
    .service-card:hover {
      transform: scale(1.05);
      box-shadow: 0 0 25px #00FFCC;
    }
    .service-card h3 {
      font-family: 'Orbitron', sans-serif;
      font-size: 1.8em;
      color: #FF007A;
      margin: 10px 0;
      text-shadow: 1px 1px 4px #FFD700;
    }
    .service-card p {
      font-size: 1em;
      color: #A0A0A0;
    }
    .service-card .price {
      color: #FFD700;
      font-weight: bold;
      font-size: 1.3em;
      text-shadow: 1px 1px 2px #000000;
    }
    .service-card a {
      display: inline-block;
      background: #00FFCC;
      color: #0A0A0A;
      padding: 10px 20px;
      border-radius: 5px;
      text-decoration: none;
      margin-top: 10px;
      font-family: 'Orbitron', sans-serif;
      border: 2px solid #FF007A;
      transition: all 0.3s;
    }
    .service-card a:hover {
      background: #00BFA5;
      transform: translateY(-3px);
      box-shadow: 0 0 10px #FFD700;
    }
    .instagram-button {
      display: inline-block;
      background: #FF007A;
      color: #FFFFFF;
      padding: 15px 30px;
      border-radius: 10px;
      text-decoration: none;
      margin: 20px auto;
      font-family: 'Orbitron', sans-serif;
      border: 2px solid #FFD700;
      transition: transform 0.3s, box-shadow 0.3s;
    }
    .instagram-button:hover {
      transform: scale(1.1);
      box-shadow: 0 0 20px #00FFCC;
    }
  </style>
</head>
<body>
  <section class="hero">
    <h1>NK Barbershop</h1>
    <p>Transforme seu estilo com cortes que arrasam!</p>
    <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20um%20corte">Agendar Agora</a>
  </section>
  <section class="services-section">
    <h2>Serviços</h2>
    <div class="services-grid">
      <div class="service-card">
        <h3>Degradê Navalhado</h3>
        <p class="price">R$ 30,00</p>
        <p>Navalha afiada, estilo que domina.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20um%20Degradê%20Navalhado">Agendar Agora</a>
      </div>
      <div class="service-card">
        <h3>Corte Social</h3>
        <p class="price">R$ 25,00</p>
        <p>Clássico com um toque de atitude.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20um%20Corte%20Social">Agendar Agora</a>
      </div>
      <div class="service-card">
        <h3>Sobrancelha</h3>
        <p class="price">R$ 10,00</p>
        <p>Definição que destaca seu olhar.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20uma%20Sobrancelha">Agendar Agora</a>
      </div>
      <div class="service-card">
        <h3>Pezinho</h3>
        <p class="price">R$ 10,00</p>
        <p>Detalhe que eleva seu corte.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20um%20Pezinho">Agendar Agora</a>
      </div>
      <div class="service-card">
        <h3>Corte Tesoura</h3>
        <p class="price">R$ 35,00</p>
        <p>Técnica refinada, estilo único.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20um%20Corte%20Tesoura">Agendar Agora</a>
      </div>
      <div class="service-card">
        <h3>Limpeza de Pele</h3>
        <p class="price">R$ 25,00</p>
        <p>Rosto limpo, vibe inabalável.</p>
        <a href="https://wa.me/5562993571882?text=Oi,%20quero%20agendar%20uma%20Limpeza%20de%20Pele">Agendar Agora</a>
      </div>
    </div>
    <a href="https://www.instagram.com/nk_.barber?igsh=MXF0MDRzajRqbGY4Nw%3D%3D&utm_source=qr" class="instagram-button">Siga no Instagram</a>
  </section>
</body>
</html>
