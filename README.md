
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Profil Perusahaan - Inovasi Teknologi</title>
    <style>
        /* Style dasar untuk halaman */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
        }

        /* Header dengan background siluet */
        header {
            background: url('images/siluet-background.jpg') no-repeat center center/cover;
            height: 300px;
            color: #fff;
            text-align: center;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        header h1 {
            font-size: 2.5rem;
            margin: 0;
            z-index: 1;
        }

        header:before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5); /* Efek siluet */
            z-index: 0;
        }

        /* Style untuk navigasi */
        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px;
        }

        nav a:hover {
            background-color: #555;
        }

        section {
            padding: 20px;
            max-width: 1200px;
            margin: 20px auto;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
        }

        h2 {
            text-align: center;
            color: #333;
        }

        .content {
            margin: 20px 0;
            text-align: center;
        }

        .image-container {
            text-align: center;
            margin: 20px 0;
        }

        .image-container img {
            width: 100%;
            max-width: 600px;
            border-radius: 8px;
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 15px;
            position: fixed;
            width: 100%;
            bottom: 0;
        }

        /* Style untuk portofolio */
        .portfolio {
            text-align: center;
        }

        .year-icon {
            display: inline-block;
            margin: 20px;
            padding: 20px;
            border: 2px solid #333;
            border-radius: 50%;
            width: 100px;
            height: 100px;
            text-align: center;
            line-height: 60px;
            font-size: 1.5rem;
            background-color: #f4f4f4;
            cursor: pointer;
        }

        .year-icon:hover {
            background-color: #ddd;
        }

        /* Style untuk modal (pop-up) */
        .modal {
            display: none;
            position: fixed;
            z-index: 999;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
        }

        .modal-content {
            margin: 10% auto;
            padding: 20px;
            width: 60%;
            background-color: white;
            border-radius: 8px;
            text-align: center;
        }

        .modal-content img {
            max-width: 100%;
            border-radius: 8px;
        }

        .close {
            color: #333;
            font-size: 2rem;
            position: absolute;
            right: 20px;
            top: 10px;
            cursor: pointer;
        }
    </style>
</head>

<body>

    <!-- Backsound yang otomatis terputar -->
    <audio id="backsound" autoplay loop>
        <source src="1 (mp3cut.net).mp3" type="audio/mpeg">
        Your browser does not support the audio element.
    </audio>

    <!-- Header dengan background siluet -->
    <header>
        <h1>Profil Perusahaan - Inovasi Teknologi</h1>
    </header>

    <!-- Navigasi Interaktif -->
    <nav>
        <a href="#tentang-kami">Tentang Kami</a>
        <a href="#layanan">Layanan</a>
        <a href="#visi-misi">Visi & Misi</a>
        <a href="#portfolio">Portofolio</a>
        <a href="#kontak">Kontak Kami</a>
    </nav>

    <!-- Tentang Kami -->
    <section id="tentang-kami">
        <h2>Tentang Kami</h2>
        <div class="content">
            <p>Perusahaan kami berdedikasi untuk memberikan solusi teknologi terbaik dengan inovasi yang terus menerus. Kami berkomitmen untuk menghadirkan layanan dan produk yang memajukan era digital di berbagai sektor industri.</p>
        </div>
    </section>

    <!-- Layanan Kami -->
    <section id="layanan">
        <h2>Layanan Kami</h2>
        <div class="content">
            <p>Kami menyediakan berbagai layanan teknologi, termasuk pengembangan software, solusi cloud, dan transformasi digital untuk membantu bisnis Anda mencapai efisiensi dan pertumbuhan.</p>
        </div>
    </section>

    <!-- Visi dan Misi -->
    <section id="visi-misi">
        <h2>Visi & Misi</h2>
        <div class="content">
            <p>Visi kami adalah menjadi pemimpin dalam inovasi teknologi global, sementara misi kami adalah menyediakan solusi teknologi yang berdampak positif bagi masyarakat dan industri.</p>
        </div>
    </section>

    <!-- Portofolio dengan tahun yang dapat diklik -->
    <section id="portfolio">
        <h2>Portofolio</h2>
        <div class="portfolio">
            <div class="year-icon" data-year="2020">2020</div>
            <div class="year-icon" data-year="2021">2021</div>
            <div class="year-icon" data-year="2022">2022</div>
        </div>
    </section>

    <!-- Modal (Pop-up) untuk portofolio -->
    <div id="modal-portfolio" class="modal">
        <div class="modal-content">
            <span class="close">&times;</span>
            <img id="portfolio-img" src="" alt="Foto Dokumentasi">
        </div>
    </div>

    <!-- Kontak Kami -->
    <section id="kontak">
        <h2>Kontak Kami</h2>
        <div class="content">
            <p>Hubungi kami melalui email di <a href="mailto:info@perusahaan.com">info@perusahaan.com</a> atau kunjungi kantor kami di Jalan Teknologi No. 5, Jakarta.</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Inovasi Teknologi. All rights reserved.</p>
    </footer>

    <script>
        // Jika pengguna tidak ingin suara otomatis diputar, ini akan memastikan bisa dijeda
        let audio = document.getElementById("backsound");
        window.addEventListener('click', function () {
            if (audio.paused) {
                audio.play();
            }
        });

        // Menampilkan foto dokumentasi berdasarkan tahun yang dipilih
        const modal = document.getElementById("modal-portfolio");
        const modalImg = document.getElementById("portfolio-img");
        const closeModal = document.querySelector(".close");
        const yearIcons = document.querySelectorAll(".year-icon");

        yearIcons.forEach(icon => {
            icon.addEventListener("click", function () {
                const year = this.getAttribute("data-year");
                modal.style.display = "block";
                modalImg.src = `images/portfolio-${year}.jpg`; // Pastikan Anda memiliki gambar sesuai tahun
            });
        });

        // Menutup modal saat tombol close diklik
        closeModal.addEventListener("click", function () {
            modal.style.display = "none";
        });

        // Menutup modal saat area luar diklik
        window.addEventListener("click", function (event) {
            if (event.target == modal) {
                modal.style.display = "none";
            }
        });
    </script>
</body>

</html>
