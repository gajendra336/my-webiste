<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TechZone - Electronics Store</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Arial', sans-serif;
        }
        
        body {
            background-color: #f5f5f5;
            color: #333;
        }
        
        header {
            background-color: #2c3e50;
            color: white;
            padding: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .logo {
            font-size: 1.8rem;
            font-weight: bold;
        }
        
        nav ul {
            display: flex;
            list-style: none;
        }
        
        nav ul li {
            margin-left: 1.5rem;
        }
        
        nav ul li a {
            color: white;
            text-decoration: none;
        }
        
        .hero {
            background-image: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('electronics-banner.jpg');
            background-size: cover;
            height: 400px;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
        }
        
        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
        }
        
        .hero button {
            background-color: #e74c3c;
            color: white;
            border: none;
            padding: 0.8rem 1.5rem;
            font-size: 1.2rem;
            cursor: pointer;
            border-radius: 5px;
        }
        
        .categories {
            padding: 2rem;
            text-align: center;
        }
        
        .category-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .category-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            transition: transform 0.3s;
        }
        
        .category-card:hover {
            transform: translateY(-5px);
        }
        
        .category-card img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }
        
        .category-card h3 {
            padding: 1rem;
        }
        
        .featured {
            padding: 2rem;
            background-color: #ecf0f1;
        }
        
        .product-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
            gap: 1.5rem;
            margin-top: 2rem;
        }
        
        .product-card {
            background-color: white;
            border-radius: 8px;
            overflow: hidden;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
        }
        
        .product-card img {
            width: 100%;
            height: 180px;
            object-fit: contain;
            padding: 1rem;
            background-color: #f9f9f9;
        }
        
        .product-info {
            padding: 1rem;
        }
        
        .product-info h3 {
            margin-bottom: 0.5rem;
        }
        
        .price {
            color: #e74c3c;
            font-weight: bold;
            font-size: 1.2rem;
            margin: 0.5rem 0;
        }
        
        .add-to-cart {
            background-color: #3498db;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            width: 100%;
            cursor: pointer;
            border-radius: 5px;
        }
        
        footer {
            background-color: #2c3e50;
            color: white;
            padding: 2rem;
            text-align: center;
        }
        
        .footer-links {
            display: flex;
            justify-content: center;
            margin: 1rem 0;
        }
        
        .footer-links a {
            color: white;
            margin: 0 1rem;
            text-decoration: none;
        }
    </style>
</head>
<body>
    <header>
        <div class="logo">TechZone</div>
        <nav>
            <ul>
                <li><a href="#">Home</a></li>
                <li><a href="#">Products</a></li>
                <li><a href="#">Categories</a></li>
                <li><a href="#">Deals</a></li>
                <li><a href="#">Contact</a></li>
                <li><a href="#">Cart (0)</a></li>
            </ul>
        </nav>
    </header>
    
    <section class="hero">
        <h1>Latest Tech Gadgets</h1>
        <p>Up to 30% off on selected items</p>
        <button>Shop Now</button>
    </section>
    
    <section class="categories">
        <h2>Shop by Category</h2>
        <div class="category-grid">
            <div class="category-card">
                <img src="smartphones.jpg" alt="Smartphones">
                <h3>Smartphones</h3>
            </div>
            <div class="category-card">
                <img src="laptops.jpg" alt="Laptops">
                <h3>Laptops</h3>
            </div>
            <div class="category-card">
                <img src="tv.jpg" alt="TVs">
                <h3>TVs</h3>
            </div>
            <div class="category-card">
                <img src="audio.jpg" alt="Audio">
                <h3>Audio</h3>
            </div>
            <div class="category-card">
                <img src="cameras.jpg" alt="Cameras">
                <h3>Cameras</h3>
            </div>
        </div>
    </section>
    
    <section class="featured">
        <h2>Featured Products</h2>
        <div class="product-grid">
            <div class="product-card">
                <img src="product1.jpg" alt="Smartphone X">
                <div class="product-info">
                    <h3>Smartphone X</h3>
                    <p>Latest model with 128GB storage</p>
                    <div class="price">$699.99</div>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="product2.jpg" alt="Ultrabook Pro">
                <div class="product-info">
                    <h3>Ultrabook Pro</h3>
                    <p>Lightweight laptop with 16GB RAM</p>
                    <div class="price">$1,199.99</div>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="product3.jpg" alt="Wireless Earbuds">
                <div class="product-info">
                    <h3>Wireless Earbuds</h3>
                    <p>Noise cancelling with 24hr battery</p>
                    <div class="price">$149.99</div>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
            <div class="product-card">
                <img src="product4.jpg" alt="4K Smart TV">
                <div class="product-info">
                    <h3>4K Smart TV</h3>
                    <p>55" with HDR and streaming apps</p>
                    <div class="price">$599.99</div>
                    <button class="add-to-cart">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>
    
    <footer>
        <div class="logo">TechZone</div>
        <div class="footer-links">
            <a href="#">About Us</a>
            <a href="#">Privacy Policy</a>
            <a href="#">Terms of Service</a>
            <a href="#">Shipping Info</a>
            <a href="#">Contact Us</a>
        </div>
        <p>&copy; 2023 TechZone Electronics. All rights reserved.</p>
    </footer>
</body>
</html>
