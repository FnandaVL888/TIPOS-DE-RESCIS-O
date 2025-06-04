<!DOCTYPE html>
<html lang="pt-br">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Informações sobre Rescisão de Trabalho - Guia para Trabalhadores</title>
<style>
  :root {
    --primary-color: #2c3e50;
    --secondary-color: #2980b9;
    --accent-color: #f39c12;
    --light-bg: #fdf6e3;
    --dark-bg: #ffffff;
    --text-color: #2d2d2d;
    --text-light: #555;
    --border-radius: 6px;
    --font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  }
  body {
    margin: 0;
    font-family: var(--font-family);
    background: var(--light-bg);
    color: var(--text-color);
    min-height: 100vh;
    display: flex;
    flex-direction: column;
  }
  header {
    background-color: var(--primary-color);
    color: white;
    padding: 1.5rem 1rem;
    text-align: center;
    font-weight: 700;
    font-size: 1.6rem;
    box-shadow: 0 3px 6px rgba(0,0,0,0.15);
  }
  header p.subtitle {
    font-weight: 400;
    font-size: 1rem;
    margin-top: 0.3rem;
    color: #cccccc;
  }
  .container {
    flex: 1;
    display: flex;
    max-width: 1100px;
    margin: 1.5rem auto 2rem;
    width: 90%;
    background: var(--dark-bg);
    border-radius: var(--border-radius);
    box-shadow: 0 0 15px rgba(0,0,0,0.1);
    overflow: hidden;
  }
  nav {
    width: 260px;
    background-color: var(--secondary-color);
    padding: 1rem 0;
    display: flex;
    flex-direction: column;
    position: sticky;
    top: 0;
    height: fit-content;
    max-height: 90vh;
    overflow-y: auto;
    border-right: 3px solid var(--accent-color);
  }
  nav a {
    color: white;
    text-decoration: none;
    padding: 12px 24px;
    font-weight: 600;
    border-left: 5px solid transparent;
    transition: background-color 0.3s, border-color 0.3s;
  }
  nav a:hover, nav a.active {
    background-color: var(--primary-color);
    border-left: 5px solid var(--accent-color);
  }
  main {
    padding: 1.5rem 2rem;
    flex: 1;
    overflow-y: auto;
  }
  main h2 {
    color: var(--primary-color);
    border-left: 6px solid var(--accent-color);
    padding-left: 10px;
    margin-bottom: 0.75rem;
  }
  main p, main ul {
    font-size: 1rem;
    line-height: 1.5;
    color: var(--text-color);
    margin-bottom: 1rem;
  }
  main ul {
    padding-left: 1.5rem;
  }
  /* Accordion Style */
  .accordion {
    margin-bottom: 1rem;
    border-radius: var(--border-radius);
    border: 1px solid #ddd;
    box-shadow: 0 1px 3px rgba(0,0,0,0.07);
  }
  .accordion-header {
    background-color: var(--secondary-color);
    color: white;
    cursor: pointer;
    padding: 1rem 1.25rem;
    user-select: none;
    font-weight: 600;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-radius: var(--border-radius) var(--border-radius) 0 0;
  }
  .accordion-header:hover {
    background-color: #1f5d8e;
  }
  .accordion-content {
    display: none;
    padding: 1rem 1.25rem;
    background: var(--dark-bg);
    color: var(--text-color);
    border-radius: 0 0 var(--border-radius) var(--border-radius);
    border-top: 1px solid #ddd;
  }
  .accordion-content.active {
    display: block;
  }
  .accordion-header .arrow {
    transition: transform 0.3s ease;
  }
  .accordion-header.active .arrow {
    transform: rotate(90deg);
  }

  /* Search */
  #searchContainer {
    margin-bottom: 1.5rem;
  }
  #searchInput {
    width: 100%;
    padding: 0.5rem 1rem;
    font-size: 1rem;
    border-radius: var(--border-radius);
    border: 1px solid #bbb;
    outline: none;
    transition: border-color 0.25s ease-in-out;
  }
  #searchInput:focus {
    border-color: var(--accent-color);
    box-shadow: 0 0 5px var(--accent-color);
  }

  /* FAQ Style */
  .faq-item {
    margin-bottom: 1rem;
    border: 1px solid #ddd;
    border-radius: var(--border-radius);
    box-shadow: 0 1px 3px rgba(0,0,0,0.05);
  }
  .faq-question {
    background-color: var(--secondary-color);
    color: white;
    padding: 1rem 1.25rem;
    cursor: pointer;
    user-select: none;
    font-weight: 600;
    border-radius: var(--border-radius) var(--border-radius) 0 0;
    display: flex;
    justify-content: space-between;
    align-items: center;
  }
  .faq-question:hover {
    background-color: #1f5d8e;
  }
  .faq-answer {
    padding: 1rem 1.25rem;
    background: var(--dark-bg);
    color: var(--text-color);
    display: none;
    border-top: 1px solid #ddd;
    border-radius: 0 0 var(--border-radius) var(--border-radius);
  }
  .faq-answer.active {
    display: block;
  }
  .faq-question .arrow {
    transition: transform 0.3s ease;
  }
  .faq-question.active .arrow {
    transform: rotate(90deg);
  }

  /* Responsive */
  @media (max-width: 900px) {
    .container {
      flex-direction: column;
      margin: 1rem auto;
    }
    nav {
      max-height: none;
      width: 100%;
      border-right: none;
      border-bottom: 3px solid var(--accent-color);
    }
    main {
      padding: 1rem;
    }
  }
