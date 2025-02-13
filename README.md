<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>POWER MUNCH</title>
  <link rel="stylesheet" href="styles.css">
</head>
<body>
  <header>
    <h1>Welcome to POWER MUNCH</h1>
    <nav>
      <a href="#products">Products</a>
      <a href="#reviews">Reviews</a>
      <a href="#contact">Contact Us</a>
    </nav>
  </header>

  <section id="products">
    <h2>Our Snacks</h2>
    <div class="product-gallery">
      <img src="snack1.jpg" alt="Snack 1">
      <img src="snack2.jpg" alt="Snack 2">
      <img src="snack3.jpg" alt="Snack 3">
    </div>
  </section>

  <section id="reviews">
    <h2>Customer Reviews</h2>
    <div id="reviews-container">
      <p>No reviews yet. Be the first to leave one!</p>
    </div>
    <form id="review-form">
      <input type="text" id="review-input" placeholder="Write your review..." required>
      <button type="submit">Submit</button>
    </form>
  </section>

  <footer>
    <p>&copy; 2025 Protein Snacks. All rights reserved.</p>
  </footer>

  <script src="script.js"></script>
</body>
</html>
/* General Styles */
body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
  background: linear-gradient(45deg, #ff9a9e, #fad0c4);
  color: #333;
}

/* Header Section */
header {
  background-color: #ff6f61;
  color: white;
  text-align: center;
  padding: 1rem;
}

header nav a {
  margin: 0 10px;
  color: white;
  text-decoration: none;
  font-weight: bold;
}

header nav a:hover {
  text-decoration: underline;
}

/* Section Styling */
section {
  padding: 2rem;
  text-align: center;
}

/* Product Gallery */
.product-gallery {
  display: flex;
  justify-content: center;
  gap: 1rem;
}

.product-gallery img {
  width: 200px;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Reviews Section */
#reviews-container {
  margin: 1rem 0;
  background-color: white;
  padding: 1rem;
  border-radius: 5px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

#review-form input {
  padding: 0.5rem;
  font-size: 1rem;
  margin-right: 0.5rem;
  border: 1px solid #ccc;
  border-radius: 5px;
}

#review-form button {
  padding: 0.5rem 1rem;
  font-size: 1rem;
  color: white;
  background-color: #ff6f61;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

#review-form button:hover {
  background-color: #e65a50;
}

/* Footer Styling */
footer {
  background-color: #ff6f61;
  color: white;
  text-align: center;
  padding: 1rem;
}
// Add a new review to the reviews container
document.getElementById('review-form').addEventListener('submit', function (e) {
  e.preventDefault(); // Prevent the form from reloading the page
  const reviewInput = document.getElementById('review-input'); // Get the input value
  const reviewsContainer = document.getElementById('reviews-container'); // Select reviews container
  
  // Create a new paragraph for the review
  const newReview = document.createElement('p');
  newReview.textContent = reviewInput.value; // Set the text to the review input
  reviewsContainer.appendChild(newReview); // Add the new review to the container
  
  reviewInput.value = ''; // Clear the input field
});
