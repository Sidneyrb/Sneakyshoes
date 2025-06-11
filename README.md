# Sneakyshoes<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>ShoeStore - Shop the Best Shoes</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0; padding: 0;
      background: #f9f9f9;
      color: #333;
    }
    header {
      background-color: #222;
      color: white;
      padding: 15px 30px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    header h1 {
      margin: 0;
      cursor: pointer;
    }
    nav a {
      color: white;
      text-decoration: none;
      margin-left: 20px;
      font-weight: bold;
    }
    nav a:hover {
      color: #ff4500;
    }
    .hero {
      background: url('https://images.unsplash.com/photo-1519741495434-6cfae9d37ed7?auto=format&fit=crop&w=1350&q=80') center/cover no-repeat;
      height: 350px;
      display: flex;
      justify-content: center;
      align-items: center;
      color: white;
      font-size: 2.5rem;
      font-weight: 700;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.7);
    }
    .container {
      max-width: 1100px;
      margin: 40px auto;
      padding: 0 20px;
    }
    h2 {
      text-align: center;
      margin-bottom: 30px;
    }
    .products {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(280px,1fr));
      gap: 25px;
    }
    .product {
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      display: flex;
      flex-direction: column;
      transition: transform 0.3s ease;
    }
    .product:hover {
      transform: scale(1.03);
    }
    .product img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }
    .product-details {
      padding: 15px 20px;
      flex-grow: 1;
      display: flex;
      flex-direction: column;
      justify-content: space-between;
    }
    .product-details h3 {
      margin: 0 0 10px;
      font-size: 1.3rem;
    }
    .product-details p {
      flex-grow: 1;
      font-size: 0.95rem;
      color: #666;
      margin-bottom: 15px;
    }
    .price {
      font-weight: 700;
      font-size: 1.2rem;
      color: #ff4500;
      margin-bottom: 15px;
    }
    button {
      background-color: #ff4500;
      border: none;
      color: white;
      padding: 12px 0;
      border-radius: 5px;
      font-weight: 700;
      cursor: pointer;
      transition: background-color 0.3s ease;
    }
    button:hover {
      background-color: #e03e00;
    }
    footer {
      background: #222;
      color: #bbb;
      text-align: center;
      padding: 20px 10px;
      margin-top: 60px;
      font-size: 0.9rem;
    }
    @media (max-width: 600px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }
      nav a {
        margin-left: 0;
        margin-right: 15px;
      }
    }
  </style>
</head>
<body>

  <header>
    <h1>ShoeStore</h1>
    <nav>
      <a href="#">Home</a>
      <a href="#">Shop</a>
      <a href="#">About</a>
      <a href="#">Contact</a>
    </nav>
  </header>

  <section class="hero">
    Step Into Style
  </section>

  <div class="container">
    <h2>Featured Shoes</h2>
    <div class="products">
      <div class="product">
        <img src="https://images.unsplash.com/photo-1600185367680-5c334e5cc8e0?auto=format&fit=crop&w=400&q=80" alt="Air Jordan 1 Retro" />
        <div class="product-details">
          <h3>Air Jordan 1 Retro</h3>
          <p>Classic silhouette, unmatched style. Perfect for any sneakerhead.</p>
          <div class="price">$180</div>
          <button>Add to Cart</button>
        </div>
      </div>

      <div class="product">
        <img src="https://images.unsplash.com/photo-1590080877777-858c9f14d9aa?auto=format&fit=crop&w=400&q=80" alt="Nike Air Max 270" />
        <div class="product-details">
          <h3>Nike Air Max 270</h3>
          <p>Innovative cushioning and sleek design for everyday comfort.</p>
          <div class="price">$150</div>
          <button>Add to Cart</button>
        </div>
      </div>

      <div class="product">
        <img src="https://images.unsplash.com/photo-1542291026-7eec264c27ff?auto=format&fit=crop&w=400&q=80" alt="Adidas Ultraboost" />
        <div class="product-details">
          <h3>Adidas Ultraboost</h3>
          <p>Run faster and further with the ultimate boost technology.</p>
          <div class="price">$180</div>
          <button>Add to Cart</button>
        </div>
      </div>
    </div>
  </div>

  <footer>
    &copy; 2025 ShoeStore. All rights reserved.
  </footer>

</body>
</html>
