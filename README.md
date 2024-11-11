<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 400">
  <!-- Previous defs remain the same -->
  <defs>
    <linearGradient id="mainGradient" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" style="stop-color:#8A2BE2;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#9370DB;stop-opacity:1" />
    </linearGradient>
    <linearGradient id="glowGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#9370DB;stop-opacity:0.4" />
      <stop offset="100%" style="stop-color:#8A2BE2;stop-opacity:0.1" />
    </linearGradient>
    <linearGradient id="textGradient" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" style="stop-color:#ffffff;stop-opacity:1" />
      <stop offset="100%" style="stop-color:#e0e0e0;stop-opacity:1" />
    </linearGradient>
    <style>
      @import url('https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600&amp;display=swap');
      .title { 
        font-family: 'Inter', sans-serif; 
        font-size: 24px; 
        font-weight: 600; 
        letter-spacing: 0.5px;
      }
      .subtitle { 
        font-family: 'Inter', sans-serif; 
        font-size: 13px; 
        fill: #ccc;
        font-weight: 300;
        letter-spacing: 0.4px;
      }
      .section-header { 
        font-family: 'Inter', sans-serif; 
        font-size: 14px; 
        fill: #fff;
        font-weight: 250;
        letter-spacing: 0.3px;
      }
      .project-link { 
        font-family: 'Inter', sans-serif; 
        font-size: 12px; 
        fill: #9370DB;
        font-weight: 400;
        letter-spacing: 0.3px;
      }
      .project-header { 
        font-family: 'Inter', sans-serif; 
        font-size: 14px; 
        fill: #fff;
        font-weight: 250;
        letter-spacing: 0.3px;
      }
    </style>
    <mask id="textFade">
      <rect x="0" y="0" width="800" height="400" fill="white" opacity="0.98"/>
    </mask>
  </defs>

  <!-- Background -->
  <rect width="800" height="400" fill="#1a1a1a"/>
  <g opacity="0.2">
    <path d="M0 80 L800 80 M0 160 L800 160 M0 240 L800 240 M0 320 L800 320" 
          stroke="#444" stroke-width="0.3"/>
    <path d="M160 0 L160 400 M320 0 L320 400 M480 0 L480 400 M640 0 L640 400" 
          stroke="#444" stroke-width="0.3"/>
  </g>

  <!-- Geometric Elements (moved slightly right) -->
  <g transform="translate(500,200)">
    <!-- Previous geometric elements -->
    <circle cx="0" cy="0" r="180" fill="url(#mainGradient)" opacity="0.05"/>
    <path d="M-180,0 L-90,-156 L90,-156 L180,0 L90,156 L-90,156 Z" 
          fill="none" stroke="url(#mainGradient)" stroke-width="1" opacity="0.4">
      <animateTransform attributeName="transform"
                        type="rotate"
                        from="0 0 0"
                        to="360 0 0"
                        dur="30s"
                        repeatCount="indefinite"/>
    </path>
    <path d="M-120,0 L-60,-104 L60,-104 L120,0 L60,104 L-60,104 Z" 
          fill="none" stroke="url(#mainGradient)" stroke-width="1.5" opacity="0.6">
      <animateTransform attributeName="transform"
                        type="rotate"
                        from="360 0 0"
                        to="0 0 0"
                        dur="25s"
                        repeatCount="indefinite"/>
    </path>
    <path d="M-60,0 L-30,-52 L30,-52 L60,0 L30,52 L-30,52 Z" 
          fill="none" stroke="url(#mainGradient)" stroke-width="2">
      <animateTransform attributeName="transform"
                        type="rotate"
                        from="0 0 0"
                        to="360 0 0"
                        dur="20s"
                        repeatCount="indefinite"/>
    </path>
    <!-- Mathematical curves -->
    <path d="M-180,0 Q-90,100 0,0 Q90,-100 180,0" 
          fill="none" stroke="url(#glowGradient)" stroke-width="1.5" opacity="0.4">
      <animate attributeName="d" 
               values="M-180,0 Q-90,100 0,0 Q90,-100 180,0;
                      M-180,0 Q-90,-100 0,0 Q90,100 180,0;
                      M-180,0 Q-90,100 0,0 Q90,-100 180,0"
               dur="15s"
               repeatCount="indefinite"/>
    </path>
  </g>
  <!-- Text Content -->
  <g mask="url(#textFade)">
    <g transform="translate(40,60)">
      <!-- Main Title -->
      <text class="title" fill="url(#textGradient)">
        Software Engineer
      </text>
      <!-- Description -->
      <text class="subtitle" x="0" y="40">
        Building AI developer tools and workflows
      </text>
      <text class="subtitle" x="0" y="65">
        Enjoy learning and exploring the unknown
      </text>
      <!-- Projects Section -->
      <g transform="translate(0,120)">
        <text class="section-header">
          <tspan>↜ Open Source</tspan>
        </text>
        <!-- Project Links -->
        <a href="https://github.com/eli64s/README-AI" target="_blank">
          <g transform="translate(0,25)">
            <rect x="-5" y="-15" width="120" height="24" 
                  fill="#2a2a2a" rx="4" opacity="0.6"/>
            <text class="project-link" x="12" y="2">
              README-AI
            </text>
          </g>
        </a>
      </g>
      <!-- Connect Section -->
      <g transform="translate(0,190)">
        <text class="section-header">
          <tspan>↜ Stay Connected</tspan>
        </text>
        <!-- Social Links -->
        <g transform="translate(0,30)">
          <!-- GitHub -->
          <a href="https://github.com/eli64s" target="_blank">
            <circle cx="15" cy="15" r="15" fill="#2a2a2a"/>
            <path d="M15,5 C9.5,5 5,9.5 5,15 C5,19.25 7.75,22.875 11.5,24.125 C12,24.1875 12.125,23.875 12.125,23.625 C12.125,23.375 12.125,22.625 12.125,21.875 C9.375,22.375 8.75,20.375 8.75,20.375 C8.25,19.125 7.5,18.875 7.5,18.875 C6.5,18.25 7.5,18.25 7.5,18.25 C8.5,18.3125 9.125,19.1875 9.125,19.1875 C10,20.6875 11.5,20.375 12.125,20.125 C12.25,19.375 12.5,18.875 12.75,18.625 C10.5,18.375 8.125,17.375 8.125,13.625 C8.125,12.5 8.5,11.625 9.125,10.875 C9,10.625 8.625,9.375 9.25,8.125 C9.25,8.125 10.125,7.875 12.125,9.125 C13,8.875 13.875,8.75 14.75,8.75 C15.625,8.75 16.5,8.875 17.375,9.125 C19.375,7.875 20.25,8.125 20.25,8.125 C20.875,9.375 20.5,10.625 20.375,10.875 C21,11.625 21.375,12.5 21.375,13.625 C21.375,17.375 19,18.375 16.75,18.625 C17.125,18.875 17.375,19.375 17.375,20.25 C17.375,21.5 17.375,23.25 17.375,23.625 C17.375,23.875 17.5,24.1875 18,24.125 C21.75,22.875 24.5,19.25 24.5,15 C24.5,9.5 20,5 14.5,5 Z" fill="#fff"/>
          </a>
          <!-- LinkedIn -->
          <g transform="translate(40,0)">
            <a href="https://www.linkedin.com/in/eli64s" target="_blank">
              <circle cx="15" cy="15" r="15" fill="#2a2a2a"/>
              <rect x="8" y="11" width="4" height="9" fill="#fff"/>
              <circle cx="10" cy="8" r="2" fill="#fff"/>
              <path d="M16,11 C16,11 17,11 18,12 C19,13 19,15 19,15 L19,20 L15,20 L15,15.5 C15,15.5 15,14 14,14 C13,14 13,15.5 13,15.5 L13,20 L9,20 L9,11 L13,11 L13,12 C13,12 14,11 16,11" fill="#fff"/>
            </a>
          </g>
          <!-- Twitter -->
          <g transform="translate(80,0)">
            <a href="https://twitter.com/eli64s" target="_blank">
              <circle cx="15" cy="15" r="15" fill="#2a2a2a"/>
              <path d="M23,9.3 C22.3,9.6 21.6,9.8 20.9,9.9 C21.6,9.4 22.2,8.6 22.5,7.7 C21.8,8.1 21,8.4 20.2,8.6 C19.6,7.8 18.7,7.3 17.7,7.3 C15.8,7.3 14.3,8.8 14.3,10.7 C14.3,11 14.3,11.3 14.4,11.5 C11.6,11.4 9.1,10.1 7.4,8.1 C7.1,8.6 6.9,9.2 6.9,9.9 C6.9,11.1 7.5,12.1 8.4,12.7 C7.8,12.7 7.3,12.5 6.8,12.3 C6.8,12.3 6.8,12.3 6.8,12.4 C6.8,14.1 8,15.4 9.5,15.7 C9.2,15.8 8.9,15.8 8.6,15.8 C8.4,15.8 8.2,15.8 8,15.7 C8.4,17 9.6,18 11.1,18 C10,18.8 8.6,19.3 7.1,19.3 C6.8,19.3 6.6,19.3 6.3,19.3 C7.8,20.2 9.5,20.7 11.3,20.7 C17.7,20.7 21.2,15.8 21.2,11.6 C21.2,11.4 21.2,11.3 21.2,11.1 C21.9,10.5 22.5,9.9 23,9.3 Z" fill="#fff" transform="scale(0.7) translate(8,8)"/>
            </a>
          </g>
        </g>
      </g>
    </g>
  </g>
</svg>
