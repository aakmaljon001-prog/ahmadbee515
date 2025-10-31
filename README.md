<!doctype html>
<html lang="uz">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>SITELABS — Biz haqimizda</title>

  <!-- Google font (agar internet mavjud bo'lsa) -->
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;800&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#1f1f1f;
      --panel:#222;
      --muted:#bdbdbd;
      --accent:#fff;
      --container:1100px;
    }
    *{box-sizing:border-box}
    html{scroll-behavior:smooth}
    body{
      margin:0;
      font-family: "Inter", system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg,#3b3b3b 0%, #565656 100%);
      color:var(--accent);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }

    /* NAVBAR */
    .nav{
      position:fixed;
      top:0;
      left:0;
      right:0;
      height:68px;
      background: rgba(12,12,12,0.95);
      display:flex;
      align-items:center;
      box-shadow: 0 4px 8px rgba(0,0,0,0.5);
      z-index:100;
      padding:0 24px;
    }
    .nav .brand{
      font-weight:800;
      letter-spacing:2px;
      margin-right:40px;
      font-size:18px;
    }
    .nav .menu{
      display:flex;
      gap:28px;
      margin-left:auto;
    }
    .nav a{
      color:var(--muted);
      text-decoration:none;
      font-size:13px;
      font-weight:600;
      letter-spacing:1px;
    }
    .nav a:hover{color:var(--accent)}

    /* LAYOUT */
    .wrap{
      max-width:var(--container);
      margin:120px auto 80px;
      padding:0 24px;
    }

    .hero{
      display:flex;
      gap:40px;
      align-items:flex-start;
      min-height:340px;
    }
    .hero .left{
      flex:1;
      max-width:760px;
    }
    .kicker{color:var(--muted); font-weight:700; letter-spacing:2px; margin-bottom:12px}
    h1{
      font-size:48px;
      margin:0 0 18px 0;
      line-height:1.02;
    }
    p.lead{color:var(--muted); margin:0 0 28px 0; font-size:18px;}

    /* two-column info */
    .grid{
      display:grid;
      grid-template-columns: repeat(2, 1fr);
      gap:28px;
      margin-top:36px;
    }
    .card{
      background: rgba(0,0,0,0.15);
      padding:22px;
      border-radius:8px;
      min-height:120px;
    }
    .card h3{margin:0 0 12px 0; font-size:22px}
    .card p{margin:0; color:var(--muted)}
    .team-row{display:flex; gap:12px; align-items:center}
    .avatar{
      width:56px; height:56px; border-radius:50%;
      background:linear-gradient(180deg,#ddd,#aaa);
      display:inline-block;
      flex:0 0 56px;
      overflow:hidden;
      box-shadow:0 2px 6px rgba(0,0,0,0.4);
    }
    .avatar img{width:100%;height:100%;object-fit:cover;display:block;filter:grayscale(1);}

    /* Services */
    .services{
      margin-top:46px;
      display:grid;
      grid-template-columns:repeat(3,1fr);
      gap:18px;
    }
    .svc{
      background: rgba(0,0,0,0.12);
      padding:18px;
      border-radius:8px;
      min-height:120px;
    }
    .svc h4{margin:0 0 8px 0}
    .svc p{margin:0;color:var(--muted);font-size:14px}

    /* Career / Contact */
    .two-col{
      display:grid;
      grid-template-columns:1fr 1fr;
      gap:28px;
      margin-top:36px;
    }

    /* Contact form */
    form input, form textarea{
      width:100%;
      padding:10px 12px;
      border-radius:6px;
      border:1px solid rgba(255,255,255,0.06);
      background:rgba(255,255,255,0.03);
      color:var(--accent);
      margin-bottom:10px;
      font-size:14px;
    }
    button.btn{
      background:#fff;color:#000;padding:10px 16px;border-radius:8px;border:0;font-weight:700;cursor:pointer;
    }

    footer{
      margin:60px auto 30px;
      text-align:center;color:var(--muted);font-size:14px;
    }

    /* Responsive */
    @media (max-width:900px){
      h1{font-size:40px}
      .services{grid-template-columns:repeat(2,1fr)}
      .grid{grid-template-columns:1fr}
      .two-col{grid-template-columns:1fr}
      .nav .menu{gap:16px}
      .wrap{margin-top:100px}
    }
    @media (max-width:520px){
      h1{font-size:30px}
      .services{grid-template-columns:1fr}
      .nav{padding:0 12px}
      .nav .brand{font-size:16px}
    }
  </style>
</head>
<body>

  <nav class="nav">
    <div class="brand">SITELABS</div>
    <div class="menu">
      <a href="#home">Asosiy</a>
      <a href="#about">Biz haqimizda</a>
      <a href="#services">Xizmatlar</a>
      <a href="#career">Karyera</a>
      <a href="#contact">Aloqa</a>
      <a href="#blog">Blog</a>
    </div>
  </nav>

  <main class="wrap">
    <!-- HERO / HOME -->
    <section id="home" class="hero" aria-label="home">
      <div class="left">
        <div class="kicker">SITELABS</div>
        <h1>IT kompaniyasi bilan raqamli dunyo sari</h1>
        <p class="lead">Sitelabs IT kompaniyasi sizlarga faqat eng yaxshisini taqdim etish uchun jamoamiz chin dildan harakat qiladi.</p>

        <div style="display:flex; gap:12px; margin-top:8px;">
          <a href="#services" class="btn" style="text-decoration:none;"><button class="btn">Bizning xizmatlar</button></a>
          <a href="#contact" style="text-decoration:none;"><button class="btn" style="background:transparent;color:#fff;border:1px solid rgba(255,255,255,0.12)">Aloqa</button></a>
        </div>
      </div>

      <!-- optional right side (empty to mimic screenshot) -->
      <div style="flex:0 0 200px;"></div>
    </section>

    <!-- ABOUT -->
    <section id="about" style="margin-top:16px;">
      <div class="grid">
        <div class="card">
          <h3>Kompaniya tarixi</h3>
          <p>SITELABS 2020-yildan beri IT xizmatlarini taqdim etadi. Biz kichik jamoa sifatida boshladik va hozir katta professional guruhmiz.</p>
        </div>

        <div class="card">
          <h3>Jamoa haqida</h3>
          <div class="team-row" style="margin-top:8px;">
            <div class="avatar"><img src="https://via.placeholder.com/150" alt="team"></div>
            <div class="avatar"><img src="https://via.placeholder.com/150" alt="team"></div>
            <div class="avatar"><img src="https://via.placeholder.com/150" alt="team"></div>
          </div>
          <p style="margin-top:10px;color:var(--muted)">Jamoamizda 15+ mutaxassislar — ishlab chiquvchilar, dizaynerlar va PMlar.</p>
        </div>

        <div class="card">
          <h3>Maqsad va missiya</h3>
          <p>Xizmatlarimizning asosiy maqsadi mijozlarga raqamli rivojlanishda yordam berishdir.</p>
        </div>

        <div class="card">
          <h3>Afzalliklar</h3>
          <ul style="margin:0;padding-left:18px;color:var(--muted)">
            <li>Tezkor yetkazish</li>
            <li>Kafolat</li>
            <li>Tajriba</li>
            <li>Moslashuvchanlik</li>
          </ul>
        </div>
      </div>
    </section>

    <!-- SERVICES -->
    <section id="services" style="margin-top:26px;">
      <h2 style="margin:0 0 14px 0;font-size:26px">Xizmatlar</h2>
      <div class="services">
        <div class="svc">
          <h4>Web sayt yaratish</h4>
          <p>Landing page, korporativ saytlar va e-commerce yechimlari.</p>
        </div>
        <div class="svc">
          <h4>Mobil ilovalar</h4>
          <p>Android va iOS uchun ilovalar — natijaga yo‘naltirilgan.</p>
        </div>
        <div class="svc">
          <h4>UX/UI dizayn</h4>
          <p>Foydalanuvchi tajribasi dizayni va prototiplash.</p>
        </div>
      </div>
    </section>

    <!-- Career + Contact -->
    <section style="margin-top:32px;">
      <div class="two-col">
        <div>
          <h3 id="career" style="margin-top:0">Karyera</h3>
          <p style="color:var(--muted)">Agar jamoamizga qo‘shilmoqchi bo‘lsangiz, hozirgi ochiq pozitsiyalar:</p>
          <ul style="color:var(--muted)">
            <li>Frontend developer</li>
            <li>Backend developer</li>
            <li>Product designer</li>
          </ul>
          <p style="margin-top:8px;color:var(--muted)">Rezyume yuborish: hr@sitelabs.example</p>
        </div>

        <div>
          <h3 id="contact" style="margin-top:0">Aloqa</h3>
          <p style="color:var(--muted)">Biz bilan bog‘laning — tez va aniq javob olasiz.</p>

          <form onsubmit="event.preventDefault(); alert('Rahmat! Xabaringiz qabul qilindi (demo).');">
            <input type="text" name="name" placeholder="Ism va familiya" required>
            <input type="tel" name="phone" placeholder="Telefon raqam" required>
            <input type="email" name="email" placeholder="Email (ixtiyoriy)">
            <textarea name="message" rows="4" placeholder="Xabaringiz..." required></textarea>
            <button class="btn" type="submit">Yuborish</button>
          </form>

          <div style="margin-top:14px;color:var(--muted);font-size:14px;">
            <div>Telefon: +998 90 123 45 67</div>
            <div>Manzil: Toshkent, O'zbekiston</div>
          </div>
        </div>
      </div>
    </section>

    <!-- BLOG -->
    <section id="blog" style="margin-top:36px;">
      <h3 style="margin-bottom:10px">Blog</h3>
      <p style="color:var(--muted);margin:0 0 12px 0">So‘nggi maqolalar va case-studylarimizni shu yerda chop etamiz.</p>
      <div class="grid" style="margin-top:10px;">
        <div class="card"><h4>Case: E-commerce sayti</h4><p style="color:var(--muted)">Savdo hajmini 2 barobar oshirdik.</p></div>
        <div class="card"><h4>UX optimizatsiya</h4><p style="color:var(--muted)">Conversion rate 18% ga oshdi.</p></div>
      </div>
    </section>

    <footer>
      © <span id="year"></span> SITELABS — Barcha huquqlar himoyalangan.
    </footer>
  </main>

<script>
  // small helpers
  document.getElementById('year').textContent = new Date().getFullYear();
</script>

</body>
</html>
