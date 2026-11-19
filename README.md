<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Zakaria Ilham — Portofolio</title>
    
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;500;600;700&family=Syne:wght@700;800&display=swap" rel="stylesheet">

    <script>
        tailwind.config = {
            theme: {
                extend: {
                    fontFamily: {
                        syne: ['Syne', 'sans-serif'],
                        sans: ['Plus Jakarta Sans', 'sans-serif'],
                    },
                    colors: {
                        dark: '#0c0c0c',
                        light: '#f7f7f7',
                        card: '#171717',
                        line: '#333333'
                    }
                }
            }
        }
    </script>
    <style>
        body {
            background-color: #0c0c0c;
            color: #f7f7f7;
            font-family: 'Plus Jakarta Sans', sans-serif;
            overflow-x: hidden;
        }
        .font-display {
            font-family: 'Syne', sans-serif;
        }
        .bg-dots {
            background-image: radial-gradient(rgba(255, 255, 255, 0.05) 1px, transparent 0);
            background-size: 24px 24px;
        }
        .text-outline {
            -webkit-text-stroke: 1.5px #f7f7f7;
            color: transparent;
        }
        .kotak-geo {
            transition: transform 0.3s ease, border-color 0.3s ease;
        }
        .kotak-geo:hover {
            transform: scale(0.95);
            border-color: #ffffff;
        }
        .menu-layar {
            clip-path: circle(0% at 50% 0%);
            transition: clip-path 0.6s ease-in-out;
        }
        .menu-layar.buka {
            clip-path: circle(150% at 50% 0%);
        }
    </style>
