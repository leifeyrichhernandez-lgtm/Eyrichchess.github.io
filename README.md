# Eyrichchess.github.io
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Modern Single Page Website</title>
  <style>
    /* Reset & Base Styles */
    * {
      box-sizing: border-box;
      margin: 0;
      padding: 0;
    }

    html {
      scroll-behavior: smooth;
      font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif;
      color: #1f2937;
      line-height: 1.6;
    }

    body {
      background-color: #ffffff;
    }

    /* Navigation Bar */
    header {
      position: fixed;
      top: 0;
      width: 100%;
      background: rgba(255, 255, 255, 0.95);
      box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
      z-index: 1000;
    }

    nav {
      max-width: 1100px;
      margin: 0 auto;
      padding: 1rem 2rem;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      font-size: 1.5rem;
      font-weight: 700;
      color: #2563eb;
      text-decoration: none;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 2rem;
    }

    .nav-links a {
      text-decoration: none;
      color: #4b5563;
      font-weight: 500;
      transition: color 0.2s;
    }

    .nav-links a:hover {
      color: #2563eb;
    }

    /* Sections */
    section {
      padding: 6rem 2rem;
      max-width: 1100px;
      margin: 0 auto;
    }

    /* Hero Section */
    #home {
      min-height: 100vh;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      text-align: center;
      padding-top: 8rem;
    }

    #home h1 {
      font-size: 3rem;
      font-weight: 800;
      margin-bottom: 1rem;
      color: #111827;
    }

    #home p {
      font-size: 1.25rem;
      color: #6b7280;
      max-width: 600px;
      margin-bottom: 2rem;
    }

    .btn {
      display: inline-block;
      background-color: #2563eb;
      color: #ffffff;
      padding: 0.85rem 2rem;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 600;
      transition: background-color 0.2s;
      border: none;
      cursor: pointer;
    }

    .btn:hover {
      background-color: #1d4ed8;
    }

    /* Section Headings */
    h2 {
      font-size: 2.25rem;
      text-align: center;
      margin-bottom: 3rem;
      color: #111827;
    }

    /* Services / Features Grid */
    .grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
      gap: 2rem;
    }

    .card {
      background: #f9fafb;
      padding: 2rem;
      border-radius: 12px;
      border: 1px solid #e5e7eb;
      transition: transform 0.2s;
    }

    .card:hover {
      transform: translateY(-5px);
    }

    .card h3 {
      font-size: 1.25rem;
      margin-bottom: 0.75rem;
      color: #111827;
    }

    .card p {
      color: #4b5563;
    }

    /* About Section */
    #about {
      background-color: #f9fafb;
      max-width: 100%;
    }

    .about-container {
      max-width: 800px;
      margin: 0 auto;
      text-align: center;
    }

    .about-container p {
      font-size: 1.125rem;
      color: #4b5563;
    }

    /* Contact Form */
    form {
      max-width: 550px;
      margin: 0 auto;
      display: flex;
      flex-direction: column;
      gap: 1.25rem;
    }

    input, textarea {
      width: 100%;
      padding: 0.85rem;
      border: 1px solid #d1d5db;
      border-radius: 8px;
      font-size: 1rem;
      font-family: inherit;
    }

    input:focus, textarea:focus {
      outline: none;
      border-color: #2563eb;
    }

    /* Footer */
    footer {
      text-align: center;
      padding: 2rem;
      background-color: #111827;
      color: #9ca3af;
      font-size: 0.9rem;
    }

    /* Mobile Responsive */
    @media (max-width: 640px) {
      #home h1 {
        font-size: 2.25rem;
      }
      .nav-links {
        gap: 1rem;
        font-size: 0.9rem;
      }
    }
  </style>
</head>
<body>

  <!-- Navigation -->
  <header>
    <nav>
      <a href="#home" class="logo">BrandName</a>
      <ul class="nav-links">
        <li><a href="#home">Home</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#contact">Contact</a></li>
      </ul>
    </nav>
  </header>

  <!-- Hero Section -->
  <section id="home">
    <h1>Leifs Chess Opening</h1>
    <p>A clean, fast, and responsive single-page website ready to showcase your product, portfolio, or business.</p>
    <a href="#contact" class="btn">Get Started</a>
  </section>

  <!-- Services Section -->
  <section id="services">
    <h2>What We Offer</h2>
    <div class="grid">
      <div class="card">
        <h3>Web Design</h3>
        <p>Clean, modern layouts tailored to look great on desktop, tablet, and mobile devices.</p>
      </div>
      <div class="card">
        <h3>Fast Performance</h3>
        <p>Lightweight code with zero external dependencies ensures instant load times.</p>
      </div>
      <div class="card">
        <h3>Easy Customization</h3>
        <p>Well-structured HTML and CSS makes changing colors, fonts, and text effortless.</p>
      </div>
    </div>
  </section>

  <!-- About Section -->
  <section id="about">
    <div class="about-container">
      <h2>About Us</h2>
      <p>We believe great websites don't need to be complicated. Our focus is on clarity, speed, and delivering a seamless experience for every visitor.</p>
    </div>
  </section>

  <!-- Contact Section -->
  <section id="contact">
    <h2>Get In Touch</h2>
    <form onsubmit="event.preventDefault(); alert('Message sent! (Connect a backend or form service to receive emails.)');">
      <input type="text" placeholder="Your Name" required />
      <input type="email" placeholder="Your Email" required />
      <textarea rows="5" placeholder="Your Message" required></textarea>
      <button type="submit" class="btn">Send Message</button>
    </form>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2026 BrandName. All rights reserved.</p>
  </footer>

</body>
</html>
s
