# Thread-Memory-
clothing brand 
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Thread Memory</title>
  <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
  <style>
    /* ===== Global Styles ===== */
    * { box-sizing: border-box; margin: 0; padding: 0; }
    body {
      font-family: 'Roboto', sans-serif;
      background-color: #f7f7f7;
      color: #1a1a1a;
      line-height: 1.6;
    }
    a { text-decoration: none; color: inherit; }

    /* ===== Header ===== */
    header {
      background-color: #1a1a1a;
      color: #f7f7f7;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
      position: sticky;
      top: 0;
      z-index: 100;
    }
    header h1 {
      font-size: 2rem;
      letter-spacing: 2px;
      font-weight: 700;
    }
    nav a {
      margin-left: 1.5rem;
      font-weight: bold;
      transition: color 0.2s;
    }
    nav a:hover { color: #a0b0c0; }

    /* ===== Hero Section ===== */
    .hero {
      background-color: #a0b0c0;
      color: #1a1a1a;
      text-align: center;
      padding: 6rem 2rem;
    }
    .hero h2 {
      font-size: 3rem;
      margin-bottom: 1rem;
      letter-spacing: 2px;
      font-weight: 700;
      font-family: 'Arial Black', sans-serif;
    }
    .hero p {
      font-size: 1.2rem;
      opacity: 0.85;
    }

    /* ===== Collections ===== */
    .collections {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 2rem;
      padding: 3rem 2rem;
    }
    .product {
      background-color: #fff;
      padding: 1rem;
      text-align: center;
      border-radius: 10px;
      box-shadow: 0 2px 6px rgba(0,0,0,0.1);
      transition: transform 0.2s, box-shadow 0.2s;
    }
    .product:hover {
      transform: translateY(-5px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }
    .product img {
      width: 100%;
      height: auto;
      margin-bottom: 1rem;
      border-radius: 6px;
    }
    .product h3 { font-size: 1.2rem; margin-bottom: 0.5rem; }
    .product p { font-weight: bold; color: #1a1a1a; }

    /* ===== Lookbook ===== */
    .lookbook {
      padding: 3rem 2rem;
      text-align: center;
      background-color: #e3e3e3;
    }
    .lookbook h2 { font-size: 2.5rem; margin-bottom: 2rem; }
    .lookbook-images {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 1rem;
    }
    .lookbook-images img {
      width: 300px;
      border-radius: 8px;
      object-fit: cover;
    }

    /* ===== About ===== */
    .about {
      padding: 3rem 2rem;
      text-align: center;
    }
    .about h2 { font-size: 2.5rem; margin-bottom: 1rem; }
    .about p { max-width: 700px; margin: 0 auto; opacity: 0.85; }

    /* ===== Contact ===== */
    .contact {
      padding: 3rem 2rem;
      text-align: center;
      background-color: #a0b0c0;
      color: #1a1a1a;
    }
    .contact input, .contact textarea {
      padding: 0.8rem;
      margin: 0.5rem 0;
      width: 300px;
      border-radius: 5px;
      border: none;
    }
    .contact button {
      padding: 0.8rem 2rem;
      margin-top: 1rem;
      border: none;
      border-radius: 5px;
      background-color: #1a1a1a;
      color: #f7f7f7;
      cursor: pointer;
      font-weight: bold;
      transition: background 0.2s;
    }
    .contact button:hover { background-color: #333; }

    /* ===== Footer ===== */
    footer {
      background-color: #1a1a1a;
      color: #f7f7f7;
      text-align: center;
      padding: 2rem;
      margin-top: 2rem;
      font-size: 0.9rem;
    }

    @media(max-width: 600px) {
      .hero h2 { font-size: 2.2rem; }
      .lookbook-images img { width: 90%; }
      .contact input, .contact textarea { width: 90%; }
    }
  </style>
</head>
<body>

  <!-- ===== Header ===== -->
  <header>
    <h1>THREAD MEMORY</h1>
    <nav>
      <a href="#shop">Shop</a>
      <a href="#lookbook">Lookbook</a>
      <a href="#about">About</a>
      <a href="#contact">Contact</a>
    </nav>
  </header>

  <!-- ===== Hero ===== -->
  <section class="hero">
    <h2>Low Effort. High Vibe.</h2>
    <p>Oversized tees, faded graphics, Y2K-inspired streetwear for the effortless skater aesthetic.</p>
  </section>

  <!-- ===== Collections / Shop ===== -->
  <section id="shop" class="collections">
    <div class="product">
      <img src="tee1.jpg" alt="Faded Tee">
      <h3>Faded Graphic Tee</h3>
      <p>$35</p>
    </div>
    <div class="product">
      <img src="hoodie1.jpg" alt="Oversized Hoodie">
      <h3>Oversized Hoodie</h3>
      <p>$60</p>
    </div>
    <div class="product">
      <img src="accessory1.jpg" alt="Chain Accessory">
      <h3>Chain Accessory</h3>
      <p>$15</p>
    </div>
  </section>

  <!-- ===== Lookbook ===== -->
  <section id="lookbook" class="lookbook">
    <h2>Lookbook</h2>
    <div class="lookbook-images">
      <img src="look1.jpg" alt="Skater Outfit 1">
      <img src="look2.jpg" alt="Skater Outfit 2">
      <img src="look3.jpg" alt="Skater Outfit 3">
    </div>
  </section>

  <!-- ===== About ===== -->
  <section id="about" class="about">
    <h2>About Thread Memory</h2>
    <p>Thread Memory is a streetwear brand inspired by thrifted style, Y2K nostalgia, and skater culture. We focus on oversized tees, faded graphics, and effortless outfits for the next generation of low-effort-high-vibe style.</p>
  </section>

  <!-- ===== Contact ===== -->
  <section id="contact" class="contact">
    <h2>Contact / Newsletter</h2>
    <p>Join the Thread Memory Club</p>
    <form>
      <input type="text" placeholder="Name" required><br>
      <input type="email" placeholder="Email" required><br>
      <textarea placeholder="Message" rows="4"></textarea><br>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- ===== Footer ===== -->
  <footer>
    <p>© 2026 Thread Memory | Follow us on TikTok & Instagram</p>
  </footer>

</body>
</html>