</head>
<body class="bg-dark text-light min-h-screen flex flex-col justify-between">

    <!-- Navbar -->
    <header class="fixed top-0 left-0 w-full z-50 mix-blend-difference px-6 sm:px-12 py-6 flex justify-between items-center">
        <div class="text-xs uppercase tracking-widest font-mono opacity-80 hidden md:block">
            Informatika — Sem. 3<br><span class="text-gray-400">255211009</span>
        </div>
        <div class="md:hidden text-xs uppercase tracking-widest font-mono">
            Zakaria Ilham
        </div>

        <button id="tombol-menu" class="group flex items-center space-x-3 cursor-pointer focus:outline-none z-50">
            <span class="text-xs font-mono uppercase tracking-widest group-hover:underline" id="teks-menu">Menu</span>
            <div class="w-6 h-4 flex flex-col justify-between items-end">
                <span class="w-full h-0.5 bg-light transition-transform duration-300" id="garis1"></span>
                <span class="w-3/4 h-0.5 bg-light transition-transform duration-300 group-hover:w-full" id="garis2"></span>
                <span class="w-full h-0.5 bg-light transition-transform duration-300" id="garis3"></span>
            </div>
        </button>

        <div class="text-xs uppercase tracking-widest font-mono text-right hidden md:block">
            HIMAFORTIC<br><span class="text-gray-400">2026</span>
        </div>
    </header>

    <!-- Menu Fullscreen -->
    <div id="overlay-menu" class="menu-layar fixed inset-0 bg-dark z-40 flex flex-col justify-between p-8 sm:p-16 border-b border-line">
        <div class="flex justify-between items-center border-b border-line pb-6 text-xs font-mono uppercase text-gray-400">
            <span>Navigasi</span>
            <span>Informatika • 255211009</span>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-2 gap-12 my-auto items-center">
            <nav class="flex flex-col space-y-4">
                <a href="#home" class="link-menu text-5xl sm:text-7xl font-display font-bold uppercase hover:text-outline transition-all">01. Home</a>
                <a href="#proyek" class="link-menu text-5xl sm:text-7xl font-display font-bold uppercase hover:text-outline transition-all">02. Proyek</a>
                <a href="#playground" class="link-menu text-5xl sm:text-7xl font-display font-bold uppercase hover:text-outline transition-all">03. Eksplorasi</a>
                <a href="#tentang" class="link-menu text-5xl sm:text-7xl font-display font-bold uppercase hover:text-outline transition-all">04. Tentang</a>
                <a href="#footer" class="link-menu text-5xl sm:text-7xl font-display font-bold uppercase hover:text-outline transition-all">05. Info</a>
            </nav>

            <div class="space-y-8 border-l border-line pl-0 md:pl-12 hidden md:block">
                <div>
                    <h4 class="text-xs font-mono uppercase text-gray-400 mb-2">Profil Mahasiswa</h4>
                    <p class="text-2xl font-display">Zakaria Ilham</p>
                    <p class="text-sm text-gray-400 mt-1">Program Studi Informatika — Semester 3</p>
                </div>
                <div>
                    <h4 class="text-xs font-mono uppercase text-gray-400 mb-2">Organisasi & Sertifikasi</h4>
                    <ul class="space-y-1 text-sm font-mono text-gray-300">
                        <li>• Anggota HIMAFORTIC</li>
                    </ul>
                </div>
            </div>
        </div>

        <div class="flex justify-between items-center text-xs font-mono text-gray-500 pt-6 border-t border-line">
            <span>© ZAKARIA ILHAM</span>
            <span>INFORMATIKA</span>
        </div>
    </div>

    <main class="w-full pt-28 pb-16 px-4 sm:px-8 max-w-7xl mx-auto space-y-28">

        <!-- Bagian Utama (Hero) -->
        <section id="home" class="min-h-[82vh] flex flex-col justify-between relative border border-line bg-dark p-6 sm:p-12 overflow-hidden bg-dots">
            <div class="flex justify-between items-start text-xs font-mono tracking-wider text-gray-400 uppercase z-10">
                <div>
                    <p class="text-light font-bold">ZAKARIA ILHAM</p>
                    <p>Mahasiswa Informatika • NIM 255211009</p>
                </div>
                <div class="text-right">
                    <p>Semester 3 • HIMAFORTIC</p>
                    <p>Portofolio</p>
                </div>
            </div>

            <div class="my-12 grid grid-cols-1 lg:grid-cols-12 gap-8 items-center z-10">
                <div class="lg:col-span-7 space-y-4">
                    <h1 class="text-6xl sm:text-8xl xl:text-9xl font-display font-extrabold tracking-tighter uppercase leading-none">
                        WEB <br>
                        <span class="text-outline">DESIGN</span>
                    </h1>
                    <div class="flex items-center space-x-4">
                        <span class="w-12 h-1 bg-light"></span>
                        <h2 class="text-4xl sm:text-6xl xl:text-7xl font-display font-extrabold tracking-tight uppercase">Development
                        </h2>
                    </div>
                </div>

                <!-- Ganti nama file foto di bagian src di bawah ini -->
                <div class="lg:col-span-5 flex flex-col items-center justify-center">
                    <div class="w-64 h-80 sm:w-72 sm:h-96 border border-line bg-card overflow-hidden">
                        <img src= "<img width="1080" height="1073" alt="zakaria" src="https://github.com/user-attachments/assets/50ac1226-aaf6-4432-a688-a1cb942f96b7" />
