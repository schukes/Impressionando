<!DOCTYPE html>
<html>
<head>
  <title>😍😍</title>
  <style>
    body {
      background-color: #f8e0e0;
      text-align: center;
      font-family: 'Roboto', sans-serif;
      margin: 0;
      padding: 0;
    }

    h1 {
      color: #ff6699;
      font-size: 40px;
      margin-top: 100px;
    }

    #mensagem {
      color: #ff6699;
      font-size: 24px;
      margin-top: 30px;
    }

    #botaoAnterior, #botaoProximo {
      background-color: #ff6699;
      color: #fff;
      padding: 10px 20px;
      font-size: 18px;
      border: none;
      border-radius: 5px;
      margin-top: 20px;
      cursor: pointer;
      display: inline-block;
    }

    #botaoAnterior:hover, #botaoProximo:hover {
      background-color: #e65c8f;
    }

    #botaoAnterior {
      margin-right: 20px;
    }

    /* Estilos específicos para botões hover */

    /* Botão Anterior */
    #botaoAnterior:hover {
      background-color: #e65c8f;
    }

    /* Botão Próximo */
    #botaoProximo:hover {
      background-color: #e65c8f;
    }
  </style>
</head>
<body>
  <h1>Passando pra te dizer que:</h1>
  <p id="mensagem"></p>
  <button id="botaoAnterior" onclick="voltarFrase()" style="display: none;">Anterior</button>
  <button id="botaoProximo" onclick="avançarFrase()">Próxima</button>

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
      "Não consigo parar de pensar em você!!! 💭",
      "Vamos fazer algumas perguntas?",
      "Como é o seu dia a dia? O que você gosta de fazer no seu tempo livre?",
      "Quais são seus hobbies ou paixões? O que te motiva?",
      "Como é a sua relação com sua família e amigos mais próximos?",
      "Quais são seus objetivos de curto e longo prazo na vida? O que você busca alcançar?",
      "Quais foram suas experiências mais significativas na vida? O que aprendeu com elas?",
      "Quais são os valores mais importantes para você? Quais crenças guiam suas decisões?",
      "O que você aprendeu em relacionamentos passados? O que considera essencial em um parceiro?",
      "Como você vê o mundo ao seu redor? Há algo que você deseja mudar ou contribuir para melhorar?",
      "Como você lida com conflitos e desacordos em um relacionamento? Como você prefere que a comunicação seja feita em situações difíceis?",
      "Quais são suas expectativas em um relacionamento? O que você procura e espera de um parceiro?"
    ];

    var contador = 0;

    function exibirElogio(numeroElogio) {
      var mensagemElemento = document.getElementById("mensagem");
      mensagemElemento.innerHTML = elogios[numeroElogio];

      if (numeroElogio === 0) {
        document.getElementById("botaoAnterior").style.display = "none";
      } else {
        document.getElementById("botaoAnterior").style.display = "inline-block";
      }

      if (numeroElogio === elogios.length - 1) {
        document.getElementById("botaoProximo").style.display = "none";
      } else {
        document.getElementById("botaoProximo").style.display = "inline-block";
      }
    }

    function avançarFrase() {
      contador++;
      exibirElogio(contador);
    }

    function voltarFrase() {
      contador--;
      exibirElogio(contador);
    }

    window.onload = function() {
      elogios = [
      "Você é incrível! 😍",
      "Seu sorriso ilumina o meu dia! 😊",
      "Você é muito linda! 😘",
      "Amo passar o tempo com você, inclusive o tempo voa! ❤️",
      "Seu charme é irresistível! 😉",
      "Você é inteligente e encantadora! 🤓",
      "Seu jeito raiz me supreende! 💓",
      "Agora todo café que tomo lembro da canela kkk 😊",
      "Sua presença torna tudo melhor! ✨",
      "Não consigo parar de pensar em você!!! 💭",
      "Vamos fazer algumas perguntas?",
      "Como é o seu dia a dia? O que você gosta de fazer no seu tempo livre?",
      "Quais são seus hobbies ou paixões? O que te motiva?",
      "Como é a sua relação com sua família e amigos mais próximos?",
      "Quais são seus objetivos de curto e longo prazo na vida? O que você busca alcançar?",
      "Quais foram suas experiências mais significativas na vida? O que aprendeu com elas?",
      "Quais são os valores mais importantes para você? Quais crenças guiam suas decisões?",
      "O que você aprendeu em relacionamentos passados? O que considera essencial em um parceiro?",
      "Como você vê o mundo ao seu redor? Há algo que você deseja mudar ou contribuir para melhorar?",
      "Como você lida com conflitos e desacordos em um relacionamento? Como você prefere que a comunicação seja feita em situações difíceis?",
      "Quais são suas expectativas em um relacionamento? O que você procura e espera de um parceiro?"
      ];

      exibirElogio(0);
    };
  </script>
</body>
</html>

/*
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
      "Não consigo parar de pensar em você!!! 💭",
      "Vamos fazer algumas perguntas?",
      "Como é o seu dia a dia? O que você gosta de fazer no seu tempo livre?",
      "Quais são seus hobbies ou paixões? O que te motiva?",
      "Como é a sua relação com sua família e amigos mais próximos?",
      "Quais são seus objetivos de curto e longo prazo na vida? O que você busca alcançar?",
      "Quais foram suas experiências mais significativas na vida? O que aprendeu com elas?",
      "Quais são os valores mais importantes para você? Quais crenças guiam suas decisões?",
      "O que você aprendeu em relacionamentos passados? O que considera essencial em um parceiro?",
      "Como você vê o mundo ao seu redor? Há algo que você deseja mudar ou contribuir para melhorar?",
      "Como você lida com conflitos e desacordos em um relacionamento? Como você prefere que a comunicação seja feita em situações difíceis?",
      "Quais são suas expectativas em um relacionamento? O que você procura e espera de um parceiro?"
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
</html> */
