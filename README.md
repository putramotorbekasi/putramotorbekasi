<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Putra Motor Bekasi</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #222; color: white; text-align: center; }
        header {
            background: linear-gradient(to bottom, red 33%, white 33%, white 66%, orange 66%);
            color: black;
            text-align: center;
            padding: 30px;
            font-size: 40px;
            font-weight: bold;
            font-family: 'Arial Black', sans-serif;
            letter-spacing: 3px;
        }
        
    
.container { max-width: 600px; margin: auto; padding: 20px; background: #333; border-radius: 10px; }
        label { display: block; margin-top: 15px; font-size: 18px; text-align: left; }
        input, select { width: 100%; padding: 10px; margin-top: 5px; border-radius: 5px; border: 1px solid #ccc; font-size: 16px; }
        .service-box { display: flex; align-items: center; justify-content: center; background: #444; padding: 10px; margin-top: 10px; border-radius: 5px; cursor: pointer; }
        .service-box.selected { background: red; }
    </style>
    <script>
        function toggleService(box) {
            box.classList.toggle('selected');
        }
    </script>
</head>
<body>
    <header>PUTRA MOTOR BEKASI</header>
    <div class="container">
        <h2>Booking Service</h2>
        <label>Nama:</label>
        <input type="text" id="name">
        <label>Jenis Motor:</label>
        <select id="bikeType">
            <option value="Manual">Manual</option>
            <option value="Matic">Matic</option>
        </select>
        <label>Merk Motor:</label>
        <select id="bikeBrand">
            <option value="Honda">Honda</option>
            <option value="Yamaha">Yamaha</option>
            <option value="Suzuki">Suzuki</option>
            <option value="Kawasaki">Kawasaki</option>
            <option value="Vespa">Vespa</option>
            <option value="Lainnya">Lainnya</option>
        </select>
        <label>Type Motor:</label>
        <input type="text" id="bikeModel">
        <label>Tahun:</label>
        <input type="number" id="year" min="2000" max="2025">
        <label>Jenis Service:</label>
       <div class="service-box" onclick="toggleService(this)">Service Ringan</div>
            <div class="service-box" onclick="toggleService(this)">Service Injeksi</div>
            <div class="service-box" onclick="toggleService(this)">Service CVT</div>
            <div class="service-box" onclick="toggleService(this)">Service Besar</div>
            <div class="service-box" onclick="toggleService(this)">Ganti Oli</div>
        <label>Merk Oli:</label>
       <input type="text" id="oilBrand">
        <button style="margin-top: 20px; padding: 12px 20px; font-size: 18px; background: #ff9800; color: white; border: none; cursor: pointer;">Booking Sekarang</button>
    </div>
    <div class="about-section">
        <h2>PUTRA MOTOR BEKASI - Motorbike Repair Shop</h2>
        <p>Putra Motor Bekasi adalah sebuah bengkel sepeda motor kecil di daerah Tambun Selatan - Bekasi yang berdiri sejak 2005 silam.</p>
        <p>Pesatnya perkembangan otomotif khususnya sepeda motor, Putra Motor Bekasi menyediakan jasa:</p>
        <ul>
            <p>SPARE PART</p>
            <p>GANTI OLI</p>
            <p>SERVICE</p>
            <p>INJECTION</p>
        </ul>
        <p>Dengan tenaga ahli yang sudah berpengalaman di bidangnya, kami hadir untuk Anda yang selalu mengutamakan kenyamanan dan keselamatan dalam berkendara.</p>
    </div>
<div class="contact-section">
        <h2>Contact Information</h2>
        <p>Phone: 087789168900</p>
        <p>WhatsApp: 085781434887</p>
        <p>Instagram: <a href="https://www.instagram.com/putramotorbekasi" target="_blank">@putramotorbekasi</a></p>
        <p>Location : Jalan Bumi Sani Permai Selatan No.6, RT.02/RW.11, Setiamekar, Kecamatan Tambun Selatan, Kabupaten Bekasi, Jawa Barat 17510</p>
    </div>
</body>
</html>
