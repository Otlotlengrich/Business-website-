# Business-website-
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Your Business Name - Home</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About</a></li>
                <li><a href="#products">Products</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home">
        <h1>Welcome to Your Business Name!</h1>
        <p>Your tagline or introduction goes here. Share the essence of your business.</p>
        <button id="cta-button">Get Started</button>
    </section>

    <section id="about">
        <h2>About Us</h2>
        <p>Tell the world what your business is about. Include your mission, values, and vision.</p>
    </section>

    <section id="products">
        <h2>Our Products</h2>
        <div class="product-list">
            <div class="product-item">
                <h3>Protein Supplement</h3>
                <p>High-quality plant-based protein supplement.</p>
                <button>Buy Now</button>
            </div>
            <div class="product-item">
                <h3>Protein Gummies</h3>
                <p>Delicious protein-packed gummy bears.</p>
                <button>Buy Now</button>
            </div>
        </div>
    </section>

    <section id="contact">
        <h2>Contact Us</h2>
        <form id="contact-form">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2025 Your Business Name. All Rights Reserved.</p>
    </footer>

    <script src="scripts.js"></script>
</body>
</html>
