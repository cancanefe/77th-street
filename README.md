<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>77th Street LAPD</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background: url('image.png') no-repeat center center fixed;
            background-size: cover;
            color: white;
            text-align: center;
        }
        .header {
            background-color: rgba(0, 51, 102, 0.8);
            padding: 20px;
            font-size: 24px;
            font-weight: bold;
        }
        .container {
            padding: 20px;
            background-color: rgba(0, 0, 0, 0.6);
            border-radius: 10px;
            display: inline-block;
        }
        .button {
            display: inline-block;
            padding: 10px 20px;
            margin: 10px;
            background-color: #ffcc00;
            color: black;
            text-decoration: none;
            border-radius: 5px;
            font-size: 18px;
        }
        .button:hover {
            background-color: #ffaa00;
        }
        .gallery {
            display: grid;
            grid-template-columns: repeat(5, 1fr); /* 5 columns */
            gap: 20px;
            justify-content: center;
            margin-top: 20px;
        }
        .gallery img {
            width: 100%;
            height: auto;
            border-radius: 10px;
            border: 2px solid white;
            cursor: pointer;
        }
        .server-name {
            position: fixed;
            bottom: 10px;
            right: 10px;
            background-color: rgba(0, 0, 0, 0.5);
            padding: 10px;
            border-radius: 5px;
            font-size: 16px;
        }
    </style>
    <script>
        function addImage() {
            const fileInput = document.getElementById('imageInput');
            const gallery = document.querySelector('.gallery');
            if (fileInput.files.length > 0) {
                const file = fileInput.files[0];
                const reader = new FileReader();
                reader.onload = function(e) {
                    const img = document.createElement('img');
                    img.src = e.target.result;
                    img.alt = 'Yeni Personel';
                    img.onclick = function() { this.remove(); };
                    gallery.appendChild(img);
                }
                reader.readAsDataURL(file);
            }
        }
    </script>
</head>
<body>
    <div class="header">77th Street LAPD</div>
    <div class="container">
        <h2>Resmi LAPD RP Sunucusuna Hoş Geldiniz!</h2>
        <p>Los Angeles'ta bir polis memuru olarak sürükleyici rol yapma deneyimimize katılın.</p>
        <a href="https://discord.com/channels/1026293394332459020/1026299774313443468" class="button" target="_blank">Başvuru Yap</a>
        <a href="#rules" class="button">Sunucu Kuralları</a>
        <a href="https://discord.gg/GafvtthZC9" class="button" target="_blank">Discord'a Katıl</a>
    </div>
    
    <div class="container">
        <h2>Personel Galerisi</h2>
        <input type="file" id="imageInput" accept="image/*">
        <button class="button" onclick="addImage()">Görsel Yükle</button>
        <p>Bir görsele tıklayarak kaldırabilirsiniz.</p>
        <div class="gallery">
            <!-- 25 Personel Resmi -->
            <img src="officer1.jpg" alt="Officer 1" onclick="this.remove()">
            <img src="officer2.jpg" alt="Officer 2" onclick="this.remove()">
            <img src="officer3.jpg" alt="Officer 3" onclick="this.remove()">
            <img src="officer4.jpg" alt="Officer 4" onclick="this.remove()">
            <img src="officer5.jpg" alt="Officer 5" onclick="this.remove()">
            <img src="officer6.jpg" alt="Officer 6" onclick="this.remove()">
            <img src="officer7.jpg" alt="Officer 7" onclick="this.remove()">
            <img src="officer8.jpg" alt="Officer 8" onclick="this.remove()">
            <img src="officer9.jpg" alt="Officer 9" onclick="this.remove()">
            <img src="officer10.jpg" alt="Officer 10" onclick="this.remove()">
            <img src="officer11.jpg" alt="Officer 11" onclick="this.remove()">
            <img src="officer12.jpg" alt="Officer 12" onclick="this.remove()">
            <img src="officer13.jpg" alt="Officer 13" onclick="this.remove()">
            <img src="officer14.jpg" alt="Officer 14" onclick="this.remove()">
            <img src="officer15.jpg" alt="Officer 15" onclick="this.remove()">
            <img src="officer16.jpg" alt="Officer 16" onclick="this.remove()">
            <img src="officer17.jpg" alt="Officer 17" onclick="this.remove()">
            <img src="officer18.jpg" alt="Officer 18" onclick="this.remove()">
            <img src="officer19.jpg" alt="Officer 19" onclick="this.remove()">
            <img src="officer20.jpg" alt="Officer 20" onclick="this.remove()">
            <img src="officer21.jpg" alt="Officer 21" onclick="this.remove()">
            <img src="officer22.jpg" alt="Officer 22" onclick="this.remove()">
            <img src="officer23.jpg" alt="Officer 23" onclick="this.remove()">
            <img src="officer24.jpg" alt="Officer 24" onclick="this.remove()">
            <img src="officer25.jpg" alt="Officer 25" onclick="this.remove()">
        </div>
    </div>

    <div class="server-name">Mevcut Sunucu: 77th Street LAPD</div>
</body>
</html>
