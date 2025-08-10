<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Trang Chủ • Cloud VIP</title>
  <style>
    body {
      margin:0; font-family: 'Segoe UI', sans-serif;
      background: radial-gradient(circle at top, #0f2027, #203a43, #2c5364);
      color:#fff;
    }
    header {
      background:linear-gradient(90deg, #0f0c29, #302b63, #24243e);
      padding:20px; text-align:center;
      box-shadow:0 0 20px #0ff;
    }
    header h1 { margin:0; font-size:2em; text-shadow:0 0 10px #0ff; }
    nav {
      display:flex; justify-content:center;
      background:#111; padding:10px;
      box-shadow:0 0 10px #0ff;
    }
    nav a {
      margin:0 15px; text-decoration:none; color:#0ff; font-weight:bold;
      padding:8px 15px; border-radius:8px; transition:0.3s;
    }
    nav a:hover { background:#0ff; color:#000; box-shadow:0 0 15px #0ff; }
    .tab-content {
      max-width:900px; margin:auto; padding:20px;
    }
    .tab-pane {
      display:none; background:rgba(0,0,0,0.6); padding:20px;
      border-radius:12px; box-shadow:0 0 20px rgba(0,255,255,0.3);
      animation: fadeIn 0.5s ease;
    }
    .tab-pane.active { display:block; }
    .btn-download {
      display:inline-flex; align-items:center; gap:10px;
      background:#0f0; color:#000; padding:12px 20px;
      border-radius:50px; text-decoration:none; font-weight:bold;
      box-shadow:0 0 15px #0f0; transition:0.3s;
    }
    .btn-download:hover { transform:scale(1.05); box-shadow:0 0 25px #0f0; }
    .game-card {
      display:flex; align-items:center; gap:15px;
      background:rgba(0,0,0,0.8); padding:15px;
      border-radius:12px; box-shadow:0 0 10px #0ff;
    }
    .game-card img {
      width:80px; height:80px; border-radius:16px; object-fit:cover;
      box-shadow:0 0 10px #0ff;
    }
    .updates .update {
      padding:10px 0; border-bottom:1px solid rgba(255,255,255,0.2);
    }
    .updates .update:last-child { border-bottom:none; }
    iframe {
      width:100%; height:400px; border:none; border-radius:8px;
      box-shadow:0 0 10px #0ff;
    }
    footer {
      text-align:center; padding:20px; margin-top:30px;
      font-size:0.9em; color:#aaa;
    }
    @keyframes fadeIn {
      from { opacity:0; transform:translateY(10px); }
      to { opacity:1; transform:translateY(0); }
    }
  </style>
  <script>
    function openTab(tabId) {
      document.querySelectorAll('.tab-pane').forEach(el => el.classList.remove('active'));
      document.getElementById(tabId).classList.add('active');
    }
    window.onload = () => {
      openTab('download');
    };
  </script>
</head>
<body>
  <header>
    <h1>Ứng Dụng Cloud VIP</h1>
    <p>Cloud Game VIP x Now.gg siu vip</p>
  </header>

  <nav>
    <a href="#" onclick="openTab('download')">Tải App</a>
    <a href="#" onclick="openTab('updates')">Cập Nhật</a>
    <a href="#" onclick="openTab('note')">Gửi văn bản & Sao chép</a>
  </nav>

  <div class="tab-content">

    <div id="download" class="tab-pane">
      <h2>Tải Ứng Dụng</h2>
      <div class="game-card">
        <img src="https://i.ibb.co/MxfJN8NF/Cloud-Vip.png" alt="App Icon">
        <div>
          <h3>Cloud VIP</h3>
          <p>Siêu phẩm cloud x now.gg siu vip</p>
          <a class="btn-download" href="https://www.mediafire.com/file/owi13w1sbru9wix/app-release.apk/file">
            <span>📥 Cài đặt</span>
          </a>
        </div>
      </div>
    </div>

    <div id="updates" class="tab-pane updates">
      <h2>Cập Nhật Mới Nhất</h2>
      <div class="update"><strong>Phiên bản 1.0</strong> - Thêm nhiều App ngon không lỗi tải app</div>
    </div>

    <div id="note" class="tab-pane">
      <h2>Gửi văn bản & Sao chép</h2>
      <iframe src="https://notevn.com"></iframe>
      <p>Hướng dẫn: Ấn vào dấu cộng và ghi những gì muốn chuyển vào cloud và ấn vào icon bút và đặt tên cho ghi chú muốn chuyển là xong việc còn lại vào cloud truy cập web này và nhập lại tên ghi chú vừa đặt thì sẽ hiện vẵn bản bạn muốn chuyển</p>
    </div>

  </div>

  <footer>
    © 2025 Gaming VIP. All rights reserved.
  </footer>
</body>
</html>
