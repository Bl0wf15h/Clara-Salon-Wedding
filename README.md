<!DOCTYPE html>
<html lang="id">
<head>
  
  <script src="https://cdn.tailwindcss.com"></script>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Clara Salon</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&display=swap" rel="stylesheet">
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #fefdfc;
    }
    .brand-logo {
      font-family: 'Georgia', serif;
      font-size: 1.5rem;
      font-weight: bold;
      letter-spacing: 0.05em;
      color: #b89c8c;
    }
    .hero-subtitle {
      font-family: 'Playfair Display', serif;
      font-size: 1.125rem;
      font-weight: 600;
    }
    @keyframes fadeInUp {
      0% {
        opacity: 0;
        transform: translateY(20px);
      }
      100% {
        opacity: 1;
        transform: translateY(0);
      }
    }
    @keyframes zoomIn {
      0% {
        opacity: 0;
        transform: scale(1.05);
      }
      100% {
        opacity: 1;
        transform: scale(1);
      }
    }
    @keyframes fadeInOut {
      0% { opacity: 0; transform: scale(1.05); }
      10% { opacity: 1; transform: scale(1); }
      45% { opacity: 1; transform: scale(1); }
      55% { opacity: 0; transform: scale(1.05); }
      100% { opacity: 0; transform: scale(1.05); }
    }
    .fade-in-up {
      animation: fadeInUp 1s ease-out both;
    }
    .fade-in-delay-1 {
      animation-delay: 0.3s;
    }
    .fade-in-delay-2 {
      animation-delay: 0.6s;
    }
    .fade-in-delay-3 {
      animation-delay: 0.9s;
    }
    .zoom-in {
      animation: zoomIn 2s ease-out forwards;
    }
    .hero-slideshow {
      position: absolute;
      inset: 0;
      z-index: 0;
    }
    .hero-slideshow img {
      position: absolute;
      width: 100%;
      height: 100%;
      object-fit: cover;
      opacity: 0;
      animation: fadeInOut 12s infinite;
    }
    .hero-slideshow img:nth-child(1) {
      animation-delay: 0s;
    }
    .hero-slideshow img:nth-child(2) {
      animation-delay: 6s;
    }
  </style>
</head>
<body>
  <!-- Header Top -->
  <div class="bg-gray-300 text-gray-800 text-sm px-4 py-2 flex justify-between items-center text-base font-bold">
    <div>#KarenaClaraSalonPeduli</div>
    <div class="flex items-center space-x-4">
      <a href="https://instagram.com/clarasalon" target="_blank" class="flex items-center space-x-1 hover:underline">
        <img src="image/ig.png" alt="Instagram" class="w-4 h-4"><span>@claraa_salon</span>
      </a>
      <a href="https://wa.me/6285724392560" class="flex items-center space-x-1 hover:underline">
        <img src="image/whatsapp-logo-png_seeklogo-168310.png" alt="WhatsApp" class="w-4 h-4"><span>+62 812-3456-7890</span>
      </a>
    </div>
  </div>

 <!-- Navbar -->
<header class="bg-white shadow-md sticky top-0 z-50 transition duration-300 ease-in-out">
  <div class="max-w-7xl mx-auto flex justify-between items-center px-6 py-4">
    <div class="text-2xl font-bold text-[#b89c8c] tracking-wide hover:scale-105 transition-transform duration-300">
      Clara Salon & Wedding
    </div>
    <nav>
      <ul class="flex space-x-8 text-gray-700 font-semibold text-base">
        <li>
          <a href="#home" class="text-[#b89c8c] text-lg hover:underline underline-offset-8 decoration-[#b89c8c] transition duration-200">HOME</a>
        </li>
        <li>
          <a href="#layanan" class="hover:text-[#b89c8c] text-lg hover:underline underline-offset-8 transition duration-200">LAYANAN</a>
        </li>
        <li>
          <a href="#kontak" class="hover:text-[#b89c8c] text-lg hover:underline underline-offset-8 transition duration-200">KONTAK</a>
        </li>
      </ul>
    </nav>
  </div>
