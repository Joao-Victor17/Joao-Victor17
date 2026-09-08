<!-- ============================================================ -->
<!-- 1. TERMINAL IBN 5100 (SVG DINÂMICO EMBUTIDO VIA DATA URI)   -->
<!-- Demonstra como rodar CSS moderno, scanlines e animação        -->
<!-- ============================================================ -->

<div align="center">
  <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 850 180' width='100%'>
    <defs>
      <linearGradient id='crtGrad' x1='0%25' y1='0%25' x2='0%25' y2='100%25'>
        <stop offset='0%25' stop-color='%23121512'/>
        <stop offset='100%25' stop-color='%23080a08'/>
      </linearGradient>
      <pattern id='scanlines' width='100' height='4' patternUnits='userSpaceOnUse'>
        <line x1='0' y1='0' x2='100' y2='0' stroke='%23000' stroke-width='1.2' opacity='0.35'/>
      </pattern>
    </defs>
    <style>
      @keyframes blink { 0%25, 49%25 { opacity: 1; } 50%25, 100%25 { opacity: 0; } }
      @keyframes phosphorGlow {
        0%25 { text-shadow: 0 0 3px %2333ff33, 0 0 8px %2333ff3388; }
        50%25 { text-shadow: 0 0 6px %2333ff33, 0 0 14px %2333ff33aa; }
        100%25 { text-shadow: 0 0 3px %2333ff33, 0 0 8px %2333ff3388; }
      }
      .crt-bg { fill: url(%23crtGrad); stroke: %232d382d; stroke-width: 2; rx: 8; }
      .term-text { font-family: 'Courier New', monospace; font-size: 14px; fill: %2339ff14; animation: phosphorGlow 3s infinite; }
      .cursor { fill: %2339ff14; animation: blink 0.8s infinite; }
      .accent { fill: %23ffaa00; font-weight: bold; }
    </style>
    <rect width='100%25' height='100%25' class='crt-bg'/>
    <rect width='100%25' height='100%25' fill='url(%23scanlines)' pointer-events='none'/>
    
    <text x='25' y='38' class='term-text'>IBN-5100 [ROUTINE: INITIALIZING LAB BOOTSTRAP...]</text>
    <text x='25' y='68' class='term-text'>OPERATOR: <tspan class='accent'>LAB MEMBER 001</tspan> | SYSTEM STATUS: ONLINE</text>
    <text x='25' y='98' class='term-text'>CURRENT DIRECTIVE: Full-stack Development &amp; Architecture</text>
    <text x='25' y='128' class='term-text'>CONNECTED TO SERN ARCHIVE... DECRYPTION KEY ACCEPTED</text>
    <text x='25' y='155' class='term-text'>EXECUTE: <tspan fill='%23ffffff'>./explore_worldlines.sh</tspan></text>
    <rect x='280' y='142' width='9' height='15' class='cursor'/>
  </svg>" alt="Terminal IBN 5100" />
</div>

<br>

<!-- ============================================================ -->
<!-- 2. LAYOUT LADO A LADO: BIO E MEDIDOR DE DIVERGÊNCIA (TABELA) -->
<!-- Tabelas são usadas como grid para contornar a falta de CSS   -->
<!-- ============================================================ -->

<table>
  <tr>
    <td width="65%" valign="top">
      <h3>📟 Transmissão Inicial</h3>
      <p>
        Engenheiro de Software focado em construir sistemas escaláveis e ferramentas analíticas. 
        Explorando arquiteturas distribuídas, microsserviços e computação na borda.
      </p>
      <p>
        Atualmente iterando entre diferentes camadas de abstração para decifrar a linha do tempo ideal.
      </p>
      <p>
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
        <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
        <img src="https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white" />
      </p>
    </td>
    <td width="35%" align="center" valign="middle">
      <!-- Medidor de Divergência Simulado em SVG (Nixie Display) -->
      <img src="data:image/svg+xml;utf8,<svg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 260 140' width='100%'>
        <style>
          @keyframes nixieFlicker {
            0%25 { opacity: 0.95; } 50%25 { opacity: 0.85; } 70%25 { opacity: 1; } 100%25 { opacity: 0.92; }
          }
          .meter-box { fill: %231a1510; stroke: %238c531b; stroke-width: 2; rx: 6; }
          .label { font-family: monospace; font-size: 10px; fill: %23a87944; letter-spacing: 1.5px; }
          .nixie-digits {
            font-family: 'Courier New', monospace; font-size: 26px; font-weight: bold;
            fill: %23ff7700; text-shadow: 0 0 6px %23ff5500, 0 0 12px %23ff2200;
            animation: nixieFlicker 0.15s infinite alternate;
          }
        </style>
        <rect width='100%25' height='100%25' class='meter-box'/>
        <text x='50%25' y='32' text-anchor='middle' class='label'>DIVERGENCE METER</text>
        <rect x='15' y='45' width='230' height='55' rx='4' fill='%23000' stroke='%2338240f'/>
        <text x='50%25' y='83' text-anchor='middle' class='nixie-digits'>1.048596%</text>
        <text x='50%25' y='122' text-anchor='middle' class='label'>STATUS: STABLE</text>
      </svg>" alt="Divergence Meter" />
    </td>
  </tr>
