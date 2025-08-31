# Ex02 Commercial Website
## Date:

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM

## index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Gadget World</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

<!-- Navigation -->
<nav>
    <div class="logo">Gadget World</div>
    
    <div class="menu">
        <a href="#about">About</a>
        <a href="#products">Products</a>
        <a href="#contact">Contact</a>
    </div>

    <div class="nav-extra">
        <input type="text" placeholder="Search gadgets...">
        <a href="#cart" class="cart-btn">🛒</a>
        <a href="#login" class="user-btn">👤</a>
    </div>
</nav>

<!-- Hero Section -->
<header class="hero">
    <div class="hero-content">
        <h1>Latest Gadgets at Best Prices</h1>
        <p>Discover cutting-edge technology and stylish electronics for your lifestyle.</p>
        <div class="hero-buttons">
            <a href="#products" class="btn">Shop Now</a>
            <a href="#about" class="btn btn-light">Learn More</a>
        </div>
    </div>
</header>

<!-- About Section -->
<section id="about">
    <h2>About Us</h2>
    <p>We bring you the latest gadgets from top brands around the world. From smartphones to smart home devices, we have it all.</p>
</section>

<!-- Featured Products -->
<section id="featured">
    <h2>Featured Gadgets</h2>
    <div class="featured-products">
        <div class="product">
            <img src="smartwatch.jpg" alt="Smartwatch">
            <span class="badge">New</span>
            <h3>Smartwatch</h3>
        </div>
        <div class="product">
            <img src="camera.jpg" alt="Camera">
            <span class="badge">Hot</span>
            <h3>Camera</h3>
        </div>
        <div class="product">
            <img src="drone.jpg" alt="Drone">
            <span class="badge">Sale</span>
            <h3>Drone</h3>
        </div>
    </div>
</section>

<!-- Products Grid -->
<section id="products">
    <h2>Our Products</h2>
    <div class="products">
        <div class="product">
            <img src="ac.jpg" alt="Air Conditioner">
            <h3>Air Conditioner</h3>
            <p>Energy-efficient cooling for ultimate comfort.</p>
        </div>
        <div class="product">
            <img src="laptop.jpg" alt="Laptop">
            <h3>High-Performance Laptop</h3>
            <p>Power and portability for work and play.</p>
        </div>
        <div class="product">
            <img src="smartphone.jpg" alt="Smartphone">
            <h3>Latest Smartphone</h3>
            <p>Stay connected with lightning speed and style.</p>
        </div>
        <div class="product">
            <img src="earpots.jpg" alt="Headphones">
            <h3>Noise-Cancelling Headphones</h3>
            <p>Experience pure sound with zero distractions.</p>
        </div>
    </div>
</section>

<!-- CTA Section -->
<section id="cta">
    <div class="cta-content">
        <img src="subcribe.jpg" alt="Subscribe">
        <div class="cta-text">
            <h2>Subscribe & Save!</h2>
            <p>Sign up for our newsletter and get the latest gadget deals.</p>
            <form>
                <input type="email" placeholder="Enter your email">
                <button type="submit">Subscribe</button>
            </form>
        </div>
    </div>
</section>

<!-- Testimonials -->
<section id="testimonials">
    <h2>What Our Customers Say</h2>
    <div class="testimonial">
        <img src="person1.jpg" alt="Alex J.">
        <p>"Amazing products and fast delivery! Highly recommended."</p>
        <h4>- Alex J.</h4>
    </div>
    <div class="testimonial">
        <img src="person 2.jpg" alt="Priya K.">
        <p>"The gadgets are top quality, and the prices are unbeatable."</p>
        <h4>- Priya K.</h4>
    </div>
</section>

<!-- Contact -->
<section id="contact">
    <h2>Contact Us</h2>
    <form>
        <input type="text" placeholder="Your Name" required>
        <input type="email" placeholder="Your Email" required>
        <textarea rows="4" placeholder="Your Message" required></textarea>
        <button type="submit">Send</button>
    </form>
</section>

<!-- Footer -->
<footer>
    <p>&copy; 2025 Gadget World. All rights reserved.</p>
    <div class="social">
        <a href="#"><img src="facebook.jpg" alt="Facebook"></a>
        <a href="#"><img src="insta.jpg" alt="Instagram"></a>
        <a href="#"><img src="twit.jpg" alt="Twitter"></a>
    </div>
</footer>

</body>
</html>
```
## style.css
```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: linear-gradient(135deg, #000000, #6a0dad);
    color: #fff;
}
section, nav, footer {
    background-color: rgba(0, 0, 0, 0.6);
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 20px;
    position: sticky;
    top: 0;
    z-index: 10;
    flex-wrap: wrap;
}

