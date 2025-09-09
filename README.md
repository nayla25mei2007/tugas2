<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Pendaftaran Lomba Taekwondo</title>
    <style>
        body {
            font: 100%/1.5 Arial, sans-serif;
            margin: auto;
            width: 50%;
            background-color: #fff8dc;
            padding: 2%;
            box-sizing: border-box;
        }

        h1 {
            text-align: center;
            color: #b08d00;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: x-large;
            font-weight: bold;
            margin-bottom: 20px;
        }

        fieldset {
            border: #b08d00 solid 2px;
            padding: 20px;
            border-radius: 5px;
            background-color: #fff;
        }

        legend {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            font-size: large;
            font-weight: bold;
            color: #6f5901;
            text-align: center;
        }

        label {
            display: block;
            font-size: medium;
            font-weight: bold;
            color: #6f5901;
            margin: 10px 0 5px;
        }

        input, textarea, select {
            width: 100%;
            padding: 10px;
            border-radius: 5px;
            border: #b08d00 solid 2px;
            font-size: medium;
            color: #6f5901;
            margin-bottom: 15px;
            box-sizing: border-box;
        }

        input::placeholder, textarea::placeholder {
            color: #6f5901;
            font-family: 'Courier New', Courier, monospace;
            font-size: medium;
        }

        textarea {
            height: 100px;
            resize: none;
        }

        input[type=radio], input[type=checkbox] {
            width: auto;
            margin-right: 8px;
        }

        button {
            font-size: medium;
            font-weight: bold;
            color: #fff;
            border-radius: 5px;
            border: none;
            padding: 10px;
            background-color: #6f5901;
            width: 48%;
            cursor: pointer;
            margin: 5px 1%;
        }

        button:hover {
            background-color: #b08d00;
            color: #fff;
            transition: 0.3s;
        }
   
   </style>
</head>
<body>

<h1>Pendaftaran Lomba Taekwondo</h1> 

<form action="index.html">
    <fieldset>
        <legend>Formulir Pendaftaran</legend>

        <label for="nama">Nama</label>
        <input type="text" name="nama" id="nama" placeholder="Masukkan nama anda" required>

        <label for="email">Email</label>
        <input type="email" name="email" id="email" placeholder="Masukkan email anda" required>

        <label for="password">Password</label>
        <input type="password" name="password" id="password" placeholder="Masukkan password anda" required>

        <label for="alasan">Alasan Ingin Ikut Lomba Ini</label>
        <textarea name="alasan" id="alasan" placeholder="Ketik alasan anda ingin ikut lomba taekwondo" required></textarea>

        <label>Jenis Pertandingan</label>
        <input type="radio" name="jp" value="poomsae" id="poomsae" required>
        <label for="poomsae" style="display:inline;">Poomsae</label>
        <input type="radio" name="jp" value="kyourugi" id="kyourugi" required>
        <label for="kyourugi" style="display:inline;">Kyourugi</label>

        <label for="kategori">Kategori Umur</label>
        <select name="kategori" id="kategori" required>
            <option value="">-- Pilih kategori --</option>
            <option value="anak-anak">Anak-anak (7 - 12 Tahun)</option>
            <option value="remaja">Remaja (13 - 17 Tahun)</option>
            <option value="dewasa">Dewasa (18 - 40 Tahun)</option>
            <option value="master">Master (41+)</option>
        </select>

        <input type="checkbox" name="setuju" id="setuju" required>
        <label for="setuju" style="display:inline;">Dengan ini saya menyetujui untuk mengikuti pertandingan taekwondo</label>

        <div style="text-align:center; margin-top:20px;">
            <button type="submit">Kirim</button>
            <button type="reset">Reset</button>
        </div>
    </fieldset>
</form>
    
</body>
</html>
