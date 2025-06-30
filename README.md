<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Profil</title>
  <style>
    /* RESET */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: linear-gradient(135deg, #0f0c29, #302b63, #24243e);
      color: #fff;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: start;
      min-height: 100vh;
      overflow-x: hidden;
    }

    header {
      margin-top: 40px;
      text-align: center;
      animation: fadeInDown 1.5s ease-in-out;
    }

    header h1 {
      font-size: 2.5rem;
      margin-bottom: 10px;
      animation: pulse 2s infinite;
    }

    .profile-pic {
      width: 180px;
      height: 180px;
      border-radius: 50%;
      border: 5px solid white;
      object-fit: cover;
      box-shadow: 0 0 30px #00ffe1;
      animation: float 3s ease-in-out infinite;
    }

    .social-links {
      margin-top: 30px;
      display: flex;
      gap: 20px;
      flex-wrap: wrap;
      justify-content: center;
    }

    .social-links a {
      text-decoration: none;
      padding: 12px 24px;
      border-radius: 30px;
      background: #ffffff22;
      color: #fff;
      border: 2px solid #00ffe1;
      transition: all 0.4s ease;
      backdrop-filter: blur(8px);
      animation: fadeInUp 1s ease forwards;
    }

    .social-links a:hover {
      background: #00ffe1;
      color: #000;
      transform: scale(1.1);
      box-shadow: 0 0 20px #00ffe1;
    }

    footer {
      position: absolute;
      bottom: 10px;
      font-size: 0.9rem;
      opacity: 0.6;
      animation: fadeIn 4s ease;
    }

    /* Animations */
    @keyframes fadeInDown {
      0% { opacity: 0; transform: translateY(-30px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeInUp {
      0% { opacity: 0; transform: translateY(30px); }
      100% { opacity: 1; transform: translateY(0); }
    }

    @keyframes fadeIn {
      0% { opacity: 0; }
      100% { opacity: 1; }
    }

    @keyframes pulse {
      0%, 100% { text-shadow: 0 0 10px #00ffe1; }
      50% { text-shadow: 0 0 30px #00ffe1; }
    }

    @keyframes float {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-10px); }
    }

    /* Background floating dots */
    .dots {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      pointer-events: none;
      z-index: -1;
      overflow: hidden;
    }

    .dot {
      position: absolute;
      width: 10px;
      height: 10px;
      background: #00ffe1;
      border-radius: 50%;
      opacity: 0.3;
      animation: floatDot linear infinite;
    }

    @keyframes floatDot {
      from {
        transform: translateY(100vh);
      }
      to {
        transform: translateY(-10vh);
      }
    }
  </style>
</head>
<body>
  <header>
    <img class="" src="" alt="">
    <h1>Ryuga Ken</h1>
  </header>

  <div class="social-links">
    <a href="https://www.instagram.com/ryugggaa?igsh=MThiNGVraGVoemsybw==" target="_blank">Instagram</a>
    <a href="https://www.tiktok.com/@ryugaangkasaa?_t=ZS-8xdkoS56rTD&_r=1" target="_blank">TikTok</a>
    <a href="https://open.spotify.com/user/31cidikt6s74pg26qf72aguajzay?si=1UoQ1AiTThmW0OAMtlD9cw" target="_blank">Spotify</a>
    <a href="https://whatsapp.com/channel/0029VbAyEEj30LKLp8xROA1e" target="_blank">Channel WhatsApp</a>
    <a href="https://yughaalfarez.github.io/Perkenalan-Diri/" target="_blank">About me</a>
  </div>

  <footer>ib:@YughaDev</footer>

  <!-- Floating dots background -->
  <div class="dots" id="dot-container"></div>

  <script>
    // Generate floating dots animasi latar belakang
    const dotContainer = document.getElementById('dot-container');
    for (let i = 0; i < 50; i++) {
      const dot = document.createElement('div');
      dot.classList.add('dot');
      dot.style.left = Math.random() * 100 + 'vw';
      dot.style.animationDuration = 4 + Math.random() * 6 + 's';
      dot.style.width = dot.style.height = Math.random() * 8 + 4 + 'px';
      dotContainer.appendChild(dot);
    }
  </script>
</body>
</html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=Edge">
  <meta name="viewport" content="width=device-width, initial-scale=1">

  <title>HTML</title>
  
  <!-- HTML -->
  

  <!-- Custom Styles -->
  <link rel="stylesheet" href="style.css">
</head>

<body>
  <p></p>
  <!-- Project -->
  <script src="main.js"></script>
</body>
</html>
