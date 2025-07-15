<!DOCTYPE html>
<html lang="th">
<head>
  <meta charset="UTF-8">
  <title>ครบรอบ 1 ปี 5 เดือน 💖</title>
  <style>
    body {
      margin: 0;
      font-family: 'Segoe UI', sans-serif;
      background: linear-gradient(to right, #ffe1f0, #d4fbff);
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
    }

    .card-container {
      background: white;
      width: 370px;
      padding: 30px;
      border-radius: 20px;
      box-shadow: 0 10px 30px rgba(0,0,0,0.2);
      text-align: center;
      position: relative;
    }

    .page {
      display: none;
      animation: fadeIn 0.5s ease-in-out;
    }

    .page.active {
      display: block;
    }

    .heart {
      font-size: 2.5em;
      animation: beat 1s infinite;
      color: red;
    }

    @keyframes beat {
      0%, 100% { transform: scale(1); }
      50% { transform: scale(1.2); }
    }

    @keyframes fadeIn {
      from { opacity: 0; }
      to { opacity: 1; }
    }

    button {
      background-color: #ff4d6d;
      border: none;
      padding: 10px 20px;
      color: white;
      font-size: 1em;
      border-radius: 10px;
      margin-top: 20px;
      cursor: pointer;
    }

    button:hover {
      background-color: #e63e5c;
    }

    img {
      width: 100%;
      border-radius: 15px;
      margin-bottom: 15px;
    }

    iframe {
      margin-top: 10px;
      border-radius: 10px;
    }
  </style>
</head>
<body>
  <div class="card-container">
    <!-- หน้า 1 -->
    <div class="page active">
      <div class="heart">❤️</div>
      <h2>สุขสันต์วันครบรอบ 1 ปี 5 เดือน</h2>
      <img src="2694f2fb-cccc-4aa2-b96f-e0fc71de7583.jpeg" alt="รูปคู่ของเรา">
      <p>ทุกนาทีที่มีคุณอยู่ข้าง ๆ คือของขวัญล้ำค่าที่สุดในชีวิต</p>

      <!-- เพลง YouTube ฝัง -->
      <iframe width="100%" height="200" 
        src="https://www.youtube.com/embed/Ll-CVHngjCI" 
        title="เพลงรัก - Big Ass" 
        frameborder="0" 
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
        allowfullscreen>
      </iframe>
    </div>

    <!-- หน้า 2 -->
    <div class="page">
      <h2>Saksit Kunphamuang</h2>
      <p>ขอบคุณที่อยู่ข้างกันเสมอ</p>
      <p>คุณคือคนเดียวที่ทำให้โลกของฉันสวยงาม 🌍💗</p>
    </div>

    <!-- หน้า 3 -->
    <div class="page">
      <h2>แค่มีคุณ...</h2>
      <p>ก็ไม่ต้องการอะไรเพิ่มเติมอีกแล้ว</p>
      <p>คุณคือคำตอบของหัวใจดวงนี้</p>
    </div>

    <!-- หน้า 4 -->
    <div class="page">
      <h2>รักคุณเสมอ 💕</h2>
      <p>Happy Anniversary!</p>
      <p>จากคนที่รักคุณที่สุดในโลกนี้</p>
    </div>

    <button onclick="nextPage()">👉 หน้าถัดไป</button>
  </div>

  <script>
    let pages = document.querySelectorAll('.page');
    let currentPage = 0;

    function nextPage() {
      pages[currentPage].classList.remove('active');
      currentPage = (currentPage + 1) % pages.length;
      pages[currentPage].classList.add('active');
    }
  </script>
</body>
</html>
