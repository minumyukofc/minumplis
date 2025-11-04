# minumplis
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minum Yuk! - Pre Order Minuman Segar</title>
    
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Lucide Icons -->
    <script src="https://unpkg.com/lucide@latest"></script>
    
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        body {
            font-family: 'Poppins', -apple-system, BlinkMacSystemFont, 'Segoe UI', 'Roboto', sans-serif;
            background-color: #ffffff;
            color: #1f2937;
        }
        
        html {
            scroll-behavior: smooth;
        }
        
        /* Custom animations */
        @keyframes bounce {
            0%, 100% {
                transform: translateY(-25%);
                animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
            }
            50% {
                transform: translateY(0);
                animation-timing-function: cubic-bezier(0, 0, 0.2, 1);
            }
        }
        
        .animate-bounce {
            animation: bounce 1s infinite;
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-md shadow-sm">
        <div class="container mx-auto px-4 py-4">
            <div class="flex items-center justify-between">
                <!-- Logo - GANTI DENGAN PATH LOGO ANDA -->
                <div class="flex items-center cursor-pointer" onclick="scrollToSection('home')">
                    <img src="logo-minum-yuk.png" alt="Minum Yuk Logo" class="h-12 w-auto object-contain">
                </div>

                <!-- Navigation Desktop -->
                <nav class="hidden md:flex items-center gap-8">
                    <button onclick="scrollToSection('home')" class="text-gray-700 hover:text-orange-500 transition-colors">
                        Home
                    </button>
                    <button onclick="scrollToSection('tentang')" class="text-gray-700 hover:text-orange-500 transition-colors">
                        Tentang
                    </button>
                    <button onclick="scrollToSection('produk')" class="text-gray-700 hover:text-orange-500 transition-colors">
                        Produk
                    </button>
                    <button onclick="scrollToSection('kontak')" class="text-gray-700 hover:text-orange-500 transition-colors">
                        Kontak
                    </button>
                </nav>

                <!-- Mobile menu button -->
                <button class="md:hidden p-2">
                    <div class="w-6 h-0.5 bg-gray-700 mb-1.5"></div>
                    <div class="w-6 h-0.5 bg-gray-700 mb-1.5"></div>
                    <div class="w-6 h-0.5 bg-gray-700"></div>
                </button>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section id="home" class="min-h-screen flex items-center justify-center pt-20 px-4 bg-gradient-to-br from-orange-50 via-pink-50 to-white relative overflow-hidden">
        <!-- Decorative circles -->
        <div class="absolute top-20 right-10 w-72 h-72 bg-orange-200/30 rounded-full blur-3xl"></div>
        <div class="absolute bottom-20 left-10 w-96 h-96 bg-pink-200/30 rounded-full blur-3xl"></div>

        <div class="container mx-auto grid md:grid-cols-2 gap-12 items-center relative z-10">
            <!-- Left Content -->
            <div class="text-center md:text-left space-y-6">
                <div class="inline-flex items-center gap-2 px-4 py-2 bg-white rounded-full shadow-md">
                    <i data-lucide="sparkles" class="w-4 h-4 text-orange-500"></i>
                    <span class="text-orange-600 font-medium">Pesan Sekarang</span>
                </div>

                <h1 class="text-5xl md:text-6xl lg:text-7xl bg-gradient-to-r from-orange-500 via-pink-500 to-orange-400 bg-clip-text text-transparent font-bold leading-tight">
                    PRE ORDER
                    <br>
                    MINUM YUK!
                </h1>

                <p class="text-2xl md:text-3xl text-gray-700 font-medium">
                    Inovasi Segar Untuk Semua
                </p>

                <p class="text-gray-600 max-w-lg">
                    Nikmati kesegaran dalam setiap tetes. Minuman praktis, sehat, dan penuh cita rasa 
                    yang siap menemani aktivitas harianmu.
                </p>

                <div class="flex flex-wrap gap-4 justify-center md:justify-start">
                    <div class="px-6 py-3 bg-gradient-to-r from-orange-500 to-pink-500 text-white rounded-full shadow-lg hover:shadow-xl transition-all transform hover:scale-105 cursor-pointer font-medium">
                        Dapatkan Update
                    </div>
                    <div class="px-6 py-3 bg-white text-orange-500 rounded-full shadow-lg hover:shadow-xl transition-all border-2 border-orange-200 cursor-pointer font-medium">
                        Pelajari Lebih Lanjut
                    </div>
                </div>
            </div>

            <!-- Right Content - Product Images -->
            <div class="relative">
                <div class="relative flex items-center justify-center gap-8">
                    <!-- Orange Drink -->
                    <div class="relative transform hover:scale-105 transition-transform duration-300">
                        <div class="absolute inset-0 bg-orange-300/40 rounded-3xl blur-2xl"></div>
                        <div class="relative bg-white p-4 rounded-3xl shadow-2xl">
                            <div class="w-48 h-64 rounded-2xl overflow-hidden">
                                <!-- GANTI DENGAN PATH GAMBAR JERUK ANDA -->
                                <img src="jeruk.png" alt="Minuman Jeruk" class="w-full h-full object-cover">
                            </div>
                            <div class="absolute -top-2 -right-2 w-12 h-12 bg-orange-500 rounded-full flex items-center justify-center text-white shadow-lg text-2xl">
                                🍊
                            </div>
                        </div>
                    </div>

                    <!-- Guava Drink -->
                    <div class="relative transform hover:scale-105 transition-transform duration-300 -mt-12">
                        <div class="absolute inset-0 bg-pink-300/40 rounded-3xl blur-2xl"></div>
                        <div class="relative bg-white p-4 rounded-3xl shadow-2xl">
                            <div class="w-48 h-64 rounded-2xl overflow-hidden">
                                <!-- GANTI DENGAN PATH GAMBAR JAMBU ANDA -->
                                <img src="jambu.png" alt="Minuman Jambu Merah" class="w-full h-full object-cover">
                            </div>
                            <div class="absolute -top-2 -right-2 w-12 h-12 bg-pink-500 rounded-full flex items-center justify-center text-white shadow-lg text-2xl">
                                🍑
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- About Section -->
    <section id="tentang" class="py-20 px-4 bg-white">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-16">
                <div class="inline-flex items-center gap-2 px-4 py-2 bg-orange-100 rounded-full mb-4">
                    <i data-lucide="sparkles" class="w-4 h-4 text-orange-500"></i>
                    <span class="text-orange-600 font-medium">Tentang Kami</span>
                </div>
                <h2 class="text-4xl md:text-5xl bg-gradient-to-r from-orange-500 to-pink-500 bg-clip-text text-transparent font-bold mb-6">
                    Kenapa Minum Yuk?
                </h2>
                <p class="text-gray-600 max-w-2xl mx-auto text-lg">
                    Kami hadir dengan inovasi minuman segar yang dirancang khusus untuk gaya hidup aktif mahasiswa 
                    dan pekerja muda yang membutuhkan kesegaran praktis setiap hari.
                </p>
            </div>

            <div class="grid md:grid-cols-3 gap-8">
                <!-- Card 1 -->
                <div class="bg-gradient-to-br from-orange-50 to-white p-8 rounded-3xl shadow-lg hover:shadow-xl transition-all transform hover:-translate-y-2">
                    <div class="w-16 h-16 bg-gradient-to-br from-orange-400 to-orange-500 rounded-2xl flex items-center justify-center mb-6 shadow-lg">
                        <i data-lucide="sparkles" class="w-8 h-8 text-white"></i>
                    </div>
                    <h3 class="text-2xl text-gray-800 mb-4 font-semibold">100% Segar</h3>
                    <p class="text-gray-600">
                        Dibuat dari buah pilihan berkualitas tinggi yang dipetik fresh setiap hari 
                        untuk menjaga kesegaran dan nutrisi optimal.
                    </p>
                </div>

                <!-- Card 2 -->
                <div class="bg-gradient-to-br from-pink-50 to-white p-8 rounded-3xl shadow-lg hover:shadow-xl transition-all transform hover:-translate-y-2">
                    <div class="w-16 h-16 bg-gradient-to-br from-pink-400 to-pink-500 rounded-2xl flex items-center justify-center mb-6 shadow-lg">
                        <i data-lucide="zap" class="w-8 h-8 text-white"></i>
                    </div>
                    <h3 class="text-2xl text-gray-800 mb-4 font-semibold">Praktis & Cepat</h3>
                    <p class="text-gray-600">
                        Kemasan praktis yang mudah dibawa kemana saja. Cocok untuk menemani kuliah, 
                        kerja, atau aktivitas outdoor kamu.
                    </p>
                </div>

                <!-- Card 3 -->
                <div class="bg-gradient-to-br from-orange-50 to-pink-50 p-8 rounded-3xl shadow-lg hover:shadow-xl transition-all transform hover:-translate-y-2">
                    <div class="w-16 h-16 bg-gradient-to-br from-orange-400 to-pink-500 rounded-2xl flex items-center justify-center mb-6 shadow-lg">
                        <i data-lucide="heart" class="w-8 h-8 text-white"></i>
                    </div>
                    <h3 class="text-2xl text-gray-800 mb-4 font-semibold">Harga Terjangkau</h3>
                    <p class="text-gray-600">
                        Nikmati kualitas premium dengan harga yang ramah di kantong mahasiswa. 
                        Sehat dan segar tanpa bikin dompet menangis!
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- Product Section -->
    <section id="produk" class="py-20 px-4 bg-gradient-to-br from-white via-orange-50 to-pink-50">
        <div class="container mx-auto max-w-6xl">
            <div class="text-center mb-16">
                <div class="inline-flex items-center gap-2 px-4 py-2 bg-white rounded-full mb-4 shadow-md">
                    <i data-lucide="sparkles" class="w-4 h-4 text-orange-500"></i>
                    <span class="text-orange-600 font-medium">Produk Kami</span>
                </div>
                <h2 class="text-4xl md:text-5xl bg-gradient-to-r from-orange-500 to-pink-500 bg-clip-text text-transparent font-bold mb-6">
                    Varian Rasa Pilihan
                </h2>
                <p class="text-gray-600 max-w-2xl mx-auto text-lg">
                    Dua varian rasa favorit yang siap menyegarkan harimu dengan kelezatan alami
                </p>
            </div>

            <div class="grid md:grid-cols-2 gap-8">
                <!-- Product 1: Jeruk Segar -->
                <div class="overflow-hidden border-0 shadow-xl hover:shadow-2xl transition-all transform hover:-translate-y-2 rounded-3xl">
                    <div class="bg-gradient-to-br from-orange-50 to-orange-100 p-8">
                        <div class="relative mb-6">
                            <div class="absolute inset-0 bg-gradient-to-br from-orange-400 to-orange-500 opacity-20 rounded-3xl blur-2xl"></div>
                            <div class="relative w-full h-80 rounded-2xl shadow-lg overflow-hidden">
                                <!-- GANTI DENGAN PATH GAMBAR JERUK ANDA -->
                                <img src="jeruk.png" alt="Jeruk Segar" class="w-full h-full object-cover">
                            </div>
                            <div class="absolute -top-4 -right-4 w-20 h-20 bg-gradient-to-br from-orange-400 to-orange-500 rounded-full flex items-center justify-center text-4xl shadow-lg">
                                🍊
                            </div>
                        </div>

                        <div class="bg-white rounded-2xl p-6 shadow-lg">
                            <h3 class="text-3xl mb-4 bg-gradient-to-r from-orange-400 to-orange-500 bg-clip-text text-transparent font-bold">
                                Jeruk Segar
                            </h3>
                            <p class="text-gray-600 mb-6">
                                Jeruk pilihan yang kaya vitamin C, memberikan kesegaran alami dan meningkatkan imunitas tubuh. Sempurna untuk memulai hari dengan energi penuh!
                            </p>

                            <div class="flex flex-wrap gap-2">
                                <span class="px-4 py-2 bg-gradient-to-r from-orange-400 to-orange-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Tinggi Vitamin C
                                </span>
                                <span class="px-4 py-2 bg-gradient-to-r from-orange-400 to-orange-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Anti Oksidan
                                </span>
                                <span class="px-4 py-2 bg-gradient-to-r from-orange-400 to-orange-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Meningkatkan Imunitas
                                </span>
                            </div>
                        </div>
                    </div>
                </div>

                <!-- Product 2: Jambu Merah -->
                <div class="overflow-hidden border-0 shadow-xl hover:shadow-2xl transition-all transform hover:-translate-y-2 rounded-3xl">
                    <div class="bg-gradient-to-br from-pink-50 to-pink-100 p-8">
                        <div class="relative mb-6">
                            <div class="absolute inset-0 bg-gradient-to-br from-pink-400 to-pink-500 opacity-20 rounded-3xl blur-2xl"></div>
                            <div class="relative w-full h-80 rounded-2xl shadow-lg overflow-hidden">
                                <!-- GANTI DENGAN PATH GAMBAR JAMBU ANDA -->
                                <img src="jambu.png" alt="Jambu Merah" class="w-full h-full object-cover">
                            </div>
                            <div class="absolute -top-4 -right-4 w-20 h-20 bg-gradient-to-br from-pink-400 to-pink-500 rounded-full flex items-center justify-center text-4xl shadow-lg">
                                🍑
                            </div>
                        </div>

                        <div class="bg-white rounded-2xl p-6 shadow-lg">
                            <h3 class="text-3xl mb-4 bg-gradient-to-r from-pink-400 to-pink-500 bg-clip-text text-transparent font-bold">
                                Jambu Merah
                            </h3>
                            <p class="text-gray-600 mb-6">
                                Jambu merah manis dengan kandungan vitamin dan mineral yang melimpah. Menyegarkan tenggorokan dan membantu menjaga kesehatan kulit.
                            </p>

                            <div class="flex flex-wrap gap-2">
                                <span class="px-4 py-2 bg-gradient-to-r from-pink-400 to-pink-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Kaya Vitamin A
                                </span>
                                <span class="px-4 py-2 bg-gradient-to-r from-pink-400 to-pink-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Baik untuk Kulit
                                </span>
                                <span class="px-4 py-2 bg-gradient-to-r from-pink-400 to-pink-500 text-white rounded-full shadow-md text-sm font-medium">
                                    Rendah Kalori
                                </span>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact Section -->
    <section id="kontak" class="py-20 px-4 bg-gradient-to-br from-orange-50 via-pink-50 to-white relative overflow-hidden">
        <!-- Decorative elements -->
        <div class="absolute top-0 right-0 w-96 h-96 bg-orange-200/20 rounded-full blur-3xl"></div>
        <div class="absolute bottom-0 left-0 w-96 h-96 bg-pink-200/20 rounded-full blur-3xl"></div>

        <div class="container mx-auto max-w-4xl relative z-10">
            <div class="text-center mb-16">
                <div class="inline-flex items-center gap-2 px-4 py-2 bg-white rounded-full mb-4 shadow-md">
                    <i data-lucide="sparkles" class="w-4 h-4 text-orange-500"></i>
                    <span class="text-orange-600 font-medium">Kontak</span>
                </div>
                <h2 class="text-4xl md:text-5xl bg-gradient-to-r from-orange-500 to-pink-500 bg-clip-text text-transparent font-bold mb-6">
                    Yuk, Ikuti Kami!
                </h2>
                <p class="text-gray-600 max-w-2xl mx-auto text-lg mb-12">
                    Dapatkan update terbaru, promo menarik, dan konten seru lainnya. 
                    Jangan sampai ketinggalan ya! ✨
                </p>
            </div>

            <div class="bg-white rounded-3xl shadow-2xl p-12">
                <div class="grid md:grid-cols-3 gap-8">
                    <!-- Instagram -->
                    <a href="https://instagram.com/minumyuk_" target="_blank" rel="noopener noreferrer" class="group">
                        <div class="bg-gradient-to-br from-pink-500 to-purple-500 hover:from-pink-600 hover:to-purple-600 rounded-2xl p-8 text-white text-center transition-all transform hover:scale-105 hover:shadow-2xl cursor-pointer">
                            <div class="flex justify-center mb-4">
                                <i data-lucide="instagram" class="w-8 h-8"></i>
                            </div>
                            <h4 class="text-xl font-semibold">Instagram</h4>
                            <p class="text-white/80 mt-2">@minumyuk_</p>
                        </div>
                    </a>

                    <!-- TikTok -->
                    <a href="https://tiktok.com/@minumyuk_" target="_blank" rel="noopener noreferrer" class="group">
                        <div class="bg-gradient-to-br from-gray-800 to-gray-900 hover:from-gray-900 hover:to-black rounded-2xl p-8 text-white text-center transition-all transform hover:scale-105 hover:shadow-2xl cursor-pointer">
                            <div class="flex justify-center mb-4">
                                <i data-lucide="music" class="w-8 h-8"></i>
                            </div>
                            <h4 class="text-xl font-semibold">TikTok</h4>
                            <p class="text-white/80 mt-2">@minumyuk_</p>
                        </div>
                    </a>

                    <!-- Email -->
                    <a href="mailto:minumyukzz04@gmail.com" class="group">
                        <div class="bg-gradient-to-br from-orange-500 to-red-500 hover:from-orange-600 hover:to-red-600 rounded-2xl p-8 text-white text-center transition-all transform hover:scale-105 hover:shadow-2xl cursor-pointer">
                            <div class="flex justify-center mb-4">
                                <i data-lucide="mail" class="w-8 h-8"></i>
                            </div>
                            <h4 class="text-xl font-semibold">Email</h4>
                            <p class="text-white/80 mt-2 text-sm">minumyukzz04@gmail.com</p>
                        </div>
                    </a>
                </div>

                <div class="mt-12 text-center">
                    <p class="text-gray-600 mb-6 font-medium">
                        Atau hubungi kami langsung via WhatsApp:
                    </p>
                    <a href="https://wa.me/6285373990853" target="_blank" rel="noopener noreferrer" class="inline-block px-8 py-4 bg-gradient-to-r from-green-500 to-green-600 text-white rounded-full shadow-lg hover:shadow-xl transition-all transform hover:scale-105 font-medium">
                        📱 085373990853
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="py-12 px-4 bg-gradient-to-r from-orange-400 via-pink-400 to-orange-400">
        <div class="container mx-auto max-w-6xl">
            <div class="flex flex-col items-center justify-center gap-6">
                <!-- Logo -->
                <div class="flex items-center">
                    <div class="bg-white rounded-2xl p-3 shadow-lg">
                        <!-- GANTI DENGAN PATH LOGO ANDA -->
                        <img src="logo-minum-yuk.png" alt="Minum Yuk Logo" class="h-16 w-auto object-contain">
                    </div>
                </div>

                <!-- Tagline -->
                <p class="text-white/90 text-center font-medium">
                    Inovasi Segar Untuk Semua
                </p>

                <!-- Divider -->
                <div class="w-full max-w-md h-px bg-white/30"></div>

                <!-- Copyright -->
                <div class="flex items-center gap-2 text-white/90">
                    <span>© 2025 Minum Yuk!</span>
                    <span>•</span>
                    <span class="flex items-center gap-1">
                        Dibuat dengan <i data-lucide="heart" class="w-4 h-4 fill-white"></i> untuk Indonesia
                    </span>
                </div>

                <!-- Additional links -->
                <div class="flex gap-6 text-white/80">
                    <a href="#" class="hover:text-white transition-colors">Syarat & Ketentuan</a>
                    <span>•</span>
                    <a href="#" class="hover:text-white transition-colors">Kebijakan Privasi</a>
                </div>
            </div>
        </div>
    </footer>

    <!-- JavaScript -->
    <script>
        // Initialize Lucide Icons
        lucide.createIcons();

        // Smooth scroll function
        function scrollToSection(id) {
            const element = document.getElementById(id);
            if (element) {
                element.scrollIntoView({ behavior: 'smooth', block: 'start' });
            }
        }

        // Re-initialize icons on page load
        document.addEventListener('DOMContentLoaded', function() {
            lucide.createIcons();
        });
    </script>

</body>
</html>
