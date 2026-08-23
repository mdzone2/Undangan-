# Undangan-
Undangan digital
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Undangan Pernikahan - Rifkie Septian surya & Neng Nurani Pitriyani</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Great+Vibes&family=Montserrat:wght@300;400;600&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #f7f5f0;
            color: #333;
            overflow-x: hidden;
        }

        /* Halaman Cover / Sambutan */
        #cover {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100vh;
            background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)), url('https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: white;
            z-index: 1000;
            transition: transform 1s ease-in-out;
        }

        #cover h1 {
            font-family: 'Great Vibes', cursive;
            font-size: 4rem;
            margin-bottom: 10px;
        }

        #cover p {
            font-size: 1.1rem;
            margin-bottom: 30px;
            font-weight: 300;
        }

        .btn-buka {
            padding: 12px 30px;
            background-color: #d4af37;
            color: white;
            border: none;
            border-radius: 25px;
            font-size: 1rem;
            cursor: pointer;
            transition: background 0.3s;
        }

        .btn-buka:hover {
            background-color: #b49428;
        }

        /* Konten Utama Undangan */
        .main-content {
            max-width: 600px;
            margin: 0 auto;
            background: white;
            box-shadow: 0 0 20px rgba(0,0,0,0.05);
            min-height: 100vh;
            display: none; /* Muncul setelah cover dibuka */
        }

        section {
            padding: 60px 20px;
            text-align: center;
        }

        .hero {
            background: linear-gradient(rgba(255,255,255,0.9), rgba(255,255,255,0.9)), url('https://images.unsplash.com/photo-1519741497674-611481863552?auto=format&fit=crop&w=1200&q=80') no-repeat center center/cover;
        }

        .hero h2 {
            font-family: 'Great Vibes', cursive;
            font-size: 3.5rem;
            color: #d4af37;
            margin-bottom: 20px;
        }

        .couple-names {
            font-size: 1.8rem;
            font-weight: 600;
            margin: 20px 0;
        }

        .event-details {
            background-color: #faf9f6;
            margin: 20px;
            padding: 30px;
            border-radius: 10px;
            border: 1px solid #eee;
        }

        .event-details h3 {
            color: #d4af37;
            margin-bottom: 15px;
            font-weight: 600;
        }

        footer {
            background-color: #333;
            color: white;
            padding: 20px;
            text-align: center;
            font-size: 0.9rem;
        }
    </style>
</head>
<body>

    <!-- Cover Depan -->
    <div id="cover">
        <p>Undangan Pernikahan</p>
        <h1>Romeo & Juliet</h1>
        <p>Kepada Yth. Bapak/Ibu/Saudara/i</p>
        <button class="btn-buka" onclick="bukaUndangan()">Buka Undangan</button>
    </div>

    <!-- Isi Undangan -->
    <div class="main-content" id="mainContent">
        <section class="hero">
            <p>The Wedding of</p>
            <h2>Rifkie & Neng nurani</h2>
            <p>06 september 2026</p>
        </section>

        <section>
            <p style="font-style: italic; line-height: 1.6;">
                "Dan di antara tanda-tanda kebesaran-Nya ialah Dia menciptakan pasangan-pasangan untukmu dari jenismu sendiri, agar kamu cenderung dan merasa tenteram kepadanya..."
                <br><strong>(QS. Ar-Rum: 21)</strong>
            </p>
        </section>

        <section class="event-details">
            <h3>Akad Nikah</h3>
            <p>Pukul 08.00 WIB - Selesai</p>
            <p>Masjid Al-fatah, kp ciseel</p>
        </section>

        <section class="event-details">
            <h3>Resepsi</h3>
            <p>Pukul 11.00 - 14.00 WIB</p>
            <p>rumah mempelai wanita, kp ciseel</p>
        </section>

        <footer>
            <p>Merupakan suatu kehormatan dan kebahagiaan bagi kami apabila Bapak/Ibu/Saudara/i berkenan hadir.</p>
            <p style="margin-top: 15px; font-weight: 600;">Romeo & Juliet</p>
        </footer>
    </div>

    <script>
        function bukaUndangan() {
            const cover = document.getElementById('cover');
            const mainContent = document.getElementById('mainContent');
            
            // Sembunyikan cover dengan efek geser ke atas
            cover.style.transform = 'translateY(-100%)';
            mainContent.style.display = 'block';
            
            // Hapus elemen cover dari DOM setelah animasi selesai
            setTimeout(() => {
                cover.style.display = 'none';
            }, 1000);
        }
    </script>
</body>
</html>
