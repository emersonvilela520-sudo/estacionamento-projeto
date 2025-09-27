<!--
  Arquivo: estacionamento_vertical_automatizado.html
  Uso: renomeie para index.html e coloque na raiz do seu repositório GitHub Pages (ou em /docs) para publicar o site.
-->
<!doctype html>
<html lang="pt-BR">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Estacionamento Vertical Automatizado — Colégio Pentágono</title>
  <meta name="description" content="Projeto de Estacionamento Vertical Automatizado — Curso Técnico em Mecatrônica, Colégio Pentágono.">
  <style>
    :root{--bg:#f7f8fb;--card:#fff;--accent:#0b63d6;--muted:#6b7280;--maxw:1000px}
    *{box-sizing:border-box}
    body{font-family:Inter, Roboto, system-ui, -apple-system, "Segoe UI", Arial;line-height:1.5;margin:0;background:var(--bg);color:#111}
    .container{max-width:var(--maxw);margin:32px auto;padding:20px}
    header{display:flex;gap:16px;align-items:center}
    .brand{display:flex;flex-direction:column}
    h1{margin:0;font-size:1.6rem}
    .subtitle{color:var(--muted);font-size:0.95rem}
    .card{background:var(--card);padding:20px;border-radius:12px;box-shadow:0 6px 18px rgba(12,18,35,0.06);margin-top:18px}
    nav{display:flex;gap:12px;flex-wrap:wrap;margin-top:12px}
    nav a{color:var(--accent);text-decoration:none;border:1px solid transparent;padding:8px 10px;border-radius:8px}
    nav a:hover{background:rgba(11,99,214,0.07)}
    .grid{display:grid;grid-template-columns:1fr;gap:18px;margin-top:14px}
    .section h2{margin-top:0}
    .meta{font-size:0.95rem;color:var(--muted);margin-bottom:8px}
    ul.team{padding-left:1rem}
    footer{margin-top:26px;text-align:center;color:var(--muted);font-size:0.9rem}
    @media(max-width:900px){.grid{grid-template-columns:1fr}}
    code{background:#f3f4f6;padding:2px 6px;border-radius:6px;font-family:monospace}
    img{max-width:100%;border-radius:8px}
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div style="width:72px;height:72px;border-radius:10px;background:linear-gradient(135deg,#0b63d6,#7bb3ff);display:flex;align-items:center;justify-content:center;color:#fff;font-weight:700;font-size:20px">CP</div>
      <div class="brand">
        <h1>Estacionamento Vertical Automatizado</h1>
        <div class="subtitle">Colégio Pentágono — Curso Técnico em Mecatrônica · Ano 2025</div>
      </div>
    </header>

    <div class="card">
      <div style="display:flex;justify-content:space-between;align-items:start;gap:18px;flex-wrap:wrap">
        <div>
          <div class="meta">Sala 507 – 1º, 2º e 3º Semestre · Noturno</div>
          <p style="margin:6px 0 12px">Resumo: O presente trabalho apresenta o desenvolvimento de um sistema de Estacionamento Vertical Automatizado, passando por protótipo mecânico e integração com Arduino e sensores.</p>
          <div style="font-weight:600;margin-bottom:6px">Integrantes</div>
          <ul class="team">
            <li>Diego Nascimento</li>
            <li>Emerson Moreira Vilela</li>
            <li>Gabriel Alves Lôredo</li>
            <li>Marco Antonio Da Silva Ribeiro</li>
            <li>Samuel Pereira Bezerra</li>
          </ul>
        </div>
        <div style="min-width:220px;max-width:320px">
          <img src="assets/foto_prototipo.png" alt="Protótipo do Estacionamento Vertical Automatizado"/>
          <div style="font-size:0.85rem;color:var(--muted);margin-top:8px">Ano 2025</div>
        </div>
      </div>
    </div>

    <nav class="card" aria-label="Sumário">
      <strong>Sumário</strong>
      <a href="#introducao">1. Introdução</a>
      <a href="#objetivo">2. Objetivo</a>
      <a href="#desenvolvimento">3. Desenvolvimento</a>
      <a href="#resultados">4. Resultados</a>
      <a href="#conclusao">5. Conclusão</a>
      <a href="#referencias">6. Referências</a>
    </nav>

    <main>
      <article class="card section" id="introducao">
        <h2>1. Introdução</h2>
        <p>O projeto de Estacionamento Vertical Automatizado teve início no primeiro semestre com a construção de um protótipo mecânico de elevação baseado em motor de vidro elétrico, fuso e guias lineares. Essa primeira etapa permitiu validar a viabilidade estrutural e a eficiência mecânica do sistema.</p>
        <p>No segundo semestre, a proposta foi expandida com a integração de componentes eletrônicos e programação utilizando Arduino, ponte H e sensores de detecção, transformando o protótipo em um modelo automatizado com aplicabilidade em sistemas reais.</p>
      </article>

      <article class="card section" id="objetivo">
        <h2>2. Objetivo</h2>
        <p>O objetivo deste trabalho é desenvolver e implementar um protótipo de Estacionamento Vertical Automatizado, integrando soluções mecânicas e eletrônicas, de forma a oferecer eficiência, segurança e escalabilidade. Também busca proporcionar experiência prática aos alunos.</p>
      </article>

      <article class="card section" id="desenvolvimento">
        <h2>3. Desenvolvimento</h2>

        <section id="estrutura">
          <h3>3.1 Estrutura Mecânica</h3>
          <p>Foi construído um sistema de elevação utilizando motor de vidro elétrico, perfil de alumínio, acrílico, fuso de 8 mm, mancais e guias lineares. Essa estrutura garantiu estabilidade e precisão no movimento da plataforma.</p>
          <img src="assets/estrutura.png" alt="Estrutura Mecânica do protótipo"/>
        </section>

        <section id="integracao">
          <h3>3.2 Integração Eletrônica</h3>
          <p>Implementou-se a automação utilizando Arduino Uno como unidade de controle, ponte H para inversão de polaridade e sensores infravermelhos para detecção de limites de curso. O controle bidirecional do motor e as paradas automáticas aumentaram a segurança.</p>
          <img src="assets/arduino.png" alt="Integração Eletrônica com Arduino e sensores"/>
        </section>

        <section id="desafios">
          <h3>3.3 Desafios Encontrados</h3>
          <p>Foram enfrentadas dificuldades na programação do Arduino, alinhamento da maquete e restrição de tempo, exigindo desmontagens e substituições de componentes para alcançar precisão e estabilidade.</p>
        </section>

        <section id="diagrama">
          <h3>3.4 Diagrama de Funcionamento</h3>
          <img src="assets/diagrama.png" alt="Diagrama de Funcionamento do Estacionamento Automatizado"/>
        </section>
      </article>

      <article class="card section" id="resultados">
        <h2>4. Resultados</h2>
        <p>O sistema apresentou movimentação vertical e transversal funcionais, paradas automáticas controladas por sensores IR e gerenciamento via Arduino. O protótipo é base para futuras expansões.</p>
      </article>

      <article class="card section" id="conclusao">
        <h2>5. Conclusão</h2>
        <p>O projeto demonstrou a eficácia da integração entre mecânica, eletrônica e programação, evoluindo de uma estrutura mecânica para um sistema automatizado capaz de simular aplicações reais de automação predial.</p>
      </article>

      <article class="card section" id="referencias">
        <h2>6. Referências</h2>
        <ol>
          <li>BOLTON, W. Mecatrônica: sistemas de controle eletromecânico. 5.ed. São Paulo: Pearson, 2015.</li>
          <li>OGATA, Katsuhiko. Engenharia de Controle Moderno. 5.ed. São Paulo: Pearson, 2010.</li>
          <li>SUNFAR. Manual do Inversor de Frequência E550. Sunfar, 2023.</li>
          <li>Material e anotações das aulas do Curso Técnico em Mecatrônica – Colégio Pentágono, 2024-2025.</li>
        </ol>
      </article>
    </main>

    <footer>
      Criado automaticamente a partir do PDF fornecido — Colégio Pentágono · 2025
    </footer>
  </div>
</body>
</html>