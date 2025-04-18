<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Profil Sekolah - SMKN 4 Kota Bengkulu</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Segoe UI', sans-serif;
    }

    body {
      background: #f0f0f0;
    }

    header {
      background: #00ccff;
      color: white;
      padding: 20px;
      display: flex;
      align-items: center;
      justify-content: space-between;
      flex-wrap: wrap;
    }

    .logo {
      display: flex;
      align-items: center;
      font-size: 24px;
      font-weight: bold;
    }

    .logo-img {
      width: 40px;
      height: 40px;
      margin-right: 10px;
      object-fit: cover;
    }

    nav {
      margin-top: 10px;
    }

    nav a {
      color: white;
      text-decoration: none;
      margin: 0 10px;
      font-weight: bold;
      transition: color 0.3s ease;
    }

    nav a:hover {
      color: #ffcc00;
    }

    main {
      padding: 40px 20px;
      background: white;
      animation: fade 0.5s ease-in;
    }

    @keyframes fade {
      from {opacity: 0;}
      to {opacity: 1;}
    }

    footer {
      background: #222;
      color: white;
      text-align: center;
      padding: 15px 0;
      margin-top: 20px;
    }

    .section {
      display: none;
      animation: fade 0.5s ease-in;
    }

    .section.active {
      display: block;
    }

    h1 {
      margin-bottom: 20px;
      color: #004080;
    }

    .gallery {
      display: flex;
      flex-wrap: wrap;
      gap: 10px;
    }

    .gallery img {
      width: 100%;
      max-width: 200px;
      border-radius: 10px;
    }

    form {
      max-width: 500px;
      margin-top: 20px;
    }

    input, textarea {
      width: 100%;
      padding: 10px;
      margin-bottom: 15px;
      border: 1px solid #ccc;
      border-radius: 5px;
    }

    input[type="submit"] {
      background-color: #004080;
      color: white;
      border: none;
      cursor: pointer;
    }

    input[type="submit"]:hover {
      background-color: #003366;
    }

    .map {
      margin-top: 20px;
    }

    iframe {
      width: 100%;
      height: 300px;
      border: none;
    }

    ul {
      margin-left: 20px;
      margin-bottom: 20px;
    }

    ul li {
      margin-bottom: 8px;
    }

    /* Responsif */
    @media (max-width: 768px) {
      header {
        flex-direction: column;
        align-items: flex-start;
      }

      .logo {
        margin-bottom: 10px;
      }

      .gallery {
        justify-content: center;
      }

      nav a {
        display: inline-block;
        margin: 5px 5px;
      }
    }
  </style>
</head>
<body>

  <header>
    <div class="logo">
      <img src="images-removebg-preview.png" alt="Logo Sekolah" class="logo-img" />
      <span>SMKN 4 Kota Bengkulu</span>
    </div>
    <nav>
      <a href="#" onclick="navigate('home')">Home</a>
      <a href="#" onclick="navigate('about')">About</a>
      <a href="#" onclick="navigate('gallery')">Gallery</a>
      <a href="#" onclick="navigate('contact')">Contact</a>
    </nav>
  </header>

  <main>
    <section id="home" class="section active">
      <h1>Selamat Datang di SMKN 4 Kota Bengkulu</h1>
      <p>SMKN 4 Kota Bengkulu adalah sekolah kejuruan unggulan yang berkomitmen mencetak lulusan yang kompeten, mandiri, dan siap kerja.</p>

      <h2>Visi & Misi</h2>
      <p><strong>Visi:</strong> Menjadi sekolah kejuruan unggulan berbasis teknologi dan karakter.</p>
      <p><strong>Misi:</strong></p>
      <ul>
        <li>Menyelenggarakan pendidikan berbasis kompetensi dan industri.</li>
        <li>Mengembangkan karakter dan etika kerja profesional.</li>
        <li>Mendorong inovasi dan kreatifitas siswa dalam teknologi.</li>
      </ul>

      <h2>Program Keahlian</h2>
      <ul>
        <li>Teknik Kendaraan Ringan (TKR)</li>
        <li>pelayaran</li>
        <li>🎨 Desain Komunikasi Visual / Multimedia</li>
        <li>💻 Rekayasa Perangkat Lunak (RPL)</li>
      </ul>

      <h2>Fasilitas Unggulan</h2>
      <ul>
        <li>💡 Laboratorium Komputer</li>
        <li>🏀 Lapangan Olahraga</li>
        <li>📚 Perpustakaan</li>
        <li>🌐 Internet Cepat & Wi-Fi</li>
      </ul>

      <h2>Statistik Sekolah</h2>
      <ul>
        <li>👨‍🎓 <strong>1.200+</strong> Siswa aktif</li>
        <li>👩‍🏫 <strong>80+</strong> Guru & Staff</li>
        <li>🎓 <strong>5.000+</strong> Alumni sukses</li>
      </ul>
    </section>

    <section id="about" class="section">
      <h1>Tentang Kami</h1>
      <p>SMKN 4 Kota Bengkulu berdiri sejak 2005, memiliki program keahlian unggulan seperti TKJ, Akuntansi, dan Multimedia. Kami membekali siswa dengan kurikulum berbasis industri dan praktik kerja lapangan.</p>
    </section>

    <section id="gallery" class="section">
      <h1>Galeri</h1>
      <div class="gallery">
        <img src="images.jpeg" alt="Kegiatan 1" />
        <img src="images (1).jpeg" alt="Upacara" />
        <img src="images (2).jpeg" alt="Kegiatan 3" />
        <img src="images (3).jpeg" alt="Kegiatan 4" />
      </div>
    </section>

    <section id="contact" class="section">
      <h1>Kontak Kami</h1>
      <form>
        <input type="text" placeholder="Nama Anda" required />
        <input type="email" placeholder="Email" required />
        <textarea rows="5" placeholder="Pesan Anda..." required></textarea>
        <input type="submit" value="Kirim" />
      </form>
      <div class="map">
        <iframe 
          src="https://www.google.com/maps/place/SMK+Negeri+4+Kota+Bengkulu/@-3.779158,102.2617122,17z/data=!3m1!4b1!4m6!3m5!1s0x2e36b02daf9ceb19:0xce912ab89fcfd3c7!8m2!3d-3.7791634!4d102.2642871!16s%2Fg%2F1pzr0n7fh?hl=ID" 
          allowfullscreen="" loading="lazy">
        </iframe>
      </div>
    </section>
  </main>

  <footer>
    &copy; 2025 SMKN 4 Kota Bengkulu. All rights reserved.
  </footer>

  <script>
    function navigate(sectionId) {
      const sections = document.querySelectorAll(".section");
      sections.forEach(section => section.classList.remove("active"));
      document.getElementById(sectionId).classList.add("active");
      window.scrollTo({ top: 0, behavior: 'smooth' });
    }
  </script>

</body>
</html>
