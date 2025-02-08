<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PUTRA MOTOR Bekasi - Bengkel Motor Profesional</title>
    <style>
        /* Reset CSS */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background-color: #f9f9f9;
            color: #333;
        }

        /* Header */
        header {
            background-color: #ff6600; /* Orange */
            color: white;
            padding: 2rem;
            text-align: center;
        }

        header h1 {
            font-size: 2.5rem;
            margin-bottom: 0.5rem;
        }

        header p {
            font-size: 1.2rem;
        }

        /* Container */
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 2rem;
        }

        /* About Section */
        .about {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 2rem;
        }

        .about h2 {
            color: #ff6600; /* Orange */
            margin-bottom: 1rem;
        }

        .about p {
            margin-bottom: 1rem;
        }

        .about ul {
            list-style: none;
            padding-left: 1rem;
        }

        .about ul li {
            margin-bottom: 0.5rem;
        }

        .about ul li::before {
            content: "✓";
            color: #ff6600; /* Orange */
            margin-right: 0.5rem;
        }

        /* Services Section */
        .services {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 1.5rem;
            margin-bottom: 2rem;
        }

        .service-card {
            background-color: white;
            padding: 1.5rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            text-align: center;
        }

        .service-card h3 {
            color: #ff0000; /* Red */
            margin-bottom: 1rem;
        }

        .service-card p {
            color: #555;
        }

        /* Booking Section */
        .booking {
            background-color: #ff6600; /* Orange */
            padding: 2rem;
            border-radius: 10px;
            text-align: center;
            margin-bottom: 2rem;
        }

        .booking h2 {
            color: white;
            margin-bottom: 1rem;
        }

        .booking button {
            background-color: #ff0000; /* Red */
            color: white;
            border: none;
            padding: 1rem 2rem;
            font-size: 1rem;
            border-radius: 5px;
            cursor: pointer;
            transition: background-color 0.3s;
        }

        .booking button:hover {
            background-color: #cc0000; /* Darker Red */
        }

        /* Contact Section */
        .contact {
            background-color: white;
            padding: 2rem;
            border-radius: 10px;
            box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1);
            margin-bottom: 2rem;
        }

        .contact h2 {
            color: #ff6600; /* Orange */
            margin-bottom: 1rem;
        }

        .contact p {
            margin-bottom: 0.5rem;
        }

        .contact a {
            color: #ff0000; /* Red */
            text-decoration: none;
        }

        .contact a:hover {
            text-decoration: underline;
        }

        /* Footer */
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 1.5rem;
            margin-top: 2rem;
        }

        footer p {
            margin: 0;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
        <h1>PUTRA MOTOR BEKASI</h1>
        <p>Bengkel Motor Profesional Sejak 2005</p>
    </header>

    <!-- Container -->
    <div class="container">
        <!-- About Section -->
        <section class="about">
            <h2>Tentang Kami</h2>
            <p>
                Putra Motor Bekasi adalah bengkel sepeda motor kecil di daerah Tambun Selatan - Bekasi yang berdiri sejak 2005. Dengan perkembangan otomotif yang pesat, kami menyediakan layanan berkualitas untuk kenyamanan dan keselamatan berkendara Anda.
            </p>
            <ul>
                <li>SPARE PART</li>
                <li>GANTI OLI</li>
                <li>SERVICE</li>
                <li>INJECTION</li>
            </ul>
        </section>

        <!-- Services Section -->
        <section class="services">
            <div class="service-card">
                <h3>Service Ringan</h3>
                <p>Perawatan rutin untuk menjaga performa motor Anda.</p>
            </div>
            <div class="service-card">
                <h3>Service Injeksi</h3>
                <p>Perbaikan dan perawatan sistem injeksi motor.</p>
            </div>
            <div class="service-card">
                <h3>Service CVT</h3>
                <p>Khusus untuk motor matic, perawatan sistem CVT.</p>
            </div>
            <div class="service-card">
                <h3>Service Besar/Turun Mesin</h3>
                <p>Perbaikan komprehensif untuk masalah mesin.</p>
            </div>
        </section>

        <!-- Booking Section -->
        <section class="booking">
            <h2>Booking Service Sekarang!</h2>
            <button onclick="window.location.href='https://wa.me/6285781434887?text=Halo,%20saya%20ingin%20booking%20service%20di%20PUTRA%20MOTOR%20Bekasi.'">
                Booking via WhatsApp
            </button>
        </section>

        <!-- Contact Section -->
        <section class="contact">
            <h2>Hubungi Kami</h2>
            <p>Telepon: <a href="tel:087789168900">0877-8916-8900</a></p>
            <p>WhatsApp: <a href="https://wa.me/6285781434887">0857-8143-4887</a></p>
            <p>Instagram: <a href="https://www.instagram.com/putramotorbekasi" target="_blank">@putramotorbekasi</a></p>
            <p>Alamat: Jalan Bumi Sani Permai Selatan No.6, RT.02/RW.11, Setiamekar, Kecamatan Tambun Selatan, Kabupaten Bekasi, Jawa Barat 17510</p>
            <p>Jam Operasional: Buka 09:00 - 17:00 (Jumat Tutup)</p>
        </section>
    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 PUTRA MOTOR Bekasi. All Rights Reserved.</p>
    </footer>
</body>
</html>
