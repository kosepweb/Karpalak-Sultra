<html lang="id">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>Karpalak - Sultra</title>
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
            background-color: rgba(0, 0, 0, 0.5);
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
            transition: background-color 0.3s;
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
            font-size: 2rem;
            margin-bottom: 20px;
        }

        .content {
            margin: 20px 0;
            text-align: center;
        }

        /* Kontainer gambar portofolio */
        .image-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }

        .image-container img {
            width: 150px; /* Ukuran gambar */
            height: auto; /* Otomatis menjaga rasio aspek */
            border-radius: 8px;
            cursor: pointer;
            transition: transform 0.2s;
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

        /* Style untuk Struktur Organisasi */
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

            .org-member {
                width: 150px;
            }

            .image-container img {
                width: 120px; /* Ukuran gambar lebih kecil di perangkat kecil */
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

            .image-container img {
                width: 100px; /* Ukuran gambar lebih kecil di perangkat lebih kecil */
            }
        }
    </style>
</head>

<body>

    <!-- Backsound yang otomatis terputar -->
    <audio id="backsound" autoplay loop>
        <source src="2.mp3" type="audio/mpeg">
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

    <!-- Portofolio dengan gambar yang dapat diklik -->
    <section id="portfolio">
        <h2>Portofolio</h2>
        <div class="image-container">
            <img src="2000.png" alt="Portofolio 2020" class="portfolio-image" data-year="2020">
            <img src="2001.png" alt="Portofolio 2021" class="portfolio-image" data-year="2021">
            <img src="2002.png" alt="Portofolio 2022" class="portfolio-image" data-year="2022">
        </div>
    </section>

    <!-- Modal untuk menampilkan gambar portofolio -->
    <div class="modal" id="modal-portfolio">
        <div class="modal-content">
            <span class="close">&times;</span>
            <div id="portfolio-images"></div>
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

        // Menampilkan foto dokumentasi berdasarkan gambar yang diklik
        const modal = document.getElementById("modal-portfolio");
        const portfolioImagesDiv = document.getElementById("portfolio-images");
        const closeModal = document.querySelector(".close");
        const portfolioImages = document.querySelectorAll(".portfolio-image");

        // Data gambar dokumentasi untuk setiap portofolio
        const portfolioData = {
            2020: ['2020-img1.jpg', '2020-img2.jpg', '2020-img3.jpg'],
            2021: ['2021-img1.jpg', '2021-img2.jpg', '2021-img3.jpg'],
            2022: ['2022-img1.jpg', '2022-img2.jpg', '2022-img3.jpg'],
        };

        portfolioImages.forEach(img => {
            img.addEventListener("click", function () {
                const year = this.dataset.year;
                portfolioImagesDiv.innerHTML = ''; // Kosongkan div sebelumnya
                portfolioData[year].forEach(src => {
                    const imageElement = document.createElement('img');
                    imageElement.src = src;
                    portfolioImagesDiv.appendChild(imageElement);
                });
                modal.style.display = "block"; // Tampilkan modal
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
