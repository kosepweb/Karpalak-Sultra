
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pencinta Alam</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f0f0f5;
            color: #333;
            line-height: 1.6;
        }
        header {
            background: #1E1E2F;
            color: white;
            padding: 20px 0;
            text-align: center;
        }
        header h1 {
            margin: 0;
            font-size: 2.5em;
        }
        nav {
            margin: 20px 0;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: white;
            font-weight: 700;
        }
        nav a:hover {
            color: #FFD700;
        }
        .container {
            max-width: 900px;
            margin: 20px auto;
            padding: 20px;
            background: white;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        h2 {
            color: #1E1E2F;
            margin-bottom: 10px;
        }
        img {
            max-width: 100%;
            border-radius: 8px;
            margin-bottom: 20px;
        }
        ul {
            padding-left: 20px;
        }
        .footer {
            text-align: center;
            margin: 20px 0;
            padding: 15px;
            background: #1E1E2F;
            color: white;
            border-radius: 5px;
        }
        /* Modal Styles */
        .modal {
            display: none;
            position: fixed;
            z-index: 1;
            left: 0;
            top: 0;
            width: 100%;
            height: 100%;
            overflow: auto;
            background-color: rgba(0, 0, 0, 0.8);
            padding-top: 60px;
        }
        .modal-content {
            background-color: #fefefe;
            margin: 5% auto;
            padding: 20px;
            border: 1px solid #888;
            width: 80%;
            max-width: 700px;
        }
        .close {
            color: #aaa;
            float: right;
            font-size: 28px;
            font-weight: bold;
        }
        .close:hover, .close:focus {
            color: black;
            text-decoration: none;
            cursor: pointer;
        }
    </style>
</head>
<body>

<audio id="background-music" loop autoplay>
    <source src="https://youtu.be/fgDPSM6oPsc?si=zf8wqQVSqTahoSlH" type="audio/mpeg">
    Your browser does not support the audio tag.
</audio>

<header>
    <h1>Pencinta Alam</h1>
    <nav>
        <a href="#about">Tentang Kami</a>
        <a href="#visi">Visi</a>
        <a href="#misi">Misi</a>
        <a href="#layanan">Layanan</a>
        <a href="#portofolio">Portofolio</a>
        <a href="#kontak">Kontak</a>
    </nav>
</header>

<div class="container" id="about">
    <h2>Tentang Kami</h2>
    <p>Pencinta Alam adalah organisasi yang didirikan untuk mempromosikan kesadaran dan kepedulian terhadap lingkungan. Kami percaya bahwa setiap individu memiliki peran dalam menjaga keanekaragaman hayati dan kelestarian alam.</p>
</div>

<div class="container" id="visi">
    <h2>Visi</h2>
    <img src="https://source.unsplash.com/800x400/?nature&format=jpg" alt="Visi Pencinta Alam">
    <p>Menjadi pelopor dalam pelestarian lingkungan dan edukasi tentang alam, serta membangun kesadaran masyarakat akan pentingnya menjaga ekosistem.</p>
</div>

<div class="container" id="misi">
    <h2>Misi</h2>
    <img src="https://source.unsplash.com/800x400/?conservation&format=jpg" alt="Misi Pencinta Alam">
    <ul>
        <li>Mengadakan program edukasi dan pelatihan tentang konservasi lingkungan.</li>
        <li>Melakukan aksi bersih-bersih dan reboisasi di berbagai lokasi.</li>
        <li>Mendorong partisipasi masyarakat dalam kegiatan pelestarian alam.</li>
        <li>Menjalin kemitraan dengan organisasi lingkungan dan pemerintah untuk mendukung proyek konservasi.</li>
    </ul>
</div>

<div class="container" id="layanan">
    <h2>Layanan</h2>
    <img src="https://source.unsplash.com/800x400/?ecotourism&format=jpg" alt="Layanan Pencinta Alam">
    <ul>
        <li><strong>Edukasi Lingkungan:</strong> Workshop, seminar, dan kegiatan lapangan.</li>
        <li><strong>Aksi Konservasi:</strong> Program penanaman pohon, pembersihan pantai, dan perlindungan satwa liar.</li>
        <li><strong>Kegiatan Ekowisata:</strong> Paket wisata ramah lingkungan.</li>
        <li><strong>Kampanye Kesadaran:</strong> Penyebaran informasi melalui media sosial dan acara komunitas.</li>
    </ul>
</div>

<div class="container" id="portofolio">
    <h2>Portofolio</h2>
    <div class="year-list">
        <div class="year-item" onclick="showModal('2021')" style="cursor: pointer; color: #1E1E2F; margin-bottom: 10px;">2021</div>
        <div class="year-item" onclick="showModal('2022')" style="cursor: pointer; color: #1E1E2F; margin-bottom: 10px;">2022</div>
        <div class="year-item" onclick="showModal('2023')" style="cursor: pointer; color: #1E1E2F; margin-bottom: 10px;">2023</div>
    </div>
</div>

<div class="container" id="kontak">
    <h2>Kontak</h2>
    <img src="https://source.unsplash.com/800x400/?contact&format=jpg" alt="Kontak Pencinta Alam">
    <p>
        <strong>Alamat:</strong> [Masukkan alamat kantor pusat]<br>
        <strong>Telepon:</strong> [Masukkan nomor telepon]<br>
        <strong>Email:</strong> [Masukkan alamat email]<br>
        <strong>Website:</strong> [Masukkan URL website]<br>
    </p>
</div>

<div class="footer">
    <p>&copy; 2024 Pencinta Alam. Semua hak dilindungi.</p>
</div>

<!-- Pop-up Modal -->
<div id="myModal" class="modal">
    <div class="modal-content">
        <span class="close" onclick="closeModal()">&times;</span>
        <h2 id="modal-title">Dokumentasi Kegiatan</h2>
        <div id="modal-body"></div>
    </div>
</div>

<script>
    const documentation = {
        '2021': [
            'https://source.unsplash.com/400x300/?forest&format=jpg',
            'https://source.unsplash.com/400x300/?community&format=jpg'
        ],
        '2022': [
            'https://source.unsplash.com/400x300/?beach&format=jpg',
            'https://source.unsplash.com/400x300/?planting&format=jpg'
        ],
        '2023': [
            'https://source.unsplash.com/400x300/?wildlife&format=jpg',
            'https://source.unsplash.com/400x300/?cleaning&format=jpg'
        ]
    };

    function showModal(year) {
        const modal = document.getElementById('myModal');
        const modalBody = document.getElementById('modal-body');
        modalBody.innerHTML = '';
        documentation[year].forEach(url => {
            const img = document.createElement('img');
            img.src = url;
            img.style.width = '100%';
            img.style.marginBottom = '10px';
            modalBody.appendChild(img);
        });
        document.getElementById('modal-title').innerText = `Dokumentasi Kegiatan ${year}`;
        modal.style.display = 'block';
    }

    function closeModal() {
        document.getElementById('myModal').style.display = 'none';
    }

    window.onclick = function(event) {
        const modal = document.getElementById('myModal');
        if (event.target == modal) {
            modal.style.display = 'none';
        }
    }
</script>

</body>
</html>
