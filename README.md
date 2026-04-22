<div align="center">
  <!-- CABEÇALHO COM ÓRBITAS ANIMADAS E NOME GLOW -->
  <svg width="800" height="220" viewBox="0 0 800 220" xmlns="http://www.w3.org/2000/svg">
    <defs>
      <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" stop-color="#ffffff" />
        <stop offset="40%" stop-color="#5dade2" />
        <stop offset="100%" stop-color="#2ecc71" />
      </linearGradient>
      <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
        <feGaussianBlur in="SourceAlpha" stdDeviation="3" />
        <feMerge>
          <feMergeNode in="offsetblur" />
          <feMergeNode in="SourceGraphic" />
        </feMerge>
      </filter>
    </defs>

    <!-- Fundo escuro -->
    <rect width="800" height="220" fill="#0a0f1a" rx="20" />

    <!-- Círculo orbital externo (animado) -->
    <circle cx="400" cy="110" r="85" stroke="#3498db" stroke-width="2" stroke-dasharray="10 6" fill="none" opacity="0.8">
      <animateTransform attributeName="transform" type="rotate" from="0 400 110" to="360 400 110" dur="25s" repeatCount="indefinite" />
    </circle>

    <!-- Círculo orbital interno (rotação inversa) -->
    <circle cx="400" cy="110" r="60" stroke="#2ecc71" stroke-width="1.5" stroke-dasharray="5 8" fill="none" opacity="0.6">
      <animateTransform attributeName="transform" type="rotate" from="360 400 110" to="0 400 110" dur="18s" repeatCount="indefinite" />
    </circle>

    <!-- Partículas orbitando -->
    <circle cx="315" cy="110" r="4" fill="#2ecc71">
      <animateTransform attributeName="transform" type="rotate" from="0 400 110" to="360 400 110" dur="25s" repeatCount="indefinite" />
      <animate attributeName="opacity" values="0.3;1;0.3" dur="2s" repeatCount="indefinite" />
    </circle>
    <circle cx="485" cy="110" r="3" fill="#3498db">
      <animateTransform attributeName="transform" type="rotate" from="0 400 110" to="360 400 110" dur="25s" repeatCount="indefinite" />
      <animate attributeName="r" values="2;5;2" dur="3s" repeatCount="indefinite" />
    </circle>

    <!-- Nome principal com gradiente e glow -->
    <text x="400" y="100" text-anchor="middle" font-family="'Segoe UI', Ubuntu, sans-serif" font-size="44" font-weight="900" fill="url(#nameGrad)" filter="url(#glow)" letter-spacing="3">ALISSON SORGATTO</text>

    <!-- Subtítulo com linha decorativa -->
    <text x="400" y="140" text-anchor="middle" font-family="'Segoe UI', Ubuntu, sans-serif" font-size="18" fill="#4cc9f0" letter-spacing="5" font-weight="500">ARQUITETO FULL STACK & MOBILE</text>

    <!-- Estrelas estáticas -->
    <circle cx="120" cy="40" r="1.5" fill="#fff" opacity="0.7" />
    <circle cx="680" cy="60" r="2" fill="#fff" opacity="0.5" />
    <circle cx="60" cy="180" r="1" fill="#fff" opacity="0.6" />
    <circle cx="740" cy="190" r="1.5" fill="#fff" opacity="0.8" />
    <circle cx="250" cy="30" r="1" fill="#fff" opacity="0.4" />
    <circle cx="550" cy="200" r="1.2" fill="#fff" opacity="0.5" />
  </svg>
</div>

<br />

<!-- SOBRE MIM COM ESTILO CÓSMICO -->
<div align="center">
  <table border="0" cellpadding="10" style="background: linear-gradient(135deg, #0f172a, #020617); border-radius: 30px; border: 1px solid #2ecc71; max-width: 800px;">
    <tr>
      <td align="center">
        <h3>✨ <strong>Sobre este arquiteto</strong> ✨</h3>
        <p>
          👨‍🚀 <strong>Alisson Sorgatto</strong> – Desenvolvedor apaixonado por <strong>código, futebol e inovação</strong>.<br>
          🚀 Especialista em <strong>React Native, Expo, Node.js e MongoDB</strong>.<br>
          🎮 Criador do <strong>Projeto Galaxy: FUT+</strong> – plataforma que une gestão esportiva e transmissões ao vivo.<br>
          ⚡ Vivo para transformar ideias em soluções que conectam pessoas e tecnologia.
        </p>
      </td>
    </tr>
  </table>
