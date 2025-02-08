<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Putra Motor Bekasi</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&display=swap');
        body { 
            font-family: Arial, sans-serif; 
            margin: 0; 
            padding: 0; 
            background: url('https://source.unsplash.com/1600x900/?garage,workshop') no-repeat center center/cover; 
            color: white; 
        }
        header { 
            background: #d32f2f; 
            color: white; 
            text-align: center; 
            padding: 20px; 
            font-size: 28px; 
            font-weight: bold; 
            font-family: 'Orbitron', sans-serif;
        }
        nav { display: flex; justify-content: center; background: #ff9800; padding: 15px; }
        nav a { color: white; text-decoration: none; margin: 0 20px; font-weight: bold; font-size: 18px; }
        .banner { text-align: center; padding: 60px 20px; font-size: 30px; font-weight: bold; }
        .container { max-width: 1000px; margin: auto; padding: 20px; text-align: center; background: rgba(0, 0, 0, 0.7); border-radius: 10px; }
        .booking-form { margin-top: 30px; text-align: left; }
        .booking-form label { font-weight: bold; display: block; margin-top: 12px; font-size: 18px; }
        .booking-form input, .booking-form select { width: 100%; padding: 10px; margin-top: 8px; border-radius: 5px; border: 1px solid #ccc; font-size: 16px; }
        .checkbox-container { display: flex; flex-direction: column; }
        .checkbox-container label { display: flex; align-items: center; margin-top: 5px; }
        .checkbox-container input { margin-right: 10px; }
        button { background: #ff9800; color: white; border: none; padding: 12px 25px; cursor: pointer; font-size: 20px; border-radius: 5px; transition: background 0.3s; }
        button:hover { background: #e65100; }
        .logo-container { display: flex; justify-content: center; margin-top: 30px; }
        .logo-container img { width: 80px; margin: 10px; }
    </style>
    <script>
        function sendBooking() {
            let name = document.getElementById('name').value;
            let date = document.getElementById('date').value;
            let time = document.getElementById('time').value;
            let brand = document.getElementById('brand').value;
            let type = document.getElementById('type').value;
            let year = document.getElementById('year').value;
            let services = Array.from(document.querySelectorAll('input[name="serviceType"]:checked')).map(e => e.value).join(', ');
            let oilType = document.getElementById('oilType').value;
            let message = `Booking Service:%0AName: ${name}%0A Tanggal: ${date}%0A Jam: ${time}%0A Merk Motor: ${brand}%0A Tipe Motor: ${type} (${year})%0A Layanan: ${services}%0A Oli: ${oilType}`;
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
            <label>Merk Motor:</label>
            <select id="brand">
                <option value="Honda">Honda</option>
                <option value="Yamaha">Yamaha</option>
                <option value="Suzuki">Suzuki</option>
                <option value="Kawasaki">Kawasaki</option>
                <option value="Vespa">Vespa</option>
                <option value="Lainnya">Lainnya</option>
            </select>
            <label>Tipe Motor:</label>
            <input type="text" id="type">
            <label>Tahun:</label>
            <input type="number" id="year" min="2000" max="2025">
            <label>Jenis Service:</label>
            <div class="checkbox-container">
                <label><input type="checkbox" name="serviceType" value="Service Ringan"> Service Ringan</label>
                <label><input type="checkbox" name="serviceType" value="Service Injeksi"> Service Injeksi</label>
                <label><input type="checkbox" name="serviceType" value="Service CVT"> Service CVT (untuk matic)</label>
                <label><input type="checkbox" name="serviceType" value="Service Besar"> Service Besar / Turun Mesin</label>
                <label><input type="checkbox" name="serviceType" value="Ganti Oli"> Ganti Oli</label>
            </div>
            <label>Merk Oli (Jika ganti oli):</label>
            <input type="text" id="oilType">
            <button onclick="sendBooking()">Booking Sekarang</button>
        </div>
    </div>
</body>
</html>
