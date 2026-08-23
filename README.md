<!DOCTYPE html><html><head><meta charset="utf-8"><style>
body{margin:0;background:#05050a;display:flex;flex-direction:column;align-items:center;font-family:sans-serif}
.wrap{margin:30px;box-shadow:0 20px 60px rgba(139,92,246,.3);border-radius:12px;overflow:hidden;max-width:1000px}
.wrap svg{display:block;width:100%;height:auto}
h3{color:#a78bfa}p{color:#666;max-width:800px;text-align:center}
</style></head><body>
<h3>KOUSHA banner — live animation preview (this is how it looks on GitHub)</h3>
<p>Watch: titles rotate Full-Stack → AI → Data → Backend/DevOps, packets flow Bronze→Silver→Gold, particles drift, cursor blinks.</p>
<div class="wrap">
<svg viewBox="0 0 1280 400" xmlns="http://www.w3.org/2000/svg" width="1280" height="400" fill="none" font-family="'Segoe UI',Helvetica,Arial,sans-serif">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0" stop-color="#0a0a14"/><stop offset="0.5" stop-color="#0d0b1e"/><stop offset="1" stop-color="#070610"/>
    </linearGradient>
    <linearGradient id="violet" x1="0" y1="0" x2="1" y2="0">
      <stop offset="0" stop-color="#a78bfa"/><stop offset="1" stop-color="#6366f1"/>
    </linearGradient>
    <linearGradient id="bronze" x1="0" y1="0" x2="1" y2="0"><stop offset="0" stop-color="#c97a3a"/><stop offset="1" stop-color="#e8a05a"/></linearGradient>
    <linearGradient id="silver" x1="0" y1="0" x2="1" y2="0"><stop offset="0" stop-color="#9ca3b8"/><stop offset="1" stop-color="#d5dbe8"/></linearGradient>
    <linearGradient id="gold" x1="0" y1="0" x2="1" y2="0"><stop offset="0" stop-color="#d4a520"/><stop offset="1" stop-color="#f5d05a"/></linearGradient>
    <radialGradient id="glow" cx="50%" cy="50%" r="50%"><stop offset="0" stop-color="#8b5cf6" stop-opacity="0.5"/><stop offset="1" stop-color="#8b5cf6" stop-opacity="0"/></radialGradient>
  </defs>

  <rect width="1280" height="400" fill="url(#bg)"/>
  <ellipse cx="360" cy="150" rx="420" ry="240" fill="url(#glow)" opacity="0.55"/>
  <ellipse cx="1000" cy="300" rx="360" ry="220" fill="url(#glow)" opacity="0.32"/>

  <g stroke="#ffffff" stroke-opacity="0.04">
    <path d="M0 100 H1280 M0 200 H1280 M0 300 H1280"/>
    <path d="M160 0 V400 M320 0 V400 M480 0 V400 M640 0 V400 M800 0 V400 M960 0 V400 M1120 0 V400"/>
  </g>

  <g fill="#a78bfa">
    <circle cx="120" cy="80" r="1.6" opacity="0.7"><animate attributeName="cy" values="80;60;80" dur="7s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.2;0.8;0.2" dur="7s" repeatCount="indefinite"/></circle>
    <circle cx="1180" cy="120" r="2" opacity="0.6"><animate attributeName="cy" values="120;100;120" dur="9s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.3;0.9;0.3" dur="9s" repeatCount="indefinite"/></circle>
    <circle cx="900" cy="70" r="1.4" opacity="0.5"><animate attributeName="cy" values="70;90;70" dur="6s" repeatCount="indefinite"/></circle>
    <circle cx="240" cy="330" r="1.8" opacity="0.6"><animate attributeName="cy" values="330;310;330" dur="8s" repeatCount="indefinite"/><animate attributeName="opacity" values="0.2;0.7;0.2" dur="8s" repeatCount="indefinite"/></circle>
    <circle cx="1080" cy="340" r="1.5" opacity="0.5"><animate attributeName="cy" values="340;360;340" dur="7.5s" repeatCount="indefinite"/></circle>
    <circle cx="60" cy="220" r="1.3" opacity="0.5"><animate attributeName="opacity" values="0.2;0.8;0.2" dur="5s" repeatCount="indefinite"/></circle>
  </g>

  <!-- identity -->
  <text x="80" y="118" font-size="19" letter-spacing="6" fill="#a78bfa" font-weight="600">HI, I'M</text>
  <text x="78" y="184" font-size="62" font-weight="800" fill="#ffffff" letter-spacing="1">KOUSHA REZAEI</text>

  <!-- rotating titles: 4 titles, each visible 3s in a 12s loop, hard on/off (no overlap) -->
  <g font-size="25" font-weight="700">
    <text x="80" y="236" fill="url(#violet)">Full-Stack Engineer<set attributeName="opacity" to="1"/>
      <animate attributeName="opacity" values="1;1;0;0;0;0;0;0;1;1" keyTimes="0;0.24;0.25;0.49;0.5;0.74;0.75;0.99;0.995;1" dur="12s" repeatCount="indefinite"/></text>
    <text x="80" y="236" fill="url(#violet)" opacity="0">AI Engineer
      <animate attributeName="opacity" values="0;0;1;1;0;0;0;0;0;0" keyTimes="0;0.24;0.25;0.49;0.5;0.74;0.75;0.99;0.995;1" dur="12s" repeatCount="indefinite"/></text>
    <text x="80" y="236" fill="url(#violet)" opacity="0">Data Engineer
      <animate attributeName="opacity" values="0;0;0;0;1;1;0;0;0;0" keyTimes="0;0.24;0.25;0.49;0.5;0.74;0.75;0.99;0.995;1" dur="12s" repeatCount="indefinite"/></text>
    <text x="80" y="236" fill="url(#violet)" opacity="0">Backend &amp; DevOps
      <animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0;0" keyTimes="0;0.24;0.25;0.49;0.5;0.74;0.75;0.99;0.995;1" dur="12s" repeatCount="indefinite"/></text>
  </g>
  <!-- blinking cursor after titles -->
  <rect x="82" y="220" width="3" height="22" fill="#a78bfa"><animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/></rect>

  <text x="80" y="280" font-size="15" fill="#9096ad">Full-stack, AI, and data engineering — I build the whole system,</text>
  <text x="80" y="302" font-size="15" fill="#9096ad">from <tspan fill="#c4b5fd" font-weight="600">pipeline to product</tspan>.</text>

  <!-- tech badges -->
  <g font-size="12.5" font-weight="600">
    <g transform="translate(80,326)"><rect width="80" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="40" y="17" fill="#c4b5fd" text-anchor="middle">Python</text></g>
    <g transform="translate(168,326)"><rect width="66" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="33" y="17" fill="#c4b5fd" text-anchor="middle">Spark</text></g>
    <g transform="translate(242,326)"><rect width="62" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="31" y="17" fill="#c4b5fd" text-anchor="middle">Kafka</text></g>
    <g transform="translate(312,326)"><rect width="72" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="36" y="17" fill="#c4b5fd" text-anchor="middle">Airflow</text></g>
    <g transform="translate(392,326)"><rect width="64" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="32" y="17" fill="#c4b5fd" text-anchor="middle">Trino</text></g>
    <g transform="translate(464,326)"><rect width="76" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#a78bfa" stroke-opacity="0.3"/><text x="38" y="17" fill="#c4b5fd" text-anchor="middle">Iceberg</text></g>
  </g>
  <g font-size="12.5" font-weight="600">
    <g transform="translate(80,360)"><rect width="86" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#6366f1" stroke-opacity="0.3"/><text x="43" y="17" fill="#a5b4fc" text-anchor="middle">Next.js</text></g>
    <g transform="translate(174,360)"><rect width="72" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#6366f1" stroke-opacity="0.3"/><text x="36" y="17" fill="#a5b4fc" text-anchor="middle">Docker</text></g>
    <g transform="translate(254,360)"><rect width="94" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#6366f1" stroke-opacity="0.3"/><text x="47" y="17" fill="#a5b4fc" text-anchor="middle">Kubernetes</text></g>
    <g transform="translate(356,360)"><rect width="60" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#6366f1" stroke-opacity="0.3"/><text x="30" y="17" fill="#a5b4fc" text-anchor="middle">AWS</text></g>
    <g transform="translate(424,360)"><rect width="80" height="26" rx="13" fill="#ffffff" fill-opacity="0.05" stroke="#6366f1" stroke-opacity="0.3"/><text x="40" y="17" fill="#a5b4fc" text-anchor="middle">LLM APIs</text></g>
  </g>

  <!-- medallion pipeline (REAL: Bronze->Silver->Gold data layers) -->
  <g transform="translate(720,150)">
    <text x="180" y="-66" font-size="13" letter-spacing="3" fill="#6b7180" text-anchor="middle" font-weight="600">DATA LAKEHOUSE — MEDALLION ARCHITECTURE</text>
    <path d="M40 0 H140" stroke="#2a2740" stroke-width="6" stroke-linecap="round"/>
    <path d="M220 0 H320" stroke="#2a2740" stroke-width="6" stroke-linecap="round"/>
    <circle r="4" fill="#e8a05a"><animateMotion path="M40 0 H140" dur="2s" repeatCount="indefinite"/></circle>
    <circle r="4" fill="#e8a05a" opacity="0.55"><animateMotion path="M40 0 H140" dur="2s" begin="1s" repeatCount="indefinite"/></circle>
    <circle r="4" fill="#d5dbe8"><animateMotion path="M220 0 H320" dur="2s" begin="0.5s" repeatCount="indefinite"/></circle>
    <circle r="4" fill="#d5dbe8" opacity="0.55"><animateMotion path="M220 0 H320" dur="2s" begin="1.5s" repeatCount="indefinite"/></circle>
    <g>
      <circle r="30" fill="url(#bronze)" opacity="0.15"/>
      <circle r="22" fill="url(#bronze)"><animate attributeName="r" values="22;24;22" dur="2s" repeatCount="indefinite"/></circle>
      <text y="5" font-size="15" font-weight="800" fill="#3a2410" text-anchor="middle">R</text>
      <text y="52" font-size="13" font-weight="700" fill="#e8a05a" text-anchor="middle">Bronze</text>
      <text y="68" font-size="10" fill="#7a6b55" text-anchor="middle">raw ingest</text>
    </g>
    <g transform="translate(180,0)">
      <circle r="30" fill="url(#silver)" opacity="0.15"/>
      <circle r="22" fill="url(#silver)"><animate attributeName="r" values="22;24;22" dur="2s" begin="0.5s" repeatCount="indefinite"/></circle>
      <text y="5" font-size="15" font-weight="800" fill="#2a2f3a" text-anchor="middle">S</text>
      <text y="52" font-size="13" font-weight="700" fill="#d5dbe8" text-anchor="middle">Silver</text>
      <text y="68" font-size="10" fill="#6b7180" text-anchor="middle">cleaned</text>
    </g>
    <g transform="translate(360,0)">
      <circle r="30" fill="url(#gold)" opacity="0.2"/>
      <circle r="22" fill="url(#gold)"><animate attributeName="r" values="22;25;22" dur="2s" begin="1s" repeatCount="indefinite"/></circle>
      <text y="5" font-size="15" font-weight="800" fill="#3a2f0a" text-anchor="middle">G</text>
      <text y="52" font-size="13" font-weight="700" fill="#f5d05a" text-anchor="middle">Gold</text>
      <text y="68" font-size="10" fill="#8a7a45" text-anchor="middle">analytics-ready</text>
    </g>
  </g>

  <rect x="0" y="396" width="1280" height="4" fill="url(#violet)" opacity="0.5"/>
  <rect x="0" y="396" width="300" height="4" fill="#c4b5fd"><animate attributeName="x" values="-300;1280" dur="4s" repeatCount="indefinite"/></rect>
</svg>
</div></body></html>
