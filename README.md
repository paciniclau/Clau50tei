<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Convite Virtual - Claudia 50 anos</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #fffbe6;
      color: #333;
      text-align: center;
      padding: 20px;
    }

    h1 {
      font-size: 2.5em;
      margin-bottom: 10px;
    }

    p {
      font-size: 1.2em;
      margin-bottom: 20px;
    }

    .buttons {
      display: flex;
      flex-direction: column;
      gap: 15px;
      max-width: 300px;
      margin: auto;
    }

    button {
      padding: 12px;
      border: none;
      background-color: #ff99cc;
      color: white;
      font-size: 1em;
      border-radius: 8px;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #ff66b2;
    }

    .content {
      margin-top: 30px;
      display: none;
      font-size: 1em;
      line-height: 1.6;
      background-color: #fff0f5;
      padding: 20px;
      border-radius: 10px;
    }
  </style>
</head>
<body>

  <h1>Olaudia Ops50tei</h1>
  <p>E PARA CELEBRAR ESSE NOVO CICLO DA MINHA VIDA, CONVIDO VOCÊ PARA ESTAR AÍ AO MEU LADO.</p>

  <div class="buttons">
    <button onclick="mostrar('data')">📅 DATA E HORÁRIO</button>
    <button onclick="mostrar('local')">📍 LOCAL</button>
    <button onclick="mostrar('confirmar')">✅ CONFIRMAR PRESENÇA</button>
    <button onclick="mostrar('presente')">🎁 SUGESTÕES DE PRESENTES</button>
    <button onclick="mostrar('dresscode')">👗 DRESS CODE</button>
  </div>

  <div id="data" class="content">
    <strong>Data:</strong> 28 de Junho<br/>
    <strong>Hora:</strong> 21h30
  </div>

  <div id="local" class="content">
    <strong>Local:</strong> Eco Buffet<br/>
    <a href="https://www.google.com/maps " target="_blank">Como chegar (clique aqui)</a>
  </div>

  <div id="confirmar" class="content">
    Por favor, confirme sua presença até dia 20/06.<br/>
    <a href="mailto:seuemail@example.com">Clique aqui para enviar um e-mail</a><br/>
    Ou ligue: <strong>(00) 99999-9999</strong>
  </div>

  <div id="presente" class="content">
    Algumas sugestões de presentes que adoraria receber:<br/>
    - Livros inspiradores<br/>
    - Experiências (jantares, passeios)<br/>
    - Itens decorativos vintage<br/>
    - Vale-presentes
  </div>

  <div id="dresscode" class="content">
    O dress code da festa é: <strong>Vintage Glam</strong><br/>
    Vista algo elegante e nostálgico! 💫
  </div>

  <script>
    function mostrar(id) {
      // Esconder todos os conteúdos
      const contents = document.querySelectorAll('.content');
      contents.forEach(c => c.style.display = 'none');

      // Mostrar apenas o selecionado
      document.getElementById(id).style.display = 'block';
    }
  </script>

</body>
</html>
