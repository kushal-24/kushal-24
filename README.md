<div align="center">

<!-- ═══════════════════════════════════════════════════
     ANIMATED SVG BANNER
════════════════════════════════════════════════════ -->

<svg width="100%" height="280" viewBox="0 0 900 280" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <!-- Background gradient -->
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#07060f"/>
      <stop offset="100%" style="stop-color:#0d0b1a"/>
    </linearGradient>

    <!-- Purple blob gradient -->
    <radialGradient id="blob1" cx="80%" cy="20%" r="55%">
      <stop offset="0%" style="stop-color:#5b35cc;stop-opacity:0.55"/>
      <stop offset="55%" style="stop-color:#2d1a66;stop-opacity:0.3"/>
      <stop offset="100%" style="stop-color:#07060f;stop-opacity:0"/>
    </radialGradient>
    <radialGradient id="blob2" cx="15%" cy="80%" r="35%">
      <stop offset="0%" style="stop-color:#6366f1;stop-opacity:0.2"/>
      <stop offset="100%" style="stop-color:#07060f;stop-opacity:0"/>
    </radialGradient>
    <radialGradient id="blob3" cx="55%" cy="90%" r="30%">
      <stop offset="0%" style="stop-color:#c084fc;stop-opacity:0.18"/>
      <stop offset="100%" style="stop-color:#07060f;stop-opacity:0"/>
    </radialGradient>

    <!-- Name text gradient -->
    <linearGradient id="nameGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#ffffff"/>
      <stop offset="45%" style="stop-color:#d4c8ff"/>
      <stop offset="100%" style="stop-color:#8a61ff"/>
    </linearGradient>

    <!-- Glow filter -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
      <feGaussianBlur stdDeviation="3" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <filter id="softglow" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="6" result="coloredBlur"/>
      <feMerge>
        <feMergeNode in="coloredBlur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Grid pattern -->
    <pattern id="grid" width="48" height="48" patternUnits="userSpaceOnUse">
      <path d="M 48 0 L 0 0 0 48" fill="none" stroke="rgba(138,97,255,0.06)" stroke-width="0.5"/>
    </pattern>

    <!-- Clip path -->
    <clipPath id="bannerClip">
      <rect width="900" height="280" rx="12"/>
    </clipPath>
  </defs>

  <g clip-path="url(#bannerClip)">
    <!-- Base -->
    <rect width="900" height="280" fill="url(#bgGrad)" rx="12"/>

    <!-- Blobs -->
    <rect width="900" height="280" fill="url(#blob1)"/>
    <rect width="900" height="280" fill="url(#blob2)"/>
    <rect width="900" height="280" fill="url(#blob3)"/>

    <!-- Grid -->
    <rect width="900" height="280" fill="url(#grid)" opacity="0.6"/>

    <!-- Scanlines -->
    <rect width="900" height="280" fill="none"
      style="fill:url(#scanlines)" opacity="0.04"/>

    <!-- ─── Decorative corner brackets ─── -->
    <!-- TL -->
    <polyline points="20,40 20,20 40,20" fill="none" stroke="#8a61ff" stroke-width="1.5" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.9;0.5" dur="3s" repeatCount="indefinite"/>
    </polyline>
    <!-- TR -->
    <polyline points="860,20 880,20 880,40" fill="none" stroke="#8a61ff" stroke-width="1.5" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.9;0.5" dur="3s" begin="0.5s" repeatCount="indefinite"/>
    </polyline>
    <!-- BL -->
    <polyline points="20,240 20,260 40,260" fill="none" stroke="#8a61ff" stroke-width="1.5" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.9;0.5" dur="3s" begin="1s" repeatCount="indefinite"/>
    </polyline>
    <!-- BR -->
    <polyline points="860,260 880,260 880,240" fill="none" stroke="#8a61ff" stroke-width="1.5" opacity="0.5">
      <animate attributeName="opacity" values="0.5;0.9;0.5" dur="3s" begin="1.5s" repeatCount="indefinite"/>
    </polyline>

    <!-- Ghost/shadow name -->
    <text x="453" y="168" text-anchor="middle"
      font-family="'Arial Black', Arial, sans-serif"
      font-size="118" font-weight="900" letter-spacing="22"
      fill="none" stroke="rgba(138,97,255,0.08)" stroke-width="1">
      NISARG
    </text>

    <!-- Main name with gradient -->
    <text x="450" y="162" text-anchor="middle"
      font-family="'Arial Black', Arial, sans-serif"
      font-size="118" font-weight="900" letter-spacing="22"
      fill="url(#nameGrad)" filter="url(#glow)">
      <animate attributeName="opacity" values="1;0.88;1;0.92;1" dur="6s" repeatCount="indefinite"/>
      NISARG
    </text>

    <!-- Decorative line under name -->
    <line x1="200" y1="182" x2="700" y2="182" stroke="url(#lineGrad)" stroke-width="1" opacity="0.7">
      <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="x1" values="250;200;250" dur="3s" repeatCount="indefinite"/>
      <animate attributeName="x2" values="650;700;650" dur="3s" repeatCount="indefinite"/>
    </line>
    <defs>
      <linearGradient id="lineGrad" x1="0%" y1="0%" x2="100%" y2="0%">
        <stop offset="0%" style="stop-color:transparent"/>
        <stop offset="30%" style="stop-color:#8a61ff"/>
        <stop offset="70%" style="stop-color:#c084fc"/>
        <stop offset="100%" style="stop-color:transparent"/>
      </linearGradient>
    </defs>

    <!-- Roles row -->
    <!-- Dot 1 -->
    <circle cx="234" cy="212" r="3" fill="#b89cff">
      <animate attributeName="r" values="3;4.5;3" dur="2s" repeatCount="indefinite"/>
      <animate attributeName="opacity" values="1;0.5;1" dur="2s" repeatCount="indefinite"/>
    </circle>
    <text x="252" y="217" font-family="Arial, sans-serif" font-size="12"
      font-weight="400" fill="rgba(238,234,248,0.7)" letter-spacing="3">Developer</text>

    <!-- Sep dot 1 -->
    <circle cx="352" cy="212" r="2.5" fill="#8a61ff" opacity="0.8"/>

    <text x="367" y="217" font-family="Arial, sans-serif" font-size="12"
      font-weight="400" fill="rgba(238,234,248,0.7)" letter-spacing="3">Hackathon Enthusiast</text>

    <!-- Sep dot 2 -->
    <circle cx="590" cy="212" r="2.5" fill="#8a61ff" opacity="0.8"/>

    <text x="605" y="217" font-family="Arial, sans-serif" font-size="12"
      font-weight="400" fill="rgba(238,234,248,0.7)" letter-spacing="3">Video Editor</text>

    <!-- Pulsing ambient dots -->
    <circle cx="60" cy="60" r="1.5" fill="#8a61ff" opacity="0.4">
      <animate attributeName="opacity" values="0.4;0.9;0.4" dur="4s" repeatCount="indefinite"/>
    </circle>
    <circle cx="840" cy="200" r="1.5" fill="#c084fc" opacity="0.4">
      <animate attributeName="opacity" values="0.4;0.9;0.4" dur="4s" begin="1s" repeatCount="indefinite"/>
    </circle>
    <circle cx="120" cy="230" r="1" fill="#6366f1" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" begin="2s" repeatCount="indefinite"/>
    </circle>
    <circle cx="780" cy="50" r="1" fill="#b89cff" opacity="0.5">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="3s" begin="0.5s" repeatCount="indefinite"/>
    </circle>
  </g>
