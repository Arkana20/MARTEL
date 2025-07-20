<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="Martabak Telor Lumpia Lezat di MARTEL. Pesan Sekarang Lewat Website!">
  <title>MARTEL - Martabak Telor Lumpia</title>
  <link href="https://fonts.googleapis.com/css2?family=Baloo+2&display=swap" rel="stylesheet">
  <style>
    body {
      margin: 0;
      font-family: 'Baloo 2', cursive;
      background-color: #ff7f00;
      color: #fff;
    }
    header {
      background-color: #e66000;
      padding: 1rem 2rem;
      text-align: center;
    }
    header h1 {
      font-size: 2.8rem;
      margin: 0;
    }
    .hero {
      text-align: center;
      padding: 2rem;
    }
    .hero img {
      max-width: 90%;
      border-radius: 16px;
      box-shadow: 0 4px 12px rgba(0,0,0,0.3);
    }
    .hero p {
      font-size: 1.4rem;
      margin-top: 1rem;
    }
    .menu {
      padding: 2rem;
      background-color: #ff5c00;
    }
    .menu h2 {
      text-align: center;
      margin-bottom: 1rem;
    }
    .menu-item {
      background-color: #b30000;
      margin: 0.5rem auto;
      padding: 1rem;
      max-width: 400px;
      border-radius: 12px;
      text-align: center;
      color: #fff;
      box-shadow: 0 4px 8px rgba(0,0,0,0.2);
    }
    .order-section {
      padding: 2rem;
      background-color: #ff6a00;
    }
    .order-section form {
      max-width: 400px;
      margin: auto;
    }
    .order-section input, .order-section select {
      width: 100%;
      padding: 0.7rem;
      margin-bottom: 1rem;
      border: none;
      border-radius: 6px;
      font-size: 1rem;
    }
    .order-section button {
      width: 100%;
      padding: 0.8rem;
      font-size: 1.1rem;
      background-color: #fff;
      color: #ff5c00;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      transition: background 0.3s;
    }
    .order-section button:hover {
      background-color: #ffddc1;
    }
    .testimonials {
      padding: 2rem;
      background-color: #ff8c1a;
      color: #fff;
    }
    .testimonial {
      background-color: rgba(0,0,0,0.2);
      margin: 1rem auto;
      padding: 1rem;
      border-radius: 10px;
      max-width: 500px;
      font-style: italic;
    }
    footer {
      text-align: center;
      background-color: #cc5200;
      padding: 1rem;
      font-size: 0.9rem;
    }
  </style>
</head>
<body>
  <header>
    <h1>MARTEL</h1>
    <p>Martabak Telor Lumpia Lezat & Terjangkau</p>
  </header>

  <section class="hero">
    <img src="https://img-global.cpcdn.com/recipes/614d51595e25ff0d/680x482cq90/martabak-telur-daging-sapi-kulit-lumpia-mudah-foto-resep-utama.jpg" alt="Martabak Telor Lumpia">
    <p>Cita rasa nikmat yang dibungkus renyahnya kulit lumpia. MARTEL, pilihan tepat buat kamu!</p>
  </section>

  <section class="menu">
    <h2>Menu Martel</h2>
    <div class="menu-item">Martel Biasa - 5k</div>
    <div class="menu-item">Martel Baso - 7k</div>
    <div class="menu-item">Martel Sosis - 8k</div>
    <div class="menu-item">Martel Spesial - 10k</div>
  </section>

  <section class="order-section">
    <h2>Pesan Sekarang</h2>
    <form id="orderForm">
      <input type="text" id="name" placeholder="Nama Anda" required>
      <input type="text" id="whatsapp" placeholder="Nomor WhatsApp" required>
      <select id="menu">
        <option value="Martel Biasa - 5k">Martel Biasa - 5k</option>
        <option value="Martel Baso - 7k">Martel Baso - 7k</option>
        <option value="Martel Sosis - 8k">Martel Sosis - 8k</option>
        <option value="Martel Spesial - 10k">Martel Spesial - 10k</option>
      </select>
      <input type="number" id="jumlah" placeholder="Jumlah Pesanan" required>
      <button type="submit">Pesan Sekarang</button>
    </form>
  </section>

  <section class="testimonials">
    <h2>Kata Mereka</h2>
    <div class="testimonial">"Martel ini bikin nagih! Kulitnya renyah, isinya mantap."</div>
    <div class="testimonial">"Pertama kali nyoba, langsung jatuh cinta sama rasa dan harga!"</div>
    <div class="testimonial">"Pas banget buat camilan sore atau teman nonton bola."</div>
  </section>

  <footer>
    &copy; 2025 MARTEL | Hubungi via WhatsApp: <a style="color: #fff; text-decoration: underline;" href="https://wa.me/6281311239882">0813-1123-9882</a>
  </footer>

  <script>
    document.getElementById('orderForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const name = document.getElementById('name').value;
      const wa = document.getElementById('whatsapp').value;
      const menu = document.getElementById('menu').value;
      const jumlah = document.getElementById('jumlah').value;

      const pesan = `Halo, saya ${name}. Saya mau pesan:\nMenu: ${menu}\nJumlah: ${jumlah}\nNo. WA: ${wa}`;
      const encoded = encodeURIComponent(pesan);
      window.open(`https://wa.me/6281311239882?text=${encoded}`);
    });
  </script>
</body>
</html>
