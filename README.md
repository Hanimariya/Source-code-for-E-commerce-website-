# Source-code-for-E-commerce-website-
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>E-Commerce Platform</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header class="header">
    <div class="container">
      <h1 class="logo">E-Commerce</h1>
      <nav>
        <ul class="nav-links">
          <li><a href="#">Home</a></li>
          <li><a href="#">Products</a></li>
          <li><a href="#">Cart</a></li>
          <li><a href="#">Login</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main class="main">
    <div class="container">
      <h2 class="title">Our Products</h2>
      <div class="products-grid">
        <!-- Product Card -->
        <div class="product-card">
          <img src="https://via.placeholder.com/150" alt="Product Image" class="product-img">
          <h3 class="product-name">Product Name</h3>
          <p class="product-price">$50.00</p>
          <button class="btn">Add to Cart</button>
        </div>
        <!-- Duplicate Product Cards for more items -->
        <div class="product-card">
          <img src="https://via.placeholder.com/150" alt="Product Image" class="product-img">
          <h3 class="product-name">Another Product</h3>
          <p class="product-price">$75.00</p>
          <button class="btn">Add to Cart</button>
        </div>
        <!-- More Product Cards -->
      </div>
    </div>
  </main>

  <footer class="footer">
    <div class="container">
      <p>&copy; 2024 E-Commerce Platform. All Rights Reserved.</p>
    </div>
  </footer>
</body>
</html>

CSS CODE 

/* Global Styles */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: Arial, sans-serif;
}

body {
  line-height: 1.6;
  color: #333;
  background-color: #f9f9f9;
}

.container {
  width: 90%;
  max-width: 1200px;
  margin: 0 auto;
}

/* Header */
.header {
  background-color: #333;
  color: #fff;
  padding: 1rem 0;
}

.header .logo {
  font-size: 2rem;
  font-weight: bold;
}

.nav-links {
  list-style: none;
  display: flex;
  gap: 1rem;
}

.nav-links a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s ease;
}

.nav-links a:hover {
  color: #ffa500;
}

/* Main */
.main {
  padding: 2rem 0;
}

.title {
  text-align: center;
  font-size: 2rem;
  margin-bottom: 1.5rem;
}

.products-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 1.5rem;
}

.product-card {
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 5px;
  overflow: hidden;
  text-align: center;
  padding: 1rem;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.product-card:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
}

.product-img {
  max-width: 100%;
  height: auto;
  margin-bottom: 1rem;
}

.product-name {
  font-size: 1.2rem;
  margin-bottom: 0.5rem;
}

.product-price {
  font-size: 1rem;
  color: #555;
  margin-bottom: 1rem;
}

.btn {
  background-color: #333;
  color: #fff;
  padding: 0.5rem 1rem;
  border: none;
  border-radius: 3px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.btn:hover {
  background-color: #ffa500;
}

/* Footer */
.footer {
  background-color: #333;
  color: #fff;
  text-align: center;
  padding: 1rem 0;
  margin-top: 2rem;
}