</style>
</head>
<body>
<header>
  Informações sobre Rescisão de Trabalho
  <p class="subtitle">Guia prático e interativo para trabalhadores entenderem seus direitos e modalidades de rescisão</p>
</header>
<div class="container">
  <nav aria-label="Menu de navegação do site">
    <a href="#introducao" class="active">Início</a>
    <a href="#tipos-rescisao">Tipos de Rescisão</a>
    <a href="#direitos">Direitos e Verbas Rescisórias</a>
    <a href="#procedimentos">Procedimentos</a>
    <a href="#faq">Perguntas Frequentes</a>
    <a href="#contato">Contato Útil</a>
  </nav>
  <main>
    <section id="introducao">
      <h2>Bem-vindo!</h2>
      <p>Este site é dedicado a explicar de forma simples e interativa as principais informações sobre as relações de trabalho e os diferentes tipos de rescisão de contrato. Aqui você encontrará explicações práticas para compreender seus direitos e deveres, além de exemplos e dicas para lidar com situações comuns nas rescisões trabalhistas.</p>
      <p>Utilize o menu para navegar e explore os tópicos conforme sua necessidade. Você também pode buscar termos específicos usando o campo de busca abaixo.</p>
      <div id="searchContainer">
        <input type="text" id="searchInput" placeholder="Buscar termos ou tópicos..." aria-label="Campo de busca para filtrar os conteúdos da página" />
      </div>
    </section>

    <section id="tipos-rescisao">
      <h2>Tipos de Rescisão do Contrato de Trabalho</h2>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Dispensa Arbitrária (Sem Justa Causa)
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>O empregador encerra o contrato sem justa causa, e o trabalhador tem direito a verbas rescisórias como saldo de salário, aviso prévio, 13º salário proporcional, férias proporcionais e multa do FGTS.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão com Justa Causa
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Decorrente de faltas graves do empregado previstas no artigo 482 da CLT, como desobediência, abandono de emprego, furto ou assédio. O empregado perde direito a algumas verbas e pode manter apenas saldo de salário, 13º proporcional e férias vencidas.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão por Vontade do Empregado
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Quando o trabalhador pede demissão, deve cumprir aviso prévio e tem direito a saldo de salário, 13º salário proporcional e férias proporcionais, mas perde direitos como saque do FGTS e multa do FGTS.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão por Acordo entre as Partes
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Introduzida pela Reforma Trabalhista de 2017, é quando empregado e empregador fazem um acordo para o fim do contrato. O trabalhador pode sacar parte do FGTS e recebe metade do aviso prévio e multa reduzida.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão Indireta
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Situação em que o empregado encerra o contrato motivado por falta grave do empregador, como atraso de salários ou condições precárias de trabalho. Neste caso, tem direito às mesmas verbas da dispensa sem justa causa.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão por Culpa Recíproca
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Quando tanto empregado quanto empregador cometem faltas graves, causando o fim da relação. O trabalhador recebe parte das verbas rescisórias proporcionalmente segundo regras específicas.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Rescisão por Motivo de Força Maior
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Quando eventos imprevisíveis impossibilitam a continuidade do contrato, como desastres naturais, cabendo indenizações previstas em lei.</p>
        </div>
      </div>

      <div class="accordion">
        <div class="accordion-header" tabindex="0">
          Plano de Demissão Voluntária
          <span class="arrow">&#9654;</span>
        </div>
        <div class="accordion-content">
          <p>Modalidade em que o empregador oferece incentivos financeiros para adesão voluntária, com pagamento das verbas determinadas pelo tipo de demissão acordado.</p>
        </div>
      </div>
    </section>

    <section id="direitos">
      <h2>Direitos e Verbas Rescisórias</h2>
      <p>Ao ser desligado da empresa, é importante conhecer os principais direitos para garantir o recebimento correto:</p>
      <ul>
        <li><strong>Saldo de salário:</strong> pagamento dos dias trabalhados no mês da rescisão.</li>
        <li><strong>Aviso Prévio:</strong> indenização ou cumprimento do período mínimo de trabalho após aviso.</li>
        <li><strong>13º salário proporcional:</strong> valor proporcional ao tempo trabalhado no ano da rescisão.</li>
        <li><strong>Férias vencidas e proporcionais:</strong> pagamento das férias não gozadas e proporcionais ao tempo trabalhado.</li>
        <li><strong>FGTS:</strong> depósito e possível saque conforme tipo de rescisão.</li>
        <li><strong>Multas e indenizações:</strong> quando aplicável, como a multa de 40% do FGTS referentes à dispensa sem justa causa.</li>
      </ul>
      <p>Caso tenha dúvidas, busque a orientação de sindicatos, advogados trabalhistas ou órgãos de defesa do trabalhador.</p>
    </section>

    <section id="procedimentos">
      <h2>Procedimentos para Quem Vai Passar pela Rescisão</h2>
      <ul>
        <li>Comunique-se formalmente sobre a rescisão (com aviso prévio escrito, se possível).</li>
        <li>Solicite a documentação correta, como Termo de Rescisão do Contrato de Trabalho (TRCT).</li>
        <li>Confira o extrato do FGTS e documentos do PIS.</li>
        <li>Tenha atenção aos prazos para recebimento das verbas rescisórias, que a legislação determina.</li>
        <li>Em caso de irregularidades, procure os órgãos de fiscalização trabalhista ou assistência jurídica.</li>
      </ul>
    </section>

    <section id="faq">
      <h2>Perguntas Frequentes (FAQ)</h2>

      <div class="faq-item">
        <div class="faq-question" tabindex="0">
          O que é aviso prévio e quando ele deve ser cumprido?
          <span class="arrow">&#9654;</span>
        </div>
        <div class="faq-answer">
          <p>O aviso prévio é um período mínimo que deve ser cumprido para informar o término do contrato, podendo ser trabalhado ou indenizado. O prazo mínimo é de 30 dias e pode variar conforme o tempo de trabalho.</p>
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-question" tabindex="0">
          Posso sacar o FGTS em qualquer tipo de rescisão?
          <span class="arrow">&#9654;</span>
        </div>
        <div class="faq-answer">
          <p>Não. O saque do FGTS depende do tipo de rescisão. Por exemplo, na demissão sem justa causa e acordo, o trabalhador tem direito a sacar. Em casos de justa causa, não há direito ao saque.</p>
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-question" tabindex="0">
          O que é rescisão indireta e como comprovar?
          <span class="arrow">&#9654;</span>
        </div>
        <div class="faq-answer">
          <p>Rescisão indireta ocorre quando o trabalhador encerra o contrato devido a faltas graves do empregador, como atraso de salários ou condições degradantes. É necessário comprovar as faltas em juízo ou órgão competente.</p>
        </div>
      </div>

      <div class="faq-item">
        <div class="faq-question" tabindex="0">
          O que fazer se a empresa não pagar as verbas rescisórias?
          <span class="arrow">&#9654;</span>
        </div>
        <div class="faq-answer">
          <p>Procure o sindicato da sua categoria ou uma assistência jurídica trabalhista para orientações e eventuais ações legais para garantir seus direitos.</p>
        </div>
      </div>

    </section>

    <section id="contato">
      <h2>Contatos Úteis e Orientações</h2>
      <p>Se estiver passando por dúvidas ou dificuldades na rescisão trabalhista, utilize estes canais de ajuda:</p>
      <ul>
        <li><strong>Sindicatos:</strong> Procure o sindicato da sua categoria para orientação e suporte.</li>
        <li><strong>Ministério do Trabalho:</strong> Site oficial: <a href="https://www.gov.br/trabalho" target="_blank" rel="noopener">gov.br/trabalho</a></li>
        <li><strong>Justiça do Trabalho:</strong> Para demandas jurídicas relacionadas ao trabalho.</li>
        <li><strong>Centros de Referência:</strong> Centros de assistência social e jurídica do seu município.</li>
      </ul>
      <p>Não deixe seus direitos de lado. Informar-se é o primeiro passo para garantir uma rescisão justa e segura.</p>
    </section>
  </main>
