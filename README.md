
<!DOCTYPE html>
<html>
<head>
  <title>supgang</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #333;
      color: #fff;
      padding: 20px;
      text-align: center;
    }

    nav {
      background-color: #f4f4f4;
      padding: 10px;
      text-align: center;
    }

    nav a {
      color: #333;
      text-decoration: none;
      margin: 0 10px;
    }

    main {
      margin: 20px;
    }

    section {
      margin-bottom: 40px;
      display: none;
    }

    footer {
      background-color: #333;
      color: #fff;
      padding: 20px;
      text-align: center;
    }

    .contact-form {
      max-width: 400px;
      margin: 0 auto;
    }

    .contact-form label {
      display: block;
      margin-bottom: 10px;
    }

    .contact-form input,
    .contact-form textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
    }

    .contact-form button {
      background-color: #333;
      color: #fff;
      padding: 10px 20px;
      border: none;
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>
    <h1>Welcome to My Complex Website</h1>
  </header>

  <nav>
    <a href="#" onclick="openTab('home')">Home</a>
    <a href="#" onclick="openTab('about')">About</a>
    <a href="#" onclick="openTab('products')">Products</a>
    <a href="#" onclick="openTab('contact')">Contact</a>
  </nav>

  <main>
    <section id="home">
      <h2>Welcome to My Website</h2>
      <p>This is the home page of my website. Feel free to explore the different tabs above to learn more about me, my products, and how to contact me.</p>
    </section>

    <section id="about">
      <h2>About Me</h2>
      <p>Hi, I'm John Doe. I'm a web developer with a passion for creating awesome websites. I have several years of experience in front-end and back-end development.</p>
    </section>

    <section id="products">
      <h2>Products</h2>
      <ul>
        <li>
          <h3>Product 1</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean gravida convallis nulla, sit amet volutpat purus ullamcorper non.</p>
        </li>
        <li>
          <h3>Product 2</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean gravida convallis nulla, sit amet volutpat purus ullamcorper non.</p>
        </li>
        <li>
          <h3>Product 3</h3>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean gravida convallis nulla, sit amet volutpat purus ullamcorper non.</p>
        </li>
      </ul>
    </section>

    <section id="contact">
      <h2>Contact</h2>
      <div class="contact-form">
        <form action="process-form.php" method="post">
          <label for="name">Name:</label>
          <input type="text" id="name" name="name" required>

          <label for="email">Email:</label>
          <input type="email" id="email" name="email" required>

          <label for="phone">Phone:</label>
          <input type="tel" id="phone" name="phone" required>

          <label for="message">Message:</label>
          <textarea id="message" name="message" rows="4" required></textarea>

          <button type="submit">Send Message</button>
        </form>
      </div>
    </section>
  </main>

  <footer>
    <p>&copy; 2023 My Complex Website. All rights reserved.</p>
  </footer>

  <script>
    // Function to switch between tabs
    function openTab(tabName) {
      // Get all sections and hide them
      var sections = document.querySelectorAll("section");
      sections.forEach(function(section) {
        section.style.display = "none";
      });

      // Show the selected tab
      document.getElementById(tabName).style.display = "block";
    }
  </script>
</body>
</html>
