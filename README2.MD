assets/cyber-hud.svg
<svg width="1200" height="330" viewBox="0 0 1200 330" fill="none" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bg" x1="0" y1="0" x2="1200" y2="330">
      <stop stop-color="#020617"/>
      <stop offset=".5" stop-color="#082F49"/>
      <stop offset="1" stop-color="#020617"/>
    </linearGradient>
    <radialGradient id="earth">
      <stop stop-color="#38BDF8"/>
      <stop offset=".55" stop-color="#075985"/>
      <stop offset="1" stop-color="#020617"/>
    </radialGradient>
    <pattern id="grid" width="42" height="42" patternUnits="userSpaceOnUse">
      <path d="M42 0H0V42" fill="none" stroke="#38BDF8" stroke-opacity=".13"/>
    </pattern>
    <filter id="glow">
      <feGaussianBlur stdDeviation="3" result="b"/>
      <feMerge><feMergeNode in="b"/><feMergeNode in="SourceGraphic"/></feMerge>
    </filter>
    <clipPath id="planetClip"><circle cx="600" cy="165" r="94"/></clipPath>
  </defs>

  <rect width="1200" height="330" fill="url(#bg)"/>
  <rect width="1200" height="330" fill="url(#grid)">
    <animateTransform attributeName="transform" type="translate" from="0 0" to="42 42" dur="3s" repeatCount="indefinite"/>
  </rect>

  <g transform="translate(600 165)" stroke="#38BDF8" fill="none" filter="url(#glow)">
    <ellipse rx="205" ry="55" stroke-opacity=".52" stroke-width="2" stroke-dasharray="12 11">
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="10s" repeatCount="indefinite"/>
    </ellipse>
    <ellipse rx="170" ry="42" stroke-opacity=".25" stroke-width="1">
      <animateTransform attributeName="transform" type="rotate" from="360" to="0" dur="14s" repeatCount="indefinite"/>
    </ellipse>
  </g>

  <circle cx="600" cy="165" r="101" fill="#38BDF8" fill-opacity=".15" filter="url(#glow)">
    <animate attributeName="r" values="96;108;96" dur="3s" repeatCount="indefinite"/>
  </circle>

  <circle cx="600" cy="165" r="94" fill="url(#earth)" stroke="#7DD3FC" stroke-width="2" filter="url(#glow)"/>

  <g clip-path="url(#planetClip)" transform="translate(600 165)" stroke="#BAE6FD" fill="none" stroke-opacity=".7">
    <g>
      <path d="M-90 0H90M-82-38H82M-62-70H62M-62 70H62M-82 38H82" stroke-width="1"/>
      <ellipse rx="35" ry="94" stroke-width="1"/>
      <ellipse rx="70" ry="94" stroke-width="1"/>
      <path d="M-10-76L30-58L42-28L17-4L-8-19L-35-5L-43 26L-20 54L-4 38L22 60L46 39L67 12" fill="#38BDF8" fill-opacity=".35" stroke="none"/>
      <path d="M-75-24L-52-44L-28-38L-20-8L-41 13L-65 8L-82-6Z" fill="#0EA5E9" fill-opacity=".42" stroke="none"/>
      <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="18s" repeatCount="indefinite"/>
    </g>
  </g>

  <g fill="#E0F2FE" filter="url(#glow)">
    <circle r="5"><animateMotion dur="10s" repeatCount="indefinite" path="M395,165 A205,55 0 1,1 805,165 A205,55 0 1,1 395,165"/></circle>
    <circle r="4"><animateMotion dur="14s" repeatCount="indefinite" path="M430,165 A170,42 0 1,0 770,165 A170,42 0 1,0 430,165"/></circle>
  </g>

  <rect width="1200" height="3" fill="#38BDF8" filter="url(#glow)">
    <animate attributeName="y" values="0;327;0" dur="3.5s" repeatCount="indefinite"/>
  </rect>

  <text x="600" y="300" text-anchor="middle" fill="#E0F2FE" font-size="16" font-family="monospace" letter-spacing="4">LIDOR BYTE // GLOBAL SYSTEM ONLINE</text>
</svg>
