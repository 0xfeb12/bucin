<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>bucin</title>
    <style>
        /* CSS untuk Tampilan */
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap');

        body {
            margin: 0;
      padding: 0;
      font-family: 'Poppins', sans-serif;
      background-color: #ffe9e3;
      background-image:
        linear-gradient(90deg, transparent 24%, rgba(255,255,255,.5) 25%, rgba(255,255,255,.5) 26%, transparent 27%, transparent 74%, rgba(255,255,255,.5) 75%, rgba(255,255,255,.5) 76%, transparent 77%, transparent),
        linear-gradient(0deg, transparent 24%, rgba(255,255,255,.5) 25%, rgba(255,255,255,.5) 26%, transparent 27%, transparent 74%, rgba(255,255,255,.5) 75%, rgba(255,255,255,.5) 76%, transparent 77%, transparent);
      background-size: 50px 50px;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      height: 100vh;
      overflow: hidden;
      color: #5b3a29;
        }

        .music-player-container {
            background-color: rgba(44, 62, 80, 0.8);
            border-radius: 15px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            width: 90%;
            max-width: 600px;
            padding: 30px;
            text-align: center;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.2);
        }

        h1 {
            margin-top: 0;
            font-size: 2.5em;
            font-weight: 700;
            color: #ffffff;
        }

        h2 {
            margin-bottom: 30px;
            font-size: 1.5em;
            font-weight: 400;
            color: #bdc3c7;
        }

        .lyrics-wrapper {
            height: 250px; /* Tinggi area lirik yang terlihat */
            overflow: hidden; /* Sembunyikan lirik yang di luar area */
            position: relative;
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            background: rgba(0,0,0,0.2);
        }
        
        #lyrics-container {
            transition: transform 0.8s ease-in-out; /* Animasi scroll yang halus */
        }

        .lyric-line {
            font-size: 1.4em;
            line-height: 1.6;
            padding: 10px 20px;
            opacity: 0; /* Lirik lain dibuat redup */
            transition: all 0.5s ease;
        }

        .lyric-line.active {
            opacity: 1; /* Lirik yang aktif menjadi terang */
            color: #f1c40f; /* Warna lirik aktif */
            font-weight: 600;
            transform: scale(1.1); /* Sedikit diperbesar */
        }

        #play-pause-btn {
            margin-top: 30px;
            padding: 15px 35px;
            font-size: 1.2em;
            font-weight: 600;
            border: none;
            border-radius: 50px;
            background-color: #f1c40f;
            color: #2c3e50;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 4px 15px rgba(241, 196, 15, 0.4);
        }

        #play-pause-btn:hover {
            background-color: #f39c12;
            transform: translateY(-2px);
            box-shadow: 0 6px 20px rgba(241, 196, 15, 0.5);
        }
            
        @media (max-width: 480px) {
            .music-player-container {
                padding: 20px;
                border-radius: 10px;
            }

            h1 {
                font-size: 1.8rem;
            }

            h2 {
                font-size: 1rem;
                margin-bottom: 20px;
            }

            .lyrics-wrapper {
                height: 150px; /* Lebih pendek di layar yang sangat kecil */
            }

            .lyric-line {
                font-size: 1rem;
                padding: 5px 10px;
                line-height: 1.6;
            }

            #play-pause-btn {
                font-size: 0.9rem;
                padding: 10px 20px;
            }
        }

        /* Untuk layar dengan lebar minimum 768px (Tablet dan Desktop) */
        @media (min-width: 768px) {
             .lyrics-wrapper {
                height: 300px; /* Lebih tinggi di layar besar */
            }

            .lyric-line {
                font-size: 1.5em; /* Ukuran font yang lebih besar */
            }
            
            #lyrics-container {
                padding-top: 0; /* Padding tidak diperlukan di layar besar */
            }
        }
        
    </style>
