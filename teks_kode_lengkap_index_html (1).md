<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SMP Muhammadiyah 1 Gadingrejo - Islami, Berprestasi, Berkarakter & Berkemajuan</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <!-- Google Fonts: Poppins -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700;800&display=swap" rel="stylesheet">
    
    <!-- Custom Tailwind Configuration for Muhammadiyah Theme -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        muhGreen: {
                            DEFAULT: '#008751',
                            dark: '#00663d',
                            light: '#00a865',
                            soft: '#e6f4ed'
                        },
                        muhGold: {
                            DEFAULT: '#F5B041',
                            dark: '#D4AC0D',
                            light: '#F9E79F'
                        }
                    },
                    fontFamily: {
                        sans: ['Poppins', 'sans-serif'],
                    }
                }
            }
        }
    </script>

    <style>
        body {
            font-family: 'Poppins', sans-serif;
        }
        .hero-bg {
            background: linear-gradient(rgba(0, 50, 30, 0.82), rgba(0, 100, 60, 0.85)), 
                        url('https://images.unsplash.com/photo-1523050854058-8df90110c9f1?q=80&w=1200&auto=format&fit=crop');
            background-size: cover;
            background-position: center;
        }
        /* Custom Scrollbar */
        ::-webkit-scrollbar {
            width: 8px;
        }
        ::-webkit-scrollbar-track {
            background: #f1f1f1;
        }
        ::-webkit-scrollbar-thumb {
            background: #008751;
            border-radius: 4px;
        }
        ::-webkit-scrollbar-thumb:hover {
            background: #00663d;
        }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 antialiased selection:bg-muhGreen selection:text-white">

    <!-- ================= NAVBAR ================= -->
    <nav id="navbar" class="fixed top-0 left-0 w-full z-50 transition-all duration-300 bg-white/95 backdrop-blur-md shadow-md">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                <!-- Logo & Brand -->
                <a href="#beranda" class="flex items-center gap-3 group">
                    <div class="w-12 h-12 bg-muhGreen rounded-full flex items-center justify-center text-white text-2xl font-bold shadow-md group-hover:scale-105 transition-transform border-2 border-muhGold">
                        <i class="fa-solid fa-sun text-muhGold"></i>
                    </div>
                    <div>
                        <span class="block text-lg font-bold text-muhGreen-dark leading-tight">SMP MUHAMMADIYAH 1</span>
                        <span class="block text-xs font-semibold tracking-wider text-muhGold-dark uppercase">Gadingrejo - Pringsewu</span>
                    </div>
                </a>

                <!-- Desktop Menu -->
                <div class="hidden lg:flex items-center space-x-6">
                    <a href="#beranda" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Beranda</a>
                    <a href="#profil" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Profil</a>
                    <a href="#visi-misi" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Visi & Misi</a>
                    <a href="#program" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Keunggulan</a>
                    <a href="#ekstrakurikuler" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Ekstrakurikuler</a>
                    <a href="#galeri" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">Galeri</a>
                    <a href="#ppdb" class="nav-link font-medium text-gray-700 hover:text-muhGreen transition-colors">PPDB</a>
                    <a href="#kontak" class="px-5 py-2.5 rounded-full bg-muhGreen text-white font-semibold hover:bg-muhGreen-dark transition-all shadow-md hover:shadow-lg transform hover:-translate-y-0.5">
                        <i class="fa-solid fa-envelope mr-1.5"></i> Kontak
                    </a>
                </div>

                <!-- Mobile Menu Button -->
                <button id="mobile-menu-btn" class="lg:hidden p-2 rounded-lg text-gray-700 hover:text-muhGreen hover:bg-gray-100 focus:outline-none" aria-label="Toggle Navigation">
                    <i id="menu-icon" class="fa-solid fa-bars text-2xl"></i>
                </button>
            </div>
        </div>

        <!-- Mobile Menu Dropdown -->
        <div id="mobile-menu" class="hidden lg:hidden bg-white border-b border-gray-200 px-4 pt-2 pb-6 space-y-3 shadow-lg">
            <a href="#beranda" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Beranda</a>
            <a href="#profil" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Profil</a>
            <a href="#visi-misi" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Visi & Misi</a>
            <a href="#program" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Keunggulan</a>
            <a href="#ekstrakurikuler" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Ekstrakurikuler</a>
            <a href="#galeri" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">Galeri</a>
            <a href="#ppdb" class="mobile-nav-link block px-3 py-2 rounded-md font-medium text-gray-700 hover:bg-muhGreen-soft hover:text-muhGreen">PPDB</a>
            <a href="#kontak" class="mobile-nav-link block w-full text-center mt-2 px-4 py-2.5 rounded-full bg-muhGreen text-white font-semibold">Kontak Kami</a>
        </div>
    </nav>

    <!-- ================= HERO SECTION ================= -->
    <section id="beranda" class="hero-bg min-h-screen flex items-center pt-24 pb-16 relative text-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 w-full text-center lg:text-left">
            <div class="grid lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-8 space-y-6">
                    <!-- Salam Badge -->
                    <div class="inline-flex items-center gap-2 px-4 py-1.5 rounded-full bg-white/10 backdrop-blur-md border border-white/20 text-muhGold text-sm font-semibold tracking-wide">
                        <i class="fa-solid fa-star text-xs"></i> Selamat Datang di Official Website
                    </div>
                    
                    <h1 class="text-4xl sm:text-5xl lg:text-6xl font-extrabold leading-tight">
                        SMP Muhammadiyah 1 <span class="text-muhGold">Gadingrejo</span>
                    </h1>
                    
                    <p class="text-lg sm:text-xl text-gray-200 max-w-2xl font-light leading-relaxed">
                        Membentuk Generasi <span class="font-semibold text-white">Islami, Berprestasi, Berkarakter & Berkemajuan</span>. Siap Menghadapi Tantangan Masa Depan Berlandaskan Al-Qur'an dan As-Sunnah.
                    </p>

                    <div class="pt-4 flex flex-col sm:flex-row gap-4 justify-center lg:justify-start">
                        <a href="#ppdb" class="px-8 py-4 rounded-full bg-muhGold text-gray-900 font-bold hover:bg-yellow-400 transition-all shadow-lg hover:shadow-xl transform hover:-translate-y-1 text-center flex items-center justify-center gap-2">
                            <i class="fa-solid fa-user-plus"></i> Info PPDB 2026/2027
                        </a>
                        <a href="#profil" class="px-8 py-4 rounded-full bg-white/20 backdrop-blur-md border border-white/30 text-white font-semibold hover:bg-white/30 transition-all text-center flex items-center justify-center gap-2">
                            <i class="fa-solid fa-compass"></i> Jelajahi Profil
                        </a>
                    </div>
                </div>

                <!-- Floating Card Stats -->
                <div class="lg:col-span-4 mt-8 lg:mt-0">
                    <div class="bg-white/10 backdrop-blur-md p-6 rounded-2xl border border-white/20 shadow-2xl grid grid-cols-2 gap-4">
                        <div class="bg-white/10 p-4 rounded-xl text-center">
                            <i class="fa-solid fa-user-graduate text-3xl text-muhGold mb-2"></i>
                            <h3 class="text-2xl font-bold">A</h3>
                            <p class="text-xs text-gray-200">Akreditasi Sekolah</p>
                        </div>
                        <div class="bg-white/10 p-4 rounded-xl text-center">
                            <i class="fa-solid fa-book-quran text-3xl text-muhGold mb-2"></i>
                            <h3 class="text-2xl font-bold">Tahfidz</h3>
                            <p class="text-xs text-gray-200">Program Unggulan</p>
                        </div>
                        <div class="bg-white/10 p-4 rounded-xl text-center">
                            <i class="fa-solid fa-trophy text-3xl text-muhGold mb-2"></i>
                            <h3 class="text-2xl font-bold">15+</h3>
                            <p class="text-xs text-gray-200">Ekstrakurikuler</p>
                        </div>
                        <div class="bg-white/10 p-4 rounded-xl text-center">
                            <i class="fa-solid fa-users text-3xl text-muhGold mb-2"></i>
                            <h3 class="text-2xl font-bold">100%</h3>
                            <p class="text-xs text-gray-200">Guru Profesional</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Wave Separator -->
        <div class="absolute bottom-0 left-0 w-full overflow-hidden leading-none">
            <svg class="relative block w-full h-12 sm:h-16 text-gray-50" viewBox="0 0 1200 120" preserveAspectRatio="none">
                <path d="M321.39,56.44c58-10.79,114.16-30.13,172-41.86,82.39-16.72,168.19-17.73,250.45-.39C823.78,31,906.67,72,985.66,92.83c70.05,18.48,146.53,26.09,214.34,3V120H0V95.8C59.71,118.06,130.83,121.61,192,112.34,236.08,105.69,279.72,83.84,321.39,56.44Z" fill="currentColor"></path>
            </svg>
        </div>
    </section>

    <!-- ================= PROFIL / TENTANG KAMI ================= -->
    <section id="profil" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Tentang Kami</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Mengenal Lebih Dekat SMP Muhammadiyah 1 Gadingrejo</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="grid lg:grid-cols-12 gap-12 items-center">
                <!-- Sambutan Kepala Sekolah -->
                <div class="lg:col-span-5 relative">
                    <div class="relative z-10 bg-white p-4 rounded-2xl shadow-xl border border-gray-100">
                        <img src="https://images.unsplash.com/photo-1560250097-0b93528c311a?q=80&w=600&auto=format&fit=crop" alt="Kepala Sekolah" class="rounded-xl w-full h-80 object-cover">
                        <div class="p-4 text-center">
                            <h3 class="text-xl font-bold text-gray-900">Kepala Sekolah SMP Muh 1</h3>
                            <p class="text-sm text-muhGreen font-medium">SMP Muhammadiyah 1 Gadingrejo</p>
                        </div>
                    </div>
                    <!-- Decorative Background Box -->
                    <div class="absolute -bottom-6 -right-6 w-full h-full bg-muhGreen/20 rounded-2xl -z-0"></div>
                </div>

                <!-- Deskripsi & Sejarah Singkat -->
                <div class="lg:col-span-7 space-y-6">
                    <div class="bg-white p-8 rounded-2xl shadow-sm border border-gray-100 space-y-4">
                        <h3 class="text-2xl font-bold text-gray-900 flex items-center gap-3">
                            <i class="fa-solid fa-quote-left text-muhGold text-3xl"></i> Sambutan Kepala Sekolah
                        </h3>
                        <p class="text-gray-600 leading-relaxed">
                            "Assalamu’alaikum Warahmatullahi Wabarakatuh. Selamat datang di website resmi SMP Muhammadiyah 1 Gadingrejo. Kami berkomitmen untuk menyajikan pendidikan berkualitas berlandaskan nilai-nilai Al-Islam dan Kemuhammadiyahan demi mencetak generasi unggul yang cerdas, santun, dan berakhlak mulia."
                        </p>
                    </div>

                    <div class="space-y-4 text-gray-600">
                        <h4 class="text-xl font-bold text-gray-900">Nilai & Dedikasi Pendidikan</h4>
                        <p class="leading-relaxed">
                            SMP Muhammadiyah 1 Gadingrejo yang berlokasi di Kecamatan Gadingrejo, Kabupaten Pringsewu, Lampung, merupakan lembaga pendidikan menengah pertama Islami yang terus berinovasi mengikuti perkembangan zaman tanpa meninggalkan akar tradisi Keislaman.
                        </p>
                        <ul class="space-y-2">
                            <li class="flex items-center gap-3 text-gray-700 font-medium">
                                <i class="fa-solid fa-circle-check text-muhGreen"></i> Pembiasaan ibadah harian & Shalat Berjamaah
                            </li>
                            <li class="flex items-center gap-3 text-gray-700 font-medium">
                                <i class="fa-solid fa-circle-check text-muhGreen"></i> Lingkungan belajar yang kondusif, aman, dan asri
                            </li>
                            <li class="flex items-center gap-3 text-gray-700 font-medium">
                                <i class="fa-solid fa-circle-check text-muhGreen"></i> Tenaga pengajar berpengalaman dan berdedikasi
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= VISI & MISI ================= -->
    <section id="visi-misi" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Arah & Tujuan</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Visi & Misi Sekolah</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="grid md:grid-cols-2 gap-8">
                <!-- Visi Card -->
                <div class="bg-gradient-to-br from-muhGreen-soft to-white p-8 rounded-2xl border border-muhGreen/20 shadow-md relative overflow-hidden group hover:shadow-xl transition-all">
                    <div class="absolute -right-6 -bottom-6 text-muhGreen/10 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-eye text-9xl"></i>
                    </div>
                    <div class="w-14 h-14 bg-muhGreen text-white rounded-xl flex items-center justify-center text-2xl mb-6 shadow-md">
                        <i class="fa-solid fa-eye"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-4">Visi Sekolah</h3>
                    <p class="text-lg text-gray-700 font-medium leading-relaxed italic">
                        "Terwujudnya Sekolah yang Unggul dalam Prestasi, Anggun dalam Moral, Berkarakter Islami, serta Berkemajuan dalam Ilmu Pengetahuan dan Teknologi."
                    </p>
                </div>

                <!-- Misi Card -->
                <div class="bg-gradient-to-br from-amber-50 to-white p-8 rounded-2xl border border-muhGold/30 shadow-md relative overflow-hidden group hover:shadow-xl transition-all">
                    <div class="absolute -right-6 -bottom-6 text-muhGold/10 group-hover:scale-110 transition-transform">
                        <i class="fa-solid fa-bullseye text-9xl"></i>
                    </div>
                    <div class="w-14 h-14 bg-muhGold text-gray-900 rounded-xl flex items-center justify-center text-2xl mb-6 shadow-md">
                        <i class="fa-solid fa-bullseye"></i>
                    </div>
                    <h3 class="text-2xl font-bold text-gray-900 mb-4">Misi Sekolah</h3>
                    <ul class="space-y-3 text-gray-700">
                        <li class="flex items-start gap-3">
                            <span class="w-6 h-6 bg-muhGold/30 text-gray-900 rounded-full flex items-center justify-center text-xs font-bold shrink-0 mt-0.5">1</span>
                            Menyelenggarakan pendidikan Al-Islam dan Kemuhammadiyahan secara terpadu.
                        </li>
                        <li class="flex items-start gap-3">
                            <span class="w-6 h-6 bg-muhGold/30 text-gray-900 rounded-full flex items-center justify-center text-xs font-bold shrink-0 mt-0.5">2</span>
                            Mengembangkan proses pembelajaran berbasis IT yang kreatif dan inovatif.
                        </li>
                        <li class="flex items-start gap-3">
                            <span class="w-6 h-6 bg-muhGold/30 text-gray-900 rounded-full flex items-center justify-center text-xs font-bold shrink-0 mt-0.5">3</span>
                            Membina kedisiplinan, kemandirian, dan karakter kepemimpinan siswa.
                        </li>
                        <li class="flex items-start gap-3">
                            <span class="w-6 h-6 bg-muhGold/30 text-gray-900 rounded-full flex items-center justify-center text-xs font-bold shrink-0 mt-0.5">4</span>
                            Menumbuhkan potensi akademik dan non-akademik siswa secara optimal.
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= PROGRAM UNGGULAN ================= -->
    <section id="program" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Nilai Tambah</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Program Unggulan Sekolah</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-6">
                <!-- Program 1 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-gray-100 hover:shadow-lg transition-all group hover:-translate-y-1">
                    <div class="w-12 h-12 bg-muhGreen-soft text-muhGreen rounded-xl flex items-center justify-center text-2xl mb-4 group-hover:bg-muhGreen group-hover:text-white transition-colors">
                        <i class="fa-solid fa-book-quran"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Tahfidzul Qur'an</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">
                        Program bimbingan hafalan Al-Qur'an terstruktur dengan target capaian juz untuk para siswa.
                    </p>
                </div>

                <!-- Program 2 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-gray-100 hover:shadow-lg transition-all group hover:-translate-y-1">
                    <div class="w-12 h-12 bg-muhGreen-soft text-muhGreen rounded-xl flex items-center justify-center text-2xl mb-4 group-hover:bg-muhGreen group-hover:text-white transition-colors">
                        <i class="fa-solid fa-hands-praying"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Kader IPMAWAN</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">
                        Pembentukan karakter kepemimpinan melalui Organisasi Ikatan Pelajar Muhammadiyah (IPM).
                    </p>
                </div>

                <!-- Program 3 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-gray-100 hover:shadow-lg transition-all group hover:-translate-y-1">
                    <div class="w-12 h-12 bg-muhGreen-soft text-muhGreen rounded-xl flex items-center justify-center text-2xl mb-4 group-hover:bg-muhGreen group-hover:text-white transition-colors">
                        <i class="fa-solid fa-laptop-code"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">Literasi Digital & IT</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">
                        Pelatihan keterampilan komputer dasar, desain grafis, dan pemanfaatan teknologi positif.
                    </p>
                </div>

                <!-- Program 4 -->
                <div class="bg-white p-6 rounded-2xl shadow-sm border border-gray-100 hover:shadow-lg transition-all group hover:-translate-y-1">
                    <div class="w-12 h-12 bg-muhGreen-soft text-muhGreen rounded-xl flex items-center justify-center text-2xl mb-4 group-hover:bg-muhGreen group-hover:text-white transition-colors">
                        <i class="fa-solid fa-language"></i>
                    </div>
                    <h3 class="text-xl font-bold text-gray-900 mb-2">English & Arabic Club</h3>
                    <p class="text-gray-600 text-sm leading-relaxed">
                        Pengembangan kemampuan komunikasi bahasa asing siswa secara aktif dan percaya diri.
                    </p>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= EKSTRAKURIKULER ================= -->
    <section id="ekstrakurikuler" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Pengembangan Bakat</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Ekstrakurikuler & Kegiatan</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-8">
                <!-- Ekskul 1: Tapak Suci -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-red-600 text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-hand-fist"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">Tapak Suci Putera Muhammadiyah</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Bela Diri & Karakter</p>
                        <p class="text-sm text-gray-600">Seni bela diri khas Muhammadiyah melatih ketangkasan dan mental siswa.</p>
                    </div>
                </div>

                <!-- Ekskul 2: Hizbul Wathan -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-amber-600 text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-compass"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">Hizbul Wathan (HW)</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Kepanduan</p>
                        <p class="text-sm text-gray-600">Gerakan kepanduan untuk membentuk kepemimpinan dan kecintaan alam.</p>
                    </div>
                </div>

                <!-- Ekskul 3: IPM -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-muhGreen text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-users-gear"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">Ikatan Pelajar Muhammadiyah</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Organisasi Siswa</p>
                        <p class="text-sm text-gray-600">Wadah latihan berorganisasi, keilmuan, dan bakat kepemimpinan.</p>
                    </div>
                </div>

                <!-- Ekskul 4: Olahraga -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-blue-600 text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-volleyball"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">Olahraga & Atletik</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Futsal, Voli, Bulutangkis</p>
                        <p class="text-sm text-gray-600">Mengembangkan potensi fisik dan ketangkasan tim siswa.</p>
                    </div>
                </div>

                <!-- Ekskul 5: Seni & Drum Band -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-purple-600 text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-drum"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">Seni & Drumband</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Kreativitas & Musik</p>
                        <p class="text-sm text-gray-600">Wadah minat bakat dalam bidang seni musik dan pertunjukan.</p>
                    </div>
                </div>

                <!-- Ekskul 6: PMR & Kesehatan -->
                <div class="bg-gray-50 rounded-2xl p-6 border border-gray-100 flex items-start gap-4 hover:border-muhGreen transition-all hover:shadow-md">
                    <div class="w-14 h-14 bg-teal-600 text-white rounded-xl flex items-center justify-center text-2xl shrink-0 shadow-md">
                        <i class="fa-solid fa-notes-medical"></i>
                    </div>
                    <div>
                        <h3 class="text-lg font-bold text-gray-900">PMR / Ke-PMR-an</h3>
                        <p class="text-xs text-muhGreen font-semibold mb-2">Kemanusiaan</p>
                        <p class="text-sm text-gray-600">Melatih kepedulian sosial, kesehatan dasar, dan pertolongan pertama.</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= GALERI FOTO ================= -->
    <section id="galeri" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-12">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Dokumentasi</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Galeri Kegiatan Sekolah</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <!-- Filter Buttons -->
            <div class="flex flex-wrap justify-center gap-2 mb-10">
                <button onclick="filterGallery('all')" class="gallery-filter-btn active px-5 py-2 rounded-full text-sm font-semibold bg-muhGreen text-white transition-all shadow-sm">Semua</button>
                <button onclick="filterGallery('akademik')" class="gallery-filter-btn px-5 py-2 rounded-full text-sm font-semibold bg-white text-gray-700 hover:bg-gray-100 transition-all border border-gray-200">Akademik</button>
                <button onclick="filterGallery('keagamaan')" class="gallery-filter-btn px-5 py-2 rounded-full text-sm font-semibold bg-white text-gray-700 hover:bg-gray-100 transition-all border border-gray-200">Keagamaan</button>
                <button onclick="filterGallery('ekskul')" class="gallery-filter-btn px-5 py-2 rounded-full text-sm font-semibold bg-white text-gray-700 hover:bg-gray-100 transition-all border border-gray-200">Ekstrakurikuler</button>
            </div>

            <!-- Gallery Grid -->
            <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Item 1 -->
                <div class="gallery-item keagamaan relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1577896851231-70ef18881754?q=80&w=800&auto=format&fit=crop', 'Kegiatan Setoran Tahfidz & Kajian Islami')">
                    <img src="https://images.unsplash.com/photo-1577896851231-70ef18881754?q=80&w=600&auto=format&fit=crop" alt="Kegiatan Agama" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Keagamaan</span>
                            <h4 class="font-bold text-lg">Kajian & Bimbingan Tahfidz</h4>
                        </div>
                    </div>
                </div>

                <!-- Item 2 -->
                <div class="gallery-item akademik relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=800&auto=format&fit=crop', 'Suasana Belajar Interaktif Kelas IT')">
                    <img src="https://images.unsplash.com/photo-1509062522246-3755977927d7?q=80&w=600&auto=format&fit=crop" alt="Kegiatan Kelas" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Akademik</span>
                            <h4 class="font-bold text-lg">Pembelajaran Berbasis Komputer</h4>
                        </div>
                    </div>
                </div>

                <!-- Item 3 -->
                <div class="gallery-item ekskul relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1517649763962-0c623266ddc0?q=80&w=800&auto=format&fit=crop', 'Latihan Tapak Suci Putra Muhammadiyah')">
                    <img src="https://images.unsplash.com/photo-1517649763962-0c623266ddc0?q=80&w=600&auto=format&fit=crop" alt="Tapak Suci" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Ekstrakurikuler</span>
                            <h4 class="font-bold text-lg">Latihan Rutin Tapak Suci</h4>
                        </div>
                    </div>
                </div>

                <!-- Item 4 -->
                <div class="gallery-item ekskul relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1?q=80&w=800&auto=format&fit=crop', 'Kemah Pandu Hizbul Wathan')">
                    <img src="https://images.unsplash.com/photo-1526778548025-fa2f459cd5c1?q=80&w=600&auto=format&fit=crop" alt="Kemah HW" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Ekstrakurikuler</span>
                            <h4 class="font-bold text-lg">Kemah Pandu Hizbul Wathan</h4>
                        </div>
                    </div>
                </div>

                <!-- Item 5 -->
                <div class="gallery-item keagamaan relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1542810634-71277d95dcbb?q=80&w=800&auto=format&fit=crop', 'Shalat Dhuha dan Berjamaah Bersama')">
                    <img src="https://images.unsplash.com/photo-1542810634-71277d95dcbb?q=80&w=600&auto=format&fit=crop" alt="Ibadah" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Keagamaan</span>
                            <h4 class="font-bold text-lg">Pembiasaan Shalat Berjamaah</h4>
                        </div>
                    </div>
                </div>

                <!-- Item 6 -->
                <div class="gallery-item akademik relative group overflow-hidden rounded-2xl shadow-sm cursor-pointer" onclick="openLightbox('https://images.unsplash.com/photo-1524178232363-1fb2b075b655?q=80&w=800&auto=format&fit=crop', 'Prestasi dan Penghargaan Siswa')">
                    <img src="https://images.unsplash.com/photo-1524178232363-1fb2b075b655?q=80&w=600&auto=format&fit=crop" alt="Prestasi Siswa" class="w-full h-64 object-cover group-hover:scale-110 transition-transform duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 via-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity flex items-end p-6">
                        <div class="text-white">
                            <span class="text-xs text-muhGold uppercase tracking-wider font-semibold">Akademik</span>
                            <h4 class="font-bold text-lg">Penyerahan Penghargaan Siswa</h4>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- Lightbox Modal -->
    <div id="lightbox" class="fixed inset-0 bg-black/90 z-50 hidden flex items-center justify-center p-4">
        <button onclick="closeLightbox()" class="absolute top-6 right-6 text-white text-3xl hover:text-muhGold transition-colors">
            <i class="fa-solid fa-xmark"></i>
        </button>
        <div class="max-w-4xl w-full text-center">
            <img id="lightbox-img" src="" alt="Galeri Preview" class="max-h-[80vh] mx-auto rounded-lg shadow-2xl">
            <p id="lightbox-caption" class="text-white text-lg font-medium mt-4"></p>
        </div>
    </div>

    <!-- ================= INFO PPDB ================= -->
    <section id="ppdb" class="py-20 bg-muhGreen text-white relative overflow-hidden">
        <!-- Background Pattern -->
        <div class="absolute -right-20 -top-20 opacity-10">
            <i class="fa-solid fa-sun text-[300px]"></i>
        </div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="grid lg:grid-cols-12 gap-8 items-center">
                <div class="lg:col-span-8 space-y-4">
                    <span class="px-4 py-1.5 rounded-full bg-muhGold text-gray-900 font-bold text-sm inline-block">
                        Penerimaan Peserta Didik Baru (PPDB)
                    </span>
                    <h2 class="text-3xl sm:text-4xl font-extrabold">Bergabunglah Bersama Keluarga Besar SMP Muhammadiyah 1 Gadingrejo</h2>
                    <p class="text-gray-100 text-lg font-light leading-relaxed">
                        Tahun Ajaran 2026/2027 telah dibuka! Dapatkan beasiswa khusus bagi siswa berprestasi & hafidz Qur'an.
                    </p>
                    <div class="flex flex-wrap gap-6 pt-2 text-sm font-medium">
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-check-circle text-muhGold"></i> Bebas Biaya Pendaftaran*
                        </div>
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-check-circle text-muhGold"></i> Beasiswa Tahfidz
                        </div>
                        <div class="flex items-center gap-2">
                            <i class="fa-solid fa-check-circle text-muhGold"></i> Fasilitas Lengkap
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-4 text-center lg:text-right">
                    <a href="#kontak" class="inline-block px-8 py-4 bg-muhGold text-gray-900 font-extrabold text-lg rounded-full shadow-lg hover:bg-yellow-400 hover:shadow-xl transition-all transform hover:-translate-y-1">
                        Daftar Sekarang <i class="fa-solid fa-arrow-right ml-2"></i>
                    </a>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= KONTAK & LOKASI ================= -->
    <section id="kontak" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center max-w-3xl mx-auto mb-16">
                <h2 class="text-sm font-bold text-muhGreen tracking-widest uppercase">Hubungi Kami</h2>
                <p class="text-3xl font-extrabold text-gray-900 mt-2">Informasi Kontak & Lokasi</p>
                <div class="w-20 h-1.5 bg-muhGold mx-auto mt-4 rounded-full"></div>
            </div>

            <div class="grid lg:grid-cols-12 gap-12">
                <!-- Info Kontak & Alamat -->
                <div class="lg:col-span-5 space-y-6">
                    <div class="bg-gray-50 p-6 rounded-2xl border border-gray-100 space-y-6">
                        <h3 class="text-xl font-bold text-gray-900 mb-4">Sekretariat PPDB / Informasi</h3>
                        
                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 bg-muhGreen/10 text-muhGreen rounded-lg flex items-center justify-center text-lg shrink-0 mt-1">
                                <i class="fa-solid fa-location-dot"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold text-gray-900">Alamat</h4>
                                <p class="text-sm text-gray-600">Gadingrejo, Kec. Gading Rejo, Kabupaten Pringsewu, Lampung 35372</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 bg-muhGreen/10 text-muhGreen rounded-lg flex items-center justify-center text-lg shrink-0 mt-1">
                                <i class="fa-solid fa-phone"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold text-gray-900">Telepon / WhatsApp</h4>
                                <p class="text-sm text-gray-600">+62 812-3456-7890</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 bg-muhGreen/10 text-muhGreen rounded-lg flex items-center justify-center text-lg shrink-0 mt-1">
                                <i class="fa-solid fa-envelope"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold text-gray-900">Email</h4>
                                <p class="text-sm text-gray-600">info@smpmuh1gadingrejo.sch.id</p>
                            </div>
                        </div>

                        <div class="flex items-start gap-4">
                            <div class="w-10 h-10 bg-muhGreen/10 text-muhGreen rounded-lg flex items-center justify-center text-lg shrink-0 mt-1">
                                <i class="fa-solid fa-clock"></i>
                            </div>
                            <div>
                                <h4 class="font-semibold text-gray-900">Jam Operasional</h4>
                                <p class="text-sm text-gray-600">Senin - Sabtu: 07.00 - 15.00 WIB</p>
                            </div>
                        </div>
                    </div>

                    <!-- Peta Lokasi Google Maps -->
                    <div class="rounded-2xl overflow-hidden shadow-md border border-gray-100 h-64">
                        <iframe 
                            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d15888.75628587123!2d105.033333!3d-5.366667!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e472cfed80bb59d%3A0x4039d80b220cc70!2sGading%20Rejo%20Kec.%20Gading%20Rejo%20Kabupaten%20Pringsewu%20Lampung!5e0!3m2!1sid!2sid!4v1650000000000!5m2!1sid!2sid" 
                            width="100%" 
                            height="100%" 
                            style="border:0;" 
                            allowfullscreen="" 
                            loading="lazy">
                        </iframe>
                    </div>
                </div>

                <!-- Formulir Pesan -->
                <div class="lg:col-span-7">
                    <div class="bg-gray-50 p-8 rounded-2xl border border-gray-100 shadow-sm">
                        <h3 class="text-2xl font-bold text-gray-900 mb-2">Kirim Pesan / Pertanyaan</h3>
                        <p class="text-gray-600 text-sm mb-6">Silakan isi formulir di bawah ini untuk bertanya seputar pendaftaran atau informasi sekolah.</p>

                        <!-- Notification Alert -->
                        <div id="form-alert" class="hidden mb-6 p-4 rounded-xl text-sm font-medium"></div>

                        <form id="contact-form" onsubmit="handleSubmit(event)" class="space-y-4">
                            <div class="grid sm:grid-cols-2 gap-4">
                                <div>
                                    <label for="name" class="block text-xs font-semibold text-gray-700 uppercase mb-1">Nama Lengkap *</label>
                                    <input type="text" id="name" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:outline-none focus:ring-2 focus:ring-muhGreen bg-white transition-all">
                                </div>
                                <div>
                                    <label for="phone" class="block text-xs font-semibold text-gray-700 uppercase mb-1">No. WhatsApp / HP *</label>
                                    <input type="tel" id="phone" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:outline-none focus:ring-2 focus:ring-muhGreen bg-white transition-all">
                                </div>
                            </div>

                            <div>
                                <label for="email" class="block text-xs font-semibold text-gray-700 uppercase mb-1">Alamat Email</label>
                                <input type="email" id="email" class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:outline-none focus:ring-2 focus:ring-muhGreen bg-white transition-all">
                            </div>

                            <div>
                                <label for="subject" class="block text-xs font-semibold text-gray-700 uppercase mb-1">Subjek / Perihal *</label>
                                <select id="subject" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:outline-none focus:ring-2 focus:ring-muhGreen bg-white transition-all">
                                    <option value="">-- Pilih Perihal --</option>
                                    <option value="PPDB / Pendaftaran">Informasi PPDB / Pendaftaran</option>
                                    <option value="Informasi Umum">Informasi Umum Sekolah</option>
                                    <option value="Kerjasama">Saran / Kerjasama</option>
                                </select>
                            </div>

                            <div>
                                <label for="message" class="block text-xs font-semibold text-gray-700 uppercase mb-1">Pesan / Pertanyaan *</label>
                                <textarea id="message" rows="4" required class="w-full px-4 py-3 rounded-xl border border-gray-200 focus:outline-none focus:ring-2 focus:ring-muhGreen bg-white transition-all"></textarea>
                            </div>

                            <button type="submit" class="w-full py-4 bg-muhGreen text-white font-bold rounded-xl shadow-md hover:bg-muhGreen-dark transition-all flex items-center justify-center gap-2">
                                <i class="fa-solid fa-paper-plane"></i> Kirim Pesan
                            </button>
                        </form>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ================= FOOTER ================= -->
    <footer class="bg-gray-900 text-gray-300 pt-16 pb-8 border-t-4 border-muhGold">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8 mb-12">
                <!-- Branding -->
                <div class="space-y-4">
                    <div class="flex items-center gap-3">
                        <div class="w-10 h-10 bg-muhGreen rounded-full flex items-center justify-center text-white text-xl font-bold border border-muhGold">
                            <i class="fa-solid fa-sun text-muhGold"></i>
                        </div>
                        <span class="text-lg font-bold text-white">SMP Muh 1 Gadingrejo</span>
                    </div>
                    <p class="text-sm text-gray-400 leading-relaxed">
                        Mewujudkan generasi terdidik, berakhlak mulia, dan berkemajuan di Gadingrejo, Pringsewu, Lampung.
                    </p>
                </div>

                <!-- Tautan Cepat -->
                <div>
                    <h4 class="text-white font-bold mb-4 border-l-2 border-muhGold pl-3">Tautan Cepat</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#beranda" class="hover:text-muhGold transition-colors">Beranda</a></li>
                        <li><a href="#profil" class="hover:text-muhGold transition-colors">Profil Sekolah</a></li>
                        <li><a href="#visi-misi" class="hover:text-muhGold transition-colors">Visi & Misi</a></li>
                        <li><a href="#program" class="hover:text-muhGold transition-colors">Program Unggulan</a></li>
                        <li><a href="#ppdb" class="hover:text-muhGold transition-colors">Info PPDB</a></li>
                    </ul>
                </div>

                <!-- Keorganisasian -->
                <div>
                    <h4 class="text-white font-bold mb-4 border-l-2 border-muhGold pl-3">Otomom Muhammadiyah</h4>
                    <ul class="space-y-2 text-sm">
                        <li><a href="#ekstrakurikuler" class="hover:text-muhGold transition-colors">PR IPM SMP Muh 1</a></li>
                        <li><a href="#ekstrakurikuler" class="hover:text-muhGold transition-colors">Pandu Hizbul Wathan</a></li>
                        <li><a href="#ekstrakurikuler" class="hover:text-muhGold transition-colors">Tapak Suci Putera Muhammadiyah</a></li>
                        <li><a href="https://muhammadiyah.or.id" target="_blank" rel="noopener" class="hover:text-muhGold transition-colors">PP Muhammadiyah</a></li>
                    </ul>
                </div>

                <!-- Media Sosial -->
                <div>
                    <h4 class="text-white font-bold mb-4 border-l-2 border-muhGold pl-3">Media Sosial</h4>
                    <p class="text-xs text-gray-400 mb-4">Ikuti akun resmi kami untuk mendapatkan pembaruan kegiatan siswa.</p>
                    <div class="flex gap-3">
                        <a href="#" class="w-10 h-10 bg-gray-800 text-white rounded-full flex items-center justify-center hover:bg-muhGreen hover:text-white transition-all" aria-label="Facebook">
                            <i class="fa-brands fa-facebook-f"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-gray-800 text-white rounded-full flex items-center justify-center hover:bg-muhGreen hover:text-white transition-all" aria-label="Instagram">
                            <i class="fa-brands fa-instagram"></i>
                        </a>
                        <a href="#" class="w-10 h-10 bg-gray-800 text-white rounded-full flex items-center justify-center hover:bg-muhGreen hover:text-white transition-all" aria-label="YouTube">
                            <i class="fa-brands fa-youtube"></i>
                        </a>
                    </div>
                </div>
            </div>

            <!-- Bottom Copyright -->
            <div class="pt-8 border-t border-gray-800 text-center text-xs text-gray-500">
                <p>&copy; 2026 SMP Muhammadiyah 1 Gadingrejo. Hak Cipta Dilindungi Undang-Undang.</p>
            </div>
        </div>
    </footer>

    <!-- ================= JAVASCRIPT ================= -->
    <script>
        // --- Mobile Menu Toggle ---
        const mobileMenuBtn = document.getElementById('mobile-menu-btn');
        const mobileMenu = document.getElementById('mobile-menu');
        const menuIcon = document.getElementById('menu-icon');

        mobileMenuBtn.addEventListener('click', () => {
            mobileMenu.classList.toggle('hidden');
            if (mobileMenu.classList.contains('hidden')) {
                menuIcon.classList.remove('fa-xmark');
                menuIcon.classList.add('fa-bars');
            } else {
                menuIcon.classList.remove('fa-bars');
                menuIcon.classList.add('fa-xmark');
            }
        });

        // Close mobile menu when clicking menu item
        document.querySelectorAll('.mobile-nav-link').forEach(link => {
            link.addEventListener('click', () => {
                mobileMenu.classList.add('hidden');
                menuIcon.classList.remove('fa-xmark');
                menuIcon.classList.add('fa-bars');
            });
        });

        // --- Navbar Shadow Effect on Scroll ---
        window.addEventListener('scroll', () => {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 20) {
                navbar.classList.add('shadow-md');
            } else {
                navbar.classList.remove('shadow-md');
            }
        });

        // --- Gallery Filter ---
        function filterGallery(category) {
            const items = document.querySelectorAll('.gallery-item');
            const buttons = document.querySelectorAll('.gallery-filter-btn');

            // Update button styles
            buttons.forEach(btn => {
                btn.classList.remove('bg-muhGreen', 'text-white', 'active');
                btn.classList.add('bg-white', 'text-gray-700');
            });
            event.target.classList.remove('bg-white', 'text-gray-700');
            event.target.classList.add('bg-muhGreen', 'text-white', 'active');

            // Show/Hide Items
            items.forEach(item => {
                if (category === 'all' || item.classList.contains(category)) {
                    item.style.display = 'block';
                } else {
                    item.style.display = 'none';
                }
            });
        }

        // --- Lightbox Functions ---
        function openLightbox(imgSrc, caption) {
            const lightbox = document.getElementById('lightbox');
            const lightboxImg = document.getElementById('lightbox-img');
            const lightboxCaption = document.getElementById('lightbox-caption');

            lightboxImg.src = imgSrc;
            lightboxCaption.textContent = caption;
            lightbox.classList.remove('hidden');
        }

        function closeLightbox() {
            document.getElementById('lightbox').classList.add('hidden');
        }

        // --- Form Handling ---
        function handleSubmit(e) {
            e.preventDefault();
            const alertBox = document.getElementById('form-alert');
            const name = document.getElementById('name').value;

            // Show Feedback Alert
            alertBox.className = "mb-6 p-4 rounded-xl text-sm font-medium bg-green-100 border border-green-300 text-green-800";
            alertBox.innerHTML = `<i class="fa-solid fa-circle-check mr-2"></i> Terima kasih, <strong>${name}</strong>! Pesan Anda telah terkirim. Panitia/Admin kami akan segera menghubungi Anda melalui WhatsApp.`;
            alertBox.classList.remove('hidden');

            // Reset Form
            document.getElementById('contact-form').reset();

            // Auto hide message after 6 seconds
            setTimeout(() => {
                alertBox.classList.add('hidden');
            }, 6000);
        }
    </script>
</body>
</html>
```