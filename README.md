# nokshi-pitha<!DOCTYPE html>
<html lang="bn">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <title>NOKSHI PITHA</title>
  <style>
    body { margin:0; font-family:'SolaimanLipi', sans-serif; background:#fff8f0; color:#333; }
    header { background:#a0522d; color:#fff; padding:30px; text-align:center; }
    nav { background:#deb887; text-align:center; padding:10px; }
    nav a { margin:0 15px; text-decoration:none; color:#4b2e1e; font-weight:bold; }
    section { padding:30px; }
    .gallery { display:grid; grid-template-columns:repeat(auto-fit, minmax(200px,1fr)); gap:15px; }
    .gallery img { width:100%; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.2); }
    .order-form { max-width:500px; margin:auto; background:#fff; padding:20px; border-radius:8px; box-shadow:0 2px 8px rgba(0,0,0,0.1); }
    .order-form input, .order-form textarea, .order-form button {
      width:100%; padding:10px; margin:8px 0; border:1px solid #ccc; border-radius:4px;
    }
    .order-form button { background:#a0522d; color:#fff; border:none; cursor:pointer; }
    .qr-code { text-align:center; margin-top:20px; }
    footer { background:#a0522d; color:#fff; text-align:center; padding:15px; }
  </style>
</head>
<body>

  <header>
    <h1>NOKSHI PITHA</h1>
    <p>স্বাদের ছোঁয়ায় ঐতিহ্য</p>
  </header>
  
  <nav>
    <a href="#home">হোম</a>
    <a href="#about">আমাদের সম্পর্কে</a>
    <a href="#products">পণ্য</a>
    <a href="#order">অর্ডার</a>
    <a href="#contact">যোগাযোগ</a>
  </nav>

  <section id="about">
    <h2>আমাদের সম্পর্কে</h2>
    <p>NOKSHI PITHA একটি ঘরোয়া পিঠার ব্যবসা, যেখানে হাতে তৈরি নকশি পিঠা পরিবেশন করা হয়। আমাদের প্রতিটি পিঠা আপনাকে নিয়ে যাবে গ্রামের সুস্বাদ ও ঐতিহ্যে।</p>
  </section>

  <section id="products">
    <h2>গ্যালারি</h2>
    <div class="gallery">
      <img src="https://via.placeholder.com/400x300?text=নকশি+পিঠা+1" alt="নকশি পিঠা 1">
      <img src="https://via.placeholder.com/400x300?text=নকশি+পিঠা+2" alt="নকশি পিঠা 2">
      <img src="https://via.placeholder.com/400x300?text=নকশি+পিঠা+3" alt="নকশি পিঠা 3">
      <img src="https://via.placeholder.com/400x300?text=নকশি+পিঠা+4" alt="নকশি পিঠা 4">
    </div>
  </section>

  <section id="order">
    <h2>অর্ডার ফর্ম</h2>
    <form class="order-form" onsubmit="alert('আপনার অর্ডার গ্রহণ হয়েছে!'); return false;">
      <label>নাম:</label>
      <input type="text" required>
      <label>ফোন নম্বার:</label>
      <input type="tel" value="+88019" required>
      <label>ঠিকানা:</label>
      <textarea rows="3" required></textarea>
      <label>পছন্দের পণ্য ও পরিমাণ:</label>
      <textarea rows="3" placeholder="উদাঃ ২০ টুকরো নকশি পিঠা" required></textarea>
      <button type="submit">অর্ডার জমা দিন</button>
    </form>
  </section>

  <section id="contact">
    <h2>যোগাযোগ</h2>
    <p><strong>ফোন:</strong> <a href="tel:+8801902892608">+880 19 0289 2608</a></p>
    <p><strong>ঠিকানা:</strong> Narsingdi Sadar, Dhaka, Bangladesh</p>
    <div class="qr-code">
      <h3>QR কোড স্ক্যান করে ওয়েবসাইট দেখুন:</h3>
      <canvas id="qrcode"></canvas>
    </div>
  </section>

  <footer>
    <p>© ২০২৫ NOKSHI PITHA | সর্বস্বত্ব সংরক্ষিত</p>
  </footer>

  <script src="https://cdnjs.cloudflare.com/ajax/libs/qrious/4.0.2/qrious.min.js"></script>
  <script>
    new QRious({ element: document.getElementById('qrcode'),
      value: location.href, size: 150 });
  </script>

</body>
</html>
