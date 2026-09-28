<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Ikbal Dental - Gigi Palsu & Perawatan Gigi</title>

    <!-- Google Font -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

    <style>

        /* =========================
           RESET
        ========================= */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: 'Poppins', sans-serif;
            background: #eaf8ff;
            color: #17324d;
            line-height: 1.7;
        }

        a {
            text-decoration: none;
        }

        /* =========================
           NAVBAR
        ========================= */
        header {
            position: sticky;
            top: 0;
            z-index: 1000;
            background: rgba(255, 255, 255, 0.95);
            box-shadow: 0 3px 15px rgba(0, 100, 150, 0.1);
        }

        .navbar {
            max-width: 1200px;
            margin: auto;
            padding: 15px 25px;
            display: flex;
            align-items: center;
            justify-content: space-between;
        }

        .logo {
            font-size: 24px;
            font-weight: 700;
            color: #087ea4;
        }

        .logo span {
            color: #36b7df;
        }

        .nav-menu {
            display: flex;
            list-style: none;
            gap: 25px;
            align-items: center;
        }

        .nav-menu a {
            color: #17324d;
            font-weight: 500;
            transition: 0.3s;
        }

        .nav-menu a:hover {
            color: #08a6d5;
        }

        .nav-button {
            background: #08a6d5;
            color: white !important;
            padding: 10px 18px;
            border-radius: 25px;
        }

        .nav-button:hover {
            background: #087ea4;
        }

        /* =========================
           HERO
        ========================= */
        .hero {
            min-height: 90vh;
            display: flex;
            align-items: center;
            background: linear-gradient(135deg, #dff7ff, #b9ebfa);
            padding: 70px 8%;
        }

        .hero-container {
            max-width: 1200px;
            margin: auto;
            width: 100%;
            display: grid;
            grid-template-columns: 1.2fr 1fr;
            gap: 50px;
            align-items: center;
        }

        .hero-text h1 {
            font-size: 55px;
            color: #087ea4;
            line-height: 1.2;
            margin-bottom: 15px;
        }

        .hero-text h2 {
            font-size: 30px;
            color: #17324d;
            margin-bottom: 20px;
        }

        .hero-text p {
            font-size: 17px;
            margin-bottom: 20px;
            color: #456477;
        }

        .hero-buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
            margin-top: 25px;
        }

        .btn {
            display: inline-block;
            padding: 13px 25px;
            border-radius: 30px;
            font-weight: 600;
            transition: 0.3s;
        }

        .btn-primary {
            background: #08a6d5;
            color: white;
        }

        .btn-primary:hover {
            background: #087ea4;
            transform: translateY(-3px);
        }

        .btn-secondary {
            background: white;
            color: #087ea4;
            border: 2px solid #08a6d5;
        }

        .btn-secondary:hover {
            background: #08a6d5;
            color: white;
        }

        .hero-image {
            display: flex;
            justify-content: center;
        }

        .tooth {
            width: 300px;
            height: 300px;
            background: white;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 150px;
            box-shadow: 0 20px 50px rgba(0, 130, 170, 0.2);
            animation: floating 3s ease-in-out infinite;
        }

        @keyframes floating {
            0%, 100% {
                transform: translateY(0);
            }

            50% {
                transform: translateY(-15px);
            }
        }

        /* =========================
           GENERAL SECTION
        ========================= */
        section {
            padding: 80px 8%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 50px;
        }

        .section-title h2 {
            font-size: 35px;
            color: #087ea4;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #607d8b;
        }

        /* =========================
           ABOUT
        ========================= */
        .about {
            background: white;
        }

        .about-card {
            max-width: 1000px;
            margin: auto;
            background: #eaf8ff;
            padding: 40px;
            border-radius: 20px;
            box-shadow: 0 10px 30px rgba(0, 100, 150, 0.08);
        }

        .about-card p {
            margin-bottom: 15px;
        }

        /* =========================
           SERVICES
        ========================= */
        .services {
            background: #eaf8ff;
        }

        .cards {
            max-width: 1200px;
            margin: auto;
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 20px;
            box-shadow: 0 8px 25px rgba(0, 100, 150, 0.08);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-8px);
            box-shadow: 0 15px 35px rgba(0, 100, 150, 0.15);
        }

        .card-icon {
            font-size: 45px;
            margin-bottom: 15px;
        }

        .card h3 {
            color: #087ea4;
            margin-bottom: 12px;
            font-size: 20px;
        }

        .card p {
            color: #607d8b;
            font-size: 14px;
            margin-bottom: 20px;
        }

        .card .btn {
            font-size: 13px;
            padding: 9px 18px;
        }

        /* =========================
           EDUKASI
        ========================= */
        .education {
            background: white;
        }

        .education-card {
            max-width: 1000px;
            margin: 0 auto 25px;
            background: #f1fbff;
            padding: 30px;
            border-radius: 18px;
            border-left: 5px solid #08a6d5;
        }

        .education-card h3 {
            color: #087ea4;
            margin-bottom: 15px;
        }

        .education-card ul {
            padding-left: 25px;
            margin-top: 15px;
        }

        /* =========================
           WHY US
        ========================= */
        .why-us {
            background: #dff7ff;
        }

        /* =========================
           CTA
        ========================= */
        .cta {
            background: linear-gradient(135deg, #087ea4, #08a6d5);
            color: white;
            text-align: center;
        }

        .cta h2 {
            font-size: 35px;
            margin-bottom: 15px;
        }

        .cta p {
            margin-bottom: 25px;
        }

        .cta .btn {
            background: white;
            color: #087ea4;
        }

        .cta .btn:hover {
            transform: scale(1.05);
        }

        /* =========================
           CONTACT
        ========================= */
        .contact {
            background: white;
        }

        .contact-container {
            max-width: 900px;
            margin: auto;
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 25px;
        }

        .contact-card {
            background: #eaf8ff;
            padding: 30px;
            border-radius: 20px;
        }

        .contact-card h3 {
            color: #087ea4;
            margin-bottom: 20px;
        }

        .contact-item {
            margin-bottom: 15px;
        }

        /* =========================
           FOOTER
        ========================= */
        footer {
            background: #063d52;
            color: white;
            text-align: center;
            padding: 35px 20px;
        }

        footer h3 {
            font-size: 25px;
            margin-bottom: 10px;
        }

        footer p {
            color: #c9eaf5;
            margin-bottom: 8px;
        }

        /* =========================
           WHATSAPP FLOATING
        ========================= */
        .whatsapp {
            position: fixed;
            right: 25px;
            bottom: 25px;
            width: 60px;
            height: 60px;
            background: #25d366;
            color: white;
            border-radius: 50%;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 30px;
            box-shadow: 0 5px 20px rgba(0,0,0,0.2);
            z-index: 999;
            transition: 0.3s;
        }

        .whatsapp:hover {
            transform: scale(1.1);
        }

        /* =========================
           BACK TO TOP
        ========================= */
        #topBtn {
            position: fixed;
            bottom: 95px;
            right: 28px;
            width: 45px;
            height: 45px;
            border: none;
            border-radius: 50%;
            background: #087ea4;
            color: white;
            cursor: pointer;
            display: none;
            font-size: 20px;
            z-index: 999;
        }

        /* =========================
           RESPONSIVE
        ========================= */
        @media (max-width: 900px) {

            .hero-container {
                grid-template-columns: 1fr;
                text-align: center;
            }

            .hero-buttons {
                justify-content: center;
            }

            .hero-text h1 {
                font-size: 42px;
            }

            .cards {
                grid-template-columns: repeat(2, 1fr);
            }

            .contact-container {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 650px) {

            .nav-menu {
                display: none;
            }

            .navbar {
                justify-content: center;
            }

            .hero {
                padding: 60px 6%;
            }

            .hero-text h1 {
                font-size: 36px;
            }

            .hero-text h2 {
                font-size: 23px;
            }

            .tooth {
                width: 220px;
                height: 220px;
                font-size: 100px;
            }

            section {
                padding: 60px 6%;
            }

            .section-title h2 {
                font-size: 28px;
            }

            .cards {
                grid-template-columns: 1fr;
            }

            .cta h2 {
                font-size: 27px;
            }
        }

    </style>
</head>

<body>

    <!-- =========================
         NAVBAR
    ========================= -->

    <header>
        <nav class="navbar">

            <div class="logo">
                🦷 IKBAL <span>DENTAL</span>
            </div>

            <ul class="nav-menu">
                <li><a href="#beranda">Beranda</a></li>
                <li><a href="#tentang">Tentang Kami</a></li>
                <li><a href="#layanan">Layanan</a></li>
                <li><a href="#edukasi">Edukasi</a></li>
                <li><a href="#mengapa">Mengapa Kami</a></li>
                <li><a href="#kontak">Kontak</a></li>
                <li>
                    <a class="nav-button"
                       href="https://wa.me/628236423003"
                       target="_blank">
                        Konsultasi
                    </a>
                </li>
            </ul>

        </nav>
    </header>


    <!-- =========================
         HERO
    ========================= -->

    <section class="hero" id="beranda">

        <div class="hero-container">

            <div class="hero-text">

                <h1>🦷 Ikbal Dental</h1>

                <h2>
                    Senyum Nyaman, Percaya Diri Lebih Baik
                </h2>

                <p>
                    Ikbal Dental hadir sebagai tempat pelayanan kesehatan
                    gigi yang membantu masyarakat menjaga kesehatan dan
                    kebersihan gigi serta mulut.
                </p>

                <p>
                    Pemeriksaan gigi secara rutin dapat membantu menemukan
                    masalah gigi lebih awal sehingga perawatan dapat
                    dilakukan dengan lebih tepat.
                </p>

                <strong>
                    Jangan tunggu sakit untuk memeriksa gigi.
                </strong>

                <div class="hero-buttons">

                    <a class="btn btn-primary"
                       href="https://wa.me/628236423003"
                       target="_blank">
                        💬 Konsultasi Gratis
                    </a>

                    <a class="btn btn-secondary"
                       href="#layanan">
                        🦷 Lihat Layanan
                    </a>

                </div>

            </div>

            <div class="hero-image">

                <div class="tooth">
                    🦷
                </div>

            </div>

        </div>

    </section>


    <!-- =========================
         TENTANG
    ========================= -->

    <section class="about" id="tentang">

        <div class="section-title">

            <h2>💙 Tentang Ikbal Dental</h2>

            <p>
                Membantu menjaga kesehatan dan kenyamanan gigi Anda
            </p>

        </div>

        <div class="about-card">

            <p>
                Ikbal Dental hadir sebagai tempat pelayanan kesehatan
                gigi yang membantu masyarakat menjaga kesehatan dan
                kebersihan gigi serta mulut.
            </p>

            <p>
                Pemeriksaan gigi secara rutin dapat membantu menemukan
                masalah gigi lebih awal sehingga perawatan dapat dilakukan
                dengan lebih tepat.
            </p>

            <p>
                Kami percaya bahwa kesehatan gigi tidak hanya berkaitan
                dengan penampilan, tetapi juga merupakan bagian penting
                dari kesehatan tubuh secara keseluruhan.
            </p>

        </div>

    </section>


    <!-- =========================
         LAYANAN
    ========================= -->

    <section class="services" id="layanan">

        <div class="section-title">

            <h2>🦷 Layanan Ikbal Dental</h2>

            <p>
                Pilihan layanan gigi untuk membantu memenuhi kebutuhan Anda
            </p>

        </div>

        <div class="cards">

            <div class="card">

                <div class="card-icon">😁</div>

                <h3>Pemasangan Gigi Palsu Akrilik</h3>

                <p>
                    Ikbal Dental melayani pemasangan gigi palsu berbahan
                    akrilik untuk membantu menggantikan gigi yang hilang.
                    Gigi palsu akrilik dapat menjadi salah satu pilihan
                    untuk membantu fungsi mengunyah, berbicara, dan
                    menunjang penampilan.
                </p>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Konsultasi
                </a>

            </div>


            <div class="card">

                <div class="card-icon">🦷</div>

                <h3>Pemasangan Gigi Palsu Valplast</h3>

                <p>
                    Tersedia juga gigi palsu Valplast, yaitu gigi palsu
                    berbahan fleksibel yang dapat menjadi pilihan bagi
                    pengguna yang menginginkan gigi palsu dengan tampilan
                    yang lebih natural dan nyaman digunakan.
                </p>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Konsultasi
                </a>

            </div>


            <div class="card">

                <div class="card-icon">🔧</div>

                <h3>Servis & Perbaikan Gigi Palsu</h3>

                <p>
                    Gigi palsu rusak, patah, atau membutuhkan perbaikan?
                    Ikbal Dental melayani servis dan perbaikan gigi palsu
                    agar dapat digunakan kembali dengan nyaman.
                </p>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Konsultasi
                </a>

            </div>


            <div class="card">

                <div class="card-icon">🏠</div>

                <h3>Home Service / Panggilan ke Rumah</h3>

                <p>
                    Tidak sempat datang ke tempat pelayanan?
                    Ikbal Dental menerima panggilan ke rumah sehingga
                    konsultasi dan pelayanan gigi palsu dapat dilakukan
                    di rumah sesuai dengan layanan yang tersedia.
                </p>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Hubungi Kami
                </a>

            </div>


            <div class="card">

                <div class="card-icon">💬</div>

                <h3>Konsultasi Gratis</h3>

                <p>
                    Masih bingung memilih jenis gigi palsu yang sesuai?
                    Konsultasi gratis untuk membantu Anda mendapatkan
                    informasi mengenai pilihan gigi palsu, proses
                    pemasangan, perawatan, maupun servis.
                </p>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Konsultasi
                </a>

            </div>

        </div>

    </section>


    <!-- =========================
         EDUKASI
    ========================= -->

    <section class="education" id="edukasi">

        <div class="section-title">

            <h2>📚 Edukasi Kesehatan Gigi</h2>

            <p>
                Kenali cara sederhana menjaga kesehatan gigi dan mulut
            </p>

        </div>


        <div class="education-card">

            <h3>🪥 1. Mengapa Harus Rajin Menyikat Gigi?</h3>

            <p>
                Menyikat gigi secara teratur membantu membersihkan sisa
                makanan dan plak yang menempel pada permukaan gigi.
                Kebiasaan ini dapat membantu menjaga kebersihan gigi
                dan mengurangi risiko terjadinya masalah gigi dan mulut.
            </p>

            <strong>Tips:</strong>

            <ul>
                <li>Sikat gigi minimal 2 kali sehari.</li>
                <li>Gunakan pasta gigi yang mengandung fluoride.</li>
                <li>Sikat gigi dengan gerakan lembut.</li>
                <li>Jangan lupa membersihkan bagian belakang gigi.</li>
            </ul>

        </div>


        <div class="education-card">

            <h3>🦷 2. Apa Itu Gigi Berlubang?</h3>

            <p>
                Gigi berlubang atau karies terjadi ketika jaringan keras
                gigi mengalami kerusakan. Salah satu faktor yang berperan
                adalah plak bakteri yang memanfaatkan gula dari makanan
                dan minuman sehingga menghasilkan asam yang dapat merusak
                permukaan gigi.
            </p>

            <strong>Cara membantu mencegahnya:</strong>

            <ul>
                <li>✅ Kurangi konsumsi makanan dan minuman tinggi gula.</li>
                <li>✅ Sikat gigi secara rutin.</li>
                <li>✅ Bersihkan sela-sela gigi.</li>
                <li>✅ Lakukan pemeriksaan gigi secara berkala.</li>
            </ul>

        </div>


        <div class="education-card">

            <h3>🧼 3. Apa Itu Karang Gigi?</h3>

            <p>
                Karang gigi merupakan plak yang mengalami pengerasan
                sehingga tidak mudah dibersihkan hanya dengan sikat
                gigi biasa. Karang gigi dapat menumpuk di sekitar
                garis gusi.
            </p>

            <p>
                Salah satu perawatan yang digunakan untuk membersihkannya
                adalah scaling.
            </p>

        </div>


        <div class="education-card">

            <h3>🍭 4. Batasi Makanan dan Minuman Manis</h3>

            <p>
                Terlalu sering mengonsumsi makanan atau minuman manis
                dapat meningkatkan risiko karies. Bukan hanya jumlah gula
                yang perlu diperhatikan, tetapi juga seberapa sering gigi
                terpapar gula.
            </p>

            <p>
                Pilih camilan yang lebih sehat dan biasakan berkumur atau
                membersihkan gigi setelah mengonsumsi makanan.
            </p>

        </div>

    </section>


    <!-- =========================
         MENGAPA KAMI
    ========================= -->

    <section class="why-us" id="mengapa">

        <div class="section-title">

            <h2>⭐ Mengapa Memilih Ikbal Dental?</h2>

            <p>
                Pelayanan dengan mengutamakan kenyamanan dan informasi
            </p>

        </div>


        <div class="cards">

            <div class="card">

                <div class="card-icon">💙</div>

                <h3>Pelayanan Ramah</h3>

                <p>
                    Memberikan pelayanan dengan mengutamakan
                    kenyamanan pasien.
                </p>

            </div>


            <div class="card">

                <div class="card-icon">🦷</div>

                <h3>Perawatan Gigi</h3>

                <p>
                    Membantu menjaga kesehatan dan kebersihan gigi
                    melalui berbagai layanan perawatan.
                </p>

            </div>


            <div class="card">

                <div class="card-icon">📖</div>

                <h3>Edukasi Kesehatan</h3>

                <p>
                    Memberikan informasi mengenai cara menjaga
                    kesehatan gigi dan mulut.
                </p>

            </div>


            <div class="card">

                <div class="card-icon">😊</div>

                <h3>Nyaman untuk Konsultasi</h3>

                <p>
                    Pasien dapat menyampaikan keluhan dan berkonsultasi
                    mengenai kondisi kesehatan giginya.
                </p>

            </div>

        </div>

    </section>


    <!-- =========================
         CTA
    ========================= -->

    <section class="cta">

        <h2>Punya Keluhan atau Membutuhkan Gigi Palsu?</h2>

        <p>
            Jangan ragu untuk berkonsultasi dengan Ikbal Dental.
        </p>

        <a class="btn"
           href="https://wa.me/628236423003"
           target="_blank">
            💬 Konsultasi Gratis via WhatsApp
        </a>

    </section>


    <!-- =========================
         KONTAK
    ========================= -->

    <section class="contact" id="kontak">

        <div class="section-title">

            <h2>📞 Hubungi Kami</h2>

            <p>
                Silakan hubungi Ikbal Dental untuk informasi lebih lanjut
            </p>

        </div>


        <div class="contact-container">

            <div class="contact-card">

                <h3>🦷 Ikbal Dental</h3>

                <div class="contact-item">
                    📱 <strong>WhatsApp</strong><br>
                    08236423003
                </div>

                <div class="contact-item">
                    🕐 <strong>Jam Pelayanan</strong><br>
                    08.00 - 21.00
                </div>

                <div class="contact-item">
                    📍 <strong>Alamat</strong><br>
                    Jl. Pabidikan No.174 B, Puhun Tembok,
                    Kec. Mandiangin Koto Selayan,
                    Kota Bukittinggi, Sumatera Barat 26136,
                    Indonesia
                </div>

            </div>


            <div class="contact-card">

                <h3>💬 Konsultasi</h3>

                <p>
                    Masih memiliki pertanyaan mengenai gigi palsu,
                    servis, atau home service?
                </p>

                <br>

                <a class="btn btn-primary"
                   href="https://wa.me/628236423003"
                   target="_blank">
                    Chat WhatsApp Sekarang
                </a>

            </div>

        </div>

    </section>


    <!-- =========================
         FOOTER
    ========================= -->

    <footer>

        <h3>🦷 IKBAL DENTAL</h3>

        <p>
            Solusi gigi palsu dan edukasi kesehatan gigi
            untuk membantu Anda menjaga senyum dan kenyamanan.
        </p>

        <p>
            📱 08236423003
        </p>

        <p>
            © 2026 Ikbal Dental. All Rights Reserved.
        </p>

    </footer>


    <!-- =========================
         FLOATING WHATSAPP
    ========================= -->

    <a class="whatsapp"
       href="https://wa.me/628236423003"
       target="_blank"
       title="Chat WhatsApp">
        💬
    </a>


    <!-- =========================
         BACK TO TOP
    ========================= -->

    <button id="topBtn" onclick="topFunction()">
        ↑
    </button>


    <!-- =========================
         JAVASCRIPT
    ========================= -->

    <script>

        // Tombol kembali ke atas
        const topBtn = document.getElementById("topBtn");

        window.onscroll = function() {

            if (
                document.body.scrollTop > 300 ||
                document.documentElement.scrollTop > 300
            ) {

                topBtn.style.display = "block";

            } else {

                topBtn.style.display = "none";

            }

        };


        // Fungsi kembali ke atas
        function topFunction() {

            window.scrollTo({
                top: 0,
                behavior: "smooth"
            });

        }

    </script>

</body>
</html>
