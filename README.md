# Mahesh
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <meta name="theme-color" content="#111827" />

  <title>Bhagvan Baba Sofa & Furniture</title>

  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    html {
      scroll-behavior: smooth;
    }

    body {
      font-family: Arial, Helvetica, sans-serif;
      background: #f7f7f5;
      color: #1f2937;
      line-height: 1.5;
    }

    img {
      width: 100%;
      display: block;
    }

    button,
    input,
    textarea {t
      font: inherit;
    }

    /* ================= HEADER ================= */

    header {
      position: sticky;
      top: 0;
      z-index: 1000;
      background: rgba(255,255,255,0.95);
      backdrop-filter: blur(12px);
      border-bottom: 1px solid #e5e7eb;
    }

    .nav {
      max-width: 1200px;
      margin: auto;
      min-height: 68px;
      padding: 10px 18px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 15px;
    }

    .logo {
      font-size: 18px;
      font-weight: 800;
      color: #111827;
      text-decoration: none;
      line-height: 1.1;
    }

    .logo span {
      display: block;
      color: #a16207;
      font-size: 11px;
      margin-top: 4px;
      letter-spacing: 1px;
      text-transform: uppercase;
    }

    .cart-btn {
      border: 0;
      background: #111827;
      color: white;
      border-radius: 50px;
      padding: 10px 15px;
      cursor: pointer;
      font-weight: 700;
    }

    /* ================= HERO ================= */

    .hero {
      position: relative;
      min-height: 72vh;
      display: flex;
      align-items: center;
      overflow: hidden;
      background: #111;
    }

    .hero img {
      position: absolute;
      inset: 0;
      height: 100%;
      width: 100%;
      object-fit: cover;
      opacity: 0.78;
    }

    .hero-overlay {
      position: absolute;
      inset: 0;
      background:
        linear-gradient(
          90deg,
          rgba(0,0,0,0.78),
          rgba(0,0,0,0.38),
          rgba(0,0,0,0.18)
        );
    }

    .hero-content {
      position: relative;
      z-index: 2;
      max-width: 1200px;
      width: 100%;
      margin: auto;
      padding: 70px 22px;
      color: white;
    }

    .hero-badge {
      display: inline-block;
      padding: 7px 13px;
      border: 1px solid rgba(255,255,255,.45);
      border-radius: 50px;
      font-size: 12px;
      margin-bottom: 18px;
      background: rgba(255,255,255,.08);
    }

    .hero h1 {
      font-size: clamp(38px, 9vw, 76px);
      line-height: 0.98;
      max-width: 760px;
      letter-spacing: -2px;
      margin-bottom: 20px;
    }

    .hero p {
      font-size: clamp(17px, 3vw, 23px);
      color: #f3f4f6;
      max-width: 580px;
      margin-bottom: 30px;
    }

    .hero-buttons {
      display: flex;
      flex-wrap: wrap;
      gap: 12px;
    }

    .btn {
      display: inline-flex;
      align-items: center;
      justify-content: center;
      padding: 14px 23px;
      border-radius: 50px;
      text-decoration: none;
      border: 0;
      cursor: pointer;
      font-weight: 800;
      transition: .2s ease;
    }

    .btn-primary {
      background: #d97706;
      color: white;
    }

    .btn-primary:hover {
      background: #b45309;
      transform: translateY(-2px);
    }

    .btn-light {
      background: white;
      color: #111827;
    }

    /* ================= GENERAL ================= */

    .section {
      max-width: 1200px;
      margin: auto;
      padding: 70px 18px;
    }

    .section-heading {
      margin-bottom: 28px;
    }

    .eyebrow {
      color: #a16207;
      font-size: 13px;
      font-weight: 800;
      text-transform: uppercase;
      letter-spacing: 2px;
      margin-bottom: 8px;
    }

    .section-heading h2 {
      font-size: clamp(28px, 5vw, 45px);
      color: #111827;
      line-height: 1.1;
    }

    .section-heading p {
      color: #6b7280;
      margin-top: 10px;
    }

    /* ================= PRODUCT CAROUSEL ================= */

    .carousel-wrapper {
      position: relative;
    }

    .products {
      display: flex;
      gap: 18px;
      overflow-x: auto;
      scroll-snap-type: x mandatory;
      padding: 5px 2px 25px;
      scrollbar-width: none;
    }

    .products::-webkit-scrollbar {
      display: none;
    }

    .product-card {
      flex: 0 0 84%;
      max-width: 340px;
      scroll-snap-align: start;
      background: white;
      border-radius: 20px;
      overflow: hidden;
      border: 1px solid #e5e7eb;
      box-shadow: 0 10px 30px rgba(0,0,0,.06);
    }

    .product-image {
      aspect-ratio: 1 / 1;
      overflow: hidden;
      background: #eee;
    }

    .product-image img {
      height: 100%;
      object-fit: cover;
      transition: .4s ease;
    }

    .product-card:hover .product-image img {
      transform: scale(1.05);
    }

    .product-info {
      padding: 18px;
    }

    .product-info h3 {
      font-size: 19px;
      margin-bottom: 8px;
      color: #111827;
    }

    .product-description {
      color: #6b7280;
      font-size: 14px;
      min-height: 42px;
      margin-bottom: 14px;
    }

    .product-bottom {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 10px;
    }

    .price {
      font-size: 20px;
      font-weight: 900;
      color: #a16207;
    }

    .add-btn {
      background: #111827;
      color: white;
      border: 0;
      padding: 10px 14px;
      border-radius: 10px;
      cursor: pointer;
      font-weight: 700;
    }

    .add-btn:hover {
      background: #374151;
    }

    .carousel-controls {
      display: flex;
      justify-content: flex-end;
      gap: 8px;
      margin-bottom: 12px;
    }

    .carousel-control {
      width: 42px;
      height: 42px;
      border: 1px solid #ddd;
      border-radius: 50%;
      background: white;
      cursor: pointer;
      font-size: 18px;
    }

    /* ================= FEATURES ================= */

    .features {
      background: #111827;
      color: white;
    }

    .feature-grid {
      max-width: 1200px;
      margin: auto;
      padding: 55px 18px;
      display: grid;
      grid-template-columns: repeat(1, 1fr);
      gap: 20px;
    }

    .feature {
      padding: 24px;
      border: 1px solid rgba(255,255,255,.12);
      border-radius: 18px;
      background: rgba(255,255,255,.05);
    }

    .feature-icon {
      font-size: 28px;
      margin-bottom: 12px;
    }

    .feature h3 {
      margin-bottom: 7px;
    }

    .feature p {
      color: #cbd5e1;
      font-size: 14px;
    }

    /* ================= CART ================= */

    .cart-section {
      background: #f0f0ed;
    }

    .cart-box {
      background: white;
      border-radius: 20px;
      padding: 22px;
      border: 1px solid #e5e7eb;
    }

    .cart-empty {
      color: #6b7280;
      text-align: center;
      padding: 15px;
    }

    .cart-item {
      display: flex;
      justify-content: space-between;
      gap: 15px;
      padding: 13px 0;
      border-bottom: 1px solid #eee;
    }

    .cart-item-name {
      font-weight: 700;
    }

    .cart-item-price {
      color: #a16207;
      font-weight: 800;
    }

    .remove-btn {
      border: 0;
      background: transparent;
      color: #dc2626;
      cursor: pointer;
      font-size: 12px;
    }

    .cart-total {
      display: flex;
      justify-content: space-between;
      margin-top: 20px;
      font-size: 20px;
      font-weight: 900;
    }

    /* ================= ORDER FORM ================= */

    .order-container {
      display: grid;
      gap: 30px;
    }

    .order-info {
      background: #111827;
      color: white;
      padding: 30px;
      border-radius: 22px;
    }

    .order-info h2 {
      font-size: 30px;
      margin-bottom: 12px;
    }

    .order-info p {
      color: #cbd5e1;
    }

    .contact-line {
      margin-top: 20px;
      padding: 13px 0;
      border-top: 1px solid rgba(255,255,255,.12);
    }

    form {
      background: white;
      border-radius: 22px;
      padding: 22px;
      border: 1px solid #e5e7eb;
    }

    .form-group {
      margin-bottom: 17px;
    }

    label {
      display: block;
      margin-bottom: 7px;
      font-size: 14px;
      font-weight: 700;
    }

    input,
    textarea {
      width: 100%;
      border: 1px solid #d1d5db;
      border-radius: 11px;
      padding: 13px;
      outline: none;
      background: #fafafa;
    }

    input:focus,
    textarea:focus {
      border-color: #a16207;
      background: white;
    }

    textarea {
      min-height: 110px;
      resize: vertical;
    }

    .submit-btn {
      width: 100%;
      border: 0;
      padding: 15px;
      border-radius: 12px;
      background: #a16207;
      color: white;
      cursor: pointer;
      font-weight: 900;
    }

    /* ================= FOOTER ================= */

    footer {
      background: #0b0f19;
      color: #cbd5e1;
      padding: 35px 18px;
      text-align: center;
    }

    footer h3 {
      color: white;
      margin-bottom: 7px;
    }

    footer a {
      color: #fbbf24;
      text-decoration: none;
    }

    /* ================= WHATSAPP ================= */

    .whatsapp {
      position: fixed;
      right: 18px;
      bottom: 18px;
      z-index: 9999;
      width: 58px;
      height: 58px;
      border-radius: 50%;
      background: #25D366;
      color: white;
      display: flex;
      align-items: center;
      justify-content: center;
      text-decoration: none;
      font-size: 27px;
      box-shadow: 0 8px 25px rgba(0,0,0,.25);
    }

    /* ================= DESKTOP ================= */

    @media (min-width: 700px) {
      .nav {
        padding-left: 28px;
        padding-right: 28px;
      }

      .product-card {
        flex-basis: 31%;
      }

      .feature-grid {
        grid-template-columns: repeat(3, 1fr);
      }

      .order-container {
        grid-template-columns: .8fr 1.2fr;
        align-items: start;
      }

      .section {
        padding-top: 90px;
        padding-bottom: 90px;
      }
    }
  </style>
