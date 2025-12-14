<!DOCTYPE html>
<html lang="ar">
<head>
  <meta charset="UTF-8">
  <title>موقعي</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #111;
      color: white;
      text-align: center;
      padding: 20px;
    }
    .hidden { display: none; }
    img, video {
      width: 90%;
      max-width: 400px;
      margin: 10px 0;
      border-radius: 10px;
    }
    .hearts {
      font-size: 40px;
      color: red;
      margin: 20px 0;
      animation: beat 1s infinite;
    }
    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.3); }
    }
    input { padding: 10px; font-size: 16px; }
    button { padding: 10px 20px; font-size: 16px; cursor: pointer; }
    .message { font-size: 20px; margin-top: 20px; display: none; }
  </style>
</head>
<body>

  <!-- صفحة الباسورد -->
  <div id="login">
    <h2>🔒 ادخل الباسورد</h2>
    <input type="password" id="pass">
    <button onclick="check()">دخول</button>
  </div>

  <!-- المحتوى بعد الباسورد -->
  <div id="content" class="hidden">
    <div class="hearts">❤️ ❤️ ❤️ ❤️ ❤️</div>

    <!-- صور -->
    <img src="img1.jpg" alt="صورة 1">
    <img src="img2.jpg" alt="صورة 2">

    <!-- فيديو -->
    <video controls>
      <source src="video.mp4" type="video/mp4">
    </video>

    <!-- الرسالة -->
    <h3>✉️ رسالتك هنا</h3>
    <p class="message" id="msg">اكتب الرسالة اللي انت عايزها هنا</p>
  </div>

  <script>
    function check