</div>

<br />

<!-- TECH STACK COM ÍCONES CUSTOMIZADOS E ANIMAÇÃO SUTIL -->
<div align="center">
  <h2>🛸 <strong>Constelação Tecnológica</strong> 🛸</h2>
  <table>
    <tr>
      <td align="center" width="50%">
        <h3>🚀 Front-end & Mobile</h3>
        <img src="https://skillicons.dev/icons?i=react,expo,ts,js,tailwind" />
      </td>
      <td align="center" width="50%">
        <h3>⚙️ Back-end & Banco</h3>
        <img src="https://skillicons.dev/icons?i=nodejs,express,mongodb,postgresql" />
      </td>
    </tr>
    <tr>
      <td align="center">
        <h3>🎥 Live Ops & Hardware</h3>
        <img src="https://skillicons.dev/icons?i=obs,arduino,raspberrypi,linux" />
      </td>
      <td align="center">
        <h3>🔧 Ferramentas & DevOps</h3>
        <img src="https://skillicons.dev/icons?i=git,github,docker,vscode" />
      </td>
    </tr>
  </table>
</div>

<br />

<!-- PROJETO DESTAQUE COM BADGES E SVG PERSONALIZADO -->
<div align="center">
  <svg width="90%" height="120" viewBox="0 0 700 120" xmlns="http://www.w3.org/2000/svg">
    <rect width="700" height="120" rx="25" fill="#0f212e" stroke="#2ecc71" stroke-width="2" />
    <text x="30" y="45" font-family="'Segoe UI', sans-serif" font-size="22" font-weight="bold" fill="#2ecc71">⚽ PROJETO GALAXY: FUT+</text>
    <text x="30" y="75" font-family="'Segoe UI', sans-serif" font-size="15" fill="#b0c4de">Plataforma completa de gestão esportiva e transmissões ao vivo.</text>
    <text x="30" y="98" font-family="'Segoe UI', sans-serif" font-size="13" fill="#7f8c8d">📱 Mobile · 🕹️ Overlay · 📊 Analytics · 🏆 Gamificação</text>
    <!-- Logo de foguete pequeno -->
    <text x="640" y="65" font-size="35">🚀</text>
  </svg>
</div>

<br />

<!-- ESTATÍSTICAS DO GITHUB COM DESIGN UNIFICADO -->
<div align="center">
  <h2>📡 <strong>Telemetria do Código</strong> 📡</h2>
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=alissonfutplus&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0a0f1a&title_color=4cc9f0&icon_color=2ecc71&text_color=ffffff" />
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=alissonfutplus&layout=compact&theme=tokyonight&hide_border=true&bg_color=0a0f1a&title_color=4cc9f0&text_color=ffffff" />
</div>

<br />

<!-- REDES SOCIAIS COM BOTÕES PERSONALIZADOS (IMAGENS LOCAIS? USAR BADGES) -->
<div align="center">
  <h2>🌌 <strong>Órbita Social</strong> 🌌</h2>
  <a href="https://www.linkedin.com/in/alisson-sorgatto-3a0136204" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" />
  </a>
  <a href="https://instagram.com/Alisson_Sorgatto98" target="_blank">
    <img src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white" />
  </a>
  <a href="mailto:alisson@futplus.com">
    <img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" />
  </a>
</div>

<br />

<!-- RODAPÉ COM ANIMAÇÃO DE ONDA E TEXTO CRIATIVO -->
<div align="center">
  <svg width="100%" height="70" viewBox="0 0 1200 120" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M0,64L80,58.7C160,53,320,43,480,48C640,53,800,75,960,80C1120,85,1280,75,1360,69.3L1440,64L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z" fill="#0d2b3e" fill-opacity="0.9"></path>
    <path d="M0,96L80,90.7C160,85,320,75,480,80C640,85,800,107,960,106.7C1120,107,1280,96,1360,90.7L1440,85L1440,120L1360,120C1280,120,1120,120,960,120C800,120,640,120,480,120C320,120,160,120,80,120L0,120Z" fill="#05161f" fill-opacity="0.7"></path>
  </svg>
  <p><strong>“Construindo o futuro, um commit por vez”</strong> 🚀✨</p>
</div>
