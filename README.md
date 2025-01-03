# Surat-Tahun-Baru-Untuk-Sharin
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Surat Spesial untuk Sharin</title>
    <style>
        /* Style umum */
        body {
            margin: 0;
            padding: 0;
            font-family: 'Arial', sans-serif;
            background: linear-gradient(to right, #ffdde1, #ee9ca7);
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            overflow: hidden;
        }

        /* Kotak Kado */
        .gift-box {
            position: relative;
            width: 200px;
            height: 200px;
            background: #ff6f61;
            border-radius: 10px;
            display: flex;
            justify-content: center;
            align-items: center;
            cursor: pointer;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
            transition: transform 0.3s ease;
        }

        .gift-box:hover {
            transform: scale(1.1);
        }

        .gift-box::before {
            content: '';
            position: absolute;
            width: 120%;
            height: 20px;
            background: #d64541;
            top: 90px;
            left: -10%;
        }

        .ribbon {
            position: absolute;
            width: 60px;
            height: 60px;
            background: #d64541;
            top: -30px;
            left: 70px;
            border-radius: 50%;
        }

        /* Animasi kado terbuka */
        .hidden {
            display: none;
        }

        /* Surat */
        .letter {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 400px;
            text-align: center;
            animation: fadeIn 1s ease-in-out;
        }

        .letter h1 {
            font-size: 24px;
            color: #e63946;
        }

        .letter p {
            font-size: 16px;
            color: #555;
            margin: 10px 0;
        }

        .signature {
            margin-top: 20px;
            font-size: 14px;
            color: #777;
        }

        @keyframes fadeIn {
            from { opacity: 0; }
            to { opacity: 1; }
        }

        /* Kucing */
        .cat {
            position: absolute;
            bottom: 20px;
            right: 20px;
            font-size: 50px;
            animation: bounce 1.5s infinite;
        }

        @keyframes bounce {
            0%, 100% {
                transform: translateY(0);
            }
            50% {
                transform: translateY(-10px);
            }
        }
    </style>
</head>
<body>
    <!-- Kotak Kado -->
    <div id="gift" class="gift-box" onclick="openGift()">
        🎁
        <div class="ribbon"></div>
    </div>

    <!-- Surat Tersembunyi -->
    <div id="letter" class="hidden">
        <div class="letter">
            <h1>halooo Incess, Selamat Tahun Baru 2025! 🎆</h1>
            <p>Semoga tahun ini jadi tahun penuh kebahagiaan dan cerita indah buat kamu.</p>
            <p>Makasih udah jadi salah satu orang spesial di hidupku. Notifikasi dari kamu selalu jadi favoritku.</p>
            <p>Apapun yang terjadi di tahun ini, aku harap kita tetap bisa punya cerita yang baik bersama.</p>
            <p>Selamat tahun baru, Sharin! ❤️</p>
            <div class="signature">- R</div>
        </div>
    </div>

    <!-- Kucing Lucu -->
    <div class="cat">🐱</div>

    <script>
        function openGift() {
            const gift = document.getElementById('gift');
            const letter = document.getElementById('letter');

            // Sembunyikan kado dan tampilkan surat
            gift.classList.add('hidden');
            letter.classList.remove('hidden');
        }
    </script>
</body>
</html>
