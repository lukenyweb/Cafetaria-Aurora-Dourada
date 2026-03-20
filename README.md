<html lang="pt">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Cafetaria Aurora Dourada</title>
<link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:ital,wght@0,300;0,400;0,600;1,300;1,400&family=Bebas+Neue&family=DM+Sans:wght@300;400;500&display=swap" rel="stylesheet">
<style>
:root {
  --gold: #C9A84C;
  --gold-light: #F0D080;
  --gold-dim: #6b5720;
  --black: #050403;
}

* { margin:0; padding:0; box-sizing:border-box; }

body {
  font-family: 'DM Sans', sans-serif;
  color: #fff;
  background: var(--black);
  overflow-x: hidden;
}

h1 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(32px, 8vw, 72px);
  font-weight: 300;
  color: var(--gold-light);
  line-height: 1.1;
  margin-bottom: 16px;
  text-shadow: 0 2px 24px rgba(0,0,0,0.8);
}
h2 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(26px, 6vw, 54px);
  font-weight: 300;
  color: var(--gold-light);
  line-height: 1.15;
  margin-bottom: 14px;
}
p {
  font-size: clamp(13px, 3vw, 16px);
  color: rgba(255,255,255,0.7);
  line-height: 1.8;
  margin: 12px 0;
  font-weight: 300;
}

.label {
  font-size: 10px;
  letter-spacing: 5px;
  text-transform: uppercase;
  color: var(--gold);
  margin-bottom: 12px;
  display: block;
}

button {
  padding: 13px 36px;
  font-family: 'DM Sans', sans-serif;
  font-size: 11px;
  font-weight: 500;
  letter-spacing: 2.5px;
  text-transform: uppercase;
  background: var(--gold);
  color: #000;
  border: none;
  cursor: pointer;
  margin: 8px;
  transition: all 0.3s;
  clip-path: polygon(8px 0%, 100% 0%, calc(100% - 8px) 100%, 0% 100%);
}
button:hover {
  background: var(--gold-light);
  transform: translateY(-2px);
  box-shadow: 0 12px 32px rgba(201,168,76,0.3);
}
button.btn-outline {
  background: transparent;
  color: var(--gold);
  border: 1px solid var(--gold-dim);
}
button.btn-outline:hover {
  background: rgba(201,168,76,0.08);
  border-color: var(--gold);
}

.page {
  width: 100%;
  min-height: 100vh;
  display: none;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-size: cover;
  background-position: center;
  animation: fadeIn 0.8s ease;
  padding: 20px;
  position: relative;
}
.page::before {
  content: '';
  position: absolute; inset: 0;
  background: rgba(5,4,3,0.78);
}
.active { display: flex; }

.overlay {
  background: rgba(0,0,0,0.55);
  border: 1px solid rgba(201,168,76,0.15);
  padding: clamp(28px, 6vw, 60px);
  width: 100%;
  max-width: 780px;
  position: relative;
  z-index: 1;
}
.overlay::before {
  content: '';
  position: absolute;
  top: 0; left: 0; right: 0;
  height: 2px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
}

.gold-line {
  width: 48px; height: 1px;
  background: linear-gradient(90deg, transparent, var(--gold), transparent);
  margin: 18px auto;
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(12px); }
  to   { opacity: 1; transform: translateY(0); }
}

.btn-group {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 4px;
  margin-top: 20px;
}

.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
  justify-content: center;
  margin: 20px 0;
}
.card {
  background: rgba(201,168,76,0.06);
  border: 1px solid rgba(201,168,76,0.2);
  padding: 20px 24px;
  width: clamp(200px, 80vw, 220px);
  text-align: left;
  transition: all 0.3s;
}
.card:hover {
  border-color: rgba(201,168,76,0.5);
  background: rgba(201,168,76,0.1);
  transform: translateY(-4px);
}
.card h3 {
  font-family: 'Cormorant Garamond', serif;
  font-size: clamp(15px, 3.5vw, 19px);
  color: var(--gold);
  font-weight: 400;
  margin-bottom: 6px;
}
.card p {
  font-size: clamp(12px, 2.8vw, 13px);
  margin: 0;
  color: rgba(255,255,255,0.55);
}
.card .preco {
  margin-top: 10px;
  font-family: 'Cormorant Garamond', serif;
  font-size: 20px;
  color: var(--gold-light);
}

.gallery {
  display: flex;
  flex-wrap: wrap;
  gap: 12px;
  justify-content: center;
  margin: 20px 0;
}
.gallery img {
  width: clamp(140px, 28vw, 200px);
  aspect-ratio: 1;
  object-fit: cover;
  border: 1px solid rgba(201,168,76,0.2);
  transition: all 0.3s;
  filter: brightness(0.85) saturate(0.7);
}
.gallery img:hover {
  transform: scale(1.04);
  border-color: var(--gold);
  filter: brightness(1) saturate(1);
}

.video-wrap {
  width: 100%;
  margin: 16px 0;
  overflow: hidden;
  border: 1px solid rgba(201,168,76,0.15);
}
.video-wrap iframe {
  width: 100%;
  height: clamp(200px, 50vw, 400px);
  display: block;
  border: none;
}
</style>
</head>
<body>