</header>

  <!-- Hero Section -->
  <section id="home" class="relative h-[80vh] flex items-center justify-center overflow-hidden">
    <div class="hero-slideshow">
      <img src="image/gambar hero.jpg" alt="Hero 1">
      <img src="image/hero 2.jpg" alt="Hero 2">
    </div>
    <div class="absolute inset-0 bg-black opacity-40 z-0"></div>
    <div class="relative z-10 text-center text-white px-4 max-w-2xl">
      <h1 class="text-4xl md:text-6xl font-bold mb-4 fade-in-up fade-in-delay-1">Pastikan Anda</h1>
      <div class="bg-white bg-opacity-20 inline-block px-4 py-2 rounded-full text-2xl font-bold fade-in-up fade-in-delay-2">
        MERASAKAN <span class="bg-[#b89c8c] text-white px-3 py-1 rounded">LAYANAN TERBAIK KAMI</span>
      </div>
      <p class="mt-4 hero-subtitle fade-in-up fade-in-delay-3" style="font-family: 'Segoe UI', sans-serif; font-size: 0.95rem;">TEMUKAN KECANTIKAN TERBAIK MU DI CLARA SALON</p>
    </div>
  </section>


<!-- Layanan Section dengan Background Gambar -->
<section id="layanan" class="relative py-20 px-4 bg-cover bg-center bg-no-repeat" style="background-image: url('image/bg.jpg');">
  <!-- Overlay gelap supaya teks/konten tetap terbaca -->
  <div class="absolute inset-0 bg-black bg-opacity-50"></div>

  <!-- Konten -->
  <div class="relative max-w-7xl mx-auto">
    <!-- Highlight Judul Layanan Kami -->
<div class="flex flex-col items-center justify-center mb-14">
  <div class="relative">
    <h2 class="text-5xl font-bold text-transparent bg-clip-text bg-gradient-to-r from-[#b89c8c] to-[#d4b9a7] tracking-wide">
    Layanan Kami 
    </h2>
    <!-- underline animasi -->
    <div class="absolute left-1/2 transform -translate-x-1/2 mt-2 h-1 w-20 bg-[#b89c8c] rounded-full animate-pulse"></div>
  </div>
 <p class="mt-4 text-center max-w-xl text-lg font-medium text-[#f7f2ee] italic tracking-wide animate-fade-in">
  Temukan berbagai layanan <span class="text-[#fcd8ba] font-semibold">Kecantikan</span> dari <span class="text-[#ffd9c0] font-bold">Clara Salon</span> untuk merawat dan mempercantik diri Anda.
</p>
</div>

    <div class="grid md:grid-cols-3 gap-10">

      <!-- Kartu layanan tetap sama -->
      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Haircut" data-deskripsi="Potong rambut dengan gaya terbaru dari stylist profesional kami." data-harga="Rp 25.000">
        <img src="image/Haircut.jpg" class="w-full h-64 object-cover" alt="Haircut">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Haircut</h3>
          <p class="text-gray-700">Rp 25.000</p>
        </div>
      </div>

      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Hair Coloring" data-deskripsi="Ubah warna rambut Anda dengan pilihan warna trendi dan aman." data-harga="Rp 30.000">
        <img src="image/hair color.jpg" class="w-full h-64 object-cover" alt="Hair Coloring">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Hair Coloring</h3>
          <p class="text-gray-700">Rp 30.000</p>
        </div>
      </div>

      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Creambath" data-deskripsi="Perawatan rambut dan kulit kepala untuk kesehatan dan relaksasi maksimal." data-harga="Rp 50.000">
        <img src="image/crambath.jpg" class="w-full h-64 object-cover" alt="Creambath">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Creambath</h3>
          <p class="text-gray-700">Rp 50.000</p>
        </div>
      </div>

      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Cuci & Catok" data-deskripsi="Layanan cuci rambut dan styling dengan catokan untuk tampilan sempurna." data-harga="Rp 30.000">
        <img src="image/cuci catok.jpg" class="w-full h-64 object-cover" alt="Cuci & Catok">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Cuci & Catok</h3>
          <p class="text-gray-700">Rp 30.000</p>
        </div>
      </div>

      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Keriting Rambut" data-deskripsi="Styling rambut keriting tahan lama yang cocok untuk berbagai acara." data-harga="Rp 100.000">
        <img src="image/keriting.jpg" class="w-full h-64 object-cover" alt="Keriting Rambut">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Keriting Rambut</h3>
          <p class="text-gray-700">Rp 100.000</p>
        </div>
      </div>

      <div class="layanan-item shadow-xl rounded-xl overflow-hidden transform hover:scale-105 transition-transform duration-300 bg-white cursor-pointer"
           data-judul="Makeup" data-deskripsi="Makeup profesional untuk berbagai kebutuhan, dari sehari-hari hingga acara spesial." data-harga="Rp 150.000">
        <img src="image/makeup.jpg" class="w-full h-64 object-cover" alt="Makeup">
        <div class="p-5">
          <h3 class="text-xl font-bold text-[#b89c8c] mb-2">Makeup</h3>
          <p class="text-gray-700">Rp 150.000</p>
        </div>
      </div>

    </div>
  </div>
