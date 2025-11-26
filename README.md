<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Professional Template</title>
  <style>
    /* ---------- Reset ---------- */
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Arial', sans-serif;
    }

    body {
      line-height: 1.6;
      color: #333;
    }

    a {
      text-decoration: none;
      color: inherit;
    }

    /* ---------- Navbar ---------- */
    header {
      background: #007BFF;
      color: white;
      padding: 15px 20px;
      position: sticky;
      top: 0;
      z-index: 1000;
    }

    .navbar {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .navbar ul {
      display: flex;
      list-style: none;
      gap: 20px;
    }

    .navbar ul li a {
      color: white;
      font-weight: bold;
      transition: 0.3s;
    }

    .navbar ul li a:hover {
      color: #FFD700;
    }

    /* ---------- Hero Section ---------- */
    .hero {
      background: url('https://images.unsplash.com/photo-1507525428034-b723cf961d3e') no-repeat center center/cover;
      height: 90vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      padding: 0 20px;
    }

    .hero h1 {
      font-size: 3rem;
      margin-bottom: 20px;
      text-shadow: 2px 2px 5px rgba(0,0,0,0.5);
    }

    .hero p {
      font-size: 1.2rem;
      margin-bottom: 30px;
      text-shadow: 1px 1px 3px rgba(0,0,0,0.5);
    }

    .hero button {
      padding: 10px 25px;
      font-size: 1rem;
      border: none;
      background: #FFD700;
      color: #333;
      cursor: pointer;
      border-radius: 5px;
      transition: 0.3s;
    }

    .hero button:hover {
      background: #FFC107;
    }

    /* ---------- Services Section ---------- */
    .services {
      padding: 60px 20px;
      background: #f9f9f9;
      text-align: center;
    }

    .services h2 {
      font-size: 2rem;
      margin-bottom: 40px;
    }

    .service-cards {
      display: flex;
      flex-wrap: wrap;
      gap: 20px;
      justify-content: center;
    }

    .card {
      background: white;
      padding: 20px;
      width: 250px;
      border-radius: 10px;
      box-shadow: 0 2px 8px rgba(0,0,0,0.1);
      transition: 0.3s;
    }

    .card:hover {
      transform: translateY(-5px);
      box-shadow: 0 5px 15px rgba(0,0,0,0.2);
    }

    .card h3 {
      margin-bottom: 10px;
      color: #007BFF;
    }

    .card p {
      font-size: 0.9rem;
      color: #555;
    }

    /* ---------- Contact Section ---------- */
    .contact {
      padding: 60px 20px;
      text-align: center;
    }

    .contact h2 {
      font-size: 2rem;
      margin-bottom: 30px;
    }

    .contact form {
      max-width: 500px;
      margin: auto;
      display: flex;
      flex-direction: column;
      gap: 15px;
    }

    .contact input, .contact textarea {
      padding: 10px;
      border-radius: 5px;
      border: 1px solid #ccc;
      font-size: 1rem;
    }

    .contact button {
      padding: 10px;
      border: none;
      background: #007BFF;
      color: white;
      font-size: 1rem;
      cursor: pointer;
      border-radius: 5px;
      transition: 0.3s;
    }

    .contact button:hover {
      background: #0056b3;
    }

    /* ---------- Footer ---------- */
    footer {
      background: #333;
      color: white;
      text-align: center;
      padding: 20px;
    }

    /* ---------- Responsive ---------- */
    @media(max-width: 768px) {
      .service-cards {
        flex-direction: column;
        align-items: center;
      }

      .hero h1 {
        font-size: 2rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <header>
    <div class="navbar">
      <h1>MyCompany</h1>
      <ul>
        <li><a href="#hero">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </div>
  </header>

  <!-- Hero Section -->
  <section class="hero" id="hero">
    <h1>Welcome to Our Company</h1>
    <p>We provide the best solutions for modern web interfaces</p>
    <button onclick="alert('Button clicked!')">Get Started</button>
  </section>

  <!-- Services Section -->
  <section class="services" id="services">
    <h2>Our Services</h2>
    <div class="service-cards">
      <div class="card">
        <h3>UI Design</h3>
        <p>Attractive and user-friendly designs for all platforms.</p>
      </div>
      <div class="card">
        <h3>Website Development</h3>
        <p>Responsive and fast websites using HTML/CSS/JS.</p>
      </div>
      <div class="card">
        <h3>Performance Optimization</h3>
        <p>Improve website speed and user experience for best results.</p>
      </div>
    </div>
  </section>

  <!-- Contact Section -->
  <section class="contact" id="contact">
    <h2>Contact Us</h2>
    <form onsubmit="event.preventDefault(); alert('Message sent!');">
      <input type="text" placeholder="Your Name" required>
      <input type="email" placeholder="Your Email" required>
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit">Send</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    &copy; 2025 All Rights Reserved
  </footer>

</body>
</html>
