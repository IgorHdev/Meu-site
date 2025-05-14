#SITE
<!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Site Pessoal – Igor</title>
  <style>
   
    html {
      scroll-behavior: smooth;
    }

    
    :root {
      --cor-primaria: #0066cc;
      --cor-secundaria: #ff6600;
      --cor-fundo: #f2f9ff;
      --cor-card: #ffffff;
      --cor-texto: #333333;
      --sombra-leve: 0 4px 8px rgba(0,0,0,0.1);
    }

    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', Tahoma, sans-serif;
    }

    body {
      background-color: var(--cor-fundo);
      color: var(--cor-texto);
      line-height: 1.6;
    }

    header {
      background: linear-gradient(90deg, var(--cor-primaria), var(--cor-secundaria));
      padding: 20px;
      display: flex;
      align-items: center;
      box-shadow: var(--sombra-leve);
    }

    .logo {
      font-size: 1.8em;
      font-weight: bold;
      color: #fff;
      letter-spacing: 1px;
    }

    nav {
      margin-left: auto;
    }
    nav ul {
      list-style: none;
      display: flex;
      gap: 30px;
    }
    nav a {
      text-decoration: none;
      color: #fff;
      font-weight: 600;
      padding: 8px 12px;
      border-radius: 4px;
      transition: background 0.3s, transform 0.2s;
    }
    nav a:hover {
      background-color: rgba(255,255,255,0.2);
      transform: translateY(-2px);
    }

    main {
      padding: 60px 20px;
      max-width: 1200px;
      margin: 0 auto;
    }

    .quem-sou {
      background-color: var(--cor-card);
      padding: 40px;
      margin-bottom: 50px;
      border-radius: 12px;
      box-shadow: var(--sombra-leve);
      transition: transform 0.3s;
    }
    .quem-sou:hover {
      transform: translateY(-4px);
    }
    .quem-sou h2 {
      color: var(--cor-primaria);
      margin-bottom: 25px;
    }
    .conteudo {
      display: flex;
      gap: 30px;
      align-items: center;
    }
    .conteudo img {
      width: 200px;
      border-radius: 50%;
      box-shadow: var(--sombra-leve);
      transition: transform 0.3s;
    }
    .conteudo img:hover {
      transform: scale(1.05);
    }
    .historia h3 {
      color: var(--cor-secundaria);
      margin-bottom: 10px;
    }
    .historia p {
      margin-bottom: 15px;
      text-align: justify;
    }

    .missao-visao {
      display: flex;
      gap: 30px;
      margin-top: 40px;
    }
    .missao, .visao {
      flex: 1;
      background-color: #e6f2ff;
      padding: 25px;
      border-radius: 10px;
      border-left: 5px solid var(--cor-primaria);
      transition: background 0.3s;
    }
    .missao:hover, .visao:hover {
      background-color: #d0e7ff;
    }

    .contato {
      background-color: var(--cor-card);
      padding: 40px;
      border-radius: 12px;
      box-shadow: var(--sombra-leve);
    }
    .contato h2 {
      color: var(--cor-primaria);
      margin-bottom: 30px;
    }
    .info-form {
      display: flex;
      gap: 40px;
      flex-wrap: wrap;
    }
    .informacoes, .horario {
      flex: 1;
      min-width: 240px;
    }
    .informacoes h3, .horario h3 {
      color: var(--cor-secundaria);
      margin-bottom: 15px;
    }
    .informacoes p, .horario p {
      margin-bottom: 10px;
      font-size: 1.05em;
    }

    form {
      display: grid;
      grid-template-columns: 1fr 1fr;
      gap: 20px 40px;
      margin-top: 30px;
    }
    form label {
      font-weight: 600;
    }
    form input, form select, form textarea {
      grid-column: span 2;
      padding: 12px;
      border: 1px solid #ccc;
      border-radius: 6px;
      transition: border-color 0.3s;
    }
    form input:focus, form select:focus, form textarea:focus {
      border-color: var(--cor-primaria);
      outline: none;
    }
    form textarea {
      resize: vertical;
      height: 120px;
    }
    button {
      grid-column: span 2;
      padding: 12px 0;
      background: var(--cor-primaria);
      color: #fff;
      border: none;
      border-radius: 6px;
      font-size: 1.1em;
      cursor: pointer;
      transition: background 0.3s, transform 0.2s;
    }
    button:hover {
      background: var(--cor-secundaria);
      transform: translateY(-2px);
    }

