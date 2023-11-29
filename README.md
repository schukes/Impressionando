<html>
<head>
  <title>😍😍</title>
  <style>
    body {
      background-color: pink;
      text-align: center;
      font-family: Arial, sans-serif;
    }
    
    h1 {
      color: white;
      font-size: 40px;
      margin-top: 200px;
    }
    
    #mensagem {
      color: white;
      font-size: 24px;
      margin-top: 50px;
    }
    
    #botao {
      background-color: white;
      color: pink;
      padding: 10px 20px;
      font-size: 18px;
      border-radius: 5px;
      margin-top: 50px;
      cursor: pointer;
    }
    
    #botao:hover {
      background-color: pink;
      color: white;
    }
  </style>
</head>
<body>
  <h1>Passando pra te dizer que:</h1>
  <p id="mensagem"></p>
  <button id="botao" onclick="impressionar()">Clique aqui!</button>

  <script>
    var elogios = [
      "Você é incrível! 😍",
      "Seu sorriso ilumina o meu dia! 😊",
      "Você é muito linda! 😘",
      "Amo passar o tempo com você, inclusive o tempo voa! ❤️",
      "Seu charme é irresistível! 😉",
      "Você é inteligente e encantadora! 🤓",
      "Seu jeito raiz me supreende! 💓",
      "Agora todo café que tomo lembro da canela kkk 😊",
      "Sua presença torna tudo melhor! ✨",
      "Não consigo parar de pensar em você!!! 💭"
    ];

    var contador = 0;

    function impressionar() {
  var mensagemElemento = document.getElementById("mensagem");
  var botaoElemento = document.getElementById("botao");

  if (contador < elogios.length) {
    mensagemElemento.innerHTML = elogios[contador];
    contador++;
  }

  // Mover a verificação para ocultar o botão aqui
  if (contador >= elogios.length) {
    botaoElemento.style.display = "none";
  }
}

</script>
</body>
</html>
