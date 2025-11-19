
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Donat Kentato - Kelompok 9</title>
    
    <!-- Memuat Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Memuat Ikon (Font Awesome) -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
    
    <!-- Memuat Font (Inter) -->
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;700;800&display=swap');
        body {
            font-family: 'Inter', sans-serif;
        }
    </style>
    
    <!-- Konfigurasi Custom Tailwind -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        'brand-orange': {
                            50: '#fff7ed',  // Sangat pastel
                            100: '#ffedd5', // Pastel
                            200: '#fed7aa',
                            300: '#fdba74',
                            400: '#fb923c',
                            500: '#f97316', // Utama
                            600: '#ea580c', // Gelap
                            700: '#c2410c', // Sangat gelap
                            800: '#9a3412',
                            900: '#7c2d12',
                        },
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-brand-orange-50 text-gray-800">

    <!-- ===== HEADER / NAVBAR ===== -->
    <header class="bg-white sticky top-0 z-50 shadow-md">
        <nav class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 flex justify-between items-center h-20">
            <!-- Logo/Brand -->
            <a href="#beranda" class="text-3xl font-extrabold text-brand-orange-600">
                Donat Kentato
            </a>
            
            <!-- Navigasi (Desktop) -->
            <div class="hidden md:flex space-x-6 items-center">
                <a href="#beranda" class="text-gray-600 hover:text-brand-orange-500 font-medium transition duration-300">Beranda</a>
                <a href="#varian" class="text-gray-600 hover:text-brand-orange-500 font-medium transition duration-300">Varian</a>
                <a href="#kenapa" class="text-gray-600 hover:text-brand-orange-500 font-medium transition duration-300">Kenapa Kami</a>
                <a href="#pesan" class="text-gray-600 hover:text-brand-orange-500 font-medium transition duration-300">Pesan</a>
                <a href="#tentang" class="text-gray-600 hover:text-brand-orange-500 font-medium transition duration-300">Tentang Kami</a>
            </div>
            
            <!-- Ikon Keranjang -->
            <button id="cart-icon" class="relative text-2xl text-gray-700 hover:text-brand-orange-500 transition duration-300" aria-label="Buka Keranjang Belanja">
                <i class="fa-solid fa-shopping-cart"></i>
                <!-- Badge (penanda jumlah) -->
                <span id="cart-badge" class="absolute -top-2 -right-3 bg-red-600 text-white text-xs font-bold rounded-full h-5 w-5 flex items-center justify-center hidden">
                    0
                </span>
            </button>
        </nav>
    </header>

    <!-- ===== MAIN CONTENT ===== -->
    <main>

        <!-- ===== 1. BERANDA / HERO ===== -->
        <section id="beranda" class="bg-gradient-to-b from-orange-100 to-brand-orange-50 pt-20 pb-24">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 grid md:grid-cols-2 gap-12 items-center">
                <!-- Teks Hero -->
                <div class="text-center md:text-left">
                    <h1 class="text-4xl md:text-6xl font-extrabold text-brand-orange-700 leading-tight">
                        Rasa Lembut, Harga Bersahabat!
                    </h1>
                    <p class="mt-6 text-lg text-gray-600 max-w-lg mx-auto md:mx-0">
                        Nikmati kelembutan donat kentang premium yang empuk dan lumer di mulut. Dibuat setiap hari dengan bahan pilihan terbaik.
                    </p>
                    <p class="mt-4 text-3xl font-bold text-brand-orange-600">
                        Hanya Rp 5.000,- / buah
                    </p>
                    <div class="mt-8">
                        <a href="#pesan" class="bg-brand-orange-600 text-white font-bold py-3 px-8 rounded-full text-lg shadow-lg hover:bg-brand-orange-700 transition duration-300 transform hover:scale-105 inline-block">
                            Pesan Sekarang
                        </a>
                    </div>
                </div>
                
                <!-- Gambar Hero (Placeholder Emoji) -->
                <div class="flex items-center justify-center">
                    <span class="text-[12rem] md:text-[16rem] drop-shadow-xl" style="transform: rotate(-15deg);">🍩</span>
                </div>
            </div>
            <!-- Info Kelompok -->
            <div class="text-center mt-16 text-gray-500">
                <p class="text-xl font-bold">12 H</p>
                <p class="mt-1">oleh <span class="font-semibold text-gray-600">Kelompok 9</span></p>
                <p class="text-sm">(Ghizzelya, Fasya dan Nadila)</p>
            </div>
        </section>

        <!-- ===== 2. PILIHAN VARIAN ===== -->
        <section id="varian" class="py-20">
            <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-brand-orange-800 mb-12">
                    Pilihan Varian Donat Kentato
                </h2>
                <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                    
                    <!-- Varian 1: Gula Halus -->
                    <div class="bg-white rounded-2xl shadow-lg overflow-hidden flex flex-col items-center p-8 transition duration-300 hover:shadow-xl hover:scale-105">
                        <img src="https://dekopin.or.id/wp-content/uploads/2024/11/032875800_1604118231-shutterstock_1729999204.webp" alt="Donat Gula Halus" class="w-48 h-48 object-cover rounded-full mb-6 shadow-md">
                        <h3 class="text-2xl font-bold text-gray-800 mb-2">Donat Gula Halus</h3>
                        <p class="text-gray-600 text-center mb-4">
                            Donat klasik dengan taburan gula halus, lembut dan manisnya pas.
                        </p>
                        <span class="text-xl font-bold text-brand-orange-600">Rp 5.000</span>
                    </div>
                    
                    <!-- Varian 2: Coklat -->
                    <div class="bg-white rounded-2xl shadow-lg overflow-hidden flex flex-col items-center p-8 transition duration-300 hover:shadow-xl hover:scale-105">
                        <img src="https://media.istockphoto.com/id/182420116/id/foto/donat-berlapis-cokelat.jpg?s=612x612&w=0&k=20&c=-mcWr0atVmmMPR58gIng7m1T-wHgXIOCgDAvmRvbf-Q=" alt="Donat Topping Coklat" class="w-48 h-48 object-cover rounded-full mb-6 shadow-md">
                        <h3 class="text-2xl font-bold text-gray-800 mb-2">Donat Topping Coklat</h3>
                        <p class="text-gray-600 text-center mb-4">
                            Donat fluffy dengan lelehan coklat premium di atasnya.
                        </p>
                        <span class="text-xl font-bold text-brand-orange-600">Rp 5.000</span>
                    </div>
                    
                    <!-- Varian 3: Strawberry -->
                    <div class="bg-white rounded-2xl shadow-lg overflow-hidden flex flex-col items-center p-8 transition duration-300 hover:shadow-xl hover:scale-105">
                        <img src="https://hypeabis.id/assets/content/20230716061419000000Bomboloni.jpg" alt="Donat Topping Strawbery" class="w-48 h-48 object-cover rounded-full mb-6 shadow-md">
                        <h3 class="text-2xl font-bold text-gray-800 mb-2">Donat Topping Strawbery</h3>
                        <p class="text-gray-600 text-center mb-4">
                            Donat dengan lelehan slai strawbery yang segar dan manis.
                        </p>
                        <span class="text-xl font-bold text-brand-orange-600">Rp 5.000</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- ===== 3. ALASAN KENAPA HARUS COBA ===== -->
        <section id="kenapa" class="py-20 bg-orange-100">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-brand-orange-800 mb-12">
                    Kenapa Harus Coba Kentato?
                </h2>
                <div class="space-y-6">
                    <div class="bg-white p-6 rounded-xl shadow-lg flex items-start space-x-4">
                        <span class="text-3xl text-brand-orange-500 pt-1">🎉</span>
                        <div>
                            <h3 class="text-xl font-semibold">Cocok untuk Semua Situasi</h3>
                            <p class="text-gray-600">Ngemil saat istirahat, bareng teman, atau oleh-oleh? Donat Kentato selalu jadi pilihan yang tepat!</p>
                        </div>
                    </div>
                    <div class="bg-white p-6 rounded-xl shadow-lg flex items-start space-x-4">
                        <span class="text-3xl text-brand-orange-500 pt-1">💖</span>
                        <div>
                            <h3 class="text-xl font-semibold">Empuk, Manis, & Terjangkau</h3>
                            <p class="text-gray-600">Cita rasa empuk dan manisnya pas, dengan harga ramah di kantong. Kualitas premium, harga minimum.</p>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- ===== 4. FORMULIR PEMESANAN ===== -->
        <section id="pesan" class="py-20">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8">
                <h2 class="text-3xl font-bold text-center text-brand-orange-800 mb-4">
                    Formulir Pemesanan
                </h2>
                <p class="text-center text-gray-600 mb-10">
                    Isi data di bawah ini, lalu klik "Tambah ke Pesanan". Pesananmu akan muncul saat kamu klik ikon keranjang di atas.
                </p>
                
                <form id="order-form" class="bg-white p-8 rounded-2xl shadow-xl space-y-6">
                    <!-- Info Pemesan -->
                    <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                        <div>
                            <label for="nama" class="block text-sm font-medium text-gray-700">Nama Lengkap</label>
                            <input type="text" id="nama" name="nama" class="mt-1 block w-full rounded-lg border-gray-300 shadow-sm focus:border-brand-orange-500 focus:ring-brand-orange-500" placeholder="cth: Fasya" required>
                        </div>
                        <div>
                            <label for="kelas" class="block text-sm font-medium text-gray-700">Kelas</label>
                            <input type="text" id="kelas" name="kelas" class="mt-1 block w-full rounded-lg border-gray-300 shadow-sm focus:border-brand-orange-500 focus:ring-brand-orange-500" placeholder="cth: 12 H" required>
                        </div>
                    </div>
                    
                    <hr class="border-gray-200">
                    
                    <!-- Pilihan Jumlah Donat -->
                    <h3 class="text-lg font-semibold text-gray-800 pt-2">Jumlah Pemesanan</h3>
                    <div class="space-y-4">
                        <!-- Item 1 -->
                        <div class="flex justify-between items-center">
                            <label for="qty-gula" class="text-gray-700">🍩 Donat Gula Halus</label>
                            <input type="number" id="qty-gula" name="qty-gula" min="0" value="0" class="w-20 rounded-lg border-gray-300 text-center shadow-sm focus:border-brand-orange-500 focus:ring-brand-orange-500">
                        </div>
                        <!-- Item 2 -->
                        <div class="flex justify-between items-center">
                            <label for="qty-coklat" class="text-gray-700">🍫 Donat Topping Coklat</label>
                            <input type="number" id="qty-coklat" name="qty-coklat" min="0" value="0" class="w-20 rounded-lg border-gray-300 text-center shadow-sm focus:border-brand-orange-500 focus:ring-brand-orange-500">
                        </div>
                        <!-- Item 3 -->
                        <div class="flex justify-between items-center">
                            <label for="qty-strawbery" class="text-gray-700">✨ Donat Topping Strawbery</label>
                            <input type="number" id="qty-strawbery" name="qty-strawbery" min="0" value="0" class="w-20 rounded-lg border-gray-300 text-center shadow-sm focus:border-brand-orange-500 focus:ring-brand-orange-500">
                        </div>
                    </div>
                    
                    <hr class="border-gray-200">
                    
                    <!-- Total -->
                    <div class="flex justify-between items-center pt-2">
                        <span class="text-xl font-bold text-gray-800">Total Harga:</span>
                        <span id="total-price" class="text-2xl font-extrabold text-brand-orange-600">Rp 0</span>
                    </div>
                    
                    <!-- Tombol Submit -->
                    <button type="submit" class="w-full bg-brand-orange-600 text-white font-bold py-3 px-8 rounded-full text-lg shadow-lg hover:bg-brand-orange-700 transition duration-300 transform hover:scale-105">
                        <i class="fa-solid fa-cart-plus mr-2"></i> Tambah ke Pesanan
                    </button>
                    
                    <!-- Pesan Konfirmasi -->
                    <p id="confirm-message" class="text-center text-green-600 font-semibold hidden">
                        Pesanan berhasil ditambahkan! Klik keranjang di kanan atas 🛒
                    </p>
                </form>
            </div>
        </section>

        <!-- ===== 5. TENTANG KAMI ===== -->
        <section id="tentang" class="py-20 bg-orange-100">
            <div class="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
                <h2 class="text-3xl font-bold text-brand-orange-800 mb-6">
                    Tentang Kami
                </h2>
                <p class="text-xl font-bold text-gray-700">Donat Kentato - 12 H</p>
                <p class="mt-4 text-lg text-gray-600">
                    Produk ini dibuat dengan penuh cinta oleh <span class="font-semibold">Kelompok 9</span>.
                </p>
                <p class="mt-2 text-gray-600 text-lg">
                    Ghizzelya • Fasya • Nadila
                </p>
            </div>
        </section>
    </main>
    
    <!-- ===== FOOTER ===== -->
    <footer class="bg-brand-orange-800 text-orange-100 py-6">
        <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 text-center">
            <p>© 2025 Donat Kentato - Hak Cipta oleh Kelompok 9</p>
        </div>
    </footer>

    <!-- ===== FLOATING WHATSAPP BUTTON ===== -->
    <a href="https://wa.me/6285773688582" target="_blank" rel="noopener noreferrer" class="fixed bottom-6 right-6 bg-green-500 text-white w-14 h-14 rounded-full flex items-center justify-center shadow-xl text-3xl hover:bg-green-600 transition duration-300 transform hover:scale-110" aria-label="Chat via WhatsApp">
        <i class="fab fa-whatsapp"></i>
    </a>

    <!-- ===== MODAL KERANJANG (CART) ===== -->
    <div id="cart-modal" class="fixed inset-0 bg-black bg-opacity-60 flex items-center justify-center z-[100] p-4 hidden" role="dialog" aria-modal="true">
        <div class="bg-white rounded-2xl shadow-2xl w-full max-w-md p-6 md:p-8">
            <!-- Header Modal -->
            <div class="flex justify-between items-center mb-6">
                <h3 class="text-2xl font-bold text-brand-orange-800">Detail Pesanan Anda</h3>
                <button id="close-modal-btn" class="text-3xl text-gray-400 hover:text-gray-600" aria-label="Tutup">&times;</button>
            </div>
            
            <!-- Konten Modal (diisi oleh JS) -->
            <div id="modal-order-summary" class="space-y-4">
                <p class="text-gray-600 text-center">Keranjang masih kosong. Silakan isi formulir pemesanan terlebih dahulu.</p>
            </div>
            
            <hr class="my-6 border-gray-200">
            
            <!-- Opsi Pembayaran -->
            <h4 class="text-xl font-semibold text-gray-800 mb-4">Opsi Pembayaran & Konfirmasi</h4>
            <div class="space-y-4">
                <p class="text-sm text-gray-500">
                    Silakan konfirmasi pesanan Anda melalui WhatsApp, lalu lakukan pembayaran.
                </D>
                
                <!-- Tombol WA (disabled by default) -->
                <a id="whatsapp-checkout-btn" href="#" target="_blank" class="block w-full text-center bg-green-500 text-white font-bold py-3 px-6 rounded-full text-lg shadow-lg hover:bg-green-600 transition duration-300 opacity-50 cursor-not-allowed">
                    <i class="fab fa-whatsapp"></i> Konfirmasi via WhatsApp
                </a>
                
                <!-- Tombol DANA -->
                <a id="dana-checkout-btn" href="https://link.dana.id/minta?full_url=https://qr.dana.id/v1/281012012025100250261187" target="_blank" rel="noopener noreferrer" class="block w-full text-center bg-blue-500 text-white font-bold py-3 px-6 rounded-full text-lg shadow-lg hover:bg-blue-600 transition duration-300 opacity-50 cursor-not-allowed">
                    Bayar via DANA (QR)
                </a>
                
                <p class="text-center text-sm text-gray-600">Atau transfer DANA ke: <strong class="text-gray-800">088975129776</strong></p>
                
                <!-- Placeholder QRIS -->
                <div class="bg-gray-100 p-4 rounded-lg text-center">
                    <p class="font-semibold">Scan QRIS DANA</p>
                    <p class="text-sm text-gray-500">(Gunakan tombol "Bayar via DANA" di atas untuk QR otomatis)</p>
                    <!-- Anda bisa meletakkan <img> QRIS di sini jika punya URL-nya -->
                    <!-- <img src="URL_QRIS_ANDA.jpg" alt="QRIS Pembayaran" class="mx-auto mt-2"> -->
                </div>
            </div>
        </div>
    </div>

    <!-- ===== JAVASCRIPT ===== -->
    <script>
        document.addEventListener('DOMContentLoaded', () => {
            // --- Elemen Form ---
            const orderForm = document.getElementById('order-form');
            const namaInput = document.getElementById('nama');
            const kelasInput = document.getElementById('kelas');
            const qtyGula = document.getElementById('qty-gula');
            const qtyCoklat = document.getElementById('qty-coklat');
            const qtyStrawbery = document.getElementById('qty-strawbery');
            const totalPriceEl = document.getElementById('total-price');
            const confirmMessage = document.getElementById('confirm-message');
            
            // --- Elemen Keranjang & Modal ---
            const cartIcon = document.getElementById('cart-icon');
            const cartBadge = document.getElementById('cart-badge');
            const cartModal = document.getElementById('cart-modal');
            const closeModalBtn = document.getElementById('close-modal-btn');
            const modalSummary = document.getElementById('modal-order-summary');
            const waCheckoutBtn = document.getElementById('whatsapp-checkout-btn');
            const danaCheckoutBtn = document.getElementById('dana-checkout-btn');

            // --- Variabel State Pesanan ---
            let currentOrder = {
                nama: '',
                kelas: '',
                gula: 0,
                coklat: 0,
                strawbery: 0,
                totalItems: 0,
                totalPrice: 0
            };
            
            const HARGA_PER_DONAT = 5000;
            const NOMOR_WA_PENJUAL = '6285773688582'; // Nomor WA tanpa 0 di depan, ganti dengan 62

            // --- Fungsi untuk menghitung total harga di form ---
            function calculateTotal() {
                const gula = parseInt(qtyGula.value) || 0;
                const coklat = parseInt(qtyCoklat.value) || 0;
                const strawbery = parseInt(qtyStrawbery.value) || 0;
                
                const total = (gula + coklat + strawbery) * HARGA_PER_DONAT;
                
                totalPriceEl.textContent = `Rp ${total.toLocaleString('id-ID')}`;
            }

            // --- Event listener untuk input jumlah ---
            [qtyGula, qtyCoklat, qtyStrawbery].forEach(input => {
                input.addEventListener('input', calculateTotal);
            });

            // --- Fungsi untuk submit form (Tambah ke Pesanan) ---
            orderForm.addEventListener('submit', (e) => {
                e.preventDefault(); // Mencegah form reload halaman
                
                // 1. Ambil data dari form dan simpan di state
                currentOrder.nama = namaInput.value.trim();
                currentOrder.kelas = kelasInput.value.trim();
                currentOrder.gula = parseInt(qtyGula.value) || 0;
                currentOrder.coklat = parseInt(qtyCoklat.value) || 0;
                currentOrder.strawbery = parseInt(qtyStrawbery.value) || 0;
                
                currentOrder.totalItems = currentOrder.gula + currentOrder.coklat + currentOrder.strawbery;
                currentOrder.totalPrice = currentOrder.totalItems * HARGA_PER_DONAT;

                // Validasi sederhana
                if (!currentOrder.nama || !currentOrder.kelas) {
                    confirmMessage.textContent = 'Nama dan Kelas wajib diisi!';
                    confirmMessage.classList.remove('text-green-600', 'hidden');
                    confirmMessage.classList.add('text-red-600');
                    return;
                }

                if (currentOrder.totalItems === 0) {
                    // Tampilkan pesan error jika belum ada barang
                    confirmMessage.textContent = 'Kamu belum memilih jumlah donat!';
                    confirmMessage.classList.remove('text-green-600', 'hidden');
                    confirmMessage.classList.add('text-red-600');
                    return;
                }

                // 2. Update Badge Keranjang
                cartBadge.textContent = currentOrder.totalItems;
                cartBadge.classList.remove('hidden');

                // 3. Update Modal Content (walaupun modal tersembunyi)
                updateModalContent();
                
                // 4. Aktifkan tombol di modal
                waCheckoutBtn.classList.remove('opacity-50', 'cursor-not-allowed');
                danaCheckoutBtn.classList.remove('opacity-50', 'cursor-not-allowed');

                // 5. Tampilkan pesan sukses di form
                confirmMessage.textContent = 'Pesanan berhasil ditambahkan! Klik keranjang di kanan atas 🛒';
                confirmMessage.classList.remove('text-red-600');
                confirmMessage.classList.add('text-green-600');
                confirmMessage.classList.remove('hidden');

                // Sembunyikan pesan setelah 3 detik
                setTimeout(() => {
                    confirmMessage.classList.add('hidden');
                }, 3000);
            });

            // --- Fungsi untuk mengupdate isi modal ---
            function updateModalContent() {
                if (currentOrder.totalItems === 0) {
                    modalSummary.innerHTML = `<p class="text-gray-600 text-center">Keranjang masih kosong. Silakan isi formulir pemesanan terlebih dahulu.</p>`;
                    return;
                }
                
                let summaryHTML = `
                    <div class="mb-4">
                        <p class="text-gray-600">Nama: <strong class="text-gray-900">${currentOrder.nama}</strong></p>
                        <p class="text-gray-600">Kelas: <strong class="text-gray-900">${currentOrder.kelas}</strong></p>
                    </div>
                    <h5 class="font-semibold text-gray-800 mb-2">Ringkasan Pesanan:</h5>
                    <ul class="space-y-1 text-gray-700">
                `;
                
                if (currentOrder.gula > 0) {
                    summaryHTML += `<li class="flex justify-between"><span>🍩 Gula Halus</span> <span>x ${currentOrder.gula}</span></li>`;
                }
                if (currentOrder.coklat > 0) {
                    summaryHTML += `<li class="flex justify-between"><span>🍫 Coklat</span> <span>x ${currentOrder.coklat}</span></li>`;
                }
                if (currentOrder.strawbery > 0) {
                    summaryHTML += `<li class="flex justify-between"><span>✨ Strawbery</span> <span>x ${currentOrder.strawbery}</span></li>`;
                }
                
                summaryHTML += `
                    </ul>
                    <hr class="my-4">
                    <div class="flex justify-between text-xl font-bold text-brand-orange-600">
                        <span>Total:</span>
                        <span>Rp ${currentOrder.totalPrice.toLocaleString('id-ID')}</span>
                    </div>
                `;
                
                modalSummary.innerHTML = summaryHTML;

                // --- Buat link WhatsApp ---
                let waMessage = `Halo Donat Kentato (Kelompok 9), saya mau pesan:\n\n`;
                waMessage += `*Nama:* ${currentOrder.nama}\n`;
                waMessage += `*Kelas:* ${currentOrder.kelas}\n\n`;
                waMessage += `*Detail Pesanan:*\n`;
                if (currentOrder.gula > 0) {
                    waMessage += `- Donat Gula Halus: ${currentOrder.gula} pcs\n`;
                }
                if (currentOrder.coklat > 0) {
                    waMessage += `- Donat Coklat: ${currentOrder.coklat} pcs\n`;
                }
                if (currentOrder.strawbery > 0) {
                    waMessage += `- Donat Strawbery: ${currentOrder.strawbery} pcs\n`;
                }
                waMessage += `\n*Total Pembayaran: Rp ${currentOrder.totalPrice.toLocaleString('id-ID')}*\n\n`;
                waMessage += `Saya akan melakukan pembayaran. Terima kasih!`;
                
                waCheckoutBtn.href = `https://wa.me/${NOMOR_WA_PENJUAL}?text=${encodeURIComponent(waMessage)}`;
            }

            // --- Fungsi untuk buka/tutup modal ---
            function toggleModal() {
                cartModal.classList.toggle('hidden');
            }

            // --- Event listener untuk modal ---
            cartIcon.addEventListener('click', toggleModal);
            closeModalBtn.addEventListener('click', toggleModal);
            
            // Tutup modal jika klik di luar area konten
            cartModal.addEventListener('click', (e) => {
                if (e.target === cartModal) {
                    toggleModal();
                }
            });

            // Tutup modal dengan tombol Escape
            document.addEventListener('keydown', (e) => {
                if (e.key === 'Escape' && !cartModal.classList.contains('hidden')) {
                    toggleModal();
                }
            });

        });
    </script>
</body>
</html>
