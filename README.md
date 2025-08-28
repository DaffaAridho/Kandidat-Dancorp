<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Daffa Arridho - Marching Band Profile</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@400;600;700;800&family=Inter:wght@300;400;500;600;700&display=swap');
        
        :root {
            --marching-red: #B22234;
            --marching-gold: #FFD700;
            --marching-navy: #002147;
            --marching-white: #FFFFFF;
            --marching-black: #000000;
            --marching-silver: #C0C0C0;
        }
        
        body {
            font-family: 'Inter', sans-serif;
            background: linear-gradient(135deg, var(--marching-navy) 0%, #000080 50%, var(--marching-black) 100%);
            background-image: 
                url("data:image/svg+xml,%3Csvg width='200' height='200' viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M40,40 C60,20 140,20 160,40 C180,60 180,140 160,160 C140,180 60,180 40,160 C20,140 20,60 40,40 Z' stroke='rgba(178,34,52,0.15)' stroke-width='2' fill='none'/%3E%3Cpath d='M80,80 C90,70 110,70 120,80 C130,90 130,110 120,120 C110,130 90,130 80,120 C70,110 70,90 80,80 Z' stroke='rgba(255,215,0,0.15)' stroke-width='1' fill='none'/%3E%3C/svg%3E"),
                radial-gradient(circle at 20% 30%, rgba(178, 34, 52, 0.1) 0%, transparent 50%),
                radial-gradient(circle at 80% 70%, rgba(255, 215, 0, 0.1) 0%, transparent 50%);
            min-height: 100vh;
            margin: 0;
            padding: 8px;
            color: var(--marching-white);
            position: relative;
            overflow-x: hidden;
        }
        
        body::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            bottom: 0;
            background-image: 
                url("data:image/svg+xml,%3Csvg width='100' height='100' viewBox='0 0 100 100' xmlns='http://www.w3.org/2000/svg'%3E%3Cpath d='M30,30 L70,30 L70,70 L30,70 Z' stroke='rgba(255,215,0,0.1)' stroke-width='1' fill='none'/%3E%3C/svg%3E");
            opacity: 0.2;
            pointer-events: none;
        }
        
        .marching-container {
            background: rgba(0, 33, 71, 0.85);
            backdrop-filter: blur(20px);
            border: 3px solid var(--marching-gold);
            border-radius: 20px;
            box-shadow: 
                0 20px 50px rgba(0, 0, 0, 0.4),
                0 0 35x rgba(255, 215, 0, 0.3),
                inset 0 2px 0 rgba(255, 255, 255, 0.15);
        }
        
       
        
        .profile-image {
            transition: all 0.6s cubic-bezier(0.4, 0, 0.2, 1);
            border: 4px solid var(--marching-gold);
            border-radius: 15px;
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.3),
                0 0 30px rgba(255, 215, 0, 0.4);
        }
        
        .profile-image:hover {
            transform: translateY(-8px) scale(1.02);
            box-shadow: 
                0 30px 60px rgba(0, 0, 0, 0.5),
                0 0 50px rgba(255, 215, 0, 0.6);
        }
        
        .name-plate {
            background: linear-gradient(135deg, var(--marching-red), #8B0000);
            border: 2px solid var(--marching-gold);
            box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3);
            position: relative;
        }
        
        .name-plate::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--marching-gold), transparent);
        }
        

        
        .marching-logo {
            transition: all 0.5s cubic-bezier(0.4, 0, 0.2, 1);
            background: linear-gradient(135deg, var(--marching-red), var(--marching-gold));
            border: 3px solid var(--marching-gold);
            box-shadow: 
                0 20px 40px rgba(0, 0, 0, 0.3),
                0 0 30px rgba(255, 215, 0, 0.4);
        }
        
        .marching-logo:hover {
            transform: scale(1.1) rotate(5deg);
            box-shadow: 
                0 25px 50px rgba(0, 0, 0, 0.4),
                0 0 40px rgba(255, 215, 0, 0.5);
        }
        
        .instagram-link {
            transition: all 0.4s ease;
            background: linear-gradient(45deg, #833ab4, #fd1d1d, #fcb045);
            border: 2px solid var(--marching-gold);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.3);
        }
        
        .instagram-link:hover {
            transform: translateY(-5px) scale(1.08);
            box-shadow: 
                0 25px 45px rgba(253, 29, 29, 0.4),
                0 0 35px rgba(131, 58, 180, 0.5);
        }
        
        .vision-card {
            transition: all 0.4s ease;
            border-left: 4px solid var(--marching-gold);
            background: linear-gradient(90deg, rgba(178, 34, 52, 0.15), rgba(0, 33, 71, 0.25));
            position: relative;
            overflow: hidden;
        }
        
        .vision-card::before {
            content: '🎵';
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 1.5rem;
            opacity: 0.2;
        }
        
        .vision-card:hover {
            transform: translateX(8px);
            border-left: 4px solid var(--marching-red);
            background: linear-gradient(90deg, rgba(178, 34, 52, 0.2), rgba(0, 33, 71, 0.35));
        }
        
        .music-note {
            animation: floatNote 4s ease-in-out infinite;
            color: var(--marching-gold);
            text-shadow: 0 0 15px rgba(255, 215, 0, 0.6);
            font-size: 2rem;
        }
        
        @keyframes floatNote {
            0%, 100% { 
                transform: translateY(0px) rotate(0deg) scale(1);
                opacity: 0.6;
            }
            50% { 
                transform: translateY(-25px) rotate(180deg) scale(1.3);
                opacity: 1;
            }
        }
        
        .marching-title {
            font-family: 'Playfair Display', serif;
            color: var(--marching-gold);
            text-shadow: 
                3px 3px 0 var(--marching-red),
                0 0 25px rgba(255, 215, 0, 0.5);
            position: relative;
            letter-spacing: 1px;
        }
        
        /* Removed decorative line below marching title */
        /* .marching-title::after {
            content: '';
            position: absolute;
            bottom: -12px;
            left: 50%;
            transform: translateX(-50%);
            width: 100px;
            height: 3px;
            background: linear-gradient(90deg, transparent, var(--marching-gold), transparent);
        } */
        
        .instrument-float {
            animation: instrumentFloat 6s ease-in-out infinite;
        }

        /* Image loading states */
        .image-loading {
            background: linear-gradient(90deg, #f0f0f0 25%, #e0e0e0 50%, #f0f0f0 75%);
            background-size: 200% 100%;
            animation: loading 1.5s infinite;
        }

        @keyframes loading {
            0% { background-position: 200% 0; }
            100% { background-position: -200% 0; }
        }

        .profile-image img {
            transition: opacity 0.3s ease;
        }

        .profile-image img[loading] {
            opacity: 0;
        }

        .profile-image img[loaded] {
            opacity: 1;
        }

        .vision-content {
            font-family: 'Playfair Display', serif;
            font-weight: 400;
            line-height: 1.6;
        }

        @keyframes instrumentFloat {
            0%, 100% {
                transform: translateY(0px) rotate(0deg) scale(1);
                filter: drop-shadow(0 5px 15px rgba(255, 215, 0, 0.4));
            }
            33% {
                transform: translateY(-20px) rotate(-10deg) scale(1.1);
                filter: drop-shadow(0 10px 20px rgba(255, 215, 0, 0.6));
            }
            66% {
                transform: translateY(-10px) rotate(10deg) scale(1.05);
                filter: drop-shadow(0 8px 18px rgba(255, 215, 0, 0.5));
            }
        }

        /* Mobile-specific optimizations */
        @media (max-width: 640px) {
            .marching-container {
                border-radius: 15px;
                margin: 5px;
                padding: 1rem;
            }

            .vision-card {
                margin-bottom: 1rem;
                padding: 1rem;
            }

            .name-plate {
                font-size: 1rem;
            }

            .marching-title {
                font-size: 1.75rem;
                line-height: 1.2;
            }

            /* Improve readability on mobile */
            .vision-content {
                word-wrap: break-word;
                hyphens: auto;
                font-size: 1.1rem;
                line-height: 1.5;
            }

            /* Better contrast for mobile */
            .text-gray-200 {
                color: #e5e7eb !important;
            }

            .text-gray-300 {
                color: #d1d5db !important;
            }

            /* Larger touch targets */
            .instagram-link {
                min-width: 60px;
                min-height: 60px;
            }

            /* Improve spacing */
            .space-y-6 > * + * {
                margin-top: 1.5rem;
            }

            .space-y-8 > * + * {
                margin-top: 2rem;
            }
        }
    </style>
</head>
<body class="flex items-center justify-center min-h-screen p-4">
    <div class="marching-container w-full max-w-6xl mx-auto p-3 sm:p-4 md:p-6 lg:p-12 relative overflow-hidden">
        <!-- Floating Music Instruments Background - Hidden on mobile for cleaner look -->
        <div class="hidden sm:block absolute top-8 left-8 text-4xl md:text-5xl instrument-float" style="animation-delay: 0s; color: #FF6B6B;">🎷</div>
        <div class="hidden sm:block absolute top-20 right-12 text-3xl md:text-4xl instrument-float" style="animation-delay: 2s; color: #FFD700;">🥁</div>
        <div class="hidden sm:block absolute bottom-16 left-16 text-4xl md:text-5xl instrument-float" style="animation-delay: 4s; color: #4ECDC4;">🎺</div>
        <div class="hidden sm:block absolute bottom-8 right-8 text-3xl md:text-4xl instrument-float" style="animation-delay: 1s; color: #FFE66D;">🎻</div>

        <!-- Floating Music Notes - Hidden on mobile for cleaner look -->
        <div class="hidden sm:block absolute top-1/4 left-1/4 text-3xl music-note" style="animation-delay: 0.5s;">♪</div>
        <div class="hidden sm:block absolute top-1/3 right-1/3 text-2xl music-note" style="animation-delay: 1.5s;">♫</div>
        <div class="hidden sm:block absolute bottom-1/4 left-1/3 text-3xl music-note" style="animation-delay: 2.5s;">🎵</div>
        <div class="hidden sm:block absolute bottom-1/3 right-1/4 text-2xl music-note" style="animation-delay: 3.5s;">♩</div>

        <!-- Header -->
        <div class="text-center mb-8 sm:mb-12 md:mb-16">
            <h1 class="marching-title text-3xl sm:text-4xl md:text-5xl lg:text-6xl font-bold mb-4 sm:mb-6">
                MB. TUNAS GURINDAM CORPS
            </h1>
            <p class="text-gray-200 text-base sm:text-lg md:text-xl font-light italic mb-6">
               • KWARDA KEPULAUAN RIAU •
            </p>
        </div>



        <!-- Main Content -->
        <div class="grid grid-cols-1 lg:grid-cols-2 gap-8 sm:gap-10 md:gap-14 lg:gap-20 items-start mb-10 sm:mb-14 md:mb-18">
            <!-- Profile Section - Foto dan Nama -->
            <div class="profile-section pr-0 lg:pr-12">
                <div class="text-center">
                    <!-- Foto -->
                    <div class="name-plate px-4 py-2 rounded-lg inline-block mb-4">
                    <h2 class="text-base sm:text-lg md:text-xl font-bold text-yellow-400 marching-title">KANDIDAT DANCROPS NO 1</h2>
                </div>
                    <div class="profile-image mx-auto mb-4 sm:mb-6 md:mb-8 w-48 h-48 sm:w-64 sm:h-64 md:w-80 md:h-80 lg:w-96 lg:h-96 overflow-hidden image-loading">
                        <img
                            src="223344.jpg"
                            alt="Daffa Arridho dengan seragam marching band merah dan emas, memegang trumpet dengan pose profesional di lapangan"
                            class="w-full h-full object-contain"
                            loading="lazy"
                            onload="this.setAttribute('loaded', 'true'); this.parentElement.classList.remove('image-loading')"
                            onerror="this.src='223344.jpg'; this.setAttribute('loaded', 'true'); this.parentElement.classList.remove('image-loading')"
                        >
                    </div>
                    
                    <!-- Nama Daffa Arridho -->
                    <div class="name-plate px-4 py-2 rounded-lg inline-block">
                        <h1 class="marching-title text-xl sm:text-2xl md:text-3xl font-bold mb-4">
                Daffa Arridho
            </h1>

                        <p class="text-gray-200 text-xs">Tuba player • MB.Tunas Gurindam Corps </p>
                    </div>
                </div>
            </div>


            

            <!-- Visi Misi Section -->
           <div class="space-y-8 sm:space-y-10 md:space-y-12">
                <!-- Visi -->
                <div class="vision-card p-4 sm:p-6 md:p-10 rounded-xl">
                    <div class="flex items-start mb-5">
                        <div class="w-12 h-12 md:w-16 md:h-16 bg-gradient-to-r from-red-600 to-yellow-500 rounded-full flex items-center justify-center mr-3 md:mr-5 shadow-xl">
                            <i class="fas fa-eye text-white text-2xl md:text-3xl"></i>
                        </div>
                        <div>
                            <h3 class="text-2xl md:text-3xl font-bold text-yellow-400 mb-4">VISI</h3>
                            <p class="vision-content text-gray-200 text-lg sm:text-xl md:text-2xl lg:text-3xl">

                            </p>
                        </div>
                    </div>
                </div>

                <!-- Misi -->
                <div class="vision-card p-4 sm:p-6 md:p-10 rounded-xl">
                    <div class="flex items-start mb-5">
                        <div class="w-12 h-12 md:w-16 md:h-16 bg-gradient-to-r from-blue-800 to-red-600 rounded-full flex items-center justify-center mr-3 md:mr-5 shadow-xl">
                            <i class="fas fa-music text-white text-2xl md:text-3xl"></i>
                        </div>
                        <div>
                            <h3 class="text-2xl md:text-3xl font-bold text-yellow-400 mb-4">MISI</h3>
                            <ul class="text-gray-200 space-y-4 text-lg md:text-xl">
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span></span>
                                </li>
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span></span>
                                </li>
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span></span>
                                </li>
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span></span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>

                <!-- Program -->
                <div class="vision-card p-4 sm:p-6 md:p-10 rounded-xl">
                    <div class="flex items-start mb-5">
                        <div class="w-12 h-12 md:w-16 md:h-16 bg-gradient-to-r from-green-600 to-yellow-500 rounded-full flex items-center justify-center mr-3 md:mr-5 shadow-xl">
                            <i class="fas fa-clipboard-list text-white text-2xl md:text-3xl"></i>
                        </div>
                        <div>
                            <h3 class="text-2xl md:text-3xl font-bold text-yellow-400 mb-4">PROGRAM</h3>
                            <ul class="text-gray-200 space-y-4 text-lg md:text-xl">
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span>Program senam pagi bersama setiap 1 bulan sekali</span>
                                </li>
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span>Rapat bulanan tim inti</span>
                                </li>
                                <li class="flex items-start">
                                    <span class="w-4 h-4 bg-yellow-400 rounded-full mt-2 mr-4"></span>
                                    <span>Outbound setiap 6 bulan sekali di setiap liburan semester</span>
                                </li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>

        <!-- Logo Bulat -->
        <div class="flex justify-center items-center space-x-3 sm:space-x-4 md:space-x-6 lg:space-x-8 mb-8 sm:mb-12 md:mb-16">
            <div class="marching-logo w-20 h-20 sm:w-28 sm:h-28 md:w-36 md:h-36 lg:w-40 lg:h-40 rounded-full flex items-center justify-center image-loading">
                <img
                    src="kwarda.jpg"
                    alt="Logo marching band dengan desain perisai merah dan emas, simbol trumpet dengan mahkota daun, latar belakang navy blue"
                    class="w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24 lg:w-28 lg:h-28 rounded-full"
                    loading="lazy"
                    onload="this.setAttribute('loaded', 'true'); this.parentElement.classList.remove('image-loading')"
                    onerror="this.style.display='none'"
                >
            </div>
            <div class="marching-logo w-20 h-20 sm:w-28 sm:h-28 md:w-36 md:h-36 lg:w-40 lg:h-40 rounded-full flex items-center justify-center image-loading">
                <img
                    src="242104513_266398215333645_4612524844173446882_n.jpg"
                    alt="Logo marching band dengan desain perisai merah dan emas, simbol trumpet dengan mahkota daun, latar belakang navy blue"
                    class="w-16 h-16 sm:w-20 sm:h-20 md:w-24 md:h-24 lg:w-28 lg:h-28 rounded-full"
                    loading="lazy"
                    onload="this.setAttribute('loaded', 'true'); this.parentElement.classList.remove('image-loading')"
                    onerror="this.style.display='none'"
                >
            </div>
        </div>

        <!-- Media Sosial Instagram -->
        <div class="text-center">
            <h3 class="text-xl sm:text-2xl font-bold text-yellow-400 mb-6 sm:mb-8 md:mb-10">
                MEDIA SOSIAL
            </h3>
            
            <div class="flex justify-center space-x-6 sm:space-x-8 md:space-x-10 mb-6 sm:mb-8">
                <!-- Instagram Link 1 -->
                <a href="https://www.instagram.com/daffaridhooo_/?utm_source=ig_web_button_share_sheet" target="_blank" class="instagram-link w-16 h-16 sm:w-20 sm:h-20 rounded-full flex items-center justify-center transform transition-all duration-300">
                    <i class="fab fa-instagram text-white text-2xl sm:text-3xl"></i>
                </a>

                <!-- Instagram Link 2 -->
                <a href="https://www.instagram.com/tunasgurindam?utm_source=ig_web_button_share_sheet&igsh=ZDNlZDc0MzIxNw==" target="_blank" class="instagram-link w-16 h-16 sm:w-20 sm:h-20 rounded-full flex items-center justify-center transform transition-all duration-300">
                    <i class="fab fa-instagram text-white text-2xl sm:text-3xl"></i>
                </a>
            </div>

            <!-- Nama Akun Instagram -->
            <div class="text-center">
                <p class="text-gray-300 text-lg mb-4">Follow akun Instagram:</p>
                <div class="flex justify-center space-x-4 sm:space-x-6 md:space-x-8 flex-wrap gap-3 sm:gap-4">
                    <span class="text-white font-bold bg-red-600 px-4 py-2 sm:px-6 sm:py-3 rounded-full border-2 border-yellow-400 text-sm sm:text-base md:text-lg">@daffaridhooo_</span>
                    <span class="text-white font-bold bg-blue-800 px-4 py-2 sm:px-6 sm:py-3 rounded-full border-2 border-yellow-400 text-sm sm:text-base md:text-lg">@tunasgurindam</span>
                </div>
                <p class="text-gray-200 text-sm mt-6 italic">
                    Saksikan momen spesial, latihan, dan pertunjukan spektakuler kami!
                </p>
                <p class="text-gray-200 text-sm mt-6 italic">
                    #TunasGurindamCorps #TGC #AKT6
                </p>
            </div>
        </div>

        <!-- Footer -->
        <div class="text-center mt-12 sm:mt-16 md:mt-20 pt-6 sm:pt-8 border-t border-yellow-400 border-opacity-30">
            <div class="flex justify-center space-x-6 mb-4">
                <span class="text-3xl text-yellow-400">🎵</span>
                <span class="text-3xl text-red-500">🎺</span>
                <span class="text-3xl text-yellow-400">🥁</span>
                <span class="text-3xl text-red-500">🎷</span>
                <span class="text-3xl text-yellow-400">📯</span>
            </div>
            <p class="text-gray-300 text-sm">
                © 2025 Daffa Arridho • Marching Band Tunas Gurindam Corps • Dancorp
            </p>
        </div>
    </div>

    <!-- Background Music with Auto Play -->
    <audio id="bgMusic" autoplay loop preload="auto" style="display: none;">
        <source src="Hujan Gerimis.mp3" type="audio/mpeg">
        <source src="background-music.ogg" type="audio/ogg">
        Your browser does not support the audio element.
    </audio>

    <script>
        // Background Music Auto Play
        document.addEventListener('DOMContentLoaded', function() {
            const bgMusic = document.getElementById('bgMusic');

            // Set volume and try to play
            if (bgMusic) {
                bgMusic.volume = 0.6; // 60% volume

                // Auto play music
                bgMusic.play().catch(function(error) {
                    console.log('Auto-play prevented:', error);
                });
            }

            // Add simple music control button
            const musicBtn = document.createElement('button');
            musicBtn.innerHTML = '🔊 Music';
            musicBtn.className = 'fixed bottom-4 left-4 bg-yellow-500 hover:bg-yellow-600 text-black px-10 py-5 rounded-full shadow-lg z-50 text-xl';
            musicBtn.onclick = function() {
                if (bgMusic.paused) {
                    bgMusic.play();
                    musicBtn.innerHTML = '🔊 Music';
                    musicBtn.className = musicBtn.className.replace('bg-red-500', 'bg-yellow-500');
                } else {
                    bgMusic.pause();
                    musicBtn.innerHTML = '🔇 Muted';
                    musicBtn.className = musicBtn.className.replace('bg-yellow-500', 'bg-red-500');
                }
            };
            document.body.appendChild(musicBtn);

            // Animasi scroll dengan Intersection Observer
            const observer = new IntersectionObserver((entries) => {
                entries.forEach(entry => {
                    if (entry.isIntersecting) {
                        entry.target.style.opacity = '1';
                        entry.target.style.transform = 'translateY(0) scale(1)';
                    }
                });
            }, {
                threshold: 0.1,
            });
        });
    </script>
</body>
</html>
