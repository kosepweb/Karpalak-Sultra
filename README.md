<!DOCTYPE html>
<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Karpalak - Sultra </title>
    <style>
        /* Style dasar untuk halaman */
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            color: #333;
            overflow-x: hidden; /* Menghindari scroll horizontal */
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
            animation: fadeIn 1s ease-in-out; /* Animasi header */
        }

        header h1 {
            font-size: 2.5rem;
            margin: 0;
            z-index: 1;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.7);
        }

        header:before {
            content: "";
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.5);
            z-index: 0;
        }

        /* Navigasi */
        nav {
            background-color: #444;
            padding: 10px;
            text-align: center;
            animation: slideDown 0.5s ease-in-out; /* Animasi menu */
        }

        nav a {
            color: #fff;
            text-decoration: none;
            margin: 0 15px;
            padding: 10px;
            transition: background-color 0.3s, transform 0.3s; /* Animasi hover */
        }

        nav a:hover {
            background-color: #555;
            transform: scale(1.1);
        }

        /* Bagian Konten */
        section {
            padding: 20px;
            max-width: 1200px;
            margin: 20px auto;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.1);
            animation: fadeInUp 0.5s ease-in-out; /* Animasi bagian konten */
        }

        h2 {
            text-align: center;
            color: #333;
            font-size: 2rem;
            margin-bottom: 20px;
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
            transition: transform 0.3s; /* Efek zoom */
        }

        .image-container img:hover {
            transform: scale(1.05);
        }

        footer {
            background-color: #333;
            color: #fff;
            text-align: center;
            padding: 15px;
            position: relative;
            bottom: 0;
            width: 100%;
            animation: fadeIn 1s ease-in-out; /* Animasi footer */
        }

        /* Portofolio */
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
            transition: background-color 0.3s, transform 0.3s; /* Animasi hover */
        }

        .year-icon:hover {
            background-color: #ddd;
            transform: scale(1.1);
        }

        /* Modal */
        .modal {
            display: none;
            position: fixed;
            z-index: 999;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            background-color: rgba(0, 0, 0, 0.7);
            animation: fadeIn 0.5s; /* Animasi modal */
        }

        .modal-content {
            margin: 10% auto;
            padding: 20px;
            width: 60%;
            max-width: 800px;
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

        /* Struktur Organisasi */
        .org-structure {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
        }

        .org-member {
            width: 200px;
            text-align: center;
            padding: 10px;
            transition: transform 0.2s;
        }

        .org-member img {
            width: 100%;
            border-radius: 50%;
            transition: transform 0.2s;
        }

        .org-member:hover {
            transform: scale(1.05);
        }

        .org-member h3 {
            margin-top: 10px;
            font-size: 1.2rem;
        }

        .org-member p {
            font-size: 0.9rem;
            color: #555;
        }

        /* Media Queries untuk responsivitas */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2rem;
            }

            nav a {
                margin: 0 10px;
            }

            h2 {
                font-size: 1.5rem;
            }

            .year-icon {
                width: 80px;
                height: 80px;
                line-height: 50px;
                font-size: 1.2rem;
            }

            .org-member {
                width: 150px;
            }
        }

        @media (max-width: 480px) {
            header h1 {
                font-size: 1.5rem;
            }

            nav {
                padding: 5px;
            }

            nav a {
                margin: 0 5px;
                font-size: 0.8rem;
            }

            h2 {
                font-size: 1.2rem;
            }

            .org-member {
                width: 120px;
            }
        }

        /* Animasi */
        @keyframes fadeIn {
            from {
                opacity: 0;
            }
            to {
                opacity: 1;
            }
        }

        @keyframes slideDown {
            from {
                transform: translateY(-20px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
        }

        @keyframes fadeInUp {
            from {
                transform: translateY(20px);
                opacity: 0;
            }
            to {
                transform: translateY(0);
                opacity: 1;
            }
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
        <h1>Karpalak - Sultra</h1>
    </header>

    <!-- Navigasi Interaktif -->
    <nav>
        <a href="#tentang-kami">Tentang Kami</a>
        <a href="#layanan">Layanan</a>
        <a href="#visi-misi">Visi & Misi</a>
        <a href="#portfolio">Portofolio</a>
        <a href="#struktur-organisasi">Struktur Organisasi</a>
        <a href="#kontak">Kontak Kami</a>
    </nav>

    <!-- Tentang Kami -->
    <section id="tentang-kami">
        <h2>Tentang Kami</h2>
        <div class="content">
            <p>Karpalak ?</p>
        </div>
    </section>

    <!-- Layanan Kami -->
    <section id="layanan">
        <h2>Layanan Kami</h2>
        <div class="content">
            <p>Karpalak ?</p>
        </div>
    </section>

    <!-- Visi dan Misi -->
    <section id="visi-misi">
        <h2>Visi & Misi</h2>
        <div class="content">
            <p>Visi Karpalak ?, sementara misi kami adalah Karpalak ?</p>
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

    <!-- Modal untuk menampilkan gambar portofolio -->
    <div class="modal" id="modal-portfolio">
        <div class="modal-content">
            <span class="close">&times;</span>
            <img id="portfolio-img" src="" alt="Gambar Portofolio">
        </div>
    </div>

    <!-- Struktur Organisasi -->
    <section id="struktur-organisasi">
        <h2>Struktur Organisasi</h2>
        <div class="org-structure">
            <div class="org-member">
                <img src="foto111.png" alt="Pendiri 1">
                <h3>Pendiri 1</h3>
                <p>Periode: 2018-2020</p>
            </div>
            <div class="org-member">
                <img src="foto111.png" alt="Pendiri 2">
                <h3>Pendiri 2</h3>
                <p>Periode: 2019-2021</p>
            </div>
            <div class="org-member">
                <img src="foto111.png" alt="Pendiri 3">
                <h3>Pendiri 3</h3>
                <p>Periode: 2020-2022</p>
            </div>
            <div class="org-member">
                <img src="foto111.png" alt="Pendiri 4">
                <h3>Pendiri 4</h3>
                <p>Periode: 2021-2023</p>
            </div>
            <div class="org-member">
                <img src="foto111.png" alt="Pendiri 5">
                <h3>Pendiri 5</h3>
                <p>Periode: 2020-2023</p>
            </div>
            <div class="org-member">
                <img src="foto111.png" alt="Ketua Sekarang">
                <h3>Ketua Sekarang</h3>
                <p>Periode: 2023-Sekarang</p>
            </div>
        </div>
    </section>

    <!-- Kontak Kami -->
    <section id="kontak">
        <h2>Kontak Kami</h2>
        <div class="content">
            <p>Hubungi kami melalui email di <a href="mailto:andiirfan1020@gmail.com">andiirfan1020@gmail.com</a> atau telepon: 085345674445</p>
        </div>
    </section>

    <!-- Footer -->
    <footer>
        <p>&copy; 2024 Andi Irfan Maulana. Semua Hak Dilindungi.</p>
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
