<!-- Блок проекта iME-Weather -->
  <h2>⚡ Featured Project</h2>

  <a href="https://github.com/Cloxoff/iME-Weather">
    <svg width="100%" max-width="850" viewBox="0 0 800 280" xmlns="http://www.w3.org/2000/svg" style="background: #0d1117; border: 1.5px solid #00e5ff; border-radius: 16px; box-shadow: 0 0 20px rgba(0, 229, 255, 0.15); font-family: 'Segoe UI', system-ui, sans-serif;">
      
      <!-- Стили для анимаций -->
      <style>
        @keyframes pulse {
          0% { transform: scale(1); filter: drop-shadow(0 0 8px rgba(0, 229, 255, 0.4)); }
          50% { transform: scale(1.03); filter: drop-shadow(0 0 22px rgba(0, 229, 255, 0.8)); }
          100% { transform: scale(1); filter: drop-shadow(0 0 8px rgba(0, 229, 255, 0.4)); }
        }
        @keyframes lightning {
          0%, 90%, 94%, 98%, 100% { opacity: 0.1; filter: drop-shadow(0 0 2px rgba(0, 229, 255, 0.2)); }
          92%, 96% { opacity: 1; filter: drop-shadow(0 0 25px #00e5ff); }
        }
        @keyframes rain {
          0% { transform: translateY(-10px); opacity: 0; }
          50% { opacity: 0.6; }
          100% { transform: translateY(25px); opacity: 0; }
        }
        @keyframes textGlow {
          0%, 100% { fill: #ffffff; filter: drop-shadow(0 0 4px rgba(0, 229, 255, 0.5)); }
          50% { fill: #00e5ff; filter: drop-shadow(0 0 15px rgba(0, 229, 255, 0.9)); }
        }
        @keyframes scanline {
          0% { transform: translateY(-100%); }
          100% { transform: translateY(280px); }
        }
        .cloud { transform-origin: 200px 120px; animation: pulse 4s ease-in-out infinite; }
        .lightning { transform-origin: 200px 170px; animation: lightning 5s infinite; }
        .rain-drop { animation: rain 1.5s linear infinite; }
        .drop-1 { animation-delay: 0s; }
        .drop-2 { animation-delay: 0.3s; }
        .drop-3 { animation-delay: 0.6s; }
        .drop-4 { animation-delay: 0.9s; }
        .title { animation: textGlow 3s ease-in-out infinite; font-weight: 800; font-size: 46px; }
      </style>

      <!-- Фоновая кибер-сетка -->
      <defs>
        <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
          <path d="M 40 0 L 0 0 0 40" fill="none" stroke="rgba(0, 229, 255, 0.04)" stroke-width="1"/>
        </pattern>
        <linearGradient id="blueGrad" x1="0%" y1="0%" x2="100%" y2="100%">
          <stop offset="0%" stop-color="#00e5ff" />
          <stop offset="100%" stop-color="#3b82f6" />
        </linearGradient>
      </defs>
      <rect width="100%" height="100%" fill="url(#grid)" />

      <!-- Сканирующая полоса (Cyber Effect) -->
      <line x1="0" y1="0" x2="800" y2="0" stroke="rgba(0, 229, 255, 0.08)" stroke-width="3" style="animation: scanline 6s linear infinite;" />

      <!-- Левая часть: Анимированная погода -->
      <g transform="translate(40, 0)">
        <!-- Капли дождя -->
        <g stroke="#00e5ff" stroke-width="3" stroke-linecap="round">
          <line class="rain-drop drop-1" x1="130" y1="180" x2="120" y2="205" />
          <line class="rain-drop drop-2" x1="165" y1="180" x2="155" y2="205" />
          <line class="rain-drop drop-3" x1="200" y1="180" x2="190" y2="205" />
          <line class="rain-drop drop-4" x1="235" y1="180" x2="225" y2="205" />
          <line class="rain-drop drop-2" x1="270" y1="180" x2="260" y2="205" />
        </g>

        <!-- Анимированная туча -->
        <path class="cloud" d="M120,150 a35,35 0 0,1 30,-25 a50,50 0 0,1 90,-15 a40,40 0 0,1 60,15 a35,35 0 0,1 10,70 l-190,0 a35,35 0 0,1 0,-45 z" fill="none" stroke="url(#blueGrad)" stroke-width="6" />

        <!-- Анимированная молния -->
        <polygon class="lightning" points="195,145 165,195 190,195 170,245 220,185 195,185" fill="none" stroke="#00e5ff" stroke-width="4" stroke-linejoin="round" />
      </g>

      <!-- Правая часть: Контент -->
      <g transform="translate(360, 95)">
        <text class="title" x="0" y="0">iME-Weather</text>
        <text x="0" y="35" fill="rgba(255, 255, 255, 0.7)" font-size="16" font-weight="500" letter-spacing="1">TURKMENISTAN'S DIGITAL FORECAST</text>
        
        <!-- Описание -->
        <text x="0" y="75" fill="rgba(255, 255, 255, 0.5)" font-size="14">A high-performance mobile app for tracking real-time weather.</text>
        <text x="0" y="95" fill="rgba(255, 255, 255, 0.5)" font-size="14">Стильный и быстрый прогноз погоды с точными данными.</text>
      </g>

      <!-- Декоративные рамки по углам -->
      <path d="M 15,30 L 15,15 L 30,15" fill="none" stroke="#00e5ff" stroke-width="3" />
      <path d="M 785,30 L 785,15 L 770,15" fill="none" stroke="#00e5ff" stroke-width="3" />
      <path d="M 15,250 L 15,265 L 30,265" fill="none" stroke="#00e5ff" stroke-width="3" />
      <path d="M 785,250 L 785,265 L 770,265" fill="none" stroke="#00e5ff" stroke-width="3" />
    </svg>
  </a>

  <br><br>

  <!-- Кнопки управления -->
  <div align="center">
    <a href="https://github.com/Cloxoff/iME-Weather">
      <img src="https://img.shields.io/badge/GitHub-Repository-0f172a?style=for-the-badge&logo=github&logoColor=00e5ff" />
    </a>
    <a href="https://github.com/Cloxoff/iME-Weather/releases">
      <img src="https://img.shields.io/badge/Download_APK-00e5ff?style=for-the-badge&logo=android&logoColor=0f172a" />
    </a>
  </div>