</head>

<body>

  <!-- ================= HEADER ================= -->

  <header>
    <nav class="nav">
      <a href="#" class="logo">
        Bhagvan Baba
        <span>Sofa & Furniture</span>
      </a>

      <button class="cart-btn" onclick="scrollToCart()">
        🛒 Cart <span id="cartCount">0</span>
      </button>
    </nav>
  </header>


  <!-- ================= HERO ================= -->

  <section class="hero">

    <img
      src="https://i.ibb.co/35pJfJhX/IMG-20260214-WA0006.jpg"
      alt="Bhagvan Baba Sofa and Furniture"
    />

    <div class="hero-overlay"></div>

    <div class="hero-content">

      <div class="hero-badge">
        QUALITY • COMFORT • STYLE
      </div>

      <h1>
        Furniture made for the way you live.
      </h1>

      <p>
        <strong>Designed for rest. Built for life.</strong><br>
        Discover stylish sofas and furniture for your home.
      </p>

      <div class="hero-buttons">
        <a href="#products" class="btn btn-primary">
          Shop Now →
        </a>

        <a href="#order" class="btn btn-light">
          Place Order
        </a>
      </div>

    </div>
  </section>


  <!-- ================= PRODUCTS ================= -->

  <section class="section" id="products">

    <div class="section-heading">
      <div class="eyebrow">Our Collection</div>
      <h2>Furniture you'll love.</h2>
      <p>
        Browse our selected sofa and furniture collection.
      </p>
    </div>

    <div class="carousel-wrapper">

      <div class="carousel-controls">
        <button
          class="carousel-control"
          onclick="scrollProducts(-1)"
        >
          ←
        </button>

        <button
          class="carousel-control"
          onclick="scrollProducts(1)"
        >
          →
        </button>
      </div>

      <div class="products" id="productCarousel">

        <!-- PRODUCT 1 -->

        <article class="product-card">

          <div class="product-image">
            <img
              src="https://i.ibb.co/dJsFtrYJ/5cc72dcdcb769463aa46f4da601a934c.jpg"
              alt="Premium Sofa"
            />
          </div>

          <div class="product-info">

            <h3>Premium Sofa</h3>

            <p class="product-description">
              Elegant and comfortable sofa for modern homes.
            </p>

            <div class="product-bottom">

              <div class="price">
                Price on request
              </div>

              <button
                class="add-btn"
                onclick="addToCart('Premium Sofa')"
              >
                Add to Cart
              </button>

            </div>

          </div>
        </article>


        <!-- PRODUCT 2 -->

        <article class="product-card">

          <div class="product-image">
            <img
              src="https://i.ibb.co/ZpWJyr75/5bd768b7ab2df091a44309e9caa5793a.jpg"
              alt="Designer Sofa"
            />
          </div>

          <div class="product-info">

            <h3>Designer Sofa</h3>

            <p class="product-description">
              Stylish design with comfort for everyday living.
            </p>

            <div class="product-bottom">

              <div class="price">
                Price on request
              </div>

              <button
                class="add-btn"
                onclick="addToCart('Designer Sofa')"
              >
                Add to Cart
              </button>

            </div>

          </div>
        </article>


        <!-- PRODUCT 3 -->

        <article class="product-card">

          <div class="product-image">
            <img
              src="https://i.ibb.co/3yt55PBg/ee1376e022ca268f6d014921be4e97d4.jpg"
              alt="Modern Furniture"
            />
          </div>

          <div class="product-info">

            <h3>Modern Furniture</h3>

            <p class="product-description">
              Contemporary furniture designed for your home.
            </p>

            <div class="product-bottom">

              <div class="price">
                Price on request
              </div>

              <button
                class="add-btn"
                onclick="addToCart('Modern Furniture')"
              >
                Add to Cart
              </button>

            </div>

          </div>
        </article>


        <!-- PRODUCT 4 -->

        <article class="product-card">

          <div class="product-image">
            <img
              src="https://i.ibb.co/B2NQ7VWb/adb11d1212eff428ddafce03b51aa8e2.jpg"
              alt="Premium Furniture"
            />
          </div>

          <div class="product-info">

            <h3>Premium Furniture</h3>

            <p class="product-description">
              Quality furniture with a premium look and feel.
            </p>

            <div class="product-bottom">

              <div class="price">
                Price on request
              </div>

              <button
                class="add-btn"
                onclick="addToCart('Premium Furniture')"
              >
                Add to Cart
              </button>

            </div>

          </div>
        </article>

      </div>
    </div>

  </section>


  <!-- ================= FEATURES ================= -->

  <section class="features">

    <div class="feature-grid">

      <div class="feature">
        <div class="feature-icon">🛋️</div>
        <h3>Comfort First</h3>
        <p>
          Furniture selected with everyday comfort and home living in mind.
        </p>
      </div>

      <div class="feature">
        <div class="feature-icon">✨</div>
        <h3>Modern Designs</h3>
        <p>
          Stylish designs that can complement different home interiors.
        </p>
      </div>

      <div class="feature">
        <div class="feature-icon">📞</div>
        <h3>Easy Ordering</h3>
        <p>
          Add your furniture to the cart and send your order enquiry easily.
        </p>
      </div>

    </div>

  </section>


  <!-- ================= CART ================= -->

  <section class="section cart-section" id="cart">

    <div class="section-heading">
      <div class="eyebrow">Your Selection</div>
      <h2>Shopping Cart</h2>
      <p>
        Review your selected furniture before placing your order.
      </p>
    </div>

    <div class="cart-box">

      <div id="cartItems">
        <div class="cart-empty">
          Your cart is empty.
        </div>
      </div>

      <div class="cart-total">
        <span>Selected Items</span>
        <span id="cartTotal">0</span>
      </div>

    </div>

  </section>


  <!-- ================= ORDER ================= -->

  <section class="section" id="order">

    <div class="order-container">

      <div class="order-info">

        <div class="eyebrow">
          Place Your Order
        </div>

        <h2>
          Ready to make your home more comfortable?
        </h2>

        <p>
          Fill in your details and send your furniture enquiry directly
          through your email app.
        </p>

        <div class="contact-line">
          📧 <strong>Email</strong><br>
          <a
            href="mailto:mrakh8832@gmail.com"
            style="color:#fbbf24;"
          >
            mrakh8832@gmail.com
          </a>
        </div>

        <div class="contact-line">
          💬 <strong>WhatsApp</strong><br>
          Contact us for product availability and pricing.
        </div>

      </div>


      <form id="orderForm">

        <div class="form-group">

          <label for="customerName">
            Customer Name *
          </label>

          <input
            type="text"
            id="customerName"
            placeholder="Enter your full name"
            required
          />

        </div>


        <div class="form-group">

          <label for="phone">
            Phone Number *
          </label>

          <input
            type="tel"
            id="phone"
            placeholder="Enter your phone number"
            required
          />

        </div>


        <div class="form-group">

          <label for="email">
            Email Address
          </label>

          <input
            type="email"
            id="email"
            placeholder="Enter your email"
          />

        </div>


        <div class="form-group">

          <label for="items">
            Selected Items *
          </label>

          <textarea
            id="items"
            placeholder="Your selected furniture will appear here..."
            required
          ></textarea>

        </div>


        <div class="form-group">

          <label for="address">
            Delivery / Address Details
          </label>

          <textarea
            id="address"
            placeholder="Enter your address or delivery requirements"
          ></textarea>

        </div>


        <button
          type="submit"
          class="submit-btn"
        >
          📧 Send Order by Email
        </button>

      </form>

    </div>

  </section>


  <!-- ================= FOOTER ================= -->

  <footer>

    <h3>
      Bhagvan Baba Sofa and Furniture
    </h3>

    <p>
      Designed for rest. Built for life.
    </p>

    <p style="margin-top:12px;">
      Email:
      <a href="mailto:mrakh8832@gmail.com">
        mrakh8832@gmail.com
      </a>
    </p>

    <p style="margin-top:15px;font-size:13px;">
      © 2026 Bhagvan Baba Sofa and Furniture. All rights reserved.
    </p>

  </footer>


  <!-- ================= WHATSAPP ================= -->

  <a
    class="whatsapp"
    href="https://wa.me/99999999"
    target="_blank"
    
