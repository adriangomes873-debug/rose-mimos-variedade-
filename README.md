<!DOCTYPE html>
<html lang="pt-BR">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0, user-scalable=no">
<title>Rose Mimo - Beleza, Mimos e Variedades</title>
<link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
<style>
*{margin:0;padding:0;box-sizing:border-box;font-family:'Poppins',sans-serif}
html,body{width:100%;overflow-x:hidden}body{background:#fff8fb;color:#333}
header{width:100%;background:linear-gradient(135deg,#c2185b,#ff4fa3);color:#fff;padding:22px 15px;text-align:center}
header h1{font-size:25px;line-height:1.2}header p{font-size:12px;line-height:1.5;margin-top:7px}
.container{width:100%;max-width:1100px;margin:0 auto;padding:12px}
h2{color:#c2185b;margin:20px 0 10px;border-left:5px solid #ff4fa3;padding-left:9px;font-size:19px;line-height:1.3}
.products{display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:10px;width:100%}
.card{min-width:0;background:#fff;border-radius:15px;padding:8px;box-shadow:0 3px 12px rgba(0,0,0,.07);text-align:center;display:flex;flex-direction:column;overflow:hidden}
.card .img{width:100%;height:125px;background:#fff;border-radius:10px;overflow:hidden;display:flex;align-items:center;justify-content:center}
.card .img img{width:100%;height:100%;object-fit:contain;display:block}
.card h3{font-size:11.5px;margin:7px 0 2px;font-weight:700;line-height:14px;min-height:28px}
.desc{font-size:9.5px;color:#777;line-height:12px;min-height:24px;max-height:24px;overflow:hidden}
.price{color:#f23896;font-weight:800;font-size:16px;margin:7px 0}.btn{background:#ff4fa3;color:#fff;border:none;padding:9px 5px;border-radius:20px;width:100%;cursor:pointer;font-weight:700;font-size:11px;margin-top:auto}
#cartIcon{position:fixed;bottom:15px;right:12px;background:#c2185b;color:#fff;padding:12px 17px;border-radius:30px;cursor:pointer;font-weight:700;font-size:12px;z-index:100;box-shadow:0 5px 20px rgba(0,0,0,.25)}
#cart{position:fixed;bottom:72px;right:10px;left:10px;background:#fff;border-radius:18px;box-shadow:0 8px 30px rgba(0,0,0,.25);padding:15px;max-height:65vh;overflow:auto;display:none;z-index:101}
.cart-item{display:flex;justify-content:space-between;gap:10px;font-size:11px;padding:6px 0;border-bottom:1px dashed #ffd0e2}
#cartTotal{font-weight:800;color:#ff4fa3;text-align:right;margin-top:8px;font-size:15px}
#btnFinalizar{background:#25D366;color:#fff;padding:12px;width:100%;border:none;border-radius:25px;margin-top:10px;font-weight:800;cursor:pointer}
footer{background:#222;color:#ddd;text-align:center;padding:20px 12px;margin-top:25px;font-size:11px;line-height:1.7}
@media (max-width:360px){.container{padding:9px}.products{gap:8px}.card .img{height:112px}.card h3{font-size:10.5px}.desc{font-size:9px}.price{font-size:15px}.btn{font-size:10px}}
@media (min-width:600px){.products{grid-template-columns:repeat(3,minmax(0,1fr))}.card .img{height:170px}}
@media (min-width:900px){.products{grid-template-columns:repeat(4,minmax(0,1fr))}.card .img{height:180px}}
</style>
</head>
<body>
<header><h1>👑 ROSE MIMO 🌹</h1><p>Beleza, Mimos e Variedades</p><p>WhatsApp: (85) 98700-5202 | @mimosdarosevariedades</p></header>
<main class="container">
<h2>💄 Maquiagem</h2><div class="products">
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380427349/Blush-duo.jpg" alt="Blush Compacto Duo Ruby Rose"></div><h3>Blush Compacto Duo Ruby Rose</h3><div class="desc">Alta pigmentação, 2 cores lindas</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Blush Duo',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380377046/Blush%20compactado.jpg" alt="Blush Compacto Playback"></div><h3>Blush Compacto Playback</h3><div class="desc">Cor intensa que dura o dia todo</div><div class="price">R$ 14,00</div><button class="btn" onclick="add('Blush Playback',14)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380515615/candylip.jpg" alt="Candy Lip Oil PhalleBeauty"></div><h3>Candy Lip Oil PhalleBeauty</h3><div class="desc">Brilho + hidratação, boca macia</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Candy Lip Oil',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380711997/Lip%20fruit.jpg" alt="Lip Gloss Lip Fruit Melancia"></div><h3>Lip Gloss Lip Fruit Melancia</h3><div class="desc">JummyJu 15g com chaveirinho</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Lip Gloss Fruit',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380737219/delineador.jpg" alt="Delineador Ultra Black Vivai"></div><h3>Delineador Ultra Black Vivai</h3><div class="desc">Preto intenso, não borra</div><div class="price">R$ 12,00</div><button class="btn" onclick="add('Delineador',12)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380853563/Lapis-pink21.jpg" alt="Lápis Olho e Lábio Pink21"></div><h3>Lápis Olho e Lábio Pink21</h3><div class="desc">2 em 1, macio e pigmentado</div><div class="price">R$ 5,00</div><button class="btn" onclick="add('Lápis Pink21',5)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380873943/P%C3%83%C2%B3%20compacto.jpg" alt="Pó Compacto Popstar"></div><h3>Pó Compacto Popstar</h3><div class="desc">Fancy Face - pele sequinha</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Pó Compacto',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380888554/P%C3%83%C2%B3%20de%20banana.jpg" alt="Pó de Banana Swiss Beauty"></div><h3>Pó de Banana Swiss Beauty</h3><div class="desc">Sela a make, não estoura no flash</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Pó de Banana',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380724811/esponja.jpg" alt="Esponja Chanfrada"></div><h3>Esponja Chanfrada</h3><div class="desc">Kit 3 cores, acabamento profissional</div><div class="price">R$ 5,00</div><button class="btn" onclick="add('Esponja',5)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381065318/Mascara-cilios.jpg" alt="Máscara de Cílios"></div><h3>Máscara de Cílios</h3><div class="desc">Volume e alongamento</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Máscara Cílios',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380442611/brilho-labial.jpg" alt="Brilho Labial"></div><h3>Brilho Labial</h3><div class="desc">Boca luminosa o dia todo</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Brilho Labial',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380669893/Candy%20lip%20oil.jpg" alt="Lip Oil Change Color Hudamoji"></div><h3>Lip Oil Change Color Hudamoji</h3><div class="desc">Lip oil hidratante com efeito change color</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Lip Oil Change Color Hudamoji',10)">Adicionar</button></div>
</div>
<h2>🧴 Cuidados e Higiene</h2><div class="products">
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381126635/Sabonete-abacaxi.jpg" alt="Sabonete Líquido Brisa Abacaxi 1L"></div><h3>Sabonete Líquido Brisa Abacaxi 1L</h3><div class="desc">Suavidade e proteção 1 litro</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Sabonete Abacaxi 1L',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381317788/Escova%20de%20cabelo.jpg" alt="Escova de Cabelo"></div><h3>Escova de Cabelo</h3><div class="desc">Desembaraça sem quebrar</div><div class="price">R$ 10,00</div><button class="btn" onclick="add('Escova Cabelo',10)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381330397/Escova%20massageadora.jpg" alt="Escova Massageadora"></div><h3>Escova Massageadora</h3><div class="desc">Massageia e ativa circulação</div><div class="price">R$ 8,00</div><button class="btn" onclick="add('Escova Massageadora',8)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790380245557/Agua-micelar.jpg" alt="Água Micelar"></div><h3>Água Micelar</h3><div class="desc">Limpa e hidrata sem arder - Rose</div><div class="price">R$ 12,00</div><button class="btn" onclick="add('Água Micelar',12)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381138795/d.jpg" alt="Esfoliante Rosto e Corpo"></div><h3>Esfoliante Rosto e Corpo</h3><div class="desc">Pele lisinha e renovada</div><div class="price">R$ 20,00</div><button class="btn" onclick="add('Esfoliante',20)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381157498/sintimo.jpg" alt="Sabonete Íntimo"></div><h3>Sabonete Íntimo</h3><div class="desc">Cuidado delicado diário</div><div class="price">R$ 12,00</div><button class="btn" onclick="add('Sabonete Íntimo',12)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381253749/touca.jpg" alt="Touca de Cetim"></div><h3>Touca de Cetim</h3><div class="desc">Dupla face, sem frizz</div><div class="price">R$ 5,00</div><button class="btn" onclick="add('Touca Cetim',5)">Adicionar</button></div>
</div>
<h2>💖 Acessórios e Variedades</h2><div class="products">
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381435300/Xuxinha.jpg" alt="Xuxinha Cetim"></div><h3>Xuxinha Cetim</h3><div class="desc">Não marca nem quebra</div><div class="price">R$ 3,00</div><button class="btn" onclick="add('Xuxinha',3)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381832502/Len%C3%83%C2%A7o%20umedecido%20P.jpg" alt="Lenço Fácil P Yasmim"></div><h3>Lenço Fácil P Yasmim</h3><div class="desc">Aloe Vera e Laranja</div><div class="price">R$ 5,00</div><button class="btn" onclick="add('Lenço P',5)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381738367/Len%C3%83%C2%A7o%20umedecido%20G.jpg" alt="Lenço Fácil G 30un Hudamoji"></div><h3>Lenço Fácil G 30un Hudamoji</h3><div class="desc">Mais folhas, mais economia</div><div class="price">R$ 8,00</div><button class="btn" onclick="add('Lenço G',8)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381650824/p.jpg" alt="Piranha Brilhosa Metalizada"></div><h3>Piranha Brilhosa Metalizada</h3><div class="desc">Brilho máximo, 6 cores</div><div class="price">R$ 6,00</div><button class="btn" onclick="add('Piranha Brilhosa',6)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381483704/p-florp.jpg" alt="Piranha Flor Plástico P"></div><h3>Piranha Flor Plástico P</h3><div class="desc">Flor plumeria delicada</div><div class="price">R$ 5,00</div><button class="btn" onclick="add('Piranha Flor',5)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381501674/Piranha%20pl%C3%83%C2%A1stico%20P%20.jpg" alt="Piranha Plástico P Trançada"></div><h3>Piranha Plástico P Trançada</h3><div class="desc">Mini mas prende firme</div><div class="price">R$ 4,00</div><button class="btn" onclick="add('Piranha P',4)">Adicionar</button></div>
<div class="card"><div class="img"><img src="https://uploads.onecompiler.io/454bxpyrs/1790381468139/Piranha%20brilhosa%20G.jpg" alt="Piranha Plástico Brilhante G"></div><h3>Piranha Plástico Brilhante G</h3><div class="desc">Tamanho grande, segura muito</div><div class="price">R$ 6,00</div><button class="btn" onclick="add('Piranha G',6)">Adicionar</button></div>
</div></main>
<div id="cartIcon" onclick="toggle()">🛒 Carrinho (<span id="qtd">0</span>)</div>
<div id="cart"><div id="itens"></div><div id="cartTotal">Total: R$ 0,00</div><button id="btnFinalizar" onclick="zap()">Finalizar no WhatsApp</button></div>
<footer><p><strong>ROSE MIMO - Beleza, Mimos e Variedades</strong></p><p>📲 (85) 98700-5202</p><p>📸 @mimosdarosevariedades</p></footer>
<script>
let carrinho=[];
function add(nome,preco){carrinho.push({nome,preco});upd();document.getElementById('cart').style.display='block';}
function upd(){let h='',t=0;carrinho.forEach(p=>{t+=p.preco;h+=`<div class="cart-item"><span>${p.nome}</span><span>R$ ${p.preco.toFixed(2).replace('.',',')}</span></div>`});document.getElementById('itens').innerHTML=h||"<p style='font-size:12px;color:#888'>Carrinho vazio</p>";document.getElementById('cartTotal').innerText='Total: R$ '+t.toFixed(2).replace('.',',');document.getElementById('qtd').innerText=carrinho.length;}
function toggle(){let c=document.getElementById('cart');c.style.display=c.style.display==='block'?'none':'block';}
function zap(){if(!carrinho.length){alert('Carrinho vazio');return;}let t=0,m='Olá Rose Mimo! 🌹 Vim pelo site e quero:%0A';carrinho.forEach(p=>{t+=p.preco;m+=`- ${p.nome} R$ ${p.preco.toFixed(2).replace('.',',')}%0A`});m+=`%0A*Total: R$ ${t.toFixed(2).replace('.',',')}*%0A%0AComo combinamos a entrega?`;window.open('https://wa.me/5585987005202?text='+m,'_blank');}
</script>
</body></html>
