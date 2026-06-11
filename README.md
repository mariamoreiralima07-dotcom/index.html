<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Agrinho 2026 - Maria Vitória 1ºA</title>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
<style>
/* RESET E BASE */
*{
margin:0;
padding:0;
box-sizing:border-box;
font-family:'Roboto',sans-serif;
scroll-behavior:smooth;
}

:root{
--verde:#2e7d32;
--verde-claro:#4caf50;
--verde-escuro:#1b5e20;
--marrom:#6d4c41;
--bege:#f5f0e6;
--branco:#ffffff;
--preto:#000000;
}

body{
background:var(--bege);
color:#333;
line-height:1.6;
}

/* CABEÇALHO */
header{
background:var(--verde);
color:white;
padding:15px 10%;
position:sticky;
top:0;
z-index:1000;
display:flex;
justify-content:space-between;
align-items:center;
}

header h1{
font-size:1.4rem;
font-weight:700;
}

header span{
font-size:1rem;
font-weight:400;
}

/* HERO */
.hero{
height:80vh;
background:
linear-gradient(rgba(0,0,0,.4), rgba(0,0,0,.5)),
url('https://images.unsplash.com/photo-1504933357569-85958b3c8fa1?auto=format&fit=crop&w=1920&q=80');
background-size:cover;
background-position:center;
display:flex;
flex-direction:column;
align-items:center;
justify-content:center;
color:white;
text-align:center;
padding:20px;
}

.hero h2{
font-size:3rem;
margin-bottom:15px;
text-shadow:2px 2px 10px black;
}

.hero p{
font-size:1.3rem;
margin-bottom:25px;
text-shadow:1px 1px 8px black;
}

.btn{
padding:15px 30px;
background:var(--verde-claro);
color:white;
text-decoration:none;
border-radius:40px;
font-weight:600;
transition:.4s;
}

.btn:hover{
transform:scale(1.05);
background:var(--verde-escuro);
}

/* SEÇÕES */
section{
padding:70px 10%;
}

.titulo{
text-align:center;
font-size:2.5rem;
margin-bottom:20px;
color:var(--verde-escuro);
}

.subtitulo{
text-align:center;
max-width:900px;
margin:auto;
margin-bottom:50px;
line-height:1.8;
color:#222;
}

/* GALERIA */
.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(280px,1fr));
gap:20px;
}

.gallery img{
width:100%;
border-radius:15px;
box-shadow:0 8px 20px rgba(0,0,0,.2);
transition:.4s;
}

.gallery img:hover{
transform:scale(1.05);
cursor:pointer;
}

/* EMOJIS */
.emojis{
display:flex;
justify-content:center;
gap:15px;
margin-top:20px;
flex-wrap:wrap;
}

.emoji-btn{
font-size:2rem;
cursor:pointer;
padding:10px 15px;
border-radius:10px;
transition:.3s;
border:2px solid transparent;
}

.emoji-btn:hover{
transform:scale(1.2);
border-color:var(--verde-escuro);
}

/* CONTADOR */
.counter{
text-align:center;
margin-top:10px;
font-weight:600;
font-size:1.2rem;
color:var(--marrom);
}

/* CTA */
.cta{
background:linear-gradient(rgba(0,0,0,.5), rgba(0,0,0,.5)), url('https://images.unsplash.com/photo-1473187983305-f615310e7daa?auto=format&fit=crop&w=1920&q=80');
background-size:cover;
background-position:center;
color:white;
text-align:center;
padding:80px 20px;
border-radius:15px;
}

.cta h2{
font-size:2.8rem;
margin-bottom:15px;
}

.cta p{
font-size:1.2rem;
margin-bottom:25px;
}

/* RODAPÉ */
footer{
background:var(--marrom);
color:white;
padding:40px 10%;
text-align:center;
}

/* ACESSIBILIDADE - CONTRASTE E FONTES GRANDES */
body, h1, h2, h3, p, .btn{
font-size:larger;
line-height:1.8;
}

/* RESPONSIVO */
@media(max-width:768px){
.hero h2{
font-size:2rem;
}
.hero p{
font-size:1rem;
}
}
</style>
</head>
<body>

<header>
<h1>Maria Vitória - 1ºA</h1>
<span>Colégio Leonardo Francisco Nogueira - Pinhalão/PR</span>
</header>

<section class="hero">
<h2>Conexão Agro Sustentável</h2>
<p>Agro Forte • Agro de Alta Performance • Tecnologia Verde</p>
<a href="#galeria" class="btn">Explorar Galeria</a>
</section>

<section id="galeria" class="reveal">
<h2 class="titulo">Fazenda Orgânica</h2>
<p class="subtitulo">Imagens de produção sustentável e conexão com a natureza.</p>

<div class="gallery">
<img src="https://images.unsplash.com/photo-1504208434309-cb69f4fe52b0?auto=format&fit=crop&w=800&q=80" alt="Plantação orgânica">
<img src="https://images.unsplash.com/photo-1581091215366-0d32a8e4f59c?auto=format&fit=crop&w=800&q=80" alt="Horta orgânica">
<img src="https://images.unsplash.com/photo-1592928300135-02e89ed1b7a2?auto=format&fit=crop&w=800&q=80" alt="Frutas e vegetais orgânicos">
<img src="https://images.unsplash.com/photo-1572415970500-fb5c6d056b95?auto=format&fit=crop&w=800&q=80" alt="Colheita sustentável">
</div>

<div class="emojis">
<button class="emoji-btn" data-emoji="👍">👍</button>
<button class="emoji-btn" data-emoji="❤️">❤️</button>
<button class="emoji-btn" data-emoji="🌱">🌱</button>
<button class="emoji-btn" data-emoji="👏">👏</button>
</div>
<div class="counter" id="counter">Curtidas: 0</div>
</section>

<section class="cta reveal">
<h2>Democratizando o Acesso à Tecnologia</h2>
<p>Nosso site conecta estudantes ao futuro do agronegócio mostrando como inovação e sustentabilidade caminham juntas.</p>
<a href="#galeria" class="btn">Interaja Agora</a>
</section>

<footer>
<p>Agrinho 2026 • Maria Vitória - 1ºA • Colégio Leonardo Francisco Nogueira - Pinhalão/PR</p>
</footer>

<script>
// ANIMAÇÃO AO ROLAR
const reveals = document.querySelectorAll('.reveal');
window.addEventListener('scroll', () => {
  reveals.forEach(el => {
    const top = el.getBoundingClientRect().top;
    if(top < window.innerHeight - 100){
      el.classList.add('active');
    }
  });
});

// EMOJIS INTERATIVOS
let totalCurtidas = 0;
const counter = document.getElementById('counter');
document.querySelectorAll('.emoji-btn').forEach(btn => {
  btn.addEventListener('click', () => {
    totalCurtidas++;
    counter.textContent = `Curtidas: ${totalCurtidas}`;
    btn.style.transform='scale(1.2)';
    setTimeout(()=>{btn.style.transform='';},150);
  });
});
</script>

</body>
</html>
