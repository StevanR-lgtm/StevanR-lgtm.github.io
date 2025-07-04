<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Web Pribadi Saya</title>
    <style>    
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;600&display=swap');

        body {
        font-family: 'Poppins', sans-serif;
        margin: 0;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        background-image: linear-gradient(240deg, #BAB0D4, #4C1A57);
        color: #f0f0f0;
        }
        .container {
        flex: 1 0 auto;
        max-width: 900px;
        margin: 40px auto 100px;
        padding: 20px;
        background: rgba(255 255 255 / 0.05);
        border-radius: 16px;
        box-shadow: 0 10px 30px rgba(0,0,0,0.3);
        display: flex;
        flex-direction: column;
        align-items: center;
        }
        .profile {
        display: flex;
        align-items: center;
        gap: 24px;
        margin-bottom: 48px;
        justify-content: center;
        flex-wrap: wrap;
        text-align: center;
        }
        .profile-photo {
        width: 120px;
        height: 120px;
        border-radius: 50%;
        object-fit: cover;
        border: 4px solid #4e99dbf6;
        box-shadow: 0 0 25px #0dd0e2fd;
        background: #222;
        }
        .profile-desc {
        max-width: 500px;
        font-size: 1.15rem;
        line-height: 1.5;
        }
        .text-row-3 {
        display: flex;
        justify-content: center;
        gap: 24px;
        width: 100%;
        margin-bottom: 40px;
        }
        .text-block {
        flex: 1;
        min-width: 100px;
        background: #334972cc;
        padding: 16px 20px;
        border-radius: 12px;
        box-shadow: 0 4px 8px #00000077;
        text-align: center;
        font-weight: 600;
        font-size: 1.1rem;
        transition: background 0.3s ease;
        }
        .text-block:hover {
        background: #460c55cc;
        color: #9faac0;
        cursor: default;
        }

        .text-row-2 {
        display: flex;
        justify-content: center;
        gap: 24px;
        width: 65%;
        margin-bottom: 48px;
        }
        .text-row-2 .text-block {
        flex: 1;
        min-width: 140px;
        }

        footer {
        flex-shrink: 0;
        background: linear-gradient(to top right, rgba(60, 60, 216, 0.798) ,rgb(20, 187, 181));
        padding: 20px 40px;
        color: #a19702;
        font-weight: 600;
        font-size: 1rem;
        position: relative;
        bottom: 0;
        left: 0;
        width: 210px;
        border-top-right-radius: 10px;
        box-shadow: 6px 8px 15px rgba(0, 0, 0, 0.87);
        }
        footer h2 {
        margin-top: 0;
        margin-bottom: 12px;
        font-weight: 700;
        font-size: 1.2rem;
        color: rgb(216, 216, 223);
        }
        footer ul {
        list-style: none;
        padding-left: 0;
        margin: 0;
        }
        footer ul li {
        margin-bottom: 8px;
        display: flex;
        align-items: center;
        gap: 10px;
        }
        .icon {
        font-size: 1.3rem;
        color: #B8E3FF;
        }

        @media (max-width: 720px) {
        .container {
            margin: 24px 12px 120px;
            width: 95%;
        }
        .profile {
            flex-direction: column;
            gap: 16px;
        }
        .text-row-3 {
            flex-direction: column;
        }
        .text-row-3 .text-block {
            margin-bottom: 16px;
            width: 100%;
        }
        .text-row-2 {
            flex-direction: column;
            width: 100%;
            gap: 16px;
        }
        .text-row-2 .text-block {
            width: 100%;
        }
        footer {
            position: fixed;
            width: auto;
            border-radius: 0;
            box-shadow: none;
            margin-top: 40px;
            padding-left: 20px;
        }
    }
    </style>
    <style type="text/css" id="operaUserStyle"></style>
</head>
<body>
    <script>
        function salam(){
            alert ("Selamat datang!");
        }
        salam();
    </script>
    <div class="container">
        <section class="profile" aria-label="profil">
            <img class="profile-photo" src="foto.jpeg" alt="foto profil">
            <div class="profile-desc">
                <h1>Stevan Christian Rengkeng</h1>
                <p>Mahasiswa Informatika</p>
            </div>
        </section>
        <section class="text-row-3" aria-label="teks bagian kedua"> 
            <div class="text-block">
                <h1>Biodata diri</h1>
                <p>TTL:</p>
                <p>Waipo, 4 juni 2003</p>
                <p>Alamat:</p>
                <p>Wainitu</p>
            </div>
            <div class="text-block">
                <h1>Pernah belajar di</h1>
                <p>Sd Inpres 2 Waipo</p>
                <p>Smp Negeri 1 Masohi</p>
                <p>Smk Negeri 1 Maluku Tengah</p>
            </div>
            <div class="text-block">
                <h1>Status saat ini</h1>
                <p>Menjadi salah satu mahasiswa di Universitas Kristen Indonesia Maluku pada Prodi Informatika</p>
            </div>
        </section>
        <section class="text-row-2" aria-label="teks bagian ketiga">
            <div class="text-block">
                <h1>Hobi</h1>
                <p>Playing video games</p>
                <p>Watching movie</p>
            </div>
            <div class="text-block">
                <h1>Harapan kedepannya</h1>
                <p></p>
            </div>
        </section>
    </div>
    <footer>
        <h2>Contact Me</h2>
        <ul>
            <li>
                <span class="icon"><img src="Email-logo.png" alt="logo-email" width="16px" width="16px"></span>
                <a href="mailto:stevanrengkeng901@gmail.com" target="_blank" rel="noopener noreferrer" style="color:#99cfff; text-decoration:none;">Gmail</a>
            </li>
            <li>
                <span class="icon"><img src="Whatsapp-logo.png" alt="logo-whatsapp" width="16px" width="16px"></span>
                <a href="https://wa.me/6281248426475" target="_blank" rel="noopener noreferrer" style="color:#99cfff; text-decoration:none;">WhatsApp</a>
            </li>
            <li>
                <span class="icon"><img src="insta-logo.png"alt="logo-instagram" height="16px" width="16px"></span>
                <a href="https://www.instagram.com/stvn_rengkeng/" target="_blank" rel="noopener noreferrer" style="color:#99cfff; text-decoration:none;">Instagram</a>
            </li>
            <li>
                <span class="icon"><img src="Facebook-logo.png" alt="logo-facebook" width="16px" width="16px"></span>
                <a href="https://www.facebook.com/stevan.rengkeng.750" target="_blank" rel="noopener noreferrer" style="color:#99cfff; text-decoration:none;">Facebook</a>
            </li>
        </ul>
    </footer>
</body>
</html>