<!-- PÁGINA 1 — ENTRADA -->
<div id="p1" class="page active" style="background-image:url('https://images.unsplash.com/photo-1509042239860-f550ce710b93?auto=format&fit=crop&w=1200&q=80');">
  <div class="overlay">
    <span class="label">°•°.Cafetaria de Luxo · Portugal</span>
    <h1>☕ Cafetaria Aurora Dourada ✨</h1>
    <div class="gold-line"></div>
    <p>Onde cada chávena conta uma história de sabor, elegância e paixão.<br>Sofisticação · Aconchego · Momentos únicos.</p>
    <div class="btn-group">
      <button onclick="goTo('p2')">Entrar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 2 — ESPECIALIDADES -->
<div id="p2" class="page" style="background-image:url('https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=1200&q=80');">
  <div class="overlay">
    <span class="label">Especialidades da Casa</span>
    <h2>🥐 O Nosso Menu</h2>
    <div class="gold-line"></div>
    <div class="cards">
      <div class="card">
        <h3>☕ Café Expresso Premium</h3>
        <p>Intenso, aromático e preparado na perfeição.</p>
        <div class="preco">1,20€</div>
      </div>
      <div class="card">
        <h3>🥐 Croissant Artesanal</h3>
        <p>Massa leve e dourada, feita diariamente.</p>
        <div class="preco">1,50€</div>
      </div>
      <div class="card">
        <h3>🍰 Tentação de Chocolate</h3>
        <p>Uma explosão de sabor irresistível.</p>
        <div class="preco">2,50€</div>
      </div>
    </div>
    <div class="btn-group">
      <button onclick="goTo('p3')">Nossa História</button>
      <button class="btn-outline" onclick="goTo('p1')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 3 — NOSSA HISTÓRIA + VÍDEOS -->
<div id="p3" class="page" style="background-image:url('https://images.unsplash.com/photo-1554118811-1e0d58224f24?auto=format&fit=crop&w=1200&q=80');">
  <div class="overlay">
    <span class="label">A Nossa História</span>
    <h2>✨ Aurora Dourada</h2>
    <div class="gold-line"></div>
    <p>A Cafetaria Aurora Dourada nasceu com o propósito de oferecer mais do que café — criamos momentos especiais num ambiente sofisticado, acolhedor e memorável.</p>
    <p style="color:var(--gold); font-size:12px; letter-spacing:2px; text-transform:uppercase; margin-top:16px;">Conheça o nosso ambiente</p>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1Coj6siZIXpQFR1hCl7_VKBNGv1WOMcgz/preview" allow="autoplay"></iframe>
    </div>
    <div class="video-wrap">
      <iframe src="https://drive.google.com/file/d/1e-kgphHyUKMtBHKCgI0CJll3sFuenmCu/preview" allow="autoplay"></iframe>
    </div>
    <div class="btn-group">
      <button onclick="goTo('p4')">Ambiente</button>
      <button class="btn-outline" onclick="goTo('p2')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 4 — GALERIA -->
<div id="p4" class="page" style="background-image:url('https://images.unsplash.com/photo-1498804103079-a6351b050096?auto=format&fit=crop&w=1200&q=80');">
  <div class="overlay">
    <span class="label">Momentos & Ambiente</span>
    <h2>📸 Galeria</h2>
    <div class="gold-line"></div>
    <div class="gallery">
      <img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085?auto=format&fit=crop&w=400&q=80" alt="Café">
      <img src="https://images.unsplash.com/photo-1504754524776-8f4f37790ca0?auto=format&fit=crop&w=400&q=80" alt="Comida">
      <img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735?auto=format&fit=crop&w=400&q=80" alt="Ambiente">
    </div>
    <div class="btn-group">
      <button onclick="goTo('p5')">Reservas</button>
      <button class="btn-outline" onclick="goTo('p3')">Voltar</button>
    </div>
  </div>
</div>

<!-- PÁGINA 5 — RESERVAS -->
<div id="p5" class="page" style="background-image:url('https://images.unsplash.com/photo-1521017432531-fbd92d768814?auto=format&fit=crop&w=1200&q=80');">
  <div class="overlay">
    <span class="label">Reservas & Contactos</span>
    <h2>📲 Reservar Mesa</h2>
    <div class="gold-line"></div>
    <p>Visite-nos e viva uma experiência única de sabor e requinte.<br>Resposta rápida e atendimento personalizado.</p>
    <div class="btn-group">
      <a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Gostaria%20de%20fazer%20uma%20reserva%20na%20Cafetaria%20Aurora%20Dourada." target="_blank">
        <button>Reservar via WhatsApp</button>
      </a>
      <button class="btn-outline" onclick="goTo('p4')">Voltar</button>
    </div>
  </div>
</div>

<script>
function goTo(page) {
  document.querySelector('.active').classList.remove('active');
  document.getElementById(page).classList.add('active');
  window.scrollTo(0,0);
}
</script>
</body>
</html>
