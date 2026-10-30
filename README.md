<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>NILO Cakes & Decor - Trang Trí Sinh Nhật & Sự Kiện Đà Nẵng</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Inter & FontAwesome Icons -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        nilo: {
                            50: '#fdf2f4',
                            100: '#fbe8ec',
                            500: '#e11d48',
                            600: '#be123c',
                            700: '#9f1239',
                        }
                    },
                    fontFamily: {
                        sans: ['Inter', 'sans-serif'],
                    }
                }
            }
        }
    </script>
    <style>
        body { font-family: 'Inter', sans-serif; scroll-behavior: smooth; }
        .flatsome-shadow { box-shadow: 0 2px 10px rgba(0,0,0,0.06); }
        .card-hover:hover { transform: translateY(-4px); transition: all 0.3s ease; }
        .cat-img-zoom:hover img { transform: scale(1.08); }
        @keyframes pulse-ring {
            0% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(225, 29, 72, 0.7); }
            70% { transform: scale(1); box-shadow: 0 0 0 12px rgba(225, 29, 72, 0); }
            100% { transform: scale(0.95); box-shadow: 0 0 0 0 rgba(225, 29, 72, 0); }
        }
        .hotline-pulse { animation: pulse-ring 2s infinite; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 antialiased">

    <!-- Top Bar (Clean, no UX builder editor text) -->
    <div class="bg-gray-900 text-gray-300 text-xs py-2 px-4">
        <div class="max-w-7xl mx-auto flex flex-col sm:flex-row justify-between items-center gap-1">
            <div class="flex items-center gap-4">
                <span><i class="fa-solid fa-location-dot text-nilo-500 mr-1"></i> 12 Phú Lộc 3, Thanh Khê, Đà Nẵng</span>
                <span class="hidden md:inline"><i class="fa-solid fa-clock text-nilo-500 mr-1"></i> 8:00 - 21:00 (T2 - CN)</span>
            </div>
            <div class="flex items-center gap-3">
                <a href="tel:0905400344" class="hover:text-white font-medium"><i class="fa-solid fa-phone text-nilo-500 mr-1"></i> 0905.400.344</a>
                <span>-</span>
                <a href="tel:0377794379" class="hover:text-white font-medium">0377.794.379</a>
            </div>
        </div>
    </div>

    <!-- Header Section (Flatsome Style Header) -->
    <header class="bg-white border-b border-gray-200 sticky top-0 z-40 flatsome-shadow">
        <div class="max-w-7xl mx-auto px-4 py-3 flex items-center justify-between gap-3">
            <!-- Mobile Menu Button -->
            <button class="md:hidden text-gray-700 text-xl focus:outline-none p-2" onclick="toggleMobileMenu()" aria-label="Menu">
                <i class="fa-solid fa-bars"></i>
            </button>

            <!-- Logo NILO Cakes & Decor (Fanpage Logo style + Fallback) -->
            <div class="flex items-center gap-2.5">
                <a href="#" class="flex items-center gap-3 group">
                    <div class="relative w-12 h-12 md:w-14 md:h-14 rounded-full overflow-hidden border-2 border-nilo-500 shadow-sm shrink-0 bg-nilo-50 flex items-center justify-center">
                        <!-- Tự động lấy ảnh đại diện Fanpage hoặc hiển thị Logo chuẩn của NILO Cakes & Decor -->
                        <img src="https://graph.facebook.com/nilodecor.danang/picture?type=large" 
                             alt="NILO Cakes & Decor Logo" 
                             class="w-full h-full object-cover"
                             onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
                        <div style="display:none;" class="w-full h-full bg-gradient-to-br from-nilo-500 to-rose-700 text-white flex-col items-center justify-center text-center p-1">
                            <i class="fa-solid fa-cake-candles text-sm md:text-base mb-0.5"></i>
                            <span class="text-[10px] font-extrabold tracking-wider leading-none">NILO</span>
                        </div>
                    </div>
                    <div>
                        <span class="text-lg md:text-xl font-extrabold tracking-tight text-gray-900 block leading-tight group-hover:text-nilo-600 transition">NILO CAKES & DECOR</span>
                        <span class="text-[11px] text-nilo-600 font-semibold block">Bánh Kem • Chibi • Trang Trí Tiệc Đà Nẵng</span>
                    </div>
                </a>
            </div>

            <!-- Search Bar (Desktop) -->
            <div class="hidden lg:flex flex-1 max-w-md mx-4">
                <div class="relative w-full">
                    <input type="text" placeholder="Tìm mẫu sinh nhật bé trai, bé gái, thôi nôi, bánh kem..." class="w-full bg-gray-100 border border-gray-300 rounded-full px-4 py-2 text-sm focus:outline-none focus:border-nilo-500 focus:bg-white transition">
                    <button class="absolute right-1 top-1 bottom-1 bg-nilo-500 text-white px-4 rounded-full hover:bg-nilo-600 transition">
                        <i class="fa-solid fa-search text-xs"></i>
                    </button>
                </div>
            </div>

            <!-- Right Actions (Added Prominent Hotline Button + Zalo + Fanpage) -->
            <div class="flex items-center gap-2">
                <a href="tel:0905400344" class="flex items-center gap-1.5 bg-nilo-500 text-white px-3.5 py-2 rounded-full text-xs font-bold hover:bg-nilo-600 transition shadow-sm">
                    <i class="fa-solid fa-phone-volume animate-pulse"></i>
                    <span class="hidden sm:inline">0905.400.344</span>
                    <span class="sm:hidden">Gọi</span>
                </a>
                <a href="https://zalo.me/0905400344" target="_blank" class="hidden sm:flex items-center gap-1.5 bg-sky-50 text-sky-600 border border-sky-200 px-3 py-2 rounded-full text-xs font-semibold hover:bg-sky-500 hover:text-white transition">
                    <i class="fa-solid fa-comment-dots"></i> Zalo
                </a>
                <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="flex items-center gap-1.5 bg-blue-50 text-blue-600 border border-blue-200 px-3 py-2 rounded-full text-xs font-semibold hover:bg-blue-600 hover:text-white transition">
                    <i class="fa-brands fa-facebook"></i> <span class="hidden md:inline">Fanpage</span>
                </a>
            </div>
        </div>

        <!-- Navigation Menu Bar (Categories synced with huyparty.com) -->
        <nav class="bg-white border-t border-gray-100 hidden md:block">
            <div class="max-w-7xl mx-auto px-4 flex items-center justify-between">
                <ul class="flex space-x-6 text-xs lg:text-sm font-semibold py-3 text-gray-700">
                    <li><a href="#" class="text-nilo-600 hover:text-nilo-700">TRANG CHỦ</a></li>
                    <li><a href="#danhmuc" class="hover:text-nilo-600 transition">DANH MỤC TRANG TRÍ</a></li>
                    <li><a href="#betrai" class="hover:text-nilo-600 transition">SINH NHẬT BÉ TRAI</a></li>
                    <li><a href="#begai" class="hover:text-nilo-600 transition">SINH NHẬT BÉ GÁI</a></li>
                    <li><a href="#thoinoi" class="hover:text-nilo-600 transition">TRANG TRÍ THÔI NÔI</a></li>
                    <li><a href="#setdecor" class="hover:text-nilo-600 transition">SET TỰ DECOR & BÁNH KEM</a></li>
                    <li><a href="#khaitruong" class="hover:text-nilo-600 transition">KHAI TRƯƠNG & SỰ KIỆN</a></li>
                    <li><a href="#diachi" class="hover:text-nilo-600 transition">BẢN ĐỒ</a></li>
                </ul>
            </div>
        </nav>

        <!-- Mobile Menu Drawer (Hidden by default) -->
        <div id="mobileMenu" class="hidden md:hidden bg-white border-b border-gray-200 px-4 pt-2 pb-4 space-y-2 text-sm font-medium">
            <a href="#" class="block py-2 text-nilo-600 font-bold border-b border-gray-100">Trang Chủ</a>
            <a href="#danhmuc" class="block py-2 text-gray-700 border-b border-gray-100">Danh Mục Trang Trí</a>
            <a href="#betrai" class="block py-2 text-gray-700 border-b border-gray-100">Trang Trí Sinh Nhật Bé Trai</a>
            <a href="#begai" class="block py-2 text-gray-700 border-b border-gray-100">Trang Trí Sinh Nhật Bé Gái</a>
            <a href="#thoinoi" class="block py-2 text-gray-700 border-b border-gray-100">Trang Trí Thôi Nôi Đà Nẵng</a>
            <a href="#setdecor" class="block py-2 text-gray-700 border-b border-gray-100">Set Sinh Nhật Tự Decor & Bánh Kem</a>
            <a href="#khaitruong" class="block py-2 text-gray-700 border-b border-gray-100">Trang Trí Khai Trương & Phòng Cưới</a>
            <a href="#diachi" class="block py-2 text-gray-700">Địa Chỉ & Bản Đồ</a>
        </div>
    </header>

    <!-- Hero Banner Section -->
    <section class="relative bg-gradient-to-r from-rose-900 via-nilo-700 to-rose-800 text-white py-10 md:py-16 px-4 overflow-hidden">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-2 gap-8 items-center relative z-10">
            <div class="space-y-4">
                <div class="inline-flex items-center gap-2 bg-white/15 backdrop-blur-sm px-3.5 py-1.5 rounded-full text-xs font-semibold tracking-wide">
                    <i class="fa-solid fa-star text-yellow-300"></i> NILO CAKES & DECOR - NILOPARTY.COM
                </div>
                <h1 class="text-3xl md:text-5xl font-extrabold tracking-tight leading-tight">
                    Trang Trí Sinh Nhật, Thôi Nôi & Bánh Kem Đà Nẵng
                </h1>
                <p class="text-rose-100 text-sm md:text-base leading-relaxed">
                    Chuyên thiết kế & thi công backdrop sinh nhật bé trai, bé gái, thôi nôi, khai trương, bóng bay nghệ thuật, phụ kiện Chibi và các mẫu bánh kem tạo hình theo yêu cầu tại Đà Nẵng.
                </p>
                <div class="flex flex-wrap gap-3 pt-2">
                    <a href="tel:0905400344" class="bg-white text-nilo-700 font-bold px-6 py-3 rounded-lg shadow-md hover:bg-rose-50 transition text-sm flex items-center">
                        <i class="fa-solid fa-phone-volume mr-2 text-nilo-600"></i> Hotline: 0905.400.344
                    </a>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-sky-500 hover:bg-sky-600 text-white font-bold px-6 py-3 rounded-lg shadow-md transition text-sm flex items-center">
                        <i class="fa-solid fa-comment-dots mr-2"></i> Tư Vấn Qua Zalo
                    </a>
                    <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="border border-white/40 hover:bg-white/10 text-white font-semibold px-5 py-3 rounded-lg transition text-sm flex items-center">
                        <i class="fa-brands fa-facebook mr-2"></i> Xem Fanpage
                    </a>
                </div>
            </div>
            <div>
                <div class="bg-white/10 backdrop-blur-md p-3 rounded-2xl border border-white/20 shadow-2xl grid grid-cols-2 gap-3">
                    <img src="https://images.unsplash.com/photo-1530103862676-de8c9debad1d?auto=format&fit=crop&w=600&q=80" alt="Trang trí sinh nhật Đà Nẵng" class="rounded-xl w-full h-40 md:h-52 object-cover">
                    <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=600&q=80" alt="Bánh kem sinh nhật NILO" class="rounded-xl w-full h-40 md:h-52 object-cover">
                    <img src="https://images.unsplash.com/photo-1513151233558-d860c5398176?auto=format&fit=crop&w=600&q=80" alt="Bong bóng nghệ thuật" class="rounded-xl w-full h-36 md:h-44 object-cover">
                    <img src="https://images.unsplash.com/photo-1464349153735-7db50ed83c84?auto=format&fit=crop&w=600&q=80" alt="Tiệc thôi nôi cho bé" class="rounded-xl w-full h-36 md:h-44 object-cover">
                </div>
            </div>
        </div>
    </section>

    <!-- Categories Section (Designed after huyparty.com & optimized for Desktop + Mobile) -->
    <section id="danhmuc" class="max-w-7xl mx-auto px-4 py-10">
        <div class="text-center mb-8">
            <span class="text-nilo-600 font-bold text-xs uppercase tracking-widest">NILO PARTY & DECOR</span>
            <h2 class="text-2xl md:text-3xl font-extrabold text-gray-900 mt-1">Danh Mục Trang Trí Sinh Nhật & Sự Kiện</h2>
            <div class="w-16 h-1 bg-nilo-500 mx-auto mt-2 rounded-full"></div>
        </div>

        <!-- 8 Visual Categories: 2 cols on mobile, 4 cols on tablet, 8 cols on desktop -->
        <div class="grid grid-cols-2 sm:grid-cols-4 lg:grid-cols-8 gap-3 md:gap-4">
            <!-- Cat 1 -->
            <a href="#betrai" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1530103862676-de8c9debad1d?auto=format&fit=crop&w=300&q=80" alt="Sinh Nhật Bé Trai" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Sinh Nhật Bé Trai</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Safari, Rồng, Gấu</span>
            </a>

            <!-- Cat 2 -->
            <a href="#begai" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=300&q=80" alt="Sinh Nhật Bé Gái" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Sinh Nhật Bé Gái</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Công chúa, Thỏ hồng</span>
            </a>

            <!-- Cat 3 -->
            <a href="#thoinoi" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1464349153735-7db50ed83c84?auto=format&fit=crop&w=300&q=80" alt="Trang Trí Thôi Nôi" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Tiệc Thôi Nôi</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Bé 1 tuổi, Đầy tháng</span>
            </a>

            <!-- Cat 4 -->
            <a href="#setdecor" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1513151233558-d860c5398176?auto=format&fit=crop&w=300&q=80" alt="Set Sinh Nhật Tự Decor" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Set Tự Decor</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Trọn gói tại nhà</span>
            </a>

            <!-- Cat 5 -->
            <a href="#setdecor" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=300&q=80" alt="Bánh Kem & Chibi" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Bánh Kem & Chibi</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Thiết kế theo mẫu</span>
            </a>

            <!-- Cat 6 -->
            <a href="#khaitruong" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1511795409834-ef04bbd61622?auto=format&fit=crop&w=300&q=80" alt="Trang Trí Khai Trương" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Khai Trương</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Backdrop, Cổng bóng</span>
            </a>

            <!-- Cat 7 -->
            <a href="#khaitruong" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1522673607200-164d1b6ce486?auto=format&fit=crop&w=300&q=80" alt="Bóng Bay Phòng Cưới" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Phòng Tân Hôn</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Bóng Jumbo, Tình yêu</span>
            </a>

            <!-- Cat 8 -->
            <a href="#khaitruong" class="bg-white p-3 rounded-xl shadow-sm border border-gray-100 text-center card-hover cat-img-zoom group">
                <div class="w-20 h-20 mx-auto mb-2.5 rounded-full overflow-hidden border-2 border-rose-100 group-hover:border-nilo-500 transition">
                    <img src="https://images.unsplash.com/photo-1504196606672-aef5c9cefc92?auto=format&fit=crop&w=300&q=80" alt="Chú Hề Hoạt Náo" class="w-full h-full object-cover transition duration-300">
                </div>
                <h3 class="font-bold text-xs md:text-sm text-gray-800 group-hover:text-nilo-600">Chú Hề & Sự Kiện</h3>
                <span class="text-[11px] text-gray-400 block mt-0.5">Vặn bóng, Hoạt náo</span>
            </a>
        </div>
    </section>

    <!-- CATEGORY 1: TRANG TRÍ SINH NHẬT BÉ TRAI (2 columns on mobile, 4 on desktop, NO stickers) -->
    <section id="betrai" class="max-w-7xl mx-auto px-4 py-8">
        <div class="flex justify-between items-center border-b border-gray-200 pb-3 mb-6">
            <div class="flex items-center gap-2">
                <span class="w-2 h-6 bg-nilo-500 rounded-full"></span>
                <h2 class="text-xl md:text-2xl font-bold text-gray-900">Trang Trí Sinh Nhật Bé Trai</h2>
            </div>
            <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="text-xs md:text-sm font-semibold text-nilo-600 hover:underline">Xem thêm mẫu <i class="fa-solid fa-angle-right ml-1"></i></a>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-4 gap-3 md:gap-6">
            <!-- Item 1 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1530103862676-de8c9debad1d?auto=format&fit=crop&w=500&q=80" alt="Mẫu Duy Anh – Safari Pastel Sang Trọng" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Trai</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Duy Anh – Safari Pastel Sang Trọng (Backdrop 4m x 2m4)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 2 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1513151233558-d860c5398176?auto=format&fit=crop&w=500&q=80" alt="Mẫu Đăng Khôi – Rồng Baby" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Trai</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Đăng Khôi – Rồng Baby Dễ Thương (Khung Tròn 2m4 x 2m4)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 3 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1504196606672-aef5c9cefc92?auto=format&fit=crop&w=500&q=80" alt="Mẫu Wilson – Gấu Phi Công" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Trai</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Wilson – Gấu Phi Công Baby (Backdrop 2m4 x 2m4)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 4 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1527529482837-4698179dc6ce?auto=format&fit=crop&w=500&q=80" alt="Mẫu Khôi Vỹ – Phi Hành Gia" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Trai</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Khôi Vỹ – Chủ Đề Phi Hành Gia & Vũ Trụ (2m4 x 2m)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>
        </div>
    </section>

    <!-- CATEGORY 2: TRANG TRÍ SINH NHẬT BÉ GÁI & THÔI NÔI (2 columns on mobile, 4 on desktop) -->
    <section id="begai" class="max-w-7xl mx-auto px-4 py-8">
        <div id="thoinoi" class="flex justify-between items-center border-b border-gray-200 pb-3 mb-6">
            <div class="flex items-center gap-2">
                <span class="w-2 h-6 bg-nilo-500 rounded-full"></span>
                <h2 class="text-xl md:text-2xl font-bold text-gray-900">Trang Trí Sinh Nhật Bé Gái & Tiệc Thôi Nôi</h2>
            </div>
            <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="text-xs md:text-sm font-semibold text-nilo-600 hover:underline">Xem thêm mẫu <i class="fa-solid fa-angle-right ml-1"></i></a>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-4 gap-3 md:gap-6">
            <!-- Item 1 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=500&q=80" alt="Sinh Nhật Bé Gái Công Chúa Pastel" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Gái</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Bảo Ngọc – Công Chúa Thỏ Hồng Pastel Ngọt Ngào</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 2 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1464349153735-7db50ed83c84?auto=format&fit=crop&w=500&q=80" alt="Trang Trí Thôi Nôi Bé 1 Tuổi" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Tiệc Thôi Nôi</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Trang Trí Thôi Nôi Khung Chữ U & Bục Kệ Chibi Cho Bé 1 Tuổi</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 3 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1519225421980-715cb0215aed?auto=format&fit=crop&w=500&q=80" alt="Mẫu Mèo Cam Baby" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Sinh Nhật Bé Gái</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Hải Đăng – Mèo Ken Dễ Thương Phối Bóng Nghệ Thuật (4m x 2m4)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>

            <!-- Item 4 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1522673607200-164d1b6ce486?auto=format&fit=crop&w=500&q=80" alt="Backdrop Trắng Bạc Hiện Đại" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Thôi Nôi & Sinh Nhật</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Mẫu Thiên Minh – Backdrop Khung Tròn 2m3 Kèm Đèn LED Lung Linh</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Tư vấn</a>
                </div>
            </div>
        </div>
    </section>

    <!-- CATEGORY 3: SET TỰ DECOR, BÁNH KEM NILO & KHAI TRƯƠNG (2 columns on mobile, 4 on desktop) -->
    <section id="setdecor" class="max-w-7xl mx-auto px-4 py-8">
        <div id="khaitruong" class="flex justify-between items-center border-b border-gray-200 pb-3 mb-6">
            <div class="flex items-center gap-2">
                <span class="w-2 h-6 bg-nilo-500 rounded-full"></span>
                <h2 class="text-xl md:text-2xl font-bold text-gray-900">Bánh Kem Thiết Kế, Set Tự Decor & Khai Trương</h2>
            </div>
            <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="text-xs md:text-sm font-semibold text-nilo-600 hover:underline">Xem tất cả <i class="fa-solid fa-angle-right ml-1"></i></a>
        </div>

        <div class="grid grid-cols-2 md:grid-cols-4 gap-3 md:gap-6">
            <!-- Item 1 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?auto=format&fit=crop&w=500&q=80" alt="Bánh Kem Sinh Nhật Thiết Kế NILO" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">NILO Cakes</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Bánh Kem Sinh Nhật Tạo Hình Theo Chủ Đề Tiệc (Ít Ngọt, Cốt Mềm)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Đặt bánh</a>
                </div>
            </div>

            <!-- Item 2 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1535141192574-5d4897c12636?auto=format&fit=crop&w=500&q=80" alt="Set Sinh Nhật Tự Decor Tại Nhà" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Set Tự Decor</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Set Sinh Nhật Tự Decor Thiết Kế Theo Tên Bé (Tặng Kèm Bơm & Phụ Kiện)</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">499.000đ</span>
                    <a href="https://zalo.me/0905400344" target="_blank" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Mua ngay</a>
                </div>
            </div>

            <!-- Item 3 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1511795409834-ef04bbd61622?auto=format&fit=crop&w=500&q=80" alt="Trang Trí Khai Trương Đà Nẵng" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Khai Trương</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Backdrop Khai Trương Cửa Hàng, Spa & Boutique Sang Trọng Đà Nẵng</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Báo giá</a>
                </div>
            </div>

            <!-- Item 4 -->
            <div class="bg-white rounded-xl shadow-sm border border-gray-100 overflow-hidden card-hover flex flex-col justify-between">
                <div>
                    <div class="overflow-hidden bg-gray-100 aspect-square">
                        <img src="https://images.unsplash.com/photo-1507504031003-b417219a0fde?auto=format&fit=crop&w=500&q=80" alt="Bóng Bay Phòng Tân Hôn & Sinh Nhật Người Lớn" class="w-full h-full object-cover">
                    </div>
                    <div class="p-3">
                        <span class="text-[11px] text-gray-400 uppercase">Bóng Nghệ Thuật</span>
                        <h3 class="font-semibold text-sm text-gray-800 line-clamp-2 mt-0.5">Combo Bơm Bóng Bay Phòng Tân Hôn & Trang Trí Sinh Nhật Người Lớn</h3>
                    </div>
                </div>
                <div class="p-3 pt-0 flex items-center justify-between">
                    <span class="text-nilo-600 font-bold text-sm">Liên hệ</span>
                    <a href="tel:0905400344" class="bg-nilo-50 text-nilo-600 hover:bg-nilo-500 hover:text-white text-xs font-semibold px-3 py-1.5 rounded-lg transition">Đặt lịch</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Address & Map Section (Map image/embed out to homepage) -->
    <section id="diachi" class="max-w-7xl mx-auto px-4 py-10">
        <div class="bg-white rounded-2xl shadow-sm border border-gray-200 overflow-hidden grid grid-cols-1 md:grid-cols-2">
            <div class="p-6 md:p-10 flex flex-col justify-center space-y-4">
                <span class="text-nilo-600 font-bold text-xs uppercase tracking-wider">Địa Chỉ & Bản Đồ Chỉ Đường</span>
                <h2 class="text-2xl md:text-3xl font-bold text-gray-900">NILO Cakes & Decor Đà Nẵng</h2>
                <p class="text-gray-600 text-sm">Chuyên cung cấp dịch vụ trang trí tiệc sinh nhật, thôi nôi, khai trương, phụ kiện Chibi và các mẫu bánh kem thiết kế riêng tại Đà Nẵng.</p>
                
                <div class="space-y-3 pt-2 text-sm">
                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-location-dot"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Địa chỉ cửa hàng:</span>
                            <span class="text-gray-600">12 Phú Lộc 3, Thanh Khê, Đà Nẵng</span>
                        </div>
                    </div>
                    
                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-phone"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Hotline / Zalo tư vấn 24/7:</span>
                            <a href="tel:0905400344" class="text-nilo-600 font-bold hover:underline">0905.400.344</a> - <a href="tel:0377794379" class="text-nilo-600 font-bold hover:underline">0377.794.379</a>
                        </div>
                    </div>

                    <div class="flex items-start gap-3">
                        <div class="bg-nilo-50 text-nilo-600 p-2.5 rounded-lg shrink-0">
                            <i class="fa-solid fa-globe"></i>
                        </div>
                        <div>
                            <span class="font-semibold block text-gray-800">Website & Fanpage:</span>
                            <span class="text-gray-600">niloparty.com | fb.com/nilodecor.danang</span>
                        </div>
                    </div>
                </div>

                <div class="pt-3 flex flex-wrap gap-3">
                    <a href="https://maps.app.goo.gl/e5YRjwo3E7bB7oao6" target="_blank" class="bg-nilo-500 hover:bg-nilo-600 text-white px-5 py-2.5 rounded-lg text-sm font-semibold transition shadow-sm">
                        <i class="fa-solid fa-map-location-dot mr-2"></i> Mở Google Maps Chỉ Đường
                    </a>
                    <a href="tel:0905400344" class="bg-gray-900 hover:bg-gray-800 text-white px-5 py-2.5 rounded-lg text-sm font-semibold transition shadow-sm">
                        <i class="fa-solid fa-phone mr-2"></i> Gọi Ngay: 0905.400.344
                    </a>
                </div>
            </div>

            <!-- Interactive Google Map Embed + Link Out on Homepage -->
            <div class="relative bg-gray-100 min-h-[320px] flex flex-col">
                <iframe 
                    src="https://www.google.com/maps?q=12+Ph%C3%BA+L%E1%BB%99c+3,+Thanh+Kh%C3%AA,+%C4%90%C3%A0+N%E1%BA%B5ng&output=embed" 
                    class="w-full h-full min-h-[320px] border-0" 
                    allowfullscreen="" 
                    loading="lazy" 
                    referrerpolicy="no-referrer-when-downgrade"
                    title="Bản đồ NILO Cakes & Decor 12 Phú Lộc 3">
                </iframe>
                <a href="https://maps.app.goo.gl/e5YRjwo3E7bB7oao6" target="_blank" class="absolute bottom-3 right-3 bg-white/95 backdrop-blur-sm border border-gray-200 text-gray-900 hover:text-nilo-600 px-3.5 py-2 rounded-lg text-xs font-bold shadow-md transition">
                    <i class="fa-solid fa-up-right-from-square mr-1 text-nilo-500"></i> Xem trên ứng dụng Google Maps
                </a>
            </div>
        </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-gray-900 text-gray-400 py-10 px-4 mt-8 text-sm">
        <div class="max-w-7xl mx-auto grid grid-cols-1 md:grid-cols-3 gap-8 mb-8">
            <div>
                <h3 class="text-white font-bold text-base mb-3">NILO CAKES & DECOR - NILOPARTY.COM</h3>
                <p class="text-xs leading-relaxed text-gray-400 mb-3">Dịch vụ trang trí sinh nhật, thôi nôi, khai trương, bóng bay nghệ thuật, in ấn Chibi và bánh kem thiết kế theo yêu cầu uy tín tại Đà Nẵng.</p>
                <p class="text-xs text-gray-300"><i class="fa-solid fa-location-dot text-nilo-500 mr-1.5"></i> 12 Phú Lộc 3, Thanh Khê, Đà Nẵng</p>
            </div>
            <div>
                <h3 class="text-white font-bold text-base mb-3">Danh Mục Dịch Vụ</h3>
                <ul class="space-y-2 text-xs">
                    <li><a href="#betrai" class="hover:text-white transition">Trang trí sinh nhật bé trai Đà Nẵng</a></li>
                    <li><a href="#begai" class="hover:text-white transition">Trang trí sinh nhật bé gái & Thôi nôi</a></li>
                    <li><a href="#setdecor" class="hover:text-white transition">Set sinh nhật tự decor & Bánh kem thiết kế</a></li>
                    <li><a href="#khaitruong" class="hover:text-white transition">Trang trí khai trương & Bóng bay phòng cưới</a></li>
                </ul>
            </div>
            <div>
                <h3 class="text-white font-bold text-base mb-3">Liên Hệ Đặt Tiệc</h3>
                <p class="text-xs mb-2">Hotline 1: <a href="tel:0905400344" class="text-white font-bold hover:text-nilo-500">0905.400.344</a></p>
                <p class="text-xs mb-4">Hotline 2: <a href="tel:0377794379" class="text-white font-bold hover:text-nilo-500">0377.794.379</a></p>
                <div class="flex gap-3">
                    <a href="tel:0905400344" class="w-9 h-9 bg-nilo-500 text-white rounded-full flex items-center justify-center hover:bg-nilo-600 transition" title="Gọi Hotline"><i class="fa-solid fa-phone"></i></a>
                    <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" class="w-9 h-9 bg-blue-600 text-white rounded-full flex items-center justify-center hover:bg-blue-700 transition" title="Fanpage Facebook"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="https://zalo.me/0905400344" target="_blank" class="w-9 h-9 bg-sky-500 text-white rounded-full flex items-center justify-center hover:bg-sky-600 transition" title="Chat Zalo"><i class="fa-solid fa-comment-dots"></i></a>
                </div>
            </div>
        </div>
        <div class="max-w-7xl mx-auto border-t border-gray-800 pt-6 text-center text-xs text-gray-500">
            <p>&copy; 2026 niloparty.com - NILO Cakes & Decor Đà Nẵng. All rights reserved.</p>
        </div>
    </footer>

    <!-- Floating Contact Buttons (Hotline + Zalo + Facebook) -->
    <div class="fixed bottom-5 right-4 z-50 flex flex-col items-end gap-3">
        <!-- Zalo Button -->
        <a href="https://zalo.me/0905400344" target="_blank" title="Chat Zalo 0905.400.344" class="flex items-center gap-2 bg-sky-500 text-white px-3.5 py-2.5 rounded-full shadow-lg hover:bg-sky-600 transition transform hover:scale-105">
            <i class="fa-solid fa-comment-dots text-lg"></i>
            <span class="text-xs font-bold">Chat Zalo</span>
        </a>
        <!-- Facebook Fanpage Button -->
        <a href="https://www.facebook.com/nilodecor.danang/" target="_blank" title="Messenger NILO Cakes & Decor" class="flex items-center gap-2 bg-blue-600 text-white px-3.5 py-2.5 rounded-full shadow-lg hover:bg-blue-700 transition transform hover:scale-105">
            <i class="fa-brands fa-facebook-messenger text-lg"></i>
            <span class="text-xs font-bold">Facebook</span>
        </a>
        <!-- Prominent Hotline Button -->
        <a href="tel:0905400344" title="Gọi Hotline 0905.400.344" class="hotline-pulse flex items-center gap-2 bg-nilo-500 text-white px-4 py-3 rounded-full shadow-xl hover:bg-nilo-600 transition transform hover:scale-105">
            <i class="fa-solid fa-phone-volume text-lg"></i>
            <span class="text-xs md:text-sm font-extrabold">0905.400.344</span>
        </a>
    </div>

    <!-- Script to toggle mobile menu -->
    <script>
        function toggleMobileMenu() {
            const menu = document.getElementById('mobileMenu');
            if (menu.classList.contains('hidden')) {
                menu.classList.remove('hidden');
            } else {
                menu.classList.add('hidden');
            }
        }
    </script>
</body>
</html>
