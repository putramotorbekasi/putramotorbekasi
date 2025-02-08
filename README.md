<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Putra Motor Bekasi</title>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Russo+One&display=swap');
        body { 
            font-family: Arial, sans-serif; 
            margin: 0; 
            padding: 0; 
            background: black; 
            color: white; 
        }
        header { 
            display: flex;
            justify-content: center;
            align-items: center;
            background: linear-gradient(to right, #d32f2f 33%, white 33%, white 66%, #ff9800 66%);
            color: black; 
            text-align: center; 
            padding: 20px; 
            font-size: 28px; 
            font-weight: bold; 
            font-family: 'Russo One', sans-serif;
        }
        nav { display: flex; justify-content: center; background: #ff9800; padding: 15px; }
        nav a { color: white; text-decoration: none; margin: 0 20px; font-weight: bold; font-size: 18px; }
        .banner { text-align: center; padding: 60px 20px; font-size: 30px; font-weight: bold; }
        .container { max-width: 600px; margin: auto; padding: 20px; text-align: left; background: rgba(0, 0, 0, 0.7); border-radius: 10px; }
        .booking-form { margin-top: 30px; }
        .booking-form label { font-weight: bold; display: block; margin-top: 12px; font-size: 18px; }
        .booking-form input, .booking-form select { width: 100%; padding: 10px; margin-top: 8px; border-radius: 5px; border: 1px solid #ccc; font-size: 16px; }
        .checkbox-container { display: grid; grid-template-columns: 1fr 1fr; gap: 5px; align-items: center; }
        .checkbox-container label { display: flex; align-items: center; gap: 10px; }
        button { background: #ff9800; color: white; border: none; padding: 12px 25px; cursor: pointer; font-size: 20px; border-radius: 5px; transition: background 0.3s; margin-top: 20px; }
        button:hover { background: #e65100; }
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
            let oil = document.getElementById('oilType').value;
            let message = `Booking Service:%0AName: ${name}%0A Tanggal: ${date}%0A Jam: ${time}%0A Merk Motor: ${brand}%0A Tipe Motor: ${type} (${year})%0A Layanan: ${services}%0A Oli: ${oil}`;
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
                <label><input type="checkbox" name="serviceType" value="Service CVT"> Service CVT</label>
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