</head>
<body>

    <audio id="song" src="sayang.mp3"></audio>

    <div class="music-player-container">
         <img id="gifAnimation" src="https://dekatutorial.github.io/v/stkr/Stiker%2016.gif" class="gif">

        <div class="lyrics-wrapper">
            <div id="lyrics-container">
                </div>
        </div>

        <button id="play-pause-btn">Mulai</button>
    </div>

    <script>
        // --- DATA LIRIK DAN WAKTU (dalam detik) ---
        // Anda bisa menyesuaikan waktu ini agar lebih sinkron dengan lagu Anda
        const lyricsData = [
            { time: 0, text: "🎶🎶" },
            { time: 1, text: "Sayang Dengarkanlah Permintaanku"},
            { time: 4, text: "Jangan Ragukan Cintaku"},
            { time: 8, text: "Sayang Percayalah Apa Kataku, Karnaku sayang kamu"},
            { time: 15, text: "sayang, dengarkanlah permintaanku"},
            { time: 18, text: "jaga hatimu untuku"},
            { time: 22, text: "sayang, dengarlah bisikan hatiku, karnaku sayang kamu"},
            { time: 30, text: "sayang apakabar dengamu?"},
            { time: 34, text: "disini ku merindukan kamu"},
            { time: 37, text: "kuharap cintamu takkan berubah"},
            { time: 40, text: "karna disiniku tetap untukmu"},
            { time: 44, text: "sayang apakabar dengamu?"},
            { time: 47, text: "cobalah kamu telfon diriku"},
            { time: 50, text: "ku rindu dengan suara indahmu"},
            { time: 54, text: "karna dirimulah semangat hidupku"},
        ];

        // --- ELEMEN DOM ---
        const song = document.getElementById('song');
        const playPauseBtn = document.getElementById('play-pause-btn');
        const lyricsContainer = document.getElementById('lyrics-container');
        
        let currentLineIndex = -1;

        // --- FUNGSI-FUNGSI ---

        // 1. Memuat lirik ke dalam container HTML
        window.onload = () => {
            lyricsData.forEach((line, index) => {
                const p = document.createElement('p');
                p.textContent = line.text;
                p.classList.add('lyric-line');
                p.dataset.index = index;
                lyricsContainer.appendChild(p);
            });
        };

        // 2. Mengatur fungsi tombol play/pause
        playPauseBtn.addEventListener('click', () => {
            if (song.paused) {
                song.play();
                playPauseBtn.textContent = 'Jeda';
            } else {
                song.pause();
                playPauseBtn.textContent = 'Lanjutkan';
            }
        });

        // 3. Event listener yang berjalan setiap kali waktu lagu berubah
        song.addEventListener('timeupdate', () => {
            const currentTime = song.currentTime;

            // Cari indeks lirik yang sesuai dengan waktu saat ini
            let activeIndex = lyricsData.findIndex((line, index) => {
                const nextLine = lyricsData[index + 1];
                // Kondisi: waktu saat ini lebih besar dari waktu lirik ini
                // DAN (tidak ada lirik berikutnya ATAU waktu saat ini lebih kecil dari waktu lirik berikutnya)
                return currentTime >= line.time && (!nextLine || currentTime < nextLine.time);
            });
            
            // Jika lirik yang aktif berubah
            if (activeIndex !== -1 && activeIndex !== currentLineIndex) {
                currentLineIndex = activeIndex;
                updateLyricsHighlight();
            }
        });

        // 4. Fungsi untuk update highlight dan scroll lirik
        function updateLyricsHighlight() {
            const allLines = lyricsContainer.querySelectorAll('.lyric-line');
            
            // Hapus kelas 'active' dari semua baris lirik
            allLines.forEach(line => line.classList.remove('active'));
            
            // Tambahkan kelas 'active' ke baris yang sedang aktif
            const activeLine = allLines[currentLineIndex];
            if (activeLine) {
                activeLine.classList.add('active');

                // Kalkulasi untuk scrolling
                const containerHeight = lyricsContainer.parentElement.clientHeight;
                const activeLineTop = activeLine.offsetTop;
                const activeLineHeight = activeLine.clientHeight;
                
                // Scroll agar lirik aktif berada di tengah
                const scrollPosition = activeLineTop - (containerHeight / 2) + (activeLineHeight / 2);
                
                lyricsContainer.style.transform = `translateY(-${scrollPosition}px)`;
            }
        }
        
        // Reset saat lagu selesai
        song.addEventListener('ended', () => {
            playPauseBtn.textContent = 'Mulai Lagi';
            currentLineIndex = -1;
            lyricsContainer.style.transform = `translateY(0px)`;
            lyricsContainer.querySelectorAll('.lyric-line').forEach(line => line.classList.remove('active'));
        });


    </script>
</body>
</html>