</table>

---

<!-- ============================================================ -->
<!-- 3. SELETOR DE LINHAS DO TEMPO (ACCORDION NATIVO COM NAME)     -->
<!-- O atributo 'name' força apenas uma aba aberta de cada vez     -->
<!-- ============================================================ -->

### ⏱️ Seletor de Linha do Tempo (World Lines)

<details name="timeline" open>
  <summary><b>[ Linha 1.048596% - Steins;Gate (Stack & Produção) ]</b></summary>
  <br>
  <blockquote>
    <b>Diretiva Atual:</b> Construção de aplicações modernas, APIs desacopladas e microsserviços de alta disponibilidade.
  </blockquote>
  <ul>
    <li><b>Backend:</b> Node.js, Python, Serverless Functions</li>
    <li><b>Cloud / Edge:</b> Vercel, Cloudflare Workers & Pages</li>
    <li><b>Bancos de Dados:</b> PostgreSQL, Redis</li>
  </ul>
</details>

<details name="timeline">
  <summary><b>[ Linha 0.571024% - Alpha (Sistemas & Baixo Nível) ]</b></summary>
  <br>
  <blockquote>
    <b>Ambiente Experimental:</b> Onde scripts de automação, manipulação direta de hardware e protocolos seriais residem.
  </blockquote>
  <ul>
    <li>Automação de workflows e rotinas de deploy</li>
    <li>Comunicação serial, microcontroladores e dispositivos embarcados</li>
    <li>Otimização de pipelines no GitHub Actions</li>
  </ul>
</details>

<details name="timeline">
  <summary><b>[ Linha 1.130205% - Beta (Algoritmos & Computação Analítica) ]</b></summary>
  <br>
  <blockquote>
    <b>Ambiente Teórico:</b> Foco em análise matemática, modelagem e resolução algorítmica.
  </blockquote>
  <ul>
    <li>Simulações estatísticas e processamento de dados brutos</li>
    <li>Modelagem física e computação científica</li>
    <li>Estruturas de dados complexas e otimização de consultas</li>
  </ul>
</details>

---

<!-- ============================================================ -->
<!-- 4. SUBMISSÃO DE D-MAIL VIA ISSUE TEMPLATE (SIMULAÇÃO)        -->
<!-- Links pré-parametrizados que abrem telas estruturadas         -->
<!-- ============================================================ -->

### 📱 Future Gadget Lab - Transmissão de D-Mail

Envie uma mensagem curta que atravessará o canal temporal do repositório:

[PhoneWave (name subject to change) - Ready for input]
Limite por pacote: 36 bytes (caracteres).

<a href="https://github.com/Joao-Victor17/Joao-Victor17/issues/new?title=%5BD-MAIL%5D+Transmiss%C3%A3o+Temporal&body=%23%23+Destino%3A+Passado%0A%23%23+Linha+Alvo%3A+Alpha%0A%0AMensagem+%28max+36+chars%29%3A%0A%3E+">
  <img src="https://img.shields.io/badge/Transmitir_D--Mail-E67E22?style=for-the-badge&logo=signal&logoColor=white" alt="Transmitir D-Mail" />
</a>

<br><br>

> *Atenção: O disparo de transmissões pode causar alterações retroativas no histórico de commits deste perfil devido ao efeito Reading Steiner.*