nav .logo {
    color: #fff;
    font-size: 1.5em;
    font-weight: bold;
}

nav .menu a {
    color: #fff;
    text-decoration: none;
    margin: 0 10px;
    transition: color 0.3s;
}

nav .menu a:hover {
    color: #ff6600;
}

.nav-extra {
    display: flex;
    align-items: center;
    gap: 10px;
}

.nav-extra input {
    padding: 5px 10px;
    border-radius: 5px;
    border: none;
}

.nav-extra .cart-btn, 
.nav-extra .user-btn {
    color: #fff;
    font-size: 1.2em;
    text-decoration: none;
    transition: transform 0.3s;
}

.nav-extra .cart-btn:hover, 
.nav-extra .user-btn:hover {
    transform: scale(1.2);
}
.hero {
    height: 80vh;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    position: relative;
    background: url('hero-bg.jpg') center/cover no-repeat;
}

.hero-content {
    background: rgba(0, 0, 0, 0.6);
    padding: 20px;
    border-radius: 10px;
}

.hero-buttons {
    margin-top: 15px;
    display: flex;
    justify-content: center;
    gap: 10px;
}

.hero-buttons .btn {
    background: #ff6600;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
    font-weight: bold;
    transition: transform 0.3s;
}

.hero-buttons .btn:hover {
    transform: scale(1.05);
}

.hero-buttons .btn-light {
    background: #fff;
    color: #000;
}
.featured-products {
    display: flex;
    overflow-x: auto;
    padding: 15px 0;
    gap: 20px;
}

.featured-products .product {
    position: relative;
    min-width: 200px;
    flex: 0 0 auto;
    background: rgba(255, 255, 255, 0.1);
    padding: 10px;
    border-radius: 10px;
    text-align: center;
    transition: transform 0.3s;
}

.featured-products .product:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 20px rgba(255,255,255,0.2);
}

.featured-products .badge {
    position: absolute;
    top: 10px;
    left: 10px;
    background: #ff6600;
    color: #fff;
    padding: 5px 10px;
    border-radius: 5px;
    font-size: 0.9em;
}

.products {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin-top: 30px;
}

.products .product {
    background: rgba(255, 255, 255, 0.1);
    border-radius: 10px;
    padding: 15px;
    transition: transform 0.3s;
    text-align: center;
}

.products .product:hover {
    transform: scale(1.05);
    box-shadow: 0 10px 20px rgba(255,255,255,0.2);
}

.products img {
    width: 100%;
    height: 180px;
    object-fit: cover;
    border-radius: 5px;
}

#cta {
    text-align: center;
    background: rgba(255,255,255,0.1);
    padding: 30px 15px;
    border-radius: 10px;
    margin: 30px;
}

#cta .cta-content {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
}

#cta .cta-content img {
    max-width: 200px;
    border-radius: 10px;
}

#cta input {
    padding: 10px;
    width: 250px;
    border-radius: 5px;
    border: none;
    margin-right: 10px;
}

#cta button {
    padding: 10px 20px;
    background: #ff6600;
    color: #fff;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

#testimonials {
    text-align: center;
    padding: 30px 15px;
}

.testimonial {
    background: rgba(255,255,255,0.1);
    margin: 15px auto;
    padding: 20px;
    border-radius: 10px;
    max-width: 500px;
    text-align: center;
}

.testimonial img {
    width: 60px;
    height: 60px;
    border-radius: 50%;
    margin-bottom: 10px;
}

form {
    max-width: 500px;
    margin: auto;
    display: flex;
    flex-direction: column;
}

form input, form textarea, form button {
    margin: 10px 0;
    padding: 10px;
    font-size: 1em;
}

form button {
    background: #ff6600;
    color: white;
    border: none;
    cursor: pointer;
}

footer {
    background: rgba(0, 0, 0, 0.6);
    text-align: center;
    padding: 15px;
}

.social {
    display: flex;
    justify-content: center;
    gap: 15px;
    margin-top: 10px;
}

.social img {
    width: 30px;
    height: 30px;
    transition: transform 0.3s;
}

.social img:hover {
    transform: scale(1.2);
}
```
## OUTPUT



<img width="543" height="307" alt="image" src="https://github.com/user-attachments/assets/3600d9e7-65d5-4bf3-8f80-295c4a194aeb" />



<img width="547" height="306" alt="image" src="https://github.com/user-attachments/assets/b835121e-f843-4266-a2a9-42234b444562" />

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
