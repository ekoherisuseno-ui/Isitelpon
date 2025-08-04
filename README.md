<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Isi Telpon - Bisnis Lancar</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      padding: 20px;
      background-color: #f4f4f4;
    }
    h1 {
      text-align: center;
      color: #333;
    }
    .produk {
      background: #fff;
      padding: 15px;
      margin: 10px auto;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      max-width: 400px;
    }
    .produk h3 {
      margin: 0;
      color: #007bff;
    }
    .produk button {
      margin-top: 10px;
      padding: 10px;
      background: #25D366;
      color: white;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      width: 100%;
    }
    .produk button:hover {
      background: #1ebe5b;
    }
  </style>
</head>
<body>
  <h1>Isi Telpon - Bisnis Lancar</h1>

  <div class="produk">
    <h3>Pulsa 5.000</h3>
    <button onclick="pesan('Pulsa 5000')">Pesan via WhatsApp</button>
  </div>
  <div class="produk">
    <h3>Pulsa 10.000</h3>
    <button onclick="pesan('Pulsa 10000')">Pesan via WhatsApp</button>
  </div>
  <div class="produk">
    <h3>Pulsa 20.000</h3>
    <button onclick="pesan('Pulsa 20000')">Pesan via WhatsApp</button>
  </div>
  <div class="produk">
    <h3>Paket Data 1 GB</h3>
    <button onclick="pesan('Paket Data 1GB')">Pesan via WhatsApp</button>
  </div>
  <div class="produk">
    <h3>Token PLN 20.000</h3>
    <button onclick="pesan('Token PLN 20000')">Pesan via WhatsApp</button>
  </div>

  <script>
    function pesan(produk) {
      const nohp = '6283876555567';
      const pesan = encodeURIComponent('Halo, saya ingin pesan: ' + produk);
      window.open('https://wa.me/' + nohp + '?text=' + pesan, '_blank');
    }
  </script>
</body>
</html>
