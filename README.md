
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>AdView BD</title>
  <style>
    body {
      font-family: sans-serif;
      padding: 20px;
      background: #f9f9f9;
      margin: 0;
      position: relative;
      min-height: 100vh;
    }
    .lang-toggle {
      position: absolute;
      top: 20px;
      right: 20px;
      padding: 10px 15px;
      background: #007bff;
      color: white;
      border: none;
      border-radius: 6px;
      cursor: pointer;
      font-size: 16px;
      user-select: none;
    }
    #english, #bangla {
      max-width: 600px;
      margin: 80px auto 0 auto;
      text-align: center;
      line-height: 1.6;
    }
  </style>
</head>
<body>

  <!-- Language Toggle Button -->
  <button class="lang-toggle" onclick="toggleLanguage()">বাংলা</button>

  <!-- English Content -->
  <div id="english">
    <h1>Welcome to AdView BD</h1>
    <p>Earn money by watching ads, referring friends, and completing tasks!</p>
    <p>Withdraw your earnings through bKash or Nagad.</p>
  </div>

  <!-- Bangla Content (hidden initially) -->
  <div id="bangla" style="display: none;">
    <h1>AdView BD-তে স্বাগতম</h1>
    <p>বিজ্ঞাপন দেখে, বন্ধুদের রেফার করে এবং ছোট ছোট কাজ করে আয় করুন!</p>
    <p>আপনার আয় বিকাশ বা নগদ এর মাধ্যমে তুলুন।</p>
  </div>

  <script>
    let isBangla = false;
    function toggleLanguage() {
      isBangla = !isBangla;
      document.getElementById('english').style.display = isBangla ? 'none' : 'block';
      document.getElementById('bangla').style.display = isBangla ? 'block' : 'none';
      document.querySelector('.lang-toggle').innerText = isBangla ? 'English' : 'বাংলা';
    }
  </script>

</body>
</html>
