#<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Direitos do Cidadão no Ambiente Digital</title>
  
  <style>
    /* ==========================================================================
       1. RESET (Seu padrão de consistência)
       ========================================================================== */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
      background-color: #f4f6f9;
      color: #333;
      line-height: 1.6;
      padding: 0 0 40px 0;
    }

    /* ==========================================================================
       2. ESTRUTURA E LAYOUT
       ========================================================================== */
    header {
      background-color: #2c3e50;
      color: white;
      text-align: center;
      padding: 40px 20px;
      margin-bottom: 30px;
    }

    header h1 {
      font-size: 2.2rem;
      margin-bottom: 10px;
    }

    header p {
      color: #bdc3c7;
      font-size: 1.1rem;
      max-width: 700px;
      margin: 0 auto;
    }

    .container {
      max-width: 1000px;
      margin: 0 auto;
      padding: 0 20px;
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
      gap: 25px;
    }

    /* ==========================================================================
       3. INTERAÇÕES E CARDS (Uso de Pseudoclasses)
       ========================================================================== */
    .lei-card {
      background-color: white;
      border-radius: 12px;
      padding: 25px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.05);
      border-top: 5px solid #bdc3c7;
      transition: transform 0.2s, box-shadow 0.2s;
    }

    /* Cores de destaque para cada lei */
    .lei-card.lgpd { border-top-color: #3498db; }
    .lei-card.marco-civil { border-top-color: #9b59b6; }
    .lei-card.cdc { border-top-color: #e67e22; }

    /* :hover - Feedback visual ao passar o mouse */
    .lei-card:hover {
      transform: translateY(-5px);
      box-shadow: 0 8px 15px rgba(0,0,0,0.1);
    }

    .lei-card h2 {
      font-size: 1.4rem;
      margin-bottom: 5px;
      color: #2c3e50;
    }

    .lei-sigla {
      display: inline-block;
      font-size: 0.8rem;
      font-weight: bold;
      text-transform: uppercase;
      padding: 2px 8px;
      border-radius: 4px;
      margin-bottom: 15px;
      background-color: #ecf0f1;
    }

    /* Cores das siglas */
    .lgpd .lei-sigla { color: #3498db; background-color: #e1f5fe; }
    .marco-civil .lei-sigla { color: #9b59b6; background-color: #f3e5f5; }
    .cdc .lei-sigla { color: #e67e22; background-color: #fff3e0; }

    .lei-card p {
      font-size: 0.95rem;
      color: #555;
      margin-bottom: 15px;
    }

    .lei-card h3 {
      font-size: 1rem;
      margin: 15px 0 8px 0;
      color: #2c3e50;
    }

    .lei-card ul {
      list-style-position: inside;
      margin-bottom: 15px;
      font-size: 0.9rem;
      color: #666;
    }

    .lei-card ul li {
      margin-bottom: 5px;
    }

    /* Links e botões internos com :focus e :active */
    .saiba-mais {
      display: inline-block;
      color: #2c3e50;
      text-decoration: none;
      font-weight: bold;
      font-size: 0.9rem;
      border-bottom: 2px solid transparent;
      transition: all 0.2s;
    }

    /* :hover e :focus no link */
    .saiba-mais:hover, .saiba-mais:focus {
      color: #34495e;
      border-bottom-color: currentColor;
      outline: none;
    }

    .saiba-mais:active {
      opacity: 0.6;
    }
  </style>
</head>
<body>

  <header>
    <h1>Cidadania Digital</h1>
    <p>Conheça as três principais leis brasileiras que protegem você, sua privacidade e seus direitos de consumidor na internet.</p>
  </header>

  <main class="container">

    <section class="lei-card lgpd">
      <span class="lei-sigla">Lei nº 13.709/2018</span>
      <h2>LGPD</h2>
      <p>Focada em proteger a privacidade dos seus dados pessoais, definindo regras rígidas para coleta e armazenamento por empresas e aplicativos.</p>
      
      <h3>Seus Principais Direitos:</h3>
      <ul>
        <li>Saber quais dados são usados;</li>
        <li>Corrigir erros e informações;</li>
        <li>Solicitar exclusão de dados;</li>
        <li>Retirar consentimento de uso.</li>
      </ul>
      <a href="https://www.gov.br/anpd/pt-br" target="_blank" class="saiba-mais">Acessar a ANPD →</a>
    </section>

    <section class="lei-card marco-civil">
      <span class="lei-sigla">Lei nº 12.965/2014</span>
      <h2>Marco Civil da Internet</h2>
      <p>Conhecido como a "Constituição da Internet", estabelece os princípios de liberdade, privacidade e neutralidade da rede no Brasil.</p>
      
      <h3>Pilares Fundamentais:</h3>
      <ul>
        <li>Neutralidade da rede;</li>
        <li>Liberdade de expressão online;</li>
        <li>Proteção do histórico de navegação;</li>
        <li>Dados liberados só por ordem judicial.</li>
      </ul>
      <a href="#" class="saiba-mais">Ver detalhes da lei →</a>
    </section>

    <section class="lei-card cdc">
      <span class="lei-sigla">Lei nº 8.078/1990</span>
      <h2>Código de Defesa do Consumidor</h2>
      <p>Garante que todas as compras e contratações feitas na internet tenham as mesmas proteções e direitos das lojas físicas.</p>
      
      <h3>Garantias no E-commerce:</h3>
      <ul>
        <li>Direito de arrependimento (7 dias);</li>
        <li>Clareza em preços e prazos;</li>
        <li>Proteção contra golpes virtuais;</li>
        <li>Defesa contra propaganda enganosa.</li>
      </ul>
      <a href="https://www.consumidor.gov.br" target="_blank" class="saiba-mais">Registrar reclamação →</a>
    </section>

  </main>

</body>
</html> desenvolvendo-interfaces-inclusivas
