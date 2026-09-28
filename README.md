<svg viewBox="0 0 1180 610" width="100%" xmlns="http://www.w3.org/2000/svg"
     font-family="'SF Mono','Fira Code',Consolas,monospace">

<defs>

  <!-- ================= BACKGROUND GLOWS ================= -->

  <radialGradient id="glowPurple">
    <stop offset="0%" stop-color="#7C3AED" stop-opacity=".55"/>
    <stop offset="100%" stop-color="#7C3AED" stop-opacity="0"/>
  </radialGradient>

  <radialGradient id="glowCyan">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity=".5"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </radialGradient>

  <radialGradient id="glowGreen">
    <stop offset="0%" stop-color="#10B981" stop-opacity=".4"/>
    <stop offset="100%" stop-color="#10B981" stop-opacity="0"/>
  </radialGradient>

  <!-- ================= ACCENT ================= -->

  <linearGradient id="accentGrad" x1="0%" y1="0%" x2="100%" y2="0%">
    <stop offset="0%" stop-color="#7C3AED"/>
    <stop offset="50%" stop-color="#22D3EE"/>
    <stop offset="100%" stop-color="#10B981"/>

    <animateTransform
      attributeName="gradientTransform"
      type="translate"
      values="-150 0;150 0;-150 0"
      dur="7s"
      repeatCount="indefinite"/>
  </linearGradient>

  <!-- ================= GLASS ================= -->

  <linearGradient id="glassSheen" x1="0" y1="0" x2="1" y2="1">
    <stop offset="0%" stop-color="#FFFFFF" stop-opacity=".08"/>
    <stop offset="35%" stop-color="#FFFFFF" stop-opacity="0"/>
    <stop offset="100%" stop-color="#FFFFFF" stop-opacity="0"/>
  </linearGradient>

  <!-- ================= SCAN ================= -->

  <linearGradient id="scanGrad">
    <stop offset="0%" stop-color="#22D3EE" stop-opacity="0"/>
    <stop offset="50%" stop-color="#22D3EE" stop-opacity=".55"/>
    <stop offset="100%" stop-color="#22D3EE" stop-opacity="0"/>
  </linearGradient>

  <!-- ================= CLIPS ================= -->

  <clipPath id="outerClip">
    <rect width="1180" height="610" rx="28"/>
  </clipPath>

  <clipPath id="leftClip">
    <rect x="24" y="24" width="424" height="562" rx="20"/>
  </clipPath>

  <clipPath id="rightClip">
    <rect x="472" y="24" width="684" height="562" rx="20"/>
  </clipPath>

  <!-- ================= GLOW FILTER ================= -->

  <filter id="glow" x="-60%" y="-60%" width="220%" height="220%">
    <feGaussianBlur stdDeviation="5" result="blur"/>
    <feMerge>
      <feMergeNode in="blur"/>
      <feMergeNode in="SourceGraphic"/>
    </feMerge>
  </filter>

</defs>


<!-- ====================================================== -->
<!-- BACKGROUND -->
<!-- ====================================================== -->

<rect width="1180" height="610" rx="28" fill="#030712"/>