</svg>

<br/>

<!-- ═══════════════════════════════════════════════════
     TYPEWRITER — readme-typing-svg
════════════════════════════════════════════════════ -->

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Space+Mono&size=16&duration=3000&pause=800&color=8A61FF&center=true&vCenter=true&multiline=false&width=600&lines=Building+things+that+matter+%E2%9C%A6;Shipping+at+hackathon+speed+%E2%9A%A1;Turning+wild+ideas+into+reality+%F0%9F%9A%80;TypeScript+by+day%2C+dreams+by+night+%F0%9F%8C%99;Code.+Create.+Compete.+Repeat.)](https://git.io/typing-svg)

<br/>

<!-- ═══════════════════════════════════════════════════
     MISSION CONTROL — GITHUB STATS
════════════════════════════════════════════════════ -->

### 🛸 &nbsp;`MISSION CONTROL — GITHUB STATS`

<br/>

<a href="https://github.com/code-nisarg">
  <img height="180em" src="https://github-readme-stats.vercel.app/api?username=code-nisarg&show_icons=true&theme=transparent&hide_border=true&title_color=8a61ff&icon_color=c084fc&text_color=d4c8ff&bg_color=0d0b1a&ring_color=8a61ff&include_all_commits=true&count_private=true"/>
</a>
<a href="https://github.com/code-nisarg">
  <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=code-nisarg&layout=compact&theme=transparent&hide_border=true&title_color=8a61ff&text_color=d4c8ff&bg_color=0d0b1a&langs_count=6"/>
</a>

<br/><br/>

<a href="https://git.io/streak-stats">
  <img src="https://streak-stats.demolab.com?user=code-nisarg&theme=transparent&hide_border=true&ring=8a61ff&fire=c084fc&currStreakLabel=b89cff&sideLabels=8a61ff&dates=7068a0&currStreakNum=d4c8ff&sideNums=d4c8ff&background=0d0b1a&stroke=1a1630"/>
</a>

<br/><br/>

<!-- ═══════════════════════════════════════════════════
     ACTIVITY GRAPH
════════════════════════════════════════════════════ -->

### 📈 &nbsp;`ACTIVITY GRAPH`

<br/>

[![Nisarg's github activity graph](https://github-readme-activity-graph.vercel.app/graph?username=code-nisarg&bg_color=0d0b1a&color=b89cff&line=8a61ff&point=c084fc&area=true&area_color=8a61ff&hide_border=true&title_color=8a61ff)](https://github.com/ashutosh00710/github-readme-activity-graph)

<br/>

<!-- ═══════════════════════════════════════════════════
     TECH STACK
════════════════════════════════════════════════════ -->

### ⚡ &nbsp;`TECH STACK`

<br/>

**Languages**

![JavaScript](https://img.shields.io/badge/JavaScript-07060f?style=for-the-badge&logo=javascript&logoColor=f1e05a&labelColor=0d0b1a&color=1a1630)
![TypeScript](https://img.shields.io/badge/TypeScript-07060f?style=for-the-badge&logo=typescript&logoColor=3178c6&labelColor=0d0b1a&color=1a1630)
![Python](https://img.shields.io/badge/Python-07060f?style=for-the-badge&logo=python&logoColor=c084fc&labelColor=0d0b1a&color=1a1630)
![C++](https://img.shields.io/badge/C++-07060f?style=for-the-badge&logo=cplusplus&logoColor=8a61ff&labelColor=0d0b1a&color=1a1630)

<br/>

**Frontend**

![React](https://img.shields.io/badge/React-07060f?style=for-the-badge&logo=react&logoColor=61dafb&labelColor=0d0b1a&color=1a1630)
![Next.js](https://img.shields.io/badge/Next.js-07060f?style=for-the-badge&logo=next.js&logoColor=ffffff&labelColor=0d0b1a&color=1a1630)
![TailwindCSS](https://img.shields.io/badge/Tailwind-07060f?style=for-the-badge&logo=tailwindcss&logoColor=38bdf8&labelColor=0d0b1a&color=1a1630)
![Figma](https://img.shields.io/badge/Figma-07060f?style=for-the-badge&logo=figma&logoColor=c084fc&labelColor=0d0b1a&color=1a1630)

<br/>

**Backend & Tools**

![Node.js](https://img.shields.io/badge/Node.js-07060f?style=for-the-badge&logo=node.js&logoColor=6dbf67&labelColor=0d0b1a&color=1a1630)
![Docker](https://img.shields.io/badge/Docker-07060f?style=for-the-badge&logo=docker&logoColor=2496ed&labelColor=0d0b1a&color=1a1630)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-07060f?style=for-the-badge&logo=postgresql&logoColor=336791&labelColor=0d0b1a&color=1a1630)
![Git](https://img.shields.io/badge/Git-07060f?style=for-the-badge&logo=git&logoColor=f05032&labelColor=0d0b1a&color=1a1630)
![GitHub](https://img.shields.io/badge/GitHub-07060f?style=for-the-badge&logo=github&logoColor=b89cff&labelColor=0d0b1a&color=1a1630)
![VS Code](https://img.shields.io/badge/VS_Code-07060f?style=for-the-badge&logo=visualstudiocode&logoColor=007acc&labelColor=0d0b1a&color=1a1630)

<br/>

**Video & Creative**

![Premiere Pro](https://img.shields.io/badge/Premiere_Pro-07060f?style=for-the-badge&logo=adobepremierepro&logoColor=9999ff&labelColor=0d0b1a&color=1a1630)
![After Effects](https://img.shields.io/badge/After_Effects-07060f?style=for-the-badge&logo=adobeaftereffects&logoColor=c084fc&labelColor=0d0b1a&color=1a1630)

<br/>

<!-- ═══════════════════════════════════════════════════
     PROFILE VIEWS + FOOTER
════════════════════════════════════════════════════ -->

---

![Profile Views](https://komarev.com/ghpvc/?username=code-nisarg&style=for-the-badge&color=8a61ff&labelColor=0d0b1a&label=PROFILE+VIEWS)

<br/>

*Built with 💜 and way too many late nights*

</div>
