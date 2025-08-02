<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Talent High School</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body {
      font-family: Arial, sans-serif;
    }

    header {
      background-color: #004080;
      color: white;
      padding: 15px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      position: relative;
    }

    .logo-title {
      display: flex;
      align-items: center;
    }

    .logo-title img {
      height: 60px;
      margin-right: 15px;
    }

    .nav-buttons {
      display: flex;
      gap: 15px;
    }

    .nav-buttons button {
      background-color: white;
      color: #004080;
      border: none;
      padding: 10px 15px;
      border-radius: 5px;
      cursor: pointer;
      font-weight: bold;
    }

    .dropdown {
      position: relative;
      display: inline-block;
    }

    .dots {
      font-size: 24px;
      cursor: pointer;
      padding: 10px;
      background: none;
      border: none;
      color: white;
    }

    .dropdown-content {
      display: none;
      position: absolute;
      right: 0;
      background-color: white;
      color: #004080;
      min-width: 120px;
      border: 1px solid #ccc;
      border-radius: 5px;
      z-index: 1;
    }

    .dropdown-content a {
      color: #004080;
      padding: 10px 15px;
      text-decoration: none;
      display: block;
    }

    .dropdown:hover .dropdown-content {
      display: block;
    }

    .scroll-images {
      margin: 50px auto;
      width: 90%;
      overflow: hidden;
      white-space: nowrap;
      border: 2px solid #ccc;
      padding: 10px;
    }

    .scroll-images img {
      height: 160px;
      margin-right: 15px;
      animation: scrollLeft 20s linear infinite;
    }

    @keyframes scrollLeft {
      0% {
        transform: translateX(100%);
      }
      100% {
        transform: translateX(-100%);
      }
    }

    .marquee-footer {
      background-color: #004080;
      color: white;
      padding: 10px;
      position: relative;
      width: 100%;
    }

    marquee {
      font-size: 16px;
    }
  </style>
</head>
<body>

  <!-- Header -->
  <header>
    <div class="logo-title">
      <img src="logo.png" alt="Logo">
      <h1>Talent High School</h1>
    </div>
    <div class="nav-buttons">
      <button>Home</button>
      <button>About</button>
      <button>Login</button>
    </div>
    <div class="dropdown">
      <button class="dots">⋮</button>
      <div class="dropdown-content">
        <a href="#">Admissions</a>
        <a href="#">Academics</a>
        <a href="#">Contact</a>
      </div>
    </div>
  </header>

  <!-- Scrolling Images -->
  <div class="scroll-images">
    <img src="img1.jpg" alt="School Image 1">
    <img src="img2.jpg" alt="School Image 2">
    <img src="img3.jpg" alt="School Image 3">
    <img src="img4.jpg" alt="School Image 4">
  </div>

  <!-- Scrolling Address -->
  <div class="marquee-footer">
    <marquee behavior="scroll" direction="left">
      Talent High School, Narendrapuram, Rajanagaram Mandalam, East Godavari, PIN Code: 533294
    </marquee>
  </div>

</body>
</html>