<g clip-path="url(#outerClip)">

  <circle cx="180" cy="120" r="220" fill="url(#glowPurple)">
    <animate attributeName="cx"
             values="180;230;180"
             dur="11s"
             repeatCount="indefinite"/>
  </circle>

  <circle cx="950" cy="480" r="260" fill="url(#glowCyan)">
    <animate attributeName="cx"
             values="950;880;950"
             dur="13s"
             repeatCount="indefinite"/>
  </circle>

  <circle cx="820" cy="60" r="180" fill="url(#glowGreen)">
    <animate attributeName="cx"
             values="820;760;820"
             dur="14s"
             repeatCount="indefinite"/>
  </circle>


  <!-- FLOATING PARTICLES -->

  <g fill="#67E8F9">

    <circle cx="452" cy="60" r="1.6">
      <animate attributeName="cy"
               values="60;44;60"
               dur="5s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="460" cy="560" r="1.8">
      <animate attributeName="cy"
               values="560;540;560"
               dur="6s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="30" cy="300" r="1.4">
      <animate attributeName="cx"
               values="30;46;30"
               dur="7s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="1155" cy="140" r="2">
      <animate attributeName="cy"
               values="140;170;140"
               dur="6.5s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="30" cy="300" r="1.4">
      <animate attributeName="cx"
               values="30;46;30"
               dur="7s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="1155" cy="140" r="2">
      <animate attributeName="cy"
               values="140;170;140"
               dur="6.5s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="1150" cy="470" r="1.6">
      <animate attributeName="cx"
               values="1150;1130;1150"
               dur="8s"
               repeatCount="indefinite"/>
    </circle>

  </g>


  <!-- ================================================== -->
  <!-- LEFT PANEL -->
  <!-- ================================================== -->

  <g>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="#0F172A"
          fill-opacity=".7"/>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="none"
          stroke="#FFFFFF"
          stroke-opacity=".1"/>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="url(#glassSheen)"
          clip-path="url(#leftClip)"/>
          <g>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="#0F172A"
          fill-opacity=".7"/>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="none"
          stroke="#FFFFFF"
          stroke-opacity=".1"/>

    <rect x="24" y="24"
          width="424"
          height="562"
          rx="20"
          fill="url(#glassSheen)"
          clip-path="url(#leftClip)"/>


    <!-- TERMINAL HEADER -->

    <circle cx="46" cy="42" r="5" fill="#FF5F56"/>
    <circle cx="63" cy="42" r="5" fill="#FFBD2E"/>
    <circle cx="80" cy="42" r="5" fill="#27C93F"/>

    <text x="428"
          y="46"
          text-anchor="end"
          font-size="11"
          fill="#94A3B8">
      profile.svg
    </text>

    <line x1="24" y1="60"
          x2="448" y2="60"
          stroke="#FFFFFF"
          stroke-opacity=".08"/>


    <!-- MONOGRAM -->

    <text x="236"
          y="185"
          text-anchor="middle"
          font-family="Arial,sans-serif"
          font-size="82"
          font-weight="900"
          letter-spacing="-4"
          fill="url(#accentGrad)"
          filter="url(#glow)">

      AP

      <animate attributeName="opacity"
               values="0;1"
               dur="1s"
               fill="freeze"/>
    </text>


    <!-- NAME -->

    <text x="236"
          y="280"
          text-anchor="middle"
          font-family="Arial,sans-serif"
          font-size="27"
          font-weight="800"
          letter-spacing="3"
          fill="url(#accentGrad)">

      ANURAG PAL

    </text>


    <!-- TAGLINE -->

    <text x="236"
          y="310"
          text-anchor="middle"
          font-size="12.5"
          font-style="italic"
          fill="#94A3B8">

      // building ideas into code

    </text>


    <!-- DIVIDER -->

    <line x1="66" y1="340"
          x2="226" y2="340"
          stroke="#94A3B8"
          stroke-opacity=".25"/>

    <rect x="232"
          y="336"
          width="8"
          height="8"
          fill="url(#accentGrad)"
          transform="rotate(45 236 340)"/>

    <line x1="246" y1="340"
          x2="406" y2="340"
          stroke="#94A3B8"
          stroke-opacity=".25"/>


    <!-- POWER -->

    <text x="42"
          y="380"
          font-size="11"
          letter-spacing="1"
          fill="#94A3B8">
      JAVA
    </text>

    <rect x="132"
          y="370"
          width="210"
          height="7"
          rx="3.5"
          fill="#FFFFFF"
          fill-opacity=".08"/>

    <rect x="132"
          y="370"
          width="0"
          height="7"
          rx="3.5"
          fill="url(#accentGrad)">

      <animate attributeName="width"
               from="0"
               to="185"
               dur="1s"
               fill="freeze"/>

    </rect>

    <text x="406"
          y="380"
          text-anchor="end"
          font-size="11"
          fill="#F8FAFC">
      88%
    </text>


    <!-- WEB -->

    <text x="42"
          y="408"
          font-size="11"
          letter-spacing="1"
          fill="#94A3B8">
      WEB
    </text>

    <rect x="132"
          y="398"
          width="210"
          height="7"
          rx="3.5"
          fill="#FFFFFF"
          fill-opacity=".08"/>

    <rect x="132"
          y="398"
          width="0"
          height="7"
          rx="3.5"
          fill="url(#accentGrad)">

      <animate attributeName="width"
               from="0"
               to="178"
               dur="1.1s"
               fill="freeze"/>

    </rect>

    <text x="406"
          y="408"
          text-anchor="end"
          font-size="11"
          fill="#F8FAFC">
      85%
    </text>
    <!-- DSA -->

    <text x="42"
          y="436"
          font-size="11"
          letter-spacing="1"
          fill="#94A3B8">
      DSA
    </text>

    <rect x="132"
          y="426"
          width="210"
          height="7"
          rx="3.5"
          fill="#FFFFFF"
          fill-opacity=".08"/>

    <rect x="132"
          y="426"
          width="0"
          height="7"
          rx="3.5"
          fill="url(#accentGrad)">

      <animate attributeName="width"
               from="0"
               to="168"
               dur="1.2s"
               fill="freeze"/>

    </rect>

    <text x="406"
          y="436"
          text-anchor="end"
          font-size="11"
          fill="#F8FAFC">
      80%
    </text>


    <!-- LINE -->

    <line x1="42"
          y1="467"
          x2="406"
          y2="467"
          stroke="#94A3B8"
          stroke-opacity=".2"/>


    <!-- TERMINAL -->

    <text x="42"
          y="495"
          font-size="12.5"
          fill="#94A3B8">

      $ whoami

    </text>

    <text x="42"
          y="515"
          font-size="12.5"
          fill="#22D3EE">

      &gt; anurag_pal

    </text>

    <text x="42"
          y="535"
          font-size="12.5"
          fill="#94A3B8">

      $ status:
      <tspan fill="#22D3EE">
        online
      </tspan>

    </text>


    <!-- SCAN LINE -->

    <rect x="24"
          y="24"
          width="424"
          height="3"
          fill="url(#scanGrad)">

      <animate attributeName="y"
               values="26;584;26"
               dur="4.5s"
               repeatCount="indefinite"/>

    </rect>

  </g>


  <!-- ================================================== -->
  <!-- RIGHT PANEL -->
  <!-- ================================================== -->

  <g>

    <rect x="472"
          y="24"
          width="684"
          height="562"
          rx="20"
          fill="#0F172A"
          fill-opacity=".7"/>

    <rect x="472"
          y="24"
          width="684"
          height="562"
          rx="20"
          fill="none"
          stroke="#FFFFFF"
          stroke-opacity=".1"/>

    <rect x="472"
          y="24"
          width="684"
          height="562"
          rx="20"
          fill="url(#glassSheen)"
          clip-path="url(#rightClip)"/>


    <!-- HEADER -->

    <circle cx="493" cy="42" r="5" fill="#FF5F56"/>
    <circle cx="510" cy="42" r="5" fill="#FFBD2E"/>
    <circle cx="527" cy="42" r="5" fill="#27C93F"/>

    <text x="1132"
          y="46"
          text-anchor="end"
          font-size="11"
          fill="#94A3B8">
      anurag@dev:~
    </text>

    <line x1="472"
          y1="60"
          x2="1156"
          y2="60"
          stroke="#FFFFFF"
          stroke-opacity=".08"/>


    <!-- GREETING -->

    <text x="504"
          y="112"
          font-family="Arial,sans-serif"
          font-size="34"
          font-weight="700"
          fill="#F8FAFC">

      Hi 👋 I'm
      <tspan fill="url(#accentGrad)">
        Anurag
      </tspan>

    </text>
    <!-- CSS -->

      <rect x="688"
            y="415"
            width="78"
            height="30"
            rx="15"
            fill="#10B981"
            fill-opacity=".14"
            stroke="#10B981"
            stroke-opacity=".55"/>

      <text x="727"
            y="435"
            text-anchor="middle"
            fill="#6EE7B7">
        CSS
      </text>


      <!-- JS -->

      <rect x="776"
            y="415"
            width="105"
            height="30"
            rx="15"
            fill="#F59E0B"
            fill-opacity=".13"
            stroke="#F59E0B"
            stroke-opacity=".5"/>

      <text x="828"
            y="435"
            text-anchor="middle"
            fill="#FCD34D">
        JavaScript
      </text>


      <!-- GIT -->

      <rect x="891"
            y="415"
            width="70"
            height="30"
            rx="15"
            fill="#EF4444"
            fill-opacity=".13"
            stroke="#EF4444"
            stroke-opacity=".5"/>

      <text x="926"
            y="435"
            text-anchor="middle"
            fill="#FCA5A5">
        Git
      </text>


      <!-- GITHUB -->

      <rect x="971"
            y="415"
            width="90"
            height="30"
            rx="15"
            fill="#FFFFFF"
            fill-opacity=".08"
            stroke="#FFFFFF"
            stroke-opacity=".25"/>

      <text x="1016"
            y="435"
            text-anchor="middle"
            fill="#E2E8F0">
        GitHub
      </text>

    </g>


    <!-- PROJECT TERMINAL -->

    <rect x="504"
          y="470"
          width="620"
          height="82"
          rx="12"
          fill="#020617"
          fill-opacity=".8"
          stroke="#FFFFFF"
          stroke-opacity=".08"/>


    <text x="524"
          y="495"
          font-size="12"
          fill="#94A3B8">

      $ current_project

    </text>

    <text x="524"
          y="518"
          font-size="13"
          font-weight="600"
          fill="#22D3EE">

      &gt; Blinkit Clone

    </text>

    <text x="524"
          y="540"
          font-size="11.5"
          fill="#94A3B8">

      Building • Learning • Improving 🚀

    </text>

  </g>

</g>

</svg>