</div>
<footer style="text-align:center; padding: 1rem 0; font-size: 0.9rem; color: #666;">
  Projeto Integrador – Curso de Direito – Centro Universitário da Região da Campanha – URCAMP © 2025
</footer>

<script>
  // Navegação ativa
  const navLinks = document.querySelectorAll('nav a');
  const sections = [...document.querySelectorAll('main section')];
  function changeActiveLink() {
    const scrollPos = window.scrollY || window.pageYOffset;
    let currentSectionId = sections[0].id;
    for (const section of sections) {
      if (section.offsetTop - 80 <= scrollPos) {
        currentSectionId = section.id;
      }
    }
    navLinks.forEach(link => {
      link.classList.toggle('active', link.getAttribute('href') === '#' + currentSectionId);
    });
  }
  window.addEventListener('scroll', changeActiveLink);

  // Accordion functionality
  function setupAccordion(containerSelector, headerSelector, contentSelector) {
    const containers = document.querySelectorAll(containerSelector);
    containers.forEach(container => {
      const header = container.querySelector(headerSelector);
      const content = container.querySelector(contentSelector);
      header.addEventListener('click', () => {
        const expanded = header.classList.contains('active');
        if (expanded) {
          content.classList.remove('active');
          header.classList.remove('active');
        } else {
          content.classList.add('active');
          header.classList.add('active');
        }
      });
      header.addEventListener('keydown', (e) => {
        if (e.key === 'Enter' || e.key === ' ') {
          e.preventDefault();
          header.click();
        }
      });
    });
  }
  setupAccordion('.accordion', '.accordion-header', '.accordion-content');
  setupAccordion('.faq-item', '.faq-question', '.faq-answer');

  // Search functionality
  const searchInput = document.getElementById('searchInput');
  searchInput.addEventListener('input', () => {
    const filter = searchInput.value.toLowerCase();
    // Sections to filter inside main
    const filterableSections = ['tipos-rescisao', 'direitos', 'procedimentos', 'faq', 'contato'];
    filterableSections.forEach(id => {
      const section = document.getElementById(id);
      if (!section) return;
      let text = section.textContent.toLowerCase();
      // Show or hide based on text match
      section.style.display = text.includes(filter) ? 'block' : 'none';
    });
  });
</script>
</body>
</html>

