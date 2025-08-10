<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Cloud Game VIP — Mô phỏng</title>
  <style>
    :root{
      --bg-1:#06121a; --bg-2:#082033; --accent-1:#00f5d4; --accent-2:#00b4ff; --card:rgba(255,255,255,0.04);
      --glass: rgba(255,255,255,0.03); --muted:#9aa6b2; --glass-strong: rgba(255,255,255,0.06);
      --shadow: 0 12px 30px rgba(2,6,23,0.6);
      --radius:14px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0; font-family:Inter,Segoe UI,system-ui,Arial; color:#eaf6ff;
      background: radial-gradient(1200px 400px at 10% 10%, rgba(0,181,255,0.08), transparent),
                  linear-gradient(180deg,var(--bg-1),var(--bg-2));
      -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
      padding:28px;
    }

    /* layout */
    .app{max-width:1100px;margin:0 auto}
    header{display:flex;align-items:center;justify-content:space-between;gap:12px;margin-bottom:18px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:54px;height:54px;border-radius:12px;display:grid;place-items:center;background:linear-gradient(135deg,var(--accent-1),var(--accent-2));box-shadow:0 8px 24px rgba(0,180,255,0.12)}
    .logo svg{width:34px;height:34px}
    h1{font-size:18px;margin:0;line-height:1}
    .subtitle{font-size:12px;color:var(--muted)}

    /* tabs */
    .tabs{display:flex;gap:8px}
    .tab{padding:8px 14px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);cursor:pointer;border:1px solid rgba(255,255,255,0.02);backdrop-filter:blur(6px)}
    .tab.active{background:linear-gradient(90deg,var(--accent-1),var(--accent-2));color:#012;font-weight:700;box-shadow:var(--shadow);transform:translateY(-2px)}

    /* cards */
    .card{background:var(--card);border-radius:var(--radius);padding:16px;box-shadow:var(--shadow);backdrop-filter:blur(8px)}
    .grid{display:grid;grid-template-columns:1fr 340px;gap:18px}

    /* devices list */
    .devices-wrap{display:flex;flex-direction:column;gap:12px}
    .toolbar{display:flex;justify-content:space-between;align-items:center;gap:10px}
    .btn{border:0;padding:8px 12px;border-radius:10px;cursor:pointer;font-weight:600}
    .btn.ghost{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted)}
    .btn.primary{background:linear-gradient(90deg,var(--accent-1),var(--accent-2));color:#012}

    .devices{display:flex;gap:14px;overflow:auto;padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), transparent)}
    .device{min-width:220px;padding:12px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));box-shadow:0 8px 20px rgba(2,6,23,0.45);display:flex;flex-direction:column;gap:8px;transition:transform .18s ease,box-shadow .18s ease}
    .device:hover{transform:translateY(-6px);box-shadow:0 18px 40px rgba(2,6,23,0.6)}
    .device .title{display:flex;align-items:center;gap:10px}
    .avatar{width:44px;height:44px;border-radius:10px;background:linear-gradient(135deg,#1b9cff,#7cffb2);display:grid;place-items:center;font-weight:800;color:#012}
    .dname{font-weight:700}
    .dmeta{font-size:12px;color:var(--muted)}
    .actions{display:flex;gap:8px;margin-top:6px}
    .pill{padding:6px 8px;border-radius:999px;font-size:12px;color:#012;background:rgba(255,255,255,0.9);display:inline-block}

    /* right column */
    .right{display:flex;flex-direction:column;gap:12px}
    .section-title{font-weight:700}
    .history{max-height:180px;overflow:auto;display:flex;flex-direction:column;gap:10px;margin-top:8px}
    .history .item{padding:10px;border-radius:10px;background:linear-gradient(180deg, rgba(255,255,255,0.02), transparent);font-size:13px;color:var(--muted)}
    .noti-list{display:flex;flex-direction:column;gap:10px;margin-top:8px}
    .noti{padding:12px;border-radius:10px;background:linear-gradient(115deg, rgba(255,255,255,0.02), transparent)}

    /* guide */
    .guide p{line-height:1.6;color:#dff9ff}

    /* modal */
    .modal-back{position:fixed;inset:0;background:rgba(0,0,0,0.6);display:none;align-items:center;justify-content:center;z-index:120}
    .modal{width:380px;background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);padding:18px;border-radius:14px;box-shadow:0 30px 80px rgba(2,6,23,0.7);backdrop-filter:blur(10px)}
    input[type=text],select{width:100%;padding:10px;border-radius:10px;border:1px solid rgba(255,255,255,0.06);background:transparent;color:inherit;margin-bottom:12px}

    /* animations */
    .fadeIn{animation:fadeIn .45s ease both}
    @keyframes fadeIn{from{opacity:0;transform:translateY(8px)}to{opacity:1;transform:none}}

    /* responsive */
    @media (max-width:980px){.grid{grid-template-columns:1fr}.right{order:2}}
    @media (max-width:520px){body{padding:12px}.tabs{flex-wrap:wrap}.devices{padding:10px}}

    /* small text */
    .muted{color:var(--muted)}
  </style>

<style>
/* Nền particle */
#particle-bg {
  position: fixed;
  top: 0; left: 0;
  width: 100%; height: 100%;
  z-index: -1;
  background: black;
}

/* Toast notification */
.toast {
  position: fixed;
  right: 20px;
  bottom: 20px;
  background: rgba(0,0,0,0.8);
  color: white;
  padding: 10px 15px;
  border-radius: 10px;
  animation: fadeInUp 0.5s, fadeOutDown 0.5s 3s forwards;
  font-family: sans-serif;
}
@keyframes fadeInUp {
  from { opacity: 0; transform: translateY(20px); }
  to { opacity: 1; transform: translateY(0); }
}
@keyframes fadeOutDown {
  to { opacity: 0; transform: translateY(20px); }
}

/* Modal animation */
.modal-content {
  animation: modalPop 0.6s ease;
  box-shadow: 0 0 20px #0ff;
}
@keyframes modalPop {
  from { transform: scale(0.7) rotate(-5deg); opacity: 0; }
  to { transform: scale(1) rotate(0); opacity: 1; }
}

/* Badge */
.badge {
  display: inline-block;
  padding: 5px 10px;
  border-radius: 20px;
  background: linear-gradient(45deg, gold, orange);
  color: black;
  font-weight: bold;
  margin: 5px;
}

/* Theme */
body.theme-neon {
  background: linear-gradient(135deg, #0ff, #00f);
  color: white;
}
body.theme-galaxy {
  background: radial-gradient(circle at center, #1a0023, #000);
  color: #fff;
}
body.theme-cyber {
  background: linear-gradient(135deg, #111, #0f0);
  color: #0f0;
}
</style>


<style>
/* Move tabs to bottom fixed bar */
.tabs {
  position: fixed !important;
  bottom: 16px;
  left: 50%;
  transform: translateX(-50%);
  z-index: 250;
  background: rgba(0,0,0,0.6);
  padding: 8px 12px;
  border-radius: 999px;
  gap: 8px;
  box-shadow: 0 8px 24px rgba(0,0,0,0.6);
}
.tabs .tab { margin: 0 6px; }
main { padding-bottom: 120px; } /* give space for fixed tabs */
</style>


<style>
/* Collapsible tab styles */
.tab-toggle {
  position: fixed;
  right: 18px;
  bottom: 18px;
  width: 56px;
  height: 56px;
  border-radius: 50%;
  background: linear-gradient(90deg,#00f5d4,#00b4ff);
  color: #012;
  font-size: 24px;
  border: none;
  z-index: 300;
  box-shadow: 0 8px 24px rgba(0,0,0,0.4);
  cursor: pointer;
  display: grid;
  place-items: center;
}
.tabs {
  position: fixed !important;
  bottom: 86px;
  left: 50%;
  transform: translateX(-50%) translateY(12px);
  z-index: 250;
  background: rgba(0,0,0,0.6);
  padding: 8px 12px;
  border-radius: 999px;
  gap: 8px;
  box-shadow: 0 8px 24px rgba(0,0,0,0.6);
  transition: transform .25s ease, opacity .25s ease;
  opacity: 0;
  pointer-events: none;
  display: flex;
  flex-direction: row; /* horizontal layout */
  align-items: center;
}
.tabs.open {
  transform: translateX(-50%) translateY(0);
  opacity: 1;
  pointer-events: auto;
}
.tabs .tab { margin: 0 6px; white-space: nowrap; }
@media (max-width:520px){
  .tabs { left: 50%; right: auto; bottom: 86px; overflow-x:auto; max-width:90%; }
}
main { padding-bottom: 160px; } /* give space for toggle button and tabs */
</style>

</head>
<body>

<!-- Floating tab toggle button -->
<button id="tabToggle" class="tab-toggle" aria-label="Hiển thị tab">☰</button>

  <div class="app">
    <header>
      <div class="brand">
        <div class="logo">
          <!-- simple cloud icon -->
          <svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M6 18h12a4 4 0 0 0 0-8 6 6 0 0 0-11-2 5 5 0 0 0-1 10z" fill="#012" opacity="0.12"/>
            <path d="M6 18h12a4 4 0 0 0 0-8 6 6 0 0 0-11-2 5 5 0 0 0-1 10z" fill="white" opacity="0.18"/>
          </svg>
        </div>
        <div>
          <h1>Cloud Game VIP</h1>
          <div class="subtitle">Quản lý thiết bị chơi game đám mây — giao diện VIP</div>
        </div>
      </div>

      <div class="tabs" role="tablist">
        <div class="tab" data-tab="othergames">Game khác</div>
        <div class="tab" data-tab="minigame">Mini Game</div>
        <div class="tab active" data-tab="home">Trang chủ</div>
        <div class="tab" data-tab="devices">Thiết bị</div>
        <div class="tab" data-tab="guide">Hướng dẫn</div>
        <div class="tab" data-tab="notifications">Thông báo</div>
      </div>
    </header>

    <main>

      <section id="home" class="card fadeIn" style="margin-top:14px">
        <div class="section-title">Chào mừng đến Cloud Game VIP</div>
        <div style="margin-top:10px;display:flex;flex-direction:column;align-items:center">
          <video width="500" height="300" controls autoplay muted loop style="border-radius:12px;box-shadow:0 8px 20px rgba(0,0,0,0.4)">
            <source src="354fb85019e2afb05b5bc8f496f30126_1754178561512.mp4" type="video/mp4">
            Trình duyệt của bạn không hỗ trợ video.
          </video>
          <div style="margin-top:12px;text-align:center;color:var(--muted)">
            Đây là bản xem trước ứng dụng Cloud Game VIP.<br>
            Bạn có thể quản lý thiết bị, xem hướng dẫn và nhận thông báo từ các tab bên trên.
          </div>
        </div>
      
<div id="rewardCodeBox" style="display:none;margin-top:10px;padding:10px;border:1px solid #ccc;border-radius:6px;background:#f9f9f9;">
  <span id="rewardCodeText" style="font-weight:bold;"></span>
  <button id="copyRewardCodeBtn" style="margin-left:10px;padding:4px 8px;">Sao chép</button>
</div>

<div style="margin-top:15px;">
  <div><strong>Số vòng quay đã quay:</strong> <span id="spinCount">0</span></div>
  <div style="margin-top:8px;"><strong>Lịch sử quay gần đây:</strong></div>
  <ul id="spinHistory" style="margin-top:5px;padding-left:20px;"></ul>
</div>
</section>

      <section id="devices" class="card fadeIn">
        <div class="grid">
          <div class="devices-wrap">
            <div class="toolbar">
              <div>
                <div class="section-title">Thiết bị </div>
                <div class="muted small">Quản lý máy ảo của bạn — Ấn thêm thiết bị để sử dụng nhé</div>
              </div>
              <div style="display:flex;gap:8px;align-items:center">
                <button id="btnAdd" class="btn primary">+ Thêm thiết bị</button>
                <button id="btnRefresh" class="btn ghost">Làm mới</button>
              </div>
            </div>

            <div class="devices" id="deviceList" aria-live="polite">
              <!-- devices go here -->
            </div>

            <div style="display:flex;justify-content:space-between;align-items:center;margin-top:10px">
              <div class="muted">Tổng thiết bị: <strong id="count">0</strong></div>
              <div class="muted">Lưu: localStorage</div>
            </div>

          </div>

          <aside class="right">
            <div class="card">
              <div class="section-title">Hoạt động gần đây</div>
              <div class="muted small">Lịch sử khởi động, thêm/xoá</div>
              <div class="history" id="history"></div>
              <div style="display:flex;gap:8px;margin-top:10px">
                <button id="clearHistory" class="btn ghost">Xoá lịch sử</button>
                <button id="exportLog" class="btn ghost">Export</button>
              </div>
            </div>

            <div class="card">
              <div class="section-title">Thông tin nhanh</div>
              <div class="muted small" style="margin-top:8px">Phiên bản VIP: 1.0 • Mượt như sunsilk </div>
              <div style="margin-top:12px;display:flex;gap:8px">
                <div class="pill">Không yêu cầu server</div>
                <div class="pill">Chế độ: Tiêu chuẩn</div>
              </div>
            </div>
          </aside>
        </div>
      </section>
<style>
  .sub-options {
    max-height: 160px;
    overflow-y: auto;
    border: 1px solid #ccc;
    border-radius: 6px;
    padding: 8px;
    margin-top: 10px;
    background: #fff;
    display: none;
  }
  .sub-options .option-item {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 6px;
    margin-bottom: 6px;
    background: #f9f9f9;
    border-radius: 4px;
  }
  .sub-options button {
    padding: 4px 8px;
    border: none;
    border-radius: 4px;
    background: #007bff;
    color: white;
    cursor: pointer;
  }
</style>

<div id="proOptions" class="sub-options">
  <div class="option-item"><span>Thiết bị Pro App Launcher</span><button data-name="App Launcher (Pro)" data-url="https://stagingngg.net/apps/uncube/10005/now.html">Thêm</button></div>
  <div class="option-item"><span>Thiết bị Pro Roblox</span><button data-name="Roblox (Pro)" data-url="https://google.com">Thêm</button></div>
</div>

<div id="vpnOptions" class="sub-options">
  <div class="option-item"><span>Thiết bị VPN 1</span><button data-name="VPN 1" data-url="https://now.gg">Thêm</button></div>
  <div class="option-item"><span>Thiết bị VPN 2</span><button data-name="VPN 2" data-url="https://turbolite.asia">Thêm</button></div>
</div>


      <section id="guide" class="card" style="display:none;margin-top:14px">
        <div class="section-title">Hướng dẫn sử dụng</div>
        <div style="margin-top:10px" class="guide">
          <p><strong>1.</strong> Nhấn <em>"Thêm thiết bị"</em> để tạo một máy ảo mới. Bạn có thể đặt tên và chọn loại.</p>
          <p><strong>2.</strong> Mỗi thiết bị có 2 nút: <em>Khởi động</em> (bật/tắt) và <em>Xoá</em>. Trạng thái được lưu trên localStorage.</p>
          <p><strong>3.</strong> Mở tab <em>Thông báo</em> để xem tất cả thông báo hệ thống. Các thông báo mới được thêm khi bạn khởi động/xoá/thêm thiết bị.</p>
          <p><strong>4.</strong> Dữ liệu được lưu cục bộ — để xóa hoàn toàn: vào DevTools -> Application -> Local Storage -> xóa key <code>cg_vip_devices</code>.</p>
        </div>
      </section>

      <section id="notifications" class="card" style="display:none;margin-top:14px">
        <div class="section-title">Thông báo</div>
        <div class="muted small">Các thông báo hệ thống mới nhất</div>
        <div class="noti-list" id="notiList"></div>
        <div style="display:flex;gap:8px;margin-top:12px">
          <button id="markAll" class="btn ghost">Đánh dấu tất cả đã đọc</button>
          <button id="clearNoti" class="btn ghost">Xoá tất cả</button>
        </div>
      </section>


      

      

<section id="minigame" class="card fadeIn" style="margin-top:14px;display:none">
  <div class="section-title">Mini Game: Flappy Bird</div>
  <canvas id="flappyCanvas" width="320" height="480" style="background:#70c5ce;display:block;margin:10px auto;border-radius:8px"></canvas>
</section>
<script>
(function(){
  const canvas = document.getElementById('flappyCanvas');
  const ctx = canvas.getContext('2d');

  // Game settings
  const gravity = 0.5;
  const jump = -8;
  const pipeWidth = 50;
  const pipeGap = 120;

  let birdX = 50;
  let birdY = 150;
  let birdVel = 0;

  let pipes = [];
  let score = 0;
  let gameOver = false;

  function resetGame(){
    birdY = 150;
    birdVel = 0;
    pipes = [];
    score = 0;
    gameOver = false;
    pipes.push({x: canvas.width, y: Math.floor(Math.random()*200)+50});
  }

  
  const birdImg = new Image();
  birdImg.src = 'bird_gif.gif'; // duck/flappy bird style sprite

  function drawBird(){
    if (birdImg.complete) {
      ctx.drawImage(birdImg, birdX - 15, birdY - 12, 30, 24);
    } else {
      ctx.fillStyle = '#ff0';
      ctx.beginPath();
      ctx.arc(birdX, birdY, 10, 0, Math.PI*2);
      ctx.fill();
    }
  }


  function drawPipes(){
    ctx.fillStyle = '#0f0';
    pipes.forEach(p=>{
      ctx.fillRect(p.x, 0, pipeWidth, p.y);
      ctx.fillRect(p.x, p.y+pipeGap, pipeWidth, canvas.height - (p.y+pipeGap));
    });
  }

  function drawScore(){
    ctx.fillStyle = '#fff';
    ctx.font = '20px Arial';
    ctx.fillText("Score: " + score, 10, 25);
  }

  function update(){
    if(gameOver) return;
    birdVel += gravity;
    birdY += birdVel;

    pipes.forEach(p=>{
      let speed = 2 + score; // speed increases by 1 per point
      p.x -= speed; // speed increases every 5 points
      if(p.x + pipeWidth < 0){
        p.x = canvas.width;
        p.y = Math.floor(Math.random()*200)+50;
        score++;
      }

      // Collision detection
      if(birdX + 10 > p.x && birdX - 10 < p.x + pipeWidth){
        if(birdY - 10 < p.y || birdY + 10 > p.y + pipeGap){
          gameOver = true;
        }
      }
    });

    if(birdY + 10 > canvas.height || birdY - 10 < 0){
      gameOver = true;
    }
  }

  function render(){
    ctx.clearRect(0,0,canvas.width,canvas.height);
    drawPipes();
    drawBird();
    drawScore();
    if(gameOver){
      ctx.fillStyle = 'rgba(0,0,0,0.5)';
      ctx.fillRect(0,0,canvas.width,canvas.height);
      ctx.fillStyle = '#fff';
      ctx.font = '24px Arial';
      ctx.fillText("Game Over", 90, 200);
      ctx.font = '16px Arial';
      ctx.fillText("Click to restart", 100, 230);
    }
  }

  function loop(){
    update();
    render();
    requestAnimationFrame(loop);
  }

  canvas.addEventListener('click', ()=>{
    if(gameOver){
      resetGame();
    } else {
      birdVel = jump;
    }
  });

  resetGame();
  loop();
})();
</script>

  




      <section id="othergames" class="card" style="display:none;margin-top:14px">
        <div class="section-title">Game khác</div>
        <div class="muted small">Danh sách game — bấm Play để chơi (không cần sử dụng vpn)</div>

        <div style="margin-top:12px;display:flex;flex-direction:column;gap:12px">
          <!-- Game item template -->
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAOEAAADhCAMAAAAJbSJIAAAAeFBMVEUAAAD////8/PwEBAT5+fn29vYICAjq6updXV20tLTk5OTr6+sjIyPV1dXf399BQUHLy8upqaliYmKEhIR1dXU2NjYTExPDw8NqamqYmJienp5KSkqRkZG7u7tEREQQEBBTU1N/f38wMDAeHh5OTk5wcHCcnJwsLCxZgUWvAAAJTElEQVR4nO2diXbiOgyGbcfZSLMBgbJNgbbT93/Da9kOMC2LUlIBvfpOT6eHgcR/LMuyvCAEwzAMwzAMwzAMwzAMwzAMwzAMwzAMwzAMwzAMwzAPRiQCIZ6GzaeXg5sU5kewUoYyXy1fD14IRPB7NBoxIpVaqjBOn8uJf8no+zUawUzDUCqllZJ6Wo+f2v/5LQpNVZWhsgqlklKGcTX6c+tC9UgAlThTyqmT/rcs0lHy8s+7HrlGA7GSR8iq+tm/IQjsk4iC4BHbpilzU3zVp1xlFrOkhHe9tN71ARUahuqrQPNj2qU2/xTT+cK+LQhs3/l4GgOxPGak0DJ969RhNm37kcfTZ/yMyE8aKVRjW8FVPf4c+DwGplL0sTr8bLSgN85n5f5j4mEsdn1R4KHSzPQjNiawfucxnE8tv3qakxJDEJmvxhP32QdQGBxthmckKg1GrWU8S2zkc/e+JxDruIM+bYNX7ZxstqqHty4/hpHqYKVe5+7PMKvGzeTWEi5Qd5N3hLzeuJjAxnfCxXj30zxfBm3ndwVqUKVrd70gCu5HnKWxoctV+KBAV6NkC5eMfGXeCZuurfBIDcJDCu3YMk9HLhliBiI3FrZjKjt7mq+VGILMUNuAXQ3qpHy5fGMSjDm9DqS8VqHa/yjXqMPpfNgmtg6GI9TVakd8w/Bqgcc1h3G1aaKdsiCK6EVarz434UnYu0Kpnfcq6tEb3Cpy96P3P4GIpuAleq9E2x5tbkvGeb12d4vIe0mowjKTPXiaLwLNBSF8NRrdtfPl0A67iOsQbpe4sXz/Cp1f1buHp4rVsrxcpt41irRnbWcJ43T4QatPiAGlQqjQZ0qFRuJH/07mnD4lC9pUTyCWhAIlNM4VsUCxolQIbmdJrHCb/0A8c0ZiqKmNNPmBaOY0xkozUoGG0U/EpOck1tQKK1KBkrqvMJAaqSGkjmreZP8B21mm1Fm5tB3kUPHrm2H4TixwMaB1pTJ+JVa4+Sd7TUAliEfANXUz3BCnUSc55IsoFf4hHOTDjRpswSDbomG4fkWFQ9Q9EMRpjDFeobb2fIVCOxuXEoqzzaFCF88UMJRX+V3b4EeCbs7GKsyQpYsL2cr7tkYwgywRPnFKBHrktNyu5wXMTFzRs4CR5hGxK52hCmaARy9eNnVuLVX5l7slWeG9KfXUIiaPGKqD3NFTskmtZRvfaqfSOubKSaf8zYMsUesTlGw9oJ9Y2S6LgbXWUHcTqCWlQFA4RJXL2OLMf2TXhprxrLJVqDtVYUGtENMMgWxx8LHIx5WTJlnFHcMh2iybIcZ4Clgzs38ofilb6ysWy/TIutTjaHBYlH40EBHKwvbN8PCz+99NsixQF9KqKIlngHEhm/Z9xWm2A6TDmdLo2pOiokwTL19I4a5xqR4t/9Lo2vGESnabt1QXckczZCinF8SD3yRDjhTmFy6Uw1w24joxiawDkMlurccXRnRa4cK3KVnQ7VfVrZD99eDklG3g1qoge331TjissFWC7a3z08MB2JsADgs35ChJm2EACQxMuZQdtJ4gMtJfYXkxph1W1HnEmRkdoJrPx+lHD5W7zvyii0tAspvOSu3KbpwnPesBA7uuUWEyksZhUXoaE2zFGCO1IduZUXkU2GZ46WGBr40b/0ioJI5x+uS5ZmgvhFirAvpVTplGhDthVnZDPxcO7YDpxIWE+EBdx0icUanzTBB5RNuP50/nHn1g4gZU6KdlQzxyKjHlUm7W/eRaZmigqK0oYAvuvlQCA/GOaYZaQch2drH2xwA5yEwF5fb3CFZ2o568DC900++okM0mu4nBZNlgxHApdzRHXAcUZhdG0f1iLGWBC9jUpZHTpEJFtwocFi1/cTGpvpjAQI2bFO2ckwXTDIFie/46CXYmY0yjy2P6igIzGDAddbZMmn8++YmVxA0OVUTcG6IfvYSTFZaHm9LEQdrUzs6hOnzyBMbRremnCeM02foDT/7pHhfYUTR1yCbQeWpbA24Wpvr77g12P32xxM6vDal3A3Wa6IRMmp1RCwfFcus1uuukyDxiTJvAwM457QVKt3/bisnSzbrt25pC4vKIKzqBgZ2DhYnRrtt+W7kgMk/HdkCVHPzPWSiT3dCEovzKTUCwzbCYr5sR8v0hZcgGzz7J7LqIb8trNxgOsFvcM8ods4EdtCKbzwlgvxYuTeepqPcEp/KatU3u1BrdxdApQ7bA7XNCJqlPSNR++I++RkO8Wq/8vrjuwP7bnHJlNzSHDaVCaPA3WNlNCAw9NpTqjJG+djjG5HqMwMHicrl65Z12C4myK7vpQCa7+9NnmiF1AmOCTWD0pFDKN2KFJfk+J2KB4plWH3UzFN0O9epDIH2yO9PXRGzdFYa0q/WE2F4xbvoW+ZZ05Tqs0Or/BIxzqJQ6B7XCrZvojxFxFTaFIt2Np9QrcRU+X7Vj4hvE1Ke1PA3TOKS00pRwF9COcrkq2v097vBVu6jpB86nMT/JTU7cMSKHy9xp1PujgPpWaNfAl9R1aE9p8s5tXeexzSrZrHb/x0TBZae0s2pWYjutYmW+jWq3Ke0nwoDQ2P6c/OsH3M3saX/+vlGzqeIfO69t2C7XpRfp5jn936/D+dRvSlN+Hd71dmuz4q+0uw3P8VIm9cC1R23z2eG1dgtPiXyDxSna0/5eR6nbYBj24nsUbZbtLNb7WJXbZFS52rvW+YArva/Tzd3UomWdVrjlaucVysG9nO/pT/x1x/96kYtN3ekA7KOQJ7s7MmnGVbbPW3XbS2k9DXkC4zsM65U7NxIOKYdfHXTG6zs7LvkrzmT/DGdu1bvueEhIfkenXR9n97UAxmLHqzxzKzLwVnrvzfDzFx88JaMUt8irZX3LwiMJDkI8SznLY2w/qe/eSE/QjOt2BhJm8314cKRq8/uJSTvgKnVSPk8zG7j676E5arrLB6xCO+aKvOku5lNIhmi3i/GrRvUQXwrxmcA7n0DYeKxMZsVJIy2a+/9ijyNAhiCKXIzni/9cV0dPuVk9oJHu+HQm94vpR/yKVdVWqZIzET2qMz3On5FNhrS+Bw6AfEQjPcpOx9O4nmp3jrfWGTilWxarRw6+dAX6kTS2h/TfJNn9Y7T6vKKn+apwpwn9HolfpJTPdn/0bzFThmEYhmEYhmEYhmEYhmEYhmEYhmEYhmEYhmEYhvkf8R8RRGG2iRPOzwAAAABJRU5ErkJggg==" alt="Uncube" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Roblox</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/a/19900/b.html">Play</button>
            </div>
          </div>

          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/com.miHoYo.GenshinImpact/icon/genshin-impact.png" alt="Roblox" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Genshin Impact</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/cognosphere-pte-ltd-/1773/genshin-impact.html">Play</button>
            </div>
          </div>

          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.dts.freefireth%252Ficon%252Ffree-fire.png%26w%3D256%26q%3D80&w=640&q=70" alt="Now.gg" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Free Fire</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/garena-international-i/1398/free-fire.html">Play</button>
            </div>
          </div>

          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/com.kurogame.gplay.punishing.grayraven.en/icon/gray-raven.png" alt="TurboLite" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Punishing</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/kuro-technology/9609/gray-raven.html">Play</button>
            </div>
          </div>

          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://st.download.com.vn/data/image/2024/01/02/Code-Fortnite-700.jpg" alt="Example" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Fortine</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/a/10004/b.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/air.com.lunime.gachalife2/icon/gacha-life-2.png" alt="Gacha Life" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Gacha Life 2</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/lunime/5691/gacha-life-2.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F19901%252Ficon%252Fb.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Roblox 2" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Roblox 2</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/Blox-fruit/19901/Blox-fruit.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/com.HoYoverse.hkrpgoversea/icon/honkai-star-rail.png" alt="Honkai Star Rail" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Honkai Star Rail</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/cognosphere-pte-ltd/1591/honkai-star-rail.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/9157/icon/cluster.png" alt="Cluster" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Cluster</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://turbolite.vercel.app/server/url?data=aHR0cHM6Ly91cHJveHkub25saW5lL3VsdHJhdmlvbGV0L2h2dHJzOCUyRi1ubXclMkNnZSUyRmNwcnMtY251cXRnciUyRmlsYy05MzU1JTJGYWx3c3ZlcC5qdG9s&fs=0">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F10539%252Ficon%252Fzombie-tsunami.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Zombie Tsunami" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Zombie Tsunami</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/mobigame/10539/zombie-tsunami.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fapps-content%2F8861%2Ficon%2Fshadow-fight-3.png&w=128&q=80" alt="Shadow Light 3" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Shadow Light 3</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://webproxy.proxyshare.com/request?p=GgkeGkYuKF0ORhMPDwsIQVRUFRQMVRwcVBoLCwhUFR4QEBJUQ0NNSlQIExofFAxWHRIcEw9WSFUTDxYX">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fnow-gg-store%2F339%2Fcom.nebulajoy.act.dmcpoc.nowgg%2F10545%2Fassets%2Fen-US%2F1749634978%2F2-2.png&w=128&q=80" alt="Devil May Cry" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Devil May Cry</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://webproxy.proxyshare.com/a3226eaf5a2143fc897797c9a194fdff/_rhsfc7Ya://7KB.Y2/w4Bd/u8hv4vSOUNgOSRNRsr3klUUDfU--6Z0z50Czz/KKjj4/ybKVwBYfBdZJdqj2EpGOvNxXdiiR.dDrr">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="512.png" alt="Assault Lily" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Assault Lily</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int1.now.gg/apps/pokelabo-inc/5139/assault-lily-last-bullet.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://images.sftcdn.net/images/t_app-icon-m/p/c02e9279-28df-462a-b7dc-4ab1f0c77036/2583136360/human-heroes-curie-on-matter-logo" alt="Human Heros" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Human Heros</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive7.now.gg/apps/plug-in-digital/9437_t1/human-heroes-curie-on-matter-ml.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F9059%252Ficon%252Ftales-of-terrarum.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Terrarum" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Terrarum</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://webproxy.proxyshare.com/request?p=GgkeGkYuKF0ORhMPDwsIQVRUDx4IDx8JEg0eT1UVFAxVHBxUGgsLCFQeFx4YDwkUFRIYVggUDhdUQktOQiQPSlQPGhceCFYUHVYPHgkJGgkOFlUTDxYX">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/9887/icon/scarlet-girls.png" alt="Scarlett Girl" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Scarlett Girl</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://webproxy.proxyshare.com/request?p=GgkeGkYuKF0ORhMPDwsIQVRUFRQMVRwcVBoLCwhUGQ4JCA8cGhYeVEJDQ0xUCBgaCRceD1YcEgkXCFUTDxYX">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F10512%252Ficon%252Fthe-walking-dead-survivors.png%26w%3D256%26q%3D80&w=1440&q=70" alt="The Walking Dead" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">The Walking Dead</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive4.now.gg/apps/galaxy-play-technology-limited/10512_t1/the-walking-dead-survivors.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F8270%252Ficon%252Fbattle-bears-heroes.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Battle Bears" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Battle Bears</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive4.now.gg/apps/battlecoin-games/8270_t1/battle-bears-heroes.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/apps-content/9030/icon/magic-forest-dragon-quest.png" alt="Magic Forest" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Magic Forest</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive4.now.gg/play/sugar-game-network-limited/9030/magic-forest-dragon-quest">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F10382%252Ficon%252Fancient-seal-the-exorcist.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Ancient Seal" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Ancient Seal</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive4.now.gg/play/lovo-entertainment-hong-kong-limited/10382/ancient-seal-the-exorcist">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252F8706%252Ficon%252Fnexus-nebula-echoes.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Nexus" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Nexus</div>
              <div class="muted small">⬇️Tạm⬇️</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive4.now.gg/apps/magic-game/8706/nexus-nebula-echoes.html">Play</button>
            </div>
          </div>       
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.aptoide.partners.nowgg.store%252Ficon%252Faptoide.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Nhiều Game" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Nhiều Game</div>
              <div class="muted small">🔥VIP PRO🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/aptoide/5874/aptoide.html">Play</button>
            </div>
          </div>

 <div class="muted small">Danh sách app — bấm Play để sử dụng app</div>
 
 <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.discord%252Ficon%252Fdiscord-talk-chat-hang-out.png%26w%3D256%26q%3D80&w=640&q=70" alt="Discord" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Discord</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://stagingngg.net/apps/discord-inc-/1430/discord-talk-chat-hang-out.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.zhiliaoapp.musically%252Ficon%252Ftiktok.png%26w%3D256%26q%3D80&w=640&q=70" alt="Tiktok" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Tiktok</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/tiktok/4478/tiktok.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.instagram.android%252Ficon%252Finstagram.png%26w%3D256%26q%3D80&w=640&q=70" alt="Instagram" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Instagram</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/instagram/1228/instagram.html">Play</button>
            </div>
          </div>
          
          <div class="game-item card" style="display:flex;align-items:center;gap:12px;padding:10px">
            <img src="https://cdn.now.gg/assets-opt/_next/image?url=https%3A%2F%2Fcdn.now.gg%2Fassets-opt%2F_next%2Fimage%3Furl%3Dhttps%253A%252F%252Fcdn.now.gg%252Fapps-content%252Fcom.google.android.youtube%252Ficon%252Fyoutube.png%26w%3D256%26q%3D80&w=1440&q=70" alt="Youtube" style="width:80px;height:80px;border-radius:8px;object-fit:cover" />
            <div style="flex:1">
              <div style="font-weight:700">Youtube</div>
              <div class="muted small">🔥VIP🔥</div>
            </div>
            <div>
              <button class="btn primary play-btn" data-url="https://testdrive-int2.now.gg/apps/google-llc/1395/youtube.html">Play</button>
            </div>
          </div>
          
          <h1> Hết r <h1>
          
        </div>
      </section>

</main>
  </div>

  <!-- modal add device -->
<div class="modal-back" id="modalBack">
  <div class="modal card">
    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
      <div style="display:flex;gap:10px;align-items:center">
        <div style="width:44px;height:44px;border-radius:10px;background:linear-gradient(90deg,var(--accent-1),var(--accent-2));display:grid;place-items:center;color:#012;font-weight:800">VD</div>
        <div>
          <div style="font-weight:700">Chọn loại thiết bị</div>
          <div class="muted small">Nhấn để thêm ngay thiết bị</div>
        </div>
      </div>
      <button id="modalClose" class="btn ghost">Đóng</button>
    </div>
    <div style="display:flex;flex-direction:column;gap:10px">
      <button id="addPro" class="btn primary">Thiết Bị PRO (Mượt)</button>
      <button id="addVPN" class="btn ghost">Thiết Bị VPN (Hơi cùi)</button>
    </div>
  </div>
</div>

  <script>
    // State and persistence
    const LS_KEY = 'cg_vip_devices';
    const LS_NOTI = 'cg_vip_noti';
    const LS_HISTORY = 'cg_vip_history';

    let state = {
      devices: JSON.parse(localStorage.getItem(LS_KEY) || '[]'),
      noti: JSON.parse(localStorage.getItem(LS_NOTI) || '[]'),
      history: JSON.parse(localStorage.getItem(LS_HISTORY) || '[]')
    }

    // Elements
    const deviceListEl = document.getElementById('deviceList');
    const countEl = document.getElementById('count');
    const historyEl = document.getElementById('history');
    const notiListEl = document.getElementById('notiList');

    // Init default noti
    if(state.noti.length === 0){ state.noti.push({text:'Chào mừng đến Cloud Game VIP!', time:Date.now()}); save(); }

    // Helpers
    function save(){
      localStorage.setItem(LS_KEY, JSON.stringify(state.devices));
      localStorage.setItem(LS_NOTI, JSON.stringify(state.noti));
      localStorage.setItem(LS_HISTORY, JSON.stringify(state.history));
    }

    function fmtTime(ts){ const d=new Date(ts); return d.toLocaleString(); }
    function escapeHtml(s){ return String(s).replace(/&/g,'&amp;').replace(/</g,'&lt;').replace(/>/g,'&gt;'); }

    // Render
    function renderDevices(){
      deviceListEl.innerHTML='';
      state.devices.forEach((d, idx)=>{
        const el = document.createElement('div'); el.className='device fadeIn';
        el.innerHTML = `
          <div class="title">
            <div class="avatar">${escapeHtml(String(d.name || '').charAt(0).toUpperCase() || 'D')}</div>
            <div style="flex:1">
              <div class="dname">${escapeHtml(d.name)}</div>
              <div class="dmeta">${escapeHtml(d.type)} • ${fmtTime(d.created)}</div>
            </div>
            <div style="margin-left:8px"><div class="pill">${d.running? 'Đang chạy':'Tắt'}</div></div>
          </div>
          <div style="flex:1"></div>
          <div class="actions">
            <button class="btn primary" data-act="toggle" data-idx="${idx}">${d.running? 'Tắt':'Khởi động'}</button>
            <button class="btn ghost" data-act="del" data-idx="${idx}">Xoá</button>
          </div>
        `;
        deviceListEl.appendChild(el);
      })
      countEl.textContent = state.devices.length;
      // attach events
      deviceListEl.querySelectorAll('[data-act]').forEach(btn=>{
        btn.onclick = (e)=>{
          const idx = Number(btn.dataset.idx);
          const act = btn.dataset.act;
          if(act==='toggle') toggleStart(idx);
          if(act==='del') removeDevice(idx);
        }
      })
    }

    function renderHistory(){
      historyEl.innerHTML = '';
      state.history.slice().reverse().forEach(h=>{
        const div = document.createElement('div'); div.className='item'; div.textContent = h; historyEl.appendChild(div);
      })
    }

    function renderNoti(){
      notiListEl.innerHTML='';
      state.noti.slice().reverse().forEach(n=>{
        const div = document.createElement('div'); div.className='noti';
        div.innerHTML = `<div style="display:flex;justify-content:space-between;align-items:center"><div>${escapeHtml(n.text)}</div><div class="muted small">${fmtTime(n.time)}</div></div>`;
        notiListEl.appendChild(div);
      })
    }

    // Actions
    function toggleStart(i){
  const d = state.devices[i]; if(!d) return;
  if (!d.running) {
    if (d.type === 'Pro') {
      window.open('https://stagingngg.net/apps/uncube/10005/now.html', '_blank');
    } else if (d.type === 'VPN') {
      window.open('https://testdrive-int2.now.gg/apps/uncube/7074/now.html', '_blank');
    }
  }
  d.running = !d.running;
  const txt = d.running? `Đã khởi động ${d.name}` : `Đã tắt ${d.name}`;
  state.history.push(txt);
  state.noti.push({text:txt,time:Date.now()});
  save(); renderDevices(); renderHistory(); renderNoti();
}

    function removeDevice(i){
      const rem = state.devices.splice(i,1)[0];
      state.history.push(`Xoá thiết bị ${rem.name}`);
      state.noti.push({text:`Xoá thiết bị ${rem.name}`,time:Date.now()});
      save(); renderDevices(); renderHistory(); renderNoti();
    }

    // Modal xử lý
const modalBack = document.getElementById('modalBack');
document.getElementById('btnAdd').addEventListener('click',()=>{ modalBack.style.display='flex'; });
document.getElementById('modalClose').addEventListener('click',()=>{ modalBack.style.display='none'; });

function addDevice(name, type){
  const device = {name,type,created:Date.now(),running:false,id:Date.now()+Math.random()};
  state.devices.push(device);
  state.history.push(`Đã thêm thiết bị ${device.name}`);
  state.noti.push({text:`Đã thêm thiết bị ${device.name}`,time:Date.now()});
  save(); renderDevices(); renderHistory(); renderNoti();
  modalBack.style.display='none';
}

document.getElementById('addPro').addEventListener('click',()=>{ addDevice('Thiết Bị PRO','Pro'); });
document.getElementById('addVPN').addEventListener('click',()=>{ addDevice('Thiết Bị VPN','VPN'); });

    document.getElementById('btnRefresh').addEventListener('click',()=>{ renderDevices(); });
    document.getElementById('clearHistory').addEventListener('click',()=>{ state.history=[]; save(); renderHistory(); });
    document.getElementById('exportLog').addEventListener('click',()=>{ const data = JSON.stringify({devices:state.devices,noti:state.noti,history:state.history},null,2); const blob = new Blob([data],{type:'application/json'}); const url = URL.createObjectURL(blob); const a = document.createElement('a'); a.href=url; a.download='cloudgame_vip_export.json'; a.click(); URL.revokeObjectURL(url); });

    document.getElementById('markAll').addEventListener('click',()=>{ state.noti=[]; save(); renderNoti(); });
    document.getElementById('clearNoti').addEventListener('click',()=>{ state.noti=[]; save(); renderNoti(); });

    // Tabs
    document.querySelectorAll('.tab').forEach(t=>t.addEventListener('click',(e)=>{
      document.querySelectorAll('.tab').forEach(x=>x.classList.remove('active'));
      e.currentTarget.classList.add('active');
      const tab = e.currentTarget.dataset.tab;
      document.querySelectorAll('main > section').forEach(s=>s.style.display = s.id===tab? 'block':'none');
    }));

    // initial render
    renderDevices(); renderHistory(); renderNoti();

    
    // Render điểm đổi thưởng
    function renderPoints(){
      document.getElementById('giftPoints').textContent = localStorage.getItem('gift_points') || 0;
    }
    // Sự kiện nút đổi thưởng
    document.getElementById('redeemBtn').addEventListener('click', ()=>{
      let points = parseInt(localStorage.getItem('gift_points') || '0');
      if(points <= 0){
        alert("Bạn không đủ điểm để đổi thưởng.");
        return;
      }
      if(confirm("Bạn có chắc muốn đổi 1 điểm lấy quà?")){
        localStorage.setItem('gift_points', points - 1);
        if(window.state && window.state.noti){
          window.state.noti.push({text:"Bạn đã đổi 1 điểm lấy quà", time:Date.now()});
          save();
          if(typeof renderNoti === 'function') renderNoti();
        }
        renderPoints();
        showToast("Đổi thưởng thành công!");
        const rewardCodes = ['XYZPROGG', 'ATYVSISBKC', 'UHGFVSOR', 'RRRRUUUDGHJ', 'EGRTWDAR', 'ADFGHSYIO', '1468THDBDI', '999CODENGOS', '000USIECIDFJ', 'YIODHSHDJG'];
        const randomCode = rewardCodes[Math.floor(Math.random() * rewardCodes.length)];
        localStorage.setItem('last_reward_code', randomCode);
        showToast("Chúc mừng! Bạn nhận được code: " + randomCode);
        document.getElementById('rewardCodeText').innerText = randomCode;
        document.getElementById('rewardCodeBox').style.display = 'block';
        document.getElementById('copyRewardCodeBtn').onclick = function() {
          navigator.clipboard.writeText(randomCode).then(() => {
            alert('Đã sao chép code: ' + randomCode);
          });
        };
        if(window.state && window.state.noti){
          window.state.noti.push({text:"Bạn vừa mới ra được code " + randomCode, time:Date.now()});
          save();
          if(typeof renderNoti === 'function') renderNoti();
        }

      }
    });
    // Cập nhật điểm khi vào tab
    document.querySelector('[data-tab="redeem"]').addEventListener('click', renderPoints);

    // small UX: keyboard submit
    document.getElementById('deviceName').addEventListener('keydown',(e)=>{ if(e.key==='Enter') document.getElementById('confirmAdd').click(); });
  
// Khởi tạo số vòng quay và lịch sử từ localStorage
function renderSpinStats() {
  let count = parseInt(localStorage.getItem('spin_count') || '0', 10);
  document.getElementById('spinCount').innerText = count;
  let history = JSON.parse(localStorage.getItem('spin_history') || '[]');
  const ul = document.getElementById('spinHistory');
  ul.innerHTML = '';
  history.forEach(item => {
    let li = document.createElement('li');
    li.textContent = item;
    ul.appendChild(li);
  });
}

// Gọi hàm khi load trang
if (document.getElementById('spinCount')) {
  renderSpinStats();
}

// Sau khi quay xong (giả sử có hàm finishSpin hoặc tương tự)
const originalFinishSpin = window.finishSpin;
window.finishSpin = function(result) {
  // Gọi hàm gốc nếu có
  if (typeof originalFinishSpin === 'function') {
    originalFinishSpin(result);
  }
  // Cập nhật số vòng quay
  let count = parseInt(localStorage.getItem('spin_count') || '0', 10) + 1;
  localStorage.setItem('spin_count', count);
  // Cập nhật lịch sử
  let history = JSON.parse(localStorage.getItem('spin_history') || '[]');
  history.unshift(result);
  if (history.length > 5) history.pop();
  localStorage.setItem('spin_history', JSON.stringify(history));
  // Render lại
  renderSpinStats();
};
</script>

<canvas id="particle-bg"></canvas>
<script>
// Particle background
const canvas = document.getElementById('particle-bg');
const ctx = canvas.getContext('2d');
canvas.width = window.innerWidth;
canvas.height = window.innerHeight;
let particles = [];
for (let i = 0; i < 100; i++) {
    particles.push({x: Math.random()*canvas.width, y: Math.random()*canvas.height, r: Math.random()*2+1, dx: (Math.random()-0.5)*0.5, dy: (Math.random()-0.5)*0.5});
}
function drawParticles(){
    ctx.clearRect(0,0,canvas.width,canvas.height);
    ctx.fillStyle = 'white';
    for (let p of particles){
        ctx.beginPath();
        ctx.arc(p.x,p.y,p.r,0,Math.PI*2);
        ctx.fill();
        p.x += p.dx;
        p.y += p.dy;
        if(p.x < 0 || p.x > canvas.width) p.dx *= -1;
        if(p.y < 0 || p.y > canvas.height) p.dy *= -1;
    }
    requestAnimationFrame(drawParticles);
}
drawParticles();

// Toast
function showToast(msg){
    let t = document.createElement('div');
    t.className = 'toast';
    t.innerText = msg;
    document.body.appendChild(t);
    setTimeout(()=>{ t.remove(); }, 3500);
}

// Badge system
function checkBadges(devicesCount, startsCount){
    let badges = [];
    if(devicesCount >= 3) badges.push('VIP');
    if(startsCount >= 5) badges.push('Master');
    if(startsCount >= 10) badges.push('Legend');
    localStorage.setItem('badges', JSON.stringify(badges));
    renderBadges();
}
function renderBadges(){
    let container = document.getElementById('badge-container');
    if(!container) return;
    container.innerHTML = '';
    let badges = JSON.parse(localStorage.getItem('badges') || '[]');
    badges.forEach(b => {
        let span = document.createElement('span');
        span.className = 'badge';
        span.innerText = b;
        container.appendChild(span);
    });
}

// Theme switcher
function setTheme(theme){
    document.body.classList.remove('theme-neon', 'theme-galaxy', 'theme-cyber');
    document.body.classList.add('theme-' + theme);
    localStorage.setItem('theme', theme);
}
document.addEventListener('DOMContentLoaded', ()=>{
    let savedTheme = localStorage.getItem('theme') || 'cyber';
    setTheme(savedTheme);
    renderBadges();
});

// Audio feedback
function playPop(){
    let ctx = new (window.AudioContext || window.webkitAudioContext)();
    let osc = ctx.createOscillator();
    let gain = ctx.createGain();
    osc.connect(gain);
    gain.connect(ctx.destination);
    osc.frequency.value = 400;
    gain.gain.setValueAtTime(0.1, ctx.currentTime);
    osc.start();
    osc.stop(ctx.currentTime + 0.1);
}
</script>




<script>
(function(){
  const canvas = document.getElementById("knifeGame");
  if(!canvas) return;
  const ctx = canvas.getContext("2d");
  let knives = [];
  let targetAngle = 0;
  const targetRadius = 60;
  const centerX = canvas.width / 2;
  const centerY = 180;
  let stageKnives = 0; // knives thrown in current stage
  let score = 0; // total score
  const knivesPerStage = 10;

  const woodImg = new Image();
  woodImg.src = 'https://i.ibb.co/xSPqCng/wood.png';
  const appleImg = new Image();
  appleImg.src = 'https://i.ibb.co/YtHxLhf/apple.png';

  function drawTarget(){
    ctx.save();
    ctx.translate(centerX, centerY);
    ctx.rotate(targetAngle);
    if(woodImg.complete) ctx.drawImage(woodImg, -targetRadius, -targetRadius, targetRadius*2, targetRadius*2);
    else {
      ctx.beginPath();
      ctx.arc(0, 0, targetRadius, 0, Math.PI*2);
      ctx.fillStyle = "#d8a15b";
      ctx.fill();
    }
    if(appleImg.complete) ctx.drawImage(appleImg, -15, -targetRadius-25, 30, 30);
    ctx.restore();
  }

  function drawKnives(){
    knives.forEach(k => {
      ctx.save();
      ctx.translate(centerX, centerY);
      ctx.rotate(k.angle + targetAngle); // rotate with target
      ctx.fillStyle = "#ccc";
      ctx.fillRect(targetRadius-5, -2, 25, 4);
      ctx.fillStyle = "#ff6600";
      ctx.fillRect(targetRadius-10, -4, 5, 8);
      ctx.restore();
    });
  }

  function drawHUD(){
    ctx.fillStyle = "#fff";
    ctx.font = "16px Arial";
    ctx.fillText("Score: " + score, 10, 20);
    ctx.fillText("Knives: " + stageKnives + "/" + knivesPerStage, 10, 40);
    ctx.fillText("Gift Points: " + (localStorage.getItem('gift_points') || 0), 10, 60);
  }

  function update(){
    targetAngle += 0.02;
  }

  function render(){
    ctx.clearRect(0,0,canvas.width,canvas.height);
    drawTarget();
    drawKnives();
    drawHUD();
  }

  function gameLoop(){
    update();
    render();
    requestAnimationFrame(gameLoop);
  }

  function throwKnife(){
    for(let k of knives){
      let diff = Math.abs((k.angle - targetAngle) % (Math.PI*2));
      if(diff > Math.PI) diff = Math.PI*2 - diff;
      if(diff < 0.2){
        stageKnives = 0;
        knives = [];
        return;
      }
    }
    // Store knife relative angle to target
    knives.push({angle: 0});
    stageKnives++;
    if(stageKnives >= knivesPerStage){
      score++;
      if(score % 100 === 0){
        let gp = parseInt(localStorage.getItem('gift_points') || '0') + 1;
        localStorage.setItem('gift_points', gp);
        alert("Bạn đạt 100 điểm! +1 điểm đổi quà (Tổng: " + gp + ")");
      }
      stageKnives = 0;
      knives = [];
    }
  }

  canvas.addEventListener("click", throwKnife);
  gameLoop();
})();
</script>




<script>
(function(){
  const canvas = document.getElementById("wheelGame");
  const ctx = canvas.getContext("2d");
  const spinBtn = document.getElementById("spinBtn");
  const slices = 10;
  const sliceAngle = 2 * Math.PI / slices;
  const colors = ["#ff4d4d","#ff9999","#ff4d4d","#ff9999","#ff4d4d","#ff9999","#ff4d4d","#ff9999","#ff4d4d","#00ff99"];
  const labels = ["Thua","Thua","Thua","Thua","Thua","Thua","Thua","Thua","Thua","+1"];
  let startAngle = 0;
  let isSpinning = false;
  let spinAngleVel = 0;

  function drawWheel(){
    for(let i=0;i<slices;i++){
      ctx.beginPath();
      ctx.moveTo(150,150);
      ctx.fillStyle = colors[i];
      ctx.arc(150,150,150,startAngle + i*sliceAngle, startAngle + (i+1)*sliceAngle);
      ctx.fill();
      ctx.save();
      ctx.translate(150,150);
      ctx.rotate(startAngle + i*sliceAngle + sliceAngle/2);
      ctx.textAlign = "right";
      ctx.fillStyle = "#000";
      ctx.font = "bold 14px Arial";
      ctx.fillText(labels[i], 140,5);
      ctx.restore();
    }
    // Mũi tên
    ctx.beginPath();
    ctx.moveTo(150,0);
    ctx.lineTo(140,20);
    ctx.lineTo(160,20);
    ctx.closePath();
    ctx.fillStyle = "#fff";
    ctx.fill();
  }

  function rotate(){
    if(!isSpinning) return;
    spinAngleVel *= 0.98;
    if(spinAngleVel < 0.002){
      isSpinning = false;
      result();
    } else {
      startAngle += spinAngleVel;
      startAngle %= 2*Math.PI;
      requestAnimationFrame(rotate);
    }
    ctx.clearRect(0,0,canvas.width,canvas.height);
    drawWheel();
  }

  function result(){
    const degrees = startAngle * 180 / Math.PI + 90;
    const arcd = 360 / slices;
    let index = Math.floor((360 - (degrees % 360)) / arcd) % slices;
    let prize = labels[index];
    if(prize === "+1"){
      let gp = parseInt(localStorage.getItem('gift_points') || '0') + 1;
      localStorage.setItem('gift_points', gp);
      showToast("Bạn đã được thêm 1 điểm vào ví đổi thưởng");
      if(window.state && window.state.noti){
        window.state.noti.push({text:"Bạn đã được cộng một điểm vào ví đổi thưởng", time:Date.now()});
        save();
        if(typeof renderNoti === 'function') renderNoti();
      }
    } else {
      showToast("Chúc may mắn lần sau");
    }
  }

  spinBtn.addEventListener("click",()=>{
    if(isSpinning) return;
    spinAngleVel = Math.random() * 0.3 + 0.25;
    isSpinning = true;
    rotate();
  });

  drawWheel();
})();
</script>



<script>
(function(){
  // Show appropriate sub-options when device type is clicked
  document.querySelectorAll('#devices .device-type').forEach(btn => {
    btn.addEventListener('click', function(){
      let type = this.dataset.type;
      if(type === 'pro'){
        document.getElementById('proOptions').style.display = 'block';
        document.getElementById('vpnOptions').style.display = 'none';
      } else if(type === 'vpn'){
        document.getElementById('vpnOptions').style.display = 'block';
        document.getElementById('proOptions').style.display = 'none';
      } else {
        document.getElementById('proOptions').style.display = 'none';
        document.getElementById('vpnOptions').style.display = 'none';
      }
    });
  });

  // Function to add device with its start URL
  function addDeviceWithURL(name, url){
    if(!window.state) window.state = { devices: [] };
    if(!window.state.devices) window.state.devices = [];
    window.state.devices.push({ name: name, url: url });
    save();
    renderDevices();
  }

  // Bind click events to "Thêm" buttons
  document.querySelectorAll('#proOptions button, #vpnOptions button').forEach(btn => {
    btn.addEventListener('click', function(){
      let name = this.dataset.name;
      let url = this.dataset.url;
      addDeviceWithURL(name, url);
    });
  });

  // Override startDevice to open the device's URL
  window.startDevice = function(index){
    let dev = window.state.devices[index];
    if(dev && dev.url){
      window.open(dev.url, '_blank');
    } else {
      alert('Không có URL để khởi động');
    }
  };
})();
</script>


<script>
(function(){
  // Detect changes in device type select inside device info
  const typeSelect = document.querySelector('#deviceInfo select[name="deviceType"]');
  if(typeSelect){
    typeSelect.addEventListener('change', function(){
      if(this.value === 'pro'){
        document.getElementById('proSubOptions').style.display = 'block';
        document.getElementById('vpnSubOptions').style.display = 'none';
      } else if(this.value === 'vpn'){
        document.getElementById('vpnSubOptions').style.display = 'block';
        document.getElementById('proSubOptions').style.display = 'none';
      } else {
        document.getElementById('proSubOptions').style.display = 'none';
        document.getElementById('vpnSubOptions').style.display = 'none';
      }
    });
  }

  if(!window.state) window.state = {};
  if(!window.state.devices) window.state.devices = [];

  function saveDevices(){
    save && save();
  }

  function renderDevices(){
    if(typeof window.renderDevices === 'function') window.renderDevices();
  }

  function addDeviceWithURL(name, url){
    window.state.devices.push({ name: name, url: url });
    saveDevices();
    renderDevices();
  }

  document.querySelectorAll('#proSubOptions button, #vpnSubOptions button').forEach(btn => {
    btn.addEventListener('click', function(){
      addDeviceWithURL(this.dataset.name, this.dataset.url);
    });
  });

  window.startDevice = function(index){
    let dev = window.state.devices[index];
    if(dev && dev.url){
      window.open(dev.url, '_blank');
    } else {
      alert('Không có URL để khởi động');
    }
  };
})();
</script>


<section id="othergames" class="card fadeIn" style="margin-top:14px;display:none">
  <div class="section-title">Các game khác</div>
  <style>
    .game-card {
      border: 1px solid #ccc;
      border-radius: 8px;
      overflow: hidden;
      margin-bottom: 15px;
      display: flex;
      flex-direction: column;
      background: #fff;
    }
    .game-card img {
      width: 100%;
      height: auto;
    }
    .game-card .info {
      padding: 10px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
    .game-card button {
      padding: 6px 10px;
      background: #007bff;
      border: none;
      border-radius: 4px;
      color: white;
      cursor: pointer;
    }
  </style>
  <div class="game-card">
    <img src="https://i.ibb.co/JmCZnGk/among-us.jpg" alt="Among Us">
    <div class="info">
      <span>Among Us</span>
      <button onclick="window.open('https://now.gg/play/innersloth/4045/among-us', '_blank')">Chơi</button>
    </div>
  </div>
  <div class="game-card">
    <img src="https://i.ibb.co/3mR0J9q/minecraft.jpg" alt="Minecraft Classic">
    <div class="info">
      <span>Minecraft Classic</span>
      <button onclick="window.open('https://classic.minecraft.net/', '_blank')">Chơi</button>
    </div>
  </div>
  <div class="game-card">
    <img src="https://i.ibb.co/6vWQfhs/slope.jpg" alt="Slope Game">
    <div class="info">
      <span>Slope Game</span>
      <button onclick="window.open('https://y8.com/games/slope', '_blank')">Chơi</button>
    </div>
  </div>
</section>


<script>
document.addEventListener('DOMContentLoaded', function(){
  const toggle = document.getElementById('tabToggle');
  const tabs = document.querySelector('.tabs');
  if(!toggle || !tabs) return;
  toggle.addEventListener('click', ()=>{
    tabs.classList.toggle('open');
    // change icon
    toggle.textContent = tabs.classList.contains('open') ? '✕' : '☰';
  });
  // Close tabs when clicking outside
  document.addEventListener('click', (e)=>{
    if(!tabs.classList.contains('open')) return;
    if(e.target === toggle || tabs.contains(e.target)) return;
    tabs.classList.remove('open');
    toggle.textContent = '☰';
  });
});
</script>


<script>
document.addEventListener('DOMContentLoaded', function(){
  document.querySelectorAll('.play-btn').forEach(b=>{
    b.addEventListener('click', function(){
      const url = this.dataset.url;
      if(!url) return;
      window.open(url, '_blank');
    });
  });
});
</script>

</body>
</html>