</section>



<!-- Modal Popup -->
<div id="modal" class="fixed inset-0 bg-black bg-opacity-50 z-50 hidden items-center justify-center">
  <div id="modalContent" class="bg-white rounded-xl p-8 max-w-md w-full transform scale-95 opacity-0 transition duration-300 relative shadow-2xl">
    <button onclick="closeModal()" class="absolute top-3 right-4 text-gray-500 text-2xl hover:text-gray-800">&times;</button>
    <h3 id="modalJudul" class="text-2xl font-bold text-[#b89c8c] mb-3"></h3>
    <p id="modalDeskripsi" class="text-gray-700 mb-2"></p>
    <p id="modalHarga" class="text-lg font-semibold mb-6"></p>
    <a id="bookingLink" target="_blank" class="block text-center bg-[#b89c8c] hover:bg-[#a58878] text-white font-bold py-2 rounded-full transition">
      Booking Sekarang
    </a>
  </div>
</div>

<script>
  const modal = document.getElementById('modal');
  const modalContent = document.getElementById('modalContent');

  document.querySelectorAll('.layanan-item').forEach(item => {
    item.addEventListener('click', () => {
      document.getElementById('modalJudul').textContent = item.dataset.judul;
      document.getElementById('modalDeskripsi').textContent = item.dataset.deskripsi;
      document.getElementById('modalHarga').textContent = item.dataset.harga;

      const waMessage = `Halo Clara Salon, saya ingin booking layanan *${item.dataset.judul}* seharga ${item.dataset.harga}.

    Nama : 
    Hari/Tanggal Booking :
    Jam Booking :

    Kira kira bisa ngga ya?`;
      document.getElementById('bookingLink').href = `https://wa.me/6285724392560?text=${encodeURIComponent(waMessage)}`;

      // Tampilkan modal dan aktifkan flex
      modal.classList.remove('hidden');
      modal.classList.add('flex');

      // Efek muncul modalContent
      setTimeout(() => {
        modalContent.classList.remove('scale-95', 'opacity-0');
        modalContent.classList.add('scale-100', 'opacity-100');
      }, 10);
    });
  });

  function closeModal() {
    // Tutup efek modalContent
    modalContent.classList.remove('scale-100', 'opacity-100');
    modalContent.classList.add('scale-95', 'opacity-0');

    // Setelah animasi, sembunyikan modal
    setTimeout(() => {
      modal.classList.remove('flex');
      modal.classList.add('hidden');
    }, 200);
  }

  // Tutup modal jika klik di luar kontennya
  modal.addEventListener('click', (e) => {
    if (e.target === modal) closeModal();
  });
</script>

  <!-- Kontak Section -->
  <section id="kontak" class="py-16 bg-white">
    <div class="max-w-4xl mx-auto px-4">
      <h2 class="text-3xl font-semibold text-center mb-8 text-gray-800">Hubungi Kami</h2>
      <div class="grid md:grid-cols-2 gap-8 text-gray-700">
        <div>
          <p class="mb-2"><strong>WhatsApp:</strong> <a href="https://wa.me/6285724392560" class="text-[#b89c8c] hover:underline">+62 812-3456-7890</a></p>
          <p class="mb-2"><strong>Instagram:</strong> <a href="https://instagram.com/claraa_salon" target="_blank" class="text-[#b89c8c] hover:underline">@claraa_salon</a></p>
          <p class="mb-2"><strong>Alamat:</strong> Jl. Gereja, Cisantana, Kec. Cigugur, Kabupaten Kuningan, Jawa Barat</p>
          <p class="mb-2"><strong>Jam Operasional:</strong><br>
            Senin - Minggu: 10.00 - 21.00 WIB<br>
            
          </p>
        </div>
        <div>
          <iframe class="w-full h-64 border" src="image/maps.jpg" allowfullscreen="" loading="lazy"></iframe>
        </div>
      </div>
    </div>
  </section>


 <!-- Footer -->
<footer class="text-center bg-[#b89c8c] text-white py-4 mt-16">
  &copy; 2025 Clara Salon. All rights reserved.
</footer>

</body>
</html>
