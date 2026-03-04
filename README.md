<!-- assets/typing.svg -->
<svg xmlns="http://www.w3.org/2000/svg" width="900" height="140" viewBox="0 0 900 140" role="img" aria-label="Typing header">
  <style>
    .bg { fill: #0f172a; }
    .text { fill: #bfe0ff; font-family: "Segoe UI", Roboto, -apple-system, "Helvetica Neue", Arial; font-weight:700; font-size:36px; }
    .cursor { fill:#60a5fa; }
    /* mask animation using rect width */
    .revealRect { fill: white; }
    .sub { fill:#9fbbe6; font-size:16px; font-weight:500; }
  </style>

  <!-- background rounded -->
  <rect rx="12" ry="12" width="900" height="140" class="bg"/>

  <!-- floating accent circles -->
  <g opacity="0.12" transform="translate(720,20)">
    <circle r="40" fill="#60a5fa">
      <animate attributeName="cy" dur="6s" values="0;12;0" repeatCount="indefinite" />
    </circle>
  </g>

  <!-- text and masked reveal -->
  <defs>
    <mask id="reveal">
      <rect x="0" y="0" width="900" height="140" fill="black"/>
      <!-- The white rect will expose the text progressively -->
      <rect id="mrect" x="30" y="40" width="0" height="60" class="revealRect">
        <animate attributeName="width" from="0" to="820" dur="4.5s" begin="0.3s" fill="freeze" />
      </rect>
    </mask>
  </defs>

  <g mask="url(#reveal)">
    <text x="40" y="75" class="text">👋 Olá — eu sou Micaias Soares</text>
    <text x="40" y="102" class="sub">Front-End Developer • HTML • CSS • JavaScript • React</text>
  </g>

  <!-- blinking cursor (positioned at end, synchronized approx.) -->
  <rect x="520" y="48" width="8" height="36" class="cursor">
    <animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite" />
    <animate attributeName="x" values="520;760" dur="4.5s" begin="0.3s" fill="freeze" />
  </rect>
</svg>
