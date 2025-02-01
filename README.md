
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Advanced GPT Website</title>
  <style>
    /* General Styles */
    body {
      font-family: 'Arial', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f9;
      color: #333;
    }

    /* Hero Section */
    .hero {
      height: 100vh;
      background: linear-gradient(135deg, #007bff, #00bfff);
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
      color: white;
      overflow: hidden;
    }

    .hero h1 {
      font-size: 4rem;
      animation: slideIn 1.5s ease-in-out;
    }

    @keyframes slideIn {
      from { transform: translateY(-100px); opacity: 0; }
      to { transform: translateY(0); opacity: 1; }
    }

    /* Sections */
    section {
      padding: 50px 20px;
      text-align: center;
    }

    h2 {
      font-size: 2.5rem;
      color: #007bff;
    }

    .cards, .feature-icons, .buttons-container {
      display: flex;
      justify-content: center;
      flex-wrap: wrap;
      margin-top: 30px;
    }

    .card, .feature-icon {
      width: 300px;
      padding: 20px;
      background-color: #f4f4f9;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
      margin: 10px;
      transition: transform 0.3s ease;
    }

    .card:hover, .feature-icon:hover {
      transform: translateY(-10px);
    }

    .feature-icon img {
      width: 80px;
      height: 80px;
    }

    .demo textarea {
      width: 80%;
      max-width: 600px;
      height: 150px;
      padding: 10px;
      font-size: 1rem;
      border: 2px solid #007bff;
      border-radius: 10px;
      margin-top: 20px;
    }

    button {
      margin: 10px;
      padding: 10px 20px;
      background-color: #007bff;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-size: 1rem;
      transition: background-color 0.3s ease;
    }

    button:hover {
      background-color: #0056b3;
    }

    .output {
      margin-top: 20px;
      font-size: 1.2rem;
      color: #333;
    }

    /* Contact Section */
    .contact {
      background-color: white;
      padding: 50px 20px;
      text-align: center;
    }

    .contact p {
      font-size: 1.2rem;
      margin: 10px 0;
    }

    .contact a {
      color: #007bff;
      text-decoration: none;
      font-weight: bold;
    }

    .contact a:hover {
      text-decoration: underline;
    }

    /* Footer */
    footer {
      padding: 20px;
      background-color: #007bff;
      color: white;
      text-align: center;
    }
  </style>
</head>
<body>

  <!-- Hero Section -->
  <section class="hero">
    <h1>Welcome to the World of GPT</h1>
  </section>

  <!-- About Section -->
  <section class="about">
    <h2>About GPT</h2>
    <div class="cards">
      <div class="card">
        <h3>What is GPT?</h3>
        <p>GPT (Generative Pre-trained Transformer) is a state-of-the-art language model developed by OpenAI.</p>
      </div>
      <div class="card">
        <h3>How Does It Work?</h3>
        <p>GPT uses deep learning techniques to analyze and generate text based on input.</p>
      </div>
      <div class="card">
        <h3>Applications</h3>
        <p>GPT is used in chatbots, content generation, translation, and much more.</p>
      </div>
    </div>
  </section>

  <!-- Features Section -->
  <section class="features">
    <h2>Features</h2>
    <div class="feature-icons">
      <div class="feature-icon">
        <img src="https://via.placeholder.com/80" alt="Icon">
        <p>Natural Language</p>
      </div>
      <div class="feature-icon">
        <img src="https://via.placeholder.com/80" alt="Icon">
        <p>Contextual Understanding</p>
      </div>
      <div class="feature-icon">
        <img src="https://via.placeholder.com/80" alt="Icon">
        <p>Multi-Language Support</p>
      </div>
    </div>
  </section>

  <!-- Demo Section -->
  <section class="demo">
    <h2>Try It Out</h2>
    <textarea id="input" placeholder="Enter your text here..."></textarea>
    <div class="buttons-container">
      <button onclick="generateResponse()">Generate Response</button>
      <button onclick="clearText()">Clear</button>
      <button onclick="alert('Feature Coming Soon!')">Advanced Mode</button>
    </div>
    <div class="output" id="output"></div>
  </section>

  <!-- Contact Section -->
  <section class="contact">
    <h2>Contact Us</h2>
    <p>Phone: <a href="tel:+251985754689">+251985754689</a></p>
    <p>Email: <a href="mailto:eyob0081@gmail.com">eyob0081@gmail.com</a></p>
    <p>Telegram: <a href="https://t.me/+251985754689" target="_blank">@Eyob0081</a></p>
  </section>

  <!-- Footer -->
  <footer>
    <p>&copy; 2023 GPT Website | Follow us: 
      <a href="#">Twitter</a> | 
      <a href="#">LinkedIn</a> | 
      <a href="#">GitHub</a>
    </p>
  </footer>

  <script>
    function generateResponse() {
      const input = document.getElementById('input').value;
      const output = document.getElementById('output');
      if (input.trim() === "") {
        output.textContent = "Please enter some text to generate a response.";
        return;
      }
      output.textContent = `GPT Response: "${input}" (This is a simulated response.)`;
    }

    function clearText() {
      document.getElementById('input').value = "";
      document.getElementById('output').textContent = "";
    }
  </script>

</body>
</html>
