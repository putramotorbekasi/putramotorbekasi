<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Putra Motor Bekasi</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #ffffff; }
        header { background: #d32f2f; color: white; text-align: center; padding: 20px; font-size: 28px; font-weight: bold; }
        nav { display: flex; justify-content: center; background: #ff9800; padding: 15px; }
        nav a { color: white; text-decoration: none; margin: 0 20px; font-weight: bold; font-size: 18px; }
        .banner { text-align: center; padding: 60px 20px; background: url('https://source.unsplash.com/1200x400/?motorcycle,workshop') no-repeat center center/cover; color: white; font-size: 30px; font-weight: bold; }
        .container { max-width: 1000px; margin: auto; padding: 20px; text-align: center; }
        .highlight { color: #ff9800; font-weight: bold; }
        .services, .contact-info { display: flex; flex-wrap: wrap; justify-content: center; }
        .service-box, .contact-box { background: #fff3e0; padding: 20px; margin: 10px; border-radius: 10px; box-shadow: 0 0 10px rgba(0,0,0,0.1); width: 45%; color: #d32f2f; font-weight: bold; transition: transform 0.3s; font-size: 18px; }
        .service-box:hover, .contact-box:hover { transform: scale(1.05); }
        .contact { margin-top: 30px; padding: 25px; background: #d32f2f; color: white; border-radius: 10px; }
        .contact a { color: #ffcc80; text-decoration: none; font-weight: bold; }
        button { background: #ff9800; color: white; border: none; padding: 12px 25px; cursor: pointer; font-size: 20px; border-radius: 5px; transition: background 0.3s; }
        button:hover { background: #e65100; }
        .booking-form { margin-top: 30px; text-align: left; }
        .booking-form label { font-weight: bold; display: block; margin-top: 12px; font-size: 18px; }
        .booking-form input, .booking-form select { width: 100%; padding: 10px; margin-top: 8px; border-radius: 5px; border: 1px solid #ccc; font-size: 16px; }
    </style>
    <script>
        function sendBooking() {
            let name = document.getElementById('name').value;
            let date = document.getElementById('date').value;
            let time = document.getElementById('time').value;
            let bikeType = document.getElementById('bikeType').value;
            let bikeModel = document.getElementById('bikeModel').value;
            let year = document.getElementById('year').value;
            let serviceType = document.getElementById('serviceType').value;
            let oilType = document.getElementById('oilType').value;
            let message = `Booking Service:%0AName: ${name}%0A
                          Tanggal: ${date}%0A
                          Jam: ${time}%0A
                          Jenis Motor: ${bikeType}%0A
                          Nama Motor: ${bikeModel} (${year})%0A
                          Layanan: ${serviceType}%0A
                          Oli: ${oilType}`;
            let url = `https://wa.me/6287789168900?text=${message}`;
            window.open(url, '_blank');
        }
    </script>
</head>
<body>
    <header>PUTRA MOTOR BEKASI</header>
    <nav>
        <a href="#services">Layanan</a>
        <a href="#booking">Booking</a>
        <a href="#contact">Hubungi Kami</a>
    </nav>
    <div class="banner">Bengkel Motor Terbaik di Tambun Selatan - Bekasi</div>
    <div class="container">
        <h2>Booking Service</h2>
        <div class="booking-form">
            <label>Nama:</label>
            <input type="text" id="name">
            <label>Tanggal:</label>
            <input type="date" id="date">
            <label>Jam:</label>
            <input type="time" id="time">
            <label>Jenis Motor:</label>
            <select id="bikeType">
                <option value="Manual">Manual</option>
                <option value="Matic">Matic</option>
            </select>
            <label>Nama Motor:</label>
            <input type="text" id="bikeModel">
            <label>Tahun:</label>
            <input type="number" id="year" min="2000" max="2025">
            <label>Jenis Service:</label>
            <select id="serviceType">
                <option value="Service Ringan">Service Ringan</option>
                <option value="Service Injeksi">Service Injeksi</option>
                <option value="Service CVT">Service CVT (untuk matic)</option>
                <option value="Service Besar">Service Besar / Turun Mesin</option>
                <option value="Ganti Oli">Ganti Oli</option>
            </select>
            <label>Merk Oli (Jika ganti oli):</label>
            <input type="text" id="oilType">
            <button onclick="sendBooking()">Booking Sekarang</button>
        </div>
    </div>
    <div class="contact">
        <h2 id="contact">Hubungi Kami</h2>
        <p>📍 Lokasi: Jalan Bumi Sani Permai Selatan No.6, Tambun Selatan, Bekasi</p>
        <p>📞 Telp: 0877-8916-8900</p>
        <p>📲 WhatsApp: 0857-8143-4887</p>
        <p>📷 Instagram: <a href="https://www.instagram.com/putramotorbekasi" target="_blank">@putramotorbekasi</a></p>
        <p>🕒 Jam Operasional: Senin - Kamis, Sabtu - Minggu (09:00 - 17:00) | Jumat Libur</p>
    </div>
    <footer>
        &copy; 2025 Putra Motor Bekasi | Semua Hak Dilindungi
    </footer>
</body>
</html>