" 
                             onerror="this.src='https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d"
                             alt="Foto Zakaria Ilham" 
                             class="w-full h-full object-cover grayscale contrast-125 transition-transform duration-500 hover:scale-105" />
                    </div>
                </div>
            </div>

            <div class="flex flex-col sm:flex-row justify-between items-start sm:items-end gap-4 pt-8 border-t border-line/60 z-10 text-xs font-mono text-gray-400">
                <span class="text-sm font-sans text-gray-300">Sederhana, Terstruktur, dan Bermanfaat.</span>
                <div class="flex space-x-6 uppercase">
                    <span>Cilacap</span>
                    <span>Love you</span>
                    <span>hihuuuu</span>
                </div>
            </div>
        </section>

        <!-- Kotak Interaktif -->
        <section id="playground" class="space-y-6">
            <div class="flex justify-between items-end border-b border-line pb-4">
                <div>
                    <span class="text-xs font-mono text-gray-400 uppercase">Latihan JavaScript</span>
                    <h2 class="text-3xl font-display font-bold uppercase">Eksplorasi Pola</h2>
                </div>
                <span class="text-xs font-mono text-gray-400 hidden sm:block">[ Arahkan kursor ke kotak ]</span>
            </div>

            <div id="wadah-pola" class="grid grid-cols-2 sm:grid-cols-4 md:grid-cols-6 lg:grid-cols-8 gap-3 p-4 bg-black border border-line"></div>
        </section>

        <!-- Daftar Tugas & Proyek -->
        <section id="proyek" class="space-y-12">
            <div class="flex justify-between items-end border-b border-line pb-4">
                <div>
                    <span class="text-xs font-mono text-gray-400 uppercase">Tugas Kuliah & Eksplorasi</span>
                    <h2 class="text-4xl sm:text-5xl font-display font-bold uppercase">Proyek & Tugas</h2>
                </div>
                <span class="text-xs font-mono text-gray-400">HIHUUU</span>
            </div>

            <!-- Proyek Utama -->
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-8 items-stretch border border-line bg-dark p-6 sm:p-10 hover:border-light transition-colors">
                <div class="lg:col-span-5 flex flex-col justify-between space-y-8">
                    <div class="space-y-4">
                        <span class="text-xs font-mono uppercase text-gray-400">Perancangan Sistem</span>
                        <h3 class="text-3xl sm:text-4xl font-display font-bold leading-tight">
                            Sistem Informasi Penjualan Daging Ayam Potong Segar
                        </h3>
                        <p class="text-sm text-gray-300 leading-relaxed">
                            Membuat rancangan sistem pemesanan, proses checkout, pembayaran, serta bukti pengiriman menggunakan Use Case, Sequence, dan Activity Diagram.
                        </p>
                    </div>

                    <div class="space-y-3 text-xs font-mono border-t border-line/60 pt-6">
                        <div class="flex justify-between">
                            <span class="text-gray-500">PENYUSUN</span>
                            <span>Zakaria Ilham</span>
                        </div>
                        <div class="flex justify-between">
                            <span class="text-gray-500">DOKUMEN</span>
                            <span>Diagram UML & Slide Presentasi</span>
                        </div>
                        <div class="flex justify-between">
                            <span class="text-gray-500">TAHUN</span>
                            <span>2026</span>
                        </div>
                    </div>
                </div>

                <div class="lg:col-span-7 bg-card min-h-[300px] flex items-center justify-center p-6 border border-line/50">
                    <div class="w-full h-full bg-black p-8 border border-light/20 flex flex-col justify-between">
                        <div class="flex justify-between text-xs font-mono text-gray-400">
                            <span>ZAKARIA ILHAM </span>
                            <span>UML MODELING</span>
                        </div>
                        <div class="my-8">
                            <h4 class="text-2xl sm:text-3xl font-display font-bold uppercase leading-snug">
                                Use Case • Sequence • Activity Diagram.<br>Alur Pemesanan & Pengiriman.
                            </h4>
                        </div>
                        <div class="flex justify-between text-xs font-mono border-t border-white/20 pt-4 text-gray-400">
                            <span>Informatika — Semester 3</span>
                            <span>HIHUUU</span>
                        </div>
                    </div>
                </div>
            </div>

            <!-- Proyek Lainnya -->
            <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
                <div class="border border-line bg-dark p-8 flex flex-col justify-between hover:border-light transition-colors">
                    <div class="space-y-6">
                        <div class="flex justify-between text-xs font-mono text-gray-500">
                            <span>Analisis Sistem</span>
                            <span>02</span>
                        </div>
                        <div class="w-full h-52 bg-card border border-line p-6 flex flex-col justify-between">
                            <div class="text-2xl sm:text-3xl font-display font-bold uppercase leading-tight">
                                Sistem Informasi<br>Perpustakaan Web
                            </div>
                            <span class="text-xs font-mono text-gray-400">SMA Negeri 2 Cilacap</span>
                        </div>
                        <h3 class="text-2xl font-display font-bold uppercase">Perancangan Use Case Perpustakaan</h3>
                        <p class="text-xs text-gray-400 leading-relaxed">
                            Tugas makalah dan pemetaan aktor serta alur peminjaman buku pada sistem informasi perpustakaan berbasis web di SMA Negeri 2 Cilacap.
                        </p>
                    </div>
                    <div class="pt-6 mt-6 border-t border-line flex justify-between text-xs font-mono text-gray-400">
                        <span>USE CASE DIAGRAM</span>
                        <span>HIHUUU</span>
                    </div>
                </div>

                <div class="border border-line bg-dark p-8 flex flex-col justify-between hover:border-light transition-colors">
                    <div class="space-y-6">
                        <div class="flex justify-between text-xs font-mono text-gray-500">
                            <span>Eksplorasi Teknis</span>
                            <span>03</span>
                        </div>
                        <div class="w-full h-52 bg-card border border-line p-6 flex flex-col justify-between">
                            <div class="text-2xl sm:text-3xl font-display font-bold uppercase leading-tight">
                                Python 3D Blender<br>& OBS Studio
                            </div>
                            <span class="text-xs font-mono text-gray-400">Scripting & Live Setup</span>
                        </div>
                        <h3 class="text-2xl font-display font-bold uppercase">3D Scripting & Tampilan Streaming</h3>
                        <p class="text-xs text-gray-400 leading-relaxed">
                            Membuat objek furnitur 3D di Blender menggunakan skrip Python serta mengatur tampilan running text dan panel kontrol pada OBS Studio.
                        </p>
                    </div>
                    <div class="pt-6 mt-6 border-t border-line flex justify-between text-xs font-mono text-gray-400">
                        <span>PYTHON • BLENDER • OBS</span>
                        <span>HIHUUU</span>
                    </div>
                </div>
            </div>
        </section>

        <!-- Tentang Saya & Keluarga -->
        <section id="tentang" class="border border-line p-8 sm:p-16 space-y-12 bg-dots">
            <div class="grid grid-cols-1 lg:grid-cols-12 gap-12 items-start">
                <div class="lg:col-span-4 space-y-3">
                    <span class="text-xs font-mono uppercase text-gray-400">Tentang Saya</span>
                    <h2 class="text-4xl font-display font-bold uppercase">Zakaria Ilham</h2>
                    <p class="text-xs font-mono text-gray-400">NIM: 255211009 • Informatika</p>
                </div>

                <div class="lg:col-span-8 space-y-8 text-gray-300 leading-relaxed text-base">
                    <p>
                        Mahasiswa Informatika Semester 3 yang berfokus pada eksplorasi antarmuka web, pemodelan sistem, dan otomasi kreatif. Saya percaya bahwa kode yang bersih dan desain yang terstruktur adalah kunci untuk menciptakan pengalaman digital yang bermakna.
                    </p>

                    <div class="border border-line bg-card/60 p-6 space-y-2">
                        <span class="text-xs font-mono uppercase tracking-wider text-light font-bold block">Ruang Keluarga</span>
                        <p class="text-sm text-gray-300 leading-relaxed">
                            Di balik setiap baris kode dan pencapaian akademik, ada doa dan dukungan keluarga yang menjadi fondasi utama. Ruang kecil ini didedikasikan untuk kebersamaan dan nilai kesederhanaan yang selalu menjadi pegangan dalam setiap langkah.
                        </p>
                    </div>

                    <div class="grid grid-cols-1 sm:grid-cols-3 gap-8 pt-6 border-t border-line font-mono text-xs">
                        <div>
                            <h4 class="text-light font-bold mb-2 uppercase">Yang Dipelajari</h4>
                            <ul class="space-y-1 text-gray-400">
                                <li>HTML5 & CSS3</li>
                                <li>Diagram UML</li>
                                <li>Python di Blender</li>
                                <li>OBS Studio</li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="text-light font-bold mb-2 uppercase">Sertifikasi</h4>
                            <ul class="space-y-1 text-gray-400">
                                <li>UX Design Professional Certificate</li>
                            </ul>
                        </div>
                        <div>
                            <h4 class="text-light font-bold mb-2 uppercase">Organisasi</h4>
                            <ul class="space-y-1 text-gray-400">
                                <li>HIMAFORTIC</li>
                                <li>MSSC</li>
                                <li>Informatika Sem. 3</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Footer -->
        <footer id="footer" class="border-t border-line pt-12 space-y-10">
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8 font-mono text-xs">
                <div>
                    <span class="text-gray-500 block mb-1">NAMA</span>
                    <p class="text-base font-sans font-semibold">Zakaria Ilham</p>
                </div>
                <div>
                    <span class="text-gray-500 block mb-1">NIM & JURUSAN</span>
                    <p class="text-base font-sans font-semibold">255211009 — Informatika</p>
                </div>
                <div>
                    <span class="text-gray-500 block mb-1">ORGANISASI</span>
                    <p class="text-base font-sans font-semibold">HIMAFORTIC</p>
                </div>
            </div>

            <div class="flex justify-between items-center text-xs font-mono text-gray-500 pt-8 border-t border-line/50">
                <span>© 2026 Zakaria Ilham</span>
                <button onclick="window.scrollTo({top: 0, behavior: 'smooth'})" class="hover:text-light uppercase cursor-pointer">Ke Atas ↑</button>
            </div>
        </footer>

    </main>

    <script>
        // Kontrol buka-tutup menu
        const tombolMenu = document.getElementById('tombol-menu');
        const overlayMenu = document.getElementById('overlay-menu');
        const teksMenu = document.getElementById('teks-menu');
        const garis1 = document.getElementById('garis1');
        const garis2 = document.getElementById('garis2');
        const garis3 = document.getElementById('garis3');
        const linkMenu = document.querySelectorAll('.link-menu');
        let terbuka = false;

        function ubahMenu() {
            terbuka = !terbuka;
            if (terbuka) {
                overlayMenu.classList.add('buka');
                teksMenu.textContent = 'Tutup';
                garis1.style.transform = 'translateY(7px) rotate(45deg)';
                garis2.style.opacity = '0';
                garis3.style.transform = 'translateY(-7px) rotate(-45deg)';
            } else {
                overlayMenu.classList.remove('buka');
                teksMenu.textContent = 'Menu';
                garis1.style.transform = 'none';
                garis2.style.opacity = '1';
                garis3.style.transform = 'none';
            }
        }

        tombolMenu.addEventListener('click', ubahMenu);
        linkMenu.forEach(item => {
            item.addEventListener('click', () => {
                if (terbuka) ubahMenu();
            });
        });

        // Pola geometris interaktif
        const wadahPola = document.getElementById('wadah-pola');
        const bentuk = [
            '<circle cx="50" cy="50" r="30" fill="none" stroke="currentColor" stroke-width="2"/>',
            '<rect x="20" y="20" width="60" height="60" fill="none" stroke="currentColor" stroke-width="2"/>',
            '<polygon points="50,15 85,80 15,80" fill="none" stroke="currentColor" stroke-width="2"/>',
            '<line x1="15" y1="15" x2="85" y2="85" stroke="currentColor" stroke-width="2"/><line x1="85" y1="15" x2="15" y2="85" stroke="currentColor" stroke-width="2"/>',
            '<circle cx="50" cy="50" r="14" fill="currentColor"/>'
        ];

        function acakBentuk() {
            return bentuk[Math.floor(Math.random() * bentuk.length)];
        }

        for (let i = 0; i < 24; i++) {
            const kotak = document.createElement('div');
            kotak.className = 'kotak-geo aspect-square border border-line/60 bg-card/40 flex items-center justify-center p-4 text-light cursor-pointer';
            kotak.innerHTML = `<svg viewBox="0 0 100 100" class="w-full h-full transition-transform duration-300">${acakBentuk()}</svg>`;
            
            kotak.addEventListener('mouseenter', () => {
                const putar = Math.floor(Math.random() * 4) * 90;
                kotak.innerHTML = `<svg viewBox="0 0 100 100" style="transform: rotate(${putar}deg)" class="w-full h-full transition-transform duration-300">${acakBentuk()}</svg>`;
            });

            wadahPola.appendChild(kotak);
        }
    </script>
</body>
</html>
