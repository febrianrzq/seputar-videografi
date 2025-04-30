# seputar-videografi
<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Blog Videografi Futuristik</title>
  <style>
    :root {
      --bg-color: #0f0f0f;
      --text-color: #e0e0e0;
      --accent: #00ffe7;
      --card-bg: rgba(255, 255, 255, 0.05);
    }

    [data-theme="light"] {
      --bg-color: #f5f5f5;
      --text-color: #111;
      --card-bg: #fff;
    }

    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: var(--bg-color);
      color: var(--text-color);
      transition: background 0.5s, color 0.5s;
    }

    header {
      background: rgba(0, 0, 0, 0.8);
      padding: 20px 40px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      border-bottom: 1px solid #444;
    }

    header h1 {
      font-size: 1.8rem;
      color: var(--accent);
    }

    nav a {
      margin-left: 20px;
      color: var(--text-color);
      text-decoration: none;
    }

    nav a:hover {
      color: var(--accent);
    }

    .theme-toggle {
      cursor: pointer;
      padding: 8px 16px;
      border: 1px solid var(--accent);
      border-radius: 20px;
      background: transparent;
      color: var(--accent);
      transition: background 0.3s;
    }

    .theme-toggle:hover {
      background: var(--accent);
      color: #000;
    }

    .container {
      padding: 40px;
      display: grid;
      gap: 20px;
    }

    .article {
      background: var(--card-bg);
      padding: 20px;
      border-radius: 10px;
      display: flex;
      gap: 20px;
      align-items: center;
      transition: transform 0.3s, box-shadow 0.3s;
      box-shadow: 0 0 10px rgba(0, 255, 231, 0.1);
    }

    .article:hover {
      transform: translateY(-5px);
      box-shadow: 0 0 20px rgba(0, 255, 231, 0.3);
    }

    .article img {
      width: 120px;
      height: 80px;
      object-fit: cover;
      border-radius: 8px;
    }

    .article-content h2 {
      margin: 0 0 10px;
      color: var(--accent);
    }

    .footer {
      text-align: center;
      padding: 20px;
      border-top: 1px solid #444;
      font-size: 0.9rem;
      color: #aaa;
    }

    @media (max-width: 600px) {
      .article {
        flex-direction: column;
        text-align: center;
      }

      .article img {
        width: 100%;
        height: auto;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>VIDEOGRAFI 2100</h1>
    <div>
      <button class="theme-toggle" onclick="toggleTheme()">Mode Gelap/Terang</button>
      <nav>
        <a href="#">Beranda</a>
        <a href="#">Tentang</a>
        <a href="#">Kontak</a>
      </nav>
    </div>
  </header>

  <div class="container">
    <div class="article">
      <img src="https://via.placeholder.com/120x80?text=Dolly" alt="Teknik Kamera">
      <div class="article-content">
        <h2>Teknik Kamera: Dolly dan Tracking</h2>
        <p>Pelajari bagaimana teknik pergerakan kamera seperti dolly dan tracking dapat meningkatkan kualitas sinematik videomu.</p>
      </div>
    </div>

    <div class="article">
      <img src="https://via.placeholder.com/120x80?text=Lighting" alt="Lighting">
      <div class="article-content">
        <h2>Lighting Futuristik untuk Videografi</h2>
        <p>Penerangan adalah segalanya dalam videografi. Kenali teknik lighting modern yang digunakan dalam film futuristik.</p>
      </div>
    </div>

    <div class="article">
      <img src="https://via.placeholder.com/120x80?text=Grading" alt="Color Grading">
      <div class="article-content">
        <h2>Color Grading Sinematik</h2>
        <p>Warna membentuk suasana. Pelajari dasar-dasar color grading untuk memberi rasa profesional dalam karyamu.</p>
      </div>
    </div>
  </div>

  <div class="footer">
    &copy; 2025 Blog Videografi Futuristik. All rights reserved.
  </div>

  <script>
    function toggleTheme() {
      const currentTheme = document.documentElement.getAttribute("data-theme");
      if (currentTheme === "light") {
        document.documentElement.removeAttribute("data-theme");
      } else {
        document.documentElement.setAttribute("data-theme", "light");
      }
    }
  </script>

</body>
</html>
