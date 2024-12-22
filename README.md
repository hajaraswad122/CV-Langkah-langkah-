# APLIKASI LOW GO
Cara penggunaan apk low go
<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Undiang Berhadiah</title>
    <link rel="stylesheet" href="style.css">
    <style>
        /* Gaya tambahan untuk form sederhana */
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 10;
            background-color: #f3f2f9;
            color: black
        }
        header {
            text-align: center;
            padding: 50px;
            background-color: Black;
            color: White ;
        }
        main {
            max-width: 800px;
            margin: 50px auto;
            padding: 40px;
            background: white;
            border-radius: 9px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }
        label {
            display: white;
            margin: 25px 0 5px;
            font-weight: bold;
        }
        input {
            width: 100%;
            padding: 10px;
            margin-bottom: 20px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            display: block;
            width: 100%;
            padding: 15px;
            background-color: Black;
            color: white;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            cursor: pointer;
        }
        button:hover {
            background-color: #45a049;
        }
        footer {
            text-align: center;
            padding: 20px;
            background-color: Black;
            color: orange;
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <!-- Header -->
    <header>
         <h1></h1>🎉SELAMAT DATANG UNDIAN BERHADIAH INI🎉</h1>
        <p>✨Silakan Masukkan Data Anda✨.</p>
    </header>

    <!-- Form Input -->
    <main>
        <form id="dataForm">
            <label for="nama">Nama:</label>
            <input type="text" id="nama" placeholder="Masukkan Nama Anda" required>

            <label for="umur">Umur:</label>
            <input type="number" id="umur" placeholder="Masukkan Umur Anda" required>

            <button type="submit">Lanjutkan</button>
        </form>

        <div id="output"></div>
    </main>

    <!-- Footer -->
    <footer>
        <p>Hak Cipta &copy; 31 Desember 2024 - Kejutan Berhadiah🎊</p>
    </footer>

    <script>
        // Tangani data input dari form
        const form = document.getElementById('dataForm');
        const output = document.getElementById('output');

        form.addEventListener('submit', function(event) {
            event.preventDefault(); // Mencegah reload halaman
            const nama = document.getElementById('nama').value;
            const umur = document.getElementById('umur').value;

            // Menyimpan data ke sessionStorage
            sessionStorage.setItem("nama", nama);
            sessionStorage.setItem("umur", umur);

            // Arahkan ke halaman baru
            window.location.href = "Undiang teracak.html";
        });
    </script>
</body>
</html>

