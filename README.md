<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Putra Motor Bekasi</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 0; background: #222; color: white; text-align: center; }
        header { background: #d32f2f; color: white; text-align: center; padding: 30px; font-size: 40px; font-weight: bold; font-family: 'Impact', sans-serif; }
        .container { max-width: 600px; margin: auto; padding: 20px; background: #333; border-radius: 10px; }
        label { display: block; margin-top: 15px; font-size: 18px; }
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
</body>
</html>
