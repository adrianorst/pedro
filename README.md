# pedro<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <title>Pedro e Adriano Pod</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <style>
    body { font-family: Arial, sans-serif; margin: 0; background: #f6f8fa; }
    header { background: #2d6cdf; color: #fff; text-align: center; padding: 40px 0 20px 0; }
    h1 { margin: 0; font-size: 2.5em; letter-spacing: 2px;}
    .pod-container {
      max-width: 800px;
      margin: 40px auto;
      background: #fff;
      box-shadow: 0 2px 8px rgba(0,0,0,0.08);
      padding: 32px;
      border-radius: 12px;
    }
    nav { margin-bottom: 16px; text-align: center;}
    nav button {
      margin: 0 6px;
      padding: 10px 20px;
      font-size: 1em;
      border: none;
      background: #2d6cdf;
      color: #fff;
      border-radius: 6px;
      cursor: pointer;
    }
    nav button:hover { background: #184fa7; }
    .iframe-wrapper {
      display: flex;
      justify-content: center;
    }
    iframe {
      width: 650px;
      height: 500px;
      border: 2px solid #2d6cdf;
      border-radius: 10px;
      background: #fff;
    }
    @media (max-width: 700px) {
      iframe { width: 100%; height: 350px; }
      .pod-container { padding: 16px;}
      h1 { font-size: 1.3em; }
    }
    footer { text-align: center; color: #888; padding: 20px 0;}
  </style>
</head>
<body>
  <header>
    <h1>Pedro e Adriano Pod</h1>
    <p>Escolha um jornal para visualizar na janela abaixo</p>
  </header>
  <div class="pod-container">
    <nav>
      <button onclick="document.getElementById('janela').src='https://www.folha.uol.com.br/'">Folha de S.Paulo</button>
      <button onclick="document.getElementById('janela').src='https://www.estadao.com.br/'">Estadão</button>
      <button onclick="document.getElementById('janela').src='https://g1.globo.com/'">G1</button>
      <button onclick="document.getElementById('janela').src='https://www.correiobraziliense.com.br/'">Correio Braziliense</button>
    </nav>
    <div class="iframe-wrapper">
      <iframe id="janela" src="https://www.folha.uol.com.br/" title="Janela de Jornais"></iframe>
    </div>
  </div>
  <footer>
    &copy; 2025 Pedro e Adriano Pod. Todos os direitos reservados.
  </footer>
</body>
</html>
