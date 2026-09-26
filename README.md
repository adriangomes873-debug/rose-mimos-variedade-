<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>Rose Mimo - Beleza, Mimos e Variedades</title>

  <style>
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #fff8fc;
      color: #333;
    }

    /* TOPO */
    header {
      background: linear-gradient(135deg, #d41470, #f52c91);
      color: white;
      padding: 35px 20px;
      text-align: center;
    }

    .logo {
      font-size: 34px;
      font-weight: bold;
      margin-bottom: 15px;
    }

    .linha {
      height: 2px;
      background: rgba(255,255,255,0.8);
      margin: 15px 0 25px;
    }

    .slogan {
      font-size: 20px;
      margin-bottom: 30px;
    }

    .contato {
      font-size: 18px;
      line-height: 1.7;
    }

    /* CONTEÚDO */
    main {
      max-width: 1100px;
      margin: auto;
      padding: 25px 15px 110px;
    }

    .titulo-secao {
      border-left: 10px solid #f23891;
      padding: 8px 15px;
      margin: 20px 0 25px;
      font-size: 32px;
      color: #c21867;
    }

    /* PRODUTOS */
    .produtos {
      display: grid;
      grid-template-columns: repeat(2, 1fr);
      gap: 20px;
    }

    .produto {
      background: white;
      border-radius: 22px;
      padding: 15px;
      text-align: center;
      box-shadow: 0 5px 20px rgba(190, 20, 100, 0.12);
      overflow: hidden;
    }

    .produto img {
      width: 100%;
      height: 210px;
      object-fit: contain;
      border-radius: 15px;
      background: #fff;
    }

    .produto h3 {
      font-size: 20px;
      margin: 15px 5px 8px;
      color: #333;
    }

    .descricao {
      color: #777;
      font-size: 16px;
      min-height: 42px;
    }

    .preco {
      font-size: 25px;
      font-weight: bold;
      color: #e32683;
      margin: 15px 0;
    }

    .botao {
      width: 100%;
      border: none;
      border-radius: 30px;
      padding: 13px;
      background: #f52c91;
      color: white;
      font-size: 17px;
      font-weight: bold;
      cursor: pointer;
    }

    .botao:hover {
      background: #c91668;
    }

    /* CARRINHO */
    .carrinho {
      position: fixed;
      right: 20px;
      bottom: 20px;
      background: #c91467;
      color: white;
      border: none;
      border-radius: 40px;
      padding: 17px 25px;
      font-size: 18px;
      font-weight: bold;
      box-shadow: 0 5px 20px rgba(0,0,0,0.25);
      cursor: pointer;
      z-index: 1000;
    }

    /* JANELA DO CARRINHO */
    .fundo-carrinho {
      display: none;
      position: fixed;
      inset: 0;
      background: rgba(0,0,0,0.55);
      z-index: 2000;
      padding: 20px;
    }

    .janela-carrinho {
      background: white;
      max-width: 500px;
      margin: 30px auto;
      border-radius: 25px;
      padding: 25px;
      max-height: 85vh;
      overflow-y: auto;
    }

    .cabecalho-carrinho {
      display: flex;
      justify-content: space-between;
      align-items: center;
      margin-bottom: 20px;
    }

    .cabecalho-carrinho h2 {
      color: #c91467;
    }

    .fechar {
      border: none;
      background: #eee;
      border-radius: 50%;
      width: 40px;
      height: 40px;
      font-size: 22px;
      cursor: pointer;
    }

    .item-carrinho {
      border-bottom: 1px solid #eee;
      padding: 15px 0;
    }

    .item-carrinho strong {
      display: block;
      font-size: 17px;
      margin-bottom: 5px;
    }

    .quantidade {
      display: flex;
      align-items: center;
      gap: 10px;
      margin-top: 8px;
    }

    .quantidade button {
      border: none;
      background: #f52c91;
      color: white;
      border-radius: 50%;
      width: 30px;
      height: 30px;
      cursor: pointer;
      font-size: 18px;
    }

    .total {
      font-size: 24px;
      font-weight: bold;
      color: #c91467;
      margin: 20px 0;
      text-align: right;
    }

    .whatsapp {
      width: 100%;
      border: none;
      background: #25D366;
      color: white;
      border-radius: 30px;
      padding: 15px;
      font-size: 18px;
      font-weight: bold;
      cursor: pointer;
    }

    .vazio {
      text-align: center;
      padding: 30px 10px;
      color: #777;
    }

    /* RODAPÉ */
    footer {
      background: #c91467;
      color: white;
      text-align: center;
      padding: 25px 15px;
      line-height: 1.7;
    }

    /* CELULAR */
    @media (max-width: 600px) {

      .logo {
        font-size: 30px;
      }

      .slogan {
        font-size: 18px;
      }

      .contato {
        font-size: 16px;
      }

      .titulo-secao {
        font-size: 27px;
      }

      .produtos {
        grid-template-columns: repeat(2, 1fr);
        gap: 12px;
      }

      .produto {
        padding: 10px;
        border-radius: 17px;
      }

      .produto img {
        height: 150px;
      }

      .produto h3 {
        font-size: 17px;
      }

      .descricao {
        font-size: 14px;
      }

      .preco {
        font-size: 21px;
      }

      .botao {
        font-size: 14px;
        padding: 11px 5px;
      }

      .carrinho {
        right: 15px;
        bottom: 15px;
        font-size: 16px;
        padding: 15px 20px;
      }
    }
  </style>
</head>

<body>

  <!-- CABEÇALHO -->
  <header>

    <div class="logo">
      👑 ROSE MIMO 🌹
    </div>

    <div class="linha"></div>

    <div class="slogan">
      Beleza, Mimos e Variedades
    </div>

    <div class="contato">
      WhatsApp: (85) 98700-5202<br>
      @mimosdarosevariedades
    </div>

  </header>


  <!-- PRODUTOS -->
  <main>

    <h2 class="titulo-secao">
      💄 Maquiagem
    </h2>

    <div class="produtos">

      <!-- PRODUTO 1 -->
      <div class="produto">

        <img
          src="https://via.placeholder.com/400x400/ffffff/cc1970?text=Blush+Ruby+Rose"
          alt="Blush Compacto Duo Ruby Rose"
        >

        <h3>
          Blush Compacto Duo Ruby Rose
        </h3>

        <p class="descricao">
          Alta pigmentação, 2 cores lindas
        </p>

        <div class="preco">
          R$ 10,00
        </div>

        <button
          class="botao"
          onclick="adicionarCarrinho('Blush Compacto Duo Ruby Rose', 10)"
        >
          🛒 Adicionar
        </button>

      </div>


      <!-- PRODUTO 2 -->
      <div class="produto">

        <img
          src="https://via.placeholder.com/400x400/ffffff/cc1970?text=Blush+Playback"
          alt="Blush Compacto Playback"
        >

        <h3>
          Blush Compacto Playback
        </h3>

        <p class="descricao">
          Cor intensa que dura o dia todo
        </p>

        <div class="preco">
          R$ 10,00
        </div>

        <button
          class="botao"
          onclick="adicionarCarrinho('Blush Compacto Playback', 10)"
        >
          🛒 Adicionar
        </button>

      </div>


      <!-- PRODUTO 3 -->
      <div class="produto">

        <img
          src="https://via.placeholder.com/400x400/ffffff/cc1970?text=Produto+de+Maquiagem"
          alt="Produto de maquiagem"
        >

        <h3>
          Produto de Maquiagem
        </h3>

        <p class="descricao">
          Beleza para o seu dia
        </p>

        <div class="preco">
          R$ 10,00
        </div>

        <button
          class="botao"
          onclick="adicionarCarrinho('Produto de Maquiagem', 10)"
        >
          🛒 Adicionar
        </button>

      </div>

    </div>

  </main>


  <!-- BOTÃO CARRINHO -->
  <button class="carrinho" onclick="abrirCarrinho()">
    🛒 Carrinho (<span id="quantidadeTotal">0</span>)
  </button>


  <!-- CARRINHO -->
  <div class="fundo-carrinho" id="fundoCarrinho">

    <div class="janela-carrinho">

      <div class="cabecalho-carrinho">

        <h2>🛒 Meu Carrinho</h2>

        <button class="fechar" onclick="fecharCarrinho()">
          ×
        </button>

      </div>

      <div id="listaCarrinho"></div>

      <div class="total">
        Total: R$ <span id="total">0,00</span>
      </div>

      <button class="whatsapp" onclick="finalizarWhatsApp()">
        📲 Finalizar pelo WhatsApp
      </button>

    </div>

  </div>


  <!-- RODAPÉ -->
  <footer>

    <strong>🌹 ROSE MIMO 🌹</strong>

    <br>

    Beleza, Mimos e Variedades

    <br>

    WhatsApp: (85) 98700-5202

    <br>

    @mimosdarosevariedades

  </footer>


  <script>

    let carrinho = [];


    function adicionarCarrinho(nome, preco) {

      const produtoExistente = carrinho.find(
        produto => produto.nome === nome
      );

      if (produtoExistente) {

        produtoExistente.quantidade++;

      } else {

        carrinho.push({
          nome: nome,
          preco: preco,
          quantidade: 1
        });

      }

      atualizarCarrinho();

      alert("Produto adicionado ao carrinho!");

    }


    function atualizarCarrinho() {

      const lista = document.getElementById("listaCarrinho");
      const quantidadeTotal = document.getElementById("quantidadeTotal");
      const totalElemento = document.getElementById("total");

      lista.innerHTML = "";

      let quantidade = 0;
      let total = 0;


      if (carrinho.length === 0) {

        lista.innerHTML = `
          <div class="vazio">
            Seu carrinho está vazio.
          </div>
        `;

      }


      carrinho.forEach((produto, indice) => {

        quantidade += produto.quantidade;

        total += produto.preco * produto.quantidade;


        const item = document.createElement("div");

        item.className = "item-carrinho";

        item.innerHTML = `

          <strong>${produto.nome}</strong>

          <div>
            R$ ${produto.preco.toFixed(2).replace(".", ",")}
          </div>

          <div class="quantidade">

            <button onclick="diminuirQuantidade(${indice})">
              −
            </button>

            <span>
              ${produto.quantidade}
            </span>

            <button onclick="aumentarQuantidade(${indice})">
              +
            </button>

            <button
              onclick="removerProduto(${indice})"
              style="background:#777; margin-left:10px;"
            >
              🗑
            </button>

          </div>

        `;

        lista.appendChild(item);

      });


      quantidadeTotal.textContent = quantidade;

      totalElemento.textContent =
        total.toFixed(2).replace(".", ",");

    }


    function aumentarQuantidade(indice) {

      carrinho[indice].quantidade++;

      atualizarCarrinho();

    }


    function diminuirQuantidade(indice) {

      carrinho[indice].quantidade--;

      if (carrinho[indice].quantidade <= 0) {

        carrinho.splice(indice, 1);

      }

      atualizarCarrinho();

    }


    function removerProduto(indice) {

      carrinho.splice(indice, 1);

      atualizarCarrinho();

    }


    function abrirCarrinho() {

      document.getElementById("fundoCarrinho").style.display = "block";

      atualizarCarrinho();

    }


    function fecharCarrinho() {

      document.getElementById("fundoCarrinho").style.display = "none";

    }


    function finalizarWhatsApp() {

      if (carrinho.length === 0) {

        alert("Seu carrinho está vazio!");

        return;

      }


      let mensagem =
        "Olá! Quero fazer um pedido na Rose Mimo:%0A%0A";


      let total = 0;


      carrinho.forEach(produto => {

        const subtotal =
          produto.preco * produto.quantidade;

        total += subtotal;


        mensagem +=
          "• " +
          produto.nome +
          " - " +
          produto.quantidade +
          "x - R$ " +
          subtotal.toFixed(2).replace(".", ",") +
          "%0A";

      });


      mensagem +=
        "%0A*Total: R$ " +
        total.toFixed(2).replace(".", ",") +
        "*";


      const numero = "5585987005202";

      const link =
        "https://wa.me/" +
        numero +
        "?text=" +
        mensagem;


      window.open(link, "_blank");

    }


    atualizarCarrinho();

  </script>

</body>
</html>
