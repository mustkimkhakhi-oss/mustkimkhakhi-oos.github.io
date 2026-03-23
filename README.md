<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>For You ❤️</title>
  <style>
    body {
      margin: 0;
      font-family: 'Poppins', sans-serif;
      background: linear-gradient(to right, #ff9a9e, #fad0c4);
      color: #fff;
      text-align: center;
      overflow-x: hidden;
    }

    nav {
      padding: 15px;
    }

    .btn {
      background: white;
      color: #ff4b5c;
      padding: 10px 20px;
      border-radius: 20px;
      text-decoration: none;
      font-weight: bold;
      margin: 5px;
      display: inline-block;
      transition: 0.3s;
    }

    .btn:hover {
      background: #ff4b5c;
      color: white;
    }

    header {
      padding: 40px 20px;
      font-size: 2.5em;
      font-weight: bold;
    }

    .section {
      padding: 60px 20px;
    }

    img {
      width: 200px;
      border-radius: 20px;
      margin: 10px;
    }

    footer {
      padding: 20px;
      font-size: 0.9em;
    }

    .heart {
      position: fixed;
      top: -10px;
      color: red;
      animation: fall linear infinite;
    }

    @keyframes fall {
      to {
        transform: translateY(100vh);
      }
    }
  </style>
</head>
<body>

<!-- NAVBAR -->
<nav>
  <a href="#home" class="btn">Home</a>
  <a href="#about" class="btn">About Her 💖</a>
  <a href="#gallery" class="btn">Gallery 📸</a>
  <a href="#message" class="btn">Message 💌</a>
</nav>

<!-- HOME -->
<header id="home">
  Hey My Love ❤️
</header>

<!-- ABOUT -->
<div class="section" id="about">
  <h2>About You 💖</h2>
  <p>You are the most beautiful and amazing person in my life 🌸</p>
</div>

<!-- GALLERY -->
<div class="section" id="gallery">
  <h2>Our Memories 📸</h2>
  <img src="https://via.placeholder.com/200" alt="photo1">
  <img src="https://via.placeholder.com/200" alt="photo2">
  <img src="https://via.placeholder.com/200" alt="photo3">
</div>

<!-- MESSAGE -->
<div class="section" id="message">
  <h2>Message for You 💌</h2>
  <p>No matter what happens, I will always be there for you ❤️</p>
</div>

<footer>
  Made with ❤️ just for you
</footer>

<script>
  // Heart animation
  function createHeart() {
    const heart = document.createElement('div');
    heart.classList.add('heart');
    heart.innerText = '❤️';
    heart.style.left = Math.random() * 100 + 'vw';
    heart.style.animationDuration = (Math.random() * 3 + 2) + 's';
    document.body.appendChild(heart);

    setTimeout(() => {
      heart.remove();
    }, 5000);
  }

  setInterval(createHeart, 300);
</script>

</body>
</html>
