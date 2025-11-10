<!doctype html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>67 GROUP — Cyber | Coffee | Billiards | Beer & VVIP</title>
  <meta name="description" content="67 Group: Cyber Game, Coffee & Tea, Billiards, Beer & VVIP — không gian giải trí đẳng cấp.">
  <style>
    :root{
      --bg:#000;
      --card:#0b0b0b;
      --muted:#b5b5b5;
      --accent:#f5b000;
      --glass: rgba(255,255,255,0.05);
      --radius:12px;
      font-family: Inter, system-ui, -apple-system, sans-serif;
    }
    *{box-sizing:border-box;}
    body{
      margin:0;
      background:var(--bg);
      color:#f2f2f2;
      line-height:1.5;
    }
    a{color:var(--accent);text-decoration:none;}
    header{
      position:sticky;top:0;z-index:10;
      background:#000000ee;backdrop-filter:blur(6px);
      border-bottom:1px solid #222;
    }
    .nav{display:flex;justify-content:space-between;align-items:center;max-width:1100px;margin:auto;padding:14px;}
    .brand{display:flex;align-items:center;gap:10px;font-weight:700;}
    .logo{width:40px;height:40px;border-radius:10px;display:grid;place-items:center;
      background:linear-gradient(135deg,var(--accent),#ffce40);color:#000;font-weight:800;}
    nav ul{display:flex;gap:14px;list-style:none;margin:0;padding:0;}
    nav li{font-weight:600;font-size:14px;}
    .cta{background:var(--accent);color:#000;padding:8px 14px;border-radius:8px;}

    .wrap{max-width:1100px;margin:auto;padding:24px;}

    h1,h2,h3{color:#fff;margin-top:0;}
    .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(260px,1fr));gap:18px;}
    .card{background:var(--card);padding:18px;border-radius:var(--radius);border:1px solid #222;}
    .meta{color:var(--muted);font-size:14px;}
    .btn{padding:10px 14px;border-radius:8px;background:var(--glass);border:none;color:#fff;cursor:pointer;}
    .btn-primary{background:var(--accent);color:#000;font-weight:700;}
    input,select,textarea{width:100%;padding:10px;border-radius:8px;border:1px solid #333;background:#111;color:#fff;}

    footer{text-align:center;padding:24px;color:#777;border-top:1px solid #111;margin-top:40px;}
  </style>
</head>
<body>
<header>
  <div class="nav">
    <div class="brand"><div class="logo">67</div> 67 GROUP</div>
    <nav>
      <ul>
        <li><a href="#services">Dịch vụ</a></li>
        <li><a href="#booking">Đặt chỗ</a></li>
        <li><a href="#contact" class="cta">Liên hệ</a></li>
      </ul>
    </nav>
  </div>
</header>

<main class="wrap">
  <section id="intro">
    <h1>67 GROUP — KHÔNG GIAN GIẢI TRÍ ĐẲNG CẤP</h1>
    <p class="meta">Chuỗi: 67 CYBER GAME • 67 COFFEE AND TEA • 67 BILLIARDS • 67 BEER & VVIP</p>
  </section>

  <section id="services">
    <h2>Dịch vụ của chúng tôi</h2>
    <div class="grid">
      <div class="card"><h3>67 Cyber Game</h3><p class="meta">Phòng máy cấu hình cao, không gian eSports chuyên nghiệp.</p></div>
      <div class="card"><h3>67 Coffee & Tea</h3><p class="meta">Không gian chill, đồ uống đa dạng, đêm nhạc acoustic.</p></div>
      <div class="card"><h3>67 Billiards</h3><p class="meta">Giải trí cùng bạn bè, bàn đạt chuẩn, phục vụ tận tâm.</p></div>
      <div class="card"><h3>67 Beer & VVIP</h3><p class="meta">Không gian Beer, VVIP sang trọng cho tiệc & sinh nhật.</p></div>
    </div>
  </section>

  <section id="booking" style="margin-top:40px;">
    <h2>Đặt chỗ trực tuyến</h2>
    <p class="meta">Điền thông tin bên dưới để đặt chỗ. Form sẽ gửi đến hệ thống Google Form (hoặc có thể thay bằng đường dẫn khác sau).</p>
    
    <!-- THAY action="" BẰNG LINK GOOGLE FORM CỦA BẠN -->
    <form action="https://docs.google.com/forms/d/e/FORM_ID/formResponse" method="POST" target="_blank" style="margin-top:16px;display:grid;gap:12px;">
      <input required name="entry.111111" placeholder="Họ và tên">
      <input required name="entry.222222" placeholder="Số điện thoại">
      <select required name="entry.333333">
        <option value="">Chọn dịch vụ</option>
        <option>67 Coffee & Tea</option>
        <option>67 Cyber Game</option>
        <option>67 Billiards</option>
        <option>67 Beer & VVIP</option>
      </select>
      <input required name="entry.444444" placeholder="Số người (ví dụ: 5)">
      <input name="entry.555555" type="datetime-local">
      <textarea name="entry.666666" rows="3" placeholder="Ghi chú thêm (ví dụ: sinh nhật, combo...)"></textarea>
      <button class="btn-primary btn" type="submit">Gửi đặt chỗ</button>
    </form>

    <p class="meta" style="margin-top:12px;">Sau khi gửi, bạn sẽ thấy trang xác nhận của Google Form. Nhân viên 67 Group sẽ liên hệ xác nhận lại trong thời gian sớm nhất.</p>
  </section>

  <section id="contact" style="margin-top:40px;">
    <h2>Liên hệ nhanh</h2>
    <p>Email: <a href="mailto:67cybergame@gmail.com">67cybergame@gmail.com</a> — Hotline: +84 67-XXX-XXXX</p>
  </section>
</main>

<footer>
  <p>© <span id="year"></span> 67 GROUP.NGUYEN THI MY YEN.</p>
</footer>

<script>
  document.getElementById("year").textContent = new Date().getFullYear();
</script>
</body>
</html>
