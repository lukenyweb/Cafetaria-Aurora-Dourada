<html lang="pt">        
<head>        
<meta charset="UTF-8">        
<meta name="viewport" content="width=device-width, initial-scale=1.0">        
<title>Cafetaria Aurora Dourada</title>        
        
<style>        
*{        
margin:0;        
padding:0;        
box-sizing:border-box;        
scroll-behavior:smooth;        
font-family:Arial, sans-serif;        
}        
        
body{        
background:#111;        
color:#fff;        
}        
        
nav{        
position:fixed;        
width:100%;        
background:#000;        
padding:15px;        
text-align:center;        
z-index:1000;        
}        
        
nav a{        
color:gold;        
margin:0 15px;        
text-decoration:none;        
font-weight:bold;        
transition:0.3s;        
}        
        
nav a:hover{        
color:white;        
}        
        
section{        
padding:100px 20px;        
min-height:100vh;        
display:flex;        
flex-direction:column;        
justify-content:center;        
align-items:center;        
text-align:center;        
background-size:cover;      
background-position:center;      
background-repeat:no-repeat;      
position:relative;      
}        
      
section::before{      
content:"";      
position:absolute;      
top:0;      
left:0;      
width:100%;      
height:100%;      
background:rgba(0,0,0,0.75);      
z-index:0;      
}      
      
section > *{      
position:relative;      
z-index:1;      
}      
      
#home{        
background:url('https://images.unsplash.com/photo-1509042239860-f550ce710b93') no-repeat center/cover;        
}        
      
#menu{      
background-image:url('https://images.unsplash.com/photo-1504674900247-0877df9cc836');      
}      
      
#sobre{      
background-image:url('https://images.unsplash.com/photo-1554118811-1e0d58224f24');      
}      
      
#galeria{      
background-image:url('https://images.unsplash.com/photo-1498804103079-a6351b050096');      
}      
      
#contacto{      
background-image:url('https://images.unsplash.com/photo-1521017432531-fbd92d768814');      
}      
      
.overlay{        
background:rgba(0,0,0,0.7);        
padding:40px;        
border-radius:20px;        
}        
        
h1{        
font-size:50px;        
margin-bottom:20px;        
color:gold;        
}        
        
h2{        
margin-bottom:20px;        
color:gold;        
}        
        
p{        
max-width:600px;        
margin-bottom:20px;        
}        
        
button{        
padding:15px 30px;        
background:gold;        
border:none;        
border-radius:10px;        
cursor:pointer;        
font-weight:bold;        
transition:0.3s;        
}        
        
button:hover{        
transform:scale(1.1);        
box-shadow:0 0 20px gold;        
}        
        
.cards{        
display:flex;        
flex-wrap:wrap;        
gap:20px;        
justify-content:center;        
}        
        
.card{        
background:#222;        
padding:20px;        
border-radius:15px;        
width:250px;        
transition:0.3s;        
}        
        
.card:hover{        
transform:translateY(-10px);        
}        
        
.gallery{        
display:flex;        
flex-wrap:wrap;        
gap:15px;        
justify-content:center;        
}        
        
.gallery img{        
width:250px;        
border-radius:15px;        
transition:0.3s;        
}        
        
.gallery img:hover{        
transform:scale(1.1);        
}        
        
video{        
width:80%;        
max-width:600px;        
border-radius:20px;        
margin-top:20px;        
}        
        
iframe{        
margin-top:20px;        
border-radius:20px;        
}        
        
footer{        
background:#000;        
padding:20px;        
text-align:center;        
}        
</style>        
</head>        
        
<body>        
        
<nav>        
<a href="#home">•Início</a>        
<a href="#menu">•Especialidades</a>        
<a href="#sobre">•Nossa História</a>        
<a href="#galeria">•Ambiente</a>        
<a href="#contacto">•Reservas</a>        
</nav>        
        
<section id="home">        
<div class="overlay">        
<h1>Cafetaria Aurora Dourada</h1>        
<p>Onde cada chávena conta uma história de sabor, elegância e paixão.</p>        
<button onclick="window.location.href='#menu'">Descobrir Sabores</button>        
</div>        
</section>        
        
<section id="menu">        
<h2>Especialidades da Casa</h2>        
<div class="cards">        
<div class="card">        
<h3>☕ Café expresso Premium</h3>        
<p>Intenso, aromático e preparado na perfeição – 1,20€</p>        
</div>        
<div class="card">        
<h3>🥐Croissant Artesanal</h3>        
<p>Massa leve e dourada, feita diariamente – 1,50€</p>        
</div>        
<div class="card">        
<h3>🍰Tentação de Chocolate</h3>        
<p>Uma explosão de sabor irresistível – 2,50€</p>        
</div>        
</div>        
</section>        
        
<section id="sobre">        
<h2>A Nossa História</h2>        
<p>A Cafetaria Aurora Dourada nasceu com o propósito de oferecer mais do que café – criamos momentos especiais num ambiente sofisticado, acolhedor e memorável.</p>        
        
<h3>Conheça o nosso ambiente:</h3>        
      
<iframe       
  width="100%"       
  height="400"       
  style="border-radius:20px; margin:20px 0;"      
  src="https://drive.google.com/file/d/1Coj6siZIXpQFR1hCl7_VKBNGv1WOMcgz/preview"      
  allow="autoplay">      
</iframe>      
      
<iframe       
  width="100%"       
  height="400"       
  style="border-radius:20px; margin:20px 0; border:none;"      
  src="https://drive.google.com/file/d/1e-kgphHyUKMtBHKCgI0CJll3sFuenmCu/preview"      
  allow="autoplay">      
</iframe>      
      
</section>        
        
<section id="galeria">        
<h2>Momentos & Ambiente</h2>        
<div class="gallery">        
<img src="https://images.unsplash.com/photo-1495474472287-4d71bcdd2085">        
<img src="https://images.unsplash.com/photo-1504754524776-8f4f37790ca0">        
<img src="https://images.unsplash.com/photo-1461023058943-07fcbe16d735">        
</div>        
</section>        
        
<section id="contacto">        
<h2>Reservas & Contactos</h2>        
<p>Visite-nos em Lisboa e viva uma experiência única de sabor e requinte.</p>        
        
<a href="https://wa.me/244XXXXXXXXX?text=Olá!%20Gostaria%20de%20fazer%20uma%20reserva%20na%20Cafetaria%20Aurora%20Dourada." target="_blank">        
<button>Reservar via WhatsApp</button>        
</a>        
        
<iframe         
src="https://www.google.com/maps/embed?pb=!1m18..."        
width="300" height="200" style="border:0;" allowfullscreen="">        
</iframe>        
        
</section>        
        
<footer>        
<p>© 2026 Cafetaria Aurora Dourada – Elegância em cada detalhe</p>        
</footer>        
        
</body>        
</html>
