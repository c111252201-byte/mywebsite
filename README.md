# mywebsite
<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>黃柏彰的個人網頁</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: 'Arial', sans-serif;
      background: linear-gradient(135deg, #ff7e5f, #feb47b); /* 背景漸變 */
      color: #333;
    }

    .container {
      width: 90%;
      max-width: 800px;
      margin: 0 auto;
      padding: 40px 0;
    }

    header {
      text-align: center;
      margin-bottom: 30px;
    }

    header h1 {
      font-size: 36px;
      color: #fff;
      letter-spacing: 2px;
      text-shadow: 2px 2px 8px rgba(0, 0, 0, 0.4); /* 標題陰影 */
    }

    nav {
      text-align: center;
      margin-bottom: 30px;
    }

    nav button {
      background-color: #3498db;
      color: white;
      border: none;
      padding: 12px 25px;
      margin: 0 15px;
      border-radius: 25px;
      cursor: pointer;
      font-size: 16px;
      transition: all 0.3s ease;
      box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); /* 按鈕陰影 */
    }

    nav button:hover {
      background-color: #2980b9;
      transform: translateY(-3px); /* 按鈕懸停效果 */
      box-shadow: 0 6px 15px rgba(0, 0, 0, 0.15); /* 增強懸停陰影 */
    }

    main {
      padding: 20px;
      background-color: #fff;
      border-radius: 15px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1); /* 卡片陰影 */
    }

    .page {
      display: none;
    }

    .page.active {
      display: block;
    }

    section h2 {
      font-size: 28px;
      margin-bottom: 15px;
      color: #333;
    }

    section p {
      font-size: 18px;
      line-height: 1.6;
      margin-bottom: 10px;
      color: #555;
    }

    .portfolio-images {
      text-align: center;
      margin-top: 20px;
    }

    .portfolio-images img {
      max-width: 80%;
      height: auto;
      border-radius: 10px;
      box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1); /* 圖片陰影 */
      transition: all 0.3s ease;
    }

    .portfolio-images img:hover {
      transform: scale(1.05); /* 圖片懸停放大效果 */
    }

    ul.social-links {
      list-style: none;
      padding: 0;
      margin-top: 15px;
    }

    ul.social-links li {
      margin: 15px 0;
    }

    ul.social-links a {
      font-size: 18px;
      color: #3498db;
      text-decoration: none;
      transition: all 0.3s ease;
    }

    ul.social-links a:hover {
      color: #2980b9;
      text-decoration: underline;
    }

    /* 小螢幕 (響應式設計) */
    @media (max-width: 768px) {
      .container {
        width: 95%;
      }

      header h1 {
        font-size: 28px;
      }

      nav button {
        font-size: 14px;
        padding: 10px 20px;
      }

      .portfolio-images img {
        max-width: 100%;
      }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <h1>黃柏彰的個人網頁</h1>
    </header>

    <nav>
      <button onclick="showPage('intro')">自我介紹</button>
      <button onclick="showPage('portfolio')">個人作品</button>
      <button onclick="showPage('social')">社群媒體資訊</button>
    </nav>

    <main>
      <!-- 自我介紹 -->
      <section id="intro" class="page active">
        <h2>自我介紹</h2>
        <p>網路應用設計</p>
        <p>進修部四子四乙</p>
        <p>學號：C111252201</p>
        <p>黃柏彰</p>
      </section>

      <!-- 個人作品 -->
      <section id="portfolio" class="page">
        <h2>個人作品</h2>
        <div class="portfolio-images">
          <img src="err_0807.jpg" alt="個人作品展示圖片">
        </div>
      </section>

      <!-- 社群媒體資訊 -->
      <section id="social" class="page">
        <h2>社群媒體資訊</h2>
        <ul class="social-links">
          <li>Instagram: <a href="https://instagram.com/err_0807" target="_blank">@err_0807</a></li>
        </ul>
      </section>
    </main>
  </div>

  <script>
    // 切換分頁顯示
    function showPage(pageId) {
      const pages = document.querySelectorAll('.page');
      pages.forEach(page => {
        page.classList.remove('active');
      });
      document.getElementById(pageId).classList.add('active');
    }
  </script>
</body>
</html>

  <script>
    // 切換分頁顯示
    function showPage(pageId) {
      const pages = document.querySelectorAll('.page');
      pages.forEach(page => {
        page.classList.remove('active');
      });
      document.getElementById(pageId).classList.add('active');
    }
  </script>
</body>
</html>