.contato {
    background-color: #fff;
    padding: 60px 20px;
    border-radius: 12px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.08);
    max-width: 1000px;
    margin: 0 auto 60px auto;
  }
  
  .contato h2 {
    text-align: center;
    font-size: 2rem;
    color: #0066cc;
    margin-bottom: 40px;
  }
  

  .contato-cards {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 20px;
    margin-bottom: 50px;
  }
  
  .card {
    background-color: #f2f9ff;
    padding: 20px;
    border-radius: 8px;
    text-align: center;
    transition: transform 0.3s;
  }
  
  .card:hover {
    transform: translateY(-5px);
  }
  
  .card i {
    font-size: 2rem;
    color: #ff6600;
    margin-bottom: 10px;
  }
  
  .card h3 {
    margin-bottom: 8px;
    font-size: 1.1rem;
    color: #333;
  }
  
  .card p, .card a {
    color: #555;
    text-decoration: none;
    font-size: 0.95rem;
  }

  .contato-form {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
    gap: 20px;
  }
  
  .form-group {
    display: flex;
    flex-direction: column;
  }
  
  .form-group.full {
    grid-column: 1 / -1;
  }
  
  .form-group label {
    margin-bottom: 8px;
    font-weight: 600;
    color: #333;
  }
  
  .form-group input,
  .form-group textarea {
    padding: 12px;
    border: 1px solid #ccc;
    border-radius: 6px;
    transition: border-color 0.3s;
  }
  
  .form-group input:focus,
  .form-group textarea:focus {
    border-color: #0066cc;
    outline: none;
  }
  
  button[type="submit"] {
    grid-column: 1 / -1;
    padding: 14px 0;
    background-color: #0066cc;
    color: #fff;
    border: none;
    border-radius: 6px;
    font-size: 1.1rem;
    cursor: pointer;
    transition: background 0.3s, transform 0.2s;
  }
  
  button[type="submit"]:hover {
    background-color: #004a99;
    transform: translateY(-2px);
  }
  
  </style>
</head>

<body id="topo">

  <header>
    <div class="logo">Meu Site</div>
    <nav>
      <ul>
        <li><a href="#topo">Home</a></li>
        <li><a href="valores.html">Valores</a></li>
        <li><a href="contato.html">Contato</a></li>
      </ul>
    </nav>
  </header>

  <main>
    <section class="quem-sou">
      <h2>Igor Henrique Souza Lima</h2>
      <div class="conteudo">
        <img src="#" alt="Imagem sobre mim">
        <div class="historia">
          <h3>Minha História</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla auctor, nisl eget ultricies.</p>
          <p>Aliquam erat volutpat. Integer tristique tincidunt, nisl nisi aliquam nisi, eget ultrices.</p>
        </div>
      </div>
      <div class="missao-visao">
        <div class="missao">
          <h3>Missão</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
        <div class="visao">
          <h3>Visão</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
        </div>
      </div>
    </section>

    <section class="contato">
        <h2>Entre em Contato</h2>
      
        <div class="contato-cards">
          <div class="card">
            <i class="fas fa-phone-alt"></i>
            <h3>Telefone</h3>
            <p>(11) 95484-7079</p>
          </div>
          <div class="card">
            <i class="fas fa-envelope"></i>
            <h3>E-mail</h3>
            <p>igorhenriquesouza813@gmail.com</p>
          </div>
          <div class="card">
            <i class="fas fa-map-marker-alt"></i>
            <h3>Localização</h3>
            <p>São Paulo – SP</p>
          </div>
          <div class="card">
            <i class="fab fa-linkedin"></i>
            <h3>LinkedIn</h3>
            <p><a href="https://linkedin.com/in/seu-perfil" target="_blank">seu-perfil</a></p>
          </div>
          <div class="card">
            <i class="fab fa-github"></i>
            <h3>GitHub</h3>
            <p><a href="https://github.com/seu-usuario" target="_blank">seu-usuario</a></p>
          </div>
        </div>
      
        <form class="contato-form">
          <div class="form-group">
            <label for="nome">Nome *</label>
            <input id="nome" type="text" required />
          </div>
          <div class="form-group">
            <label for="email">E-mail *</label>
            <input id="email" type="email" required />
          </div>
          <div class="form-group">
            <label for="assunto">Assunto *</label>
            <input id="assunto" type="text" required />
          </div>
          <div class="form-group full">
            <label for="mensagem">Mensagem *</label>
            <textarea id="mensagem" rows="5" required></textarea>
          </div>
          <button type="submit">Enviar Mensagem</button>
        </form>
      </section>
      
  </main>

</body>
</html>
