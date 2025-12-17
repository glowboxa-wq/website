# website[index.html](https://github.com/user-attachments/files/24205697/index.html)
<!DOCTYPE html>
<html>
<head>
    <title>Glowbox - Tempat Cerita (Terbatas)</title>
    <style>
        /* Gaya dasar Dark Mode & Modern */
        body {
            background-color: #121212;
            color: #E0E0E0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            text-align: center;
            padding: 20px;
            margin: 0;
            display: flex;
            flex-direction: column; 
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }

        /* BILAH MERAH DI ATAS (Fixed) - Hanya muncul setelah login */
        .top-alert-bar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: #d9534f;
            color: white;
            font-size: 0.85rem;
            font-weight: bold;
            padding: 8px 0;
            z-index: 1000;
        }

        /* Kontainer utama untuk konten Glowbox */
        .container {
            max-width: 450px;
            width: 90%;
            padding: 30px;
            background: #1e1e1e;
            border-radius: 15px;
            box-shadow: 0 8px 30px rgba(0, 0, 0, 0.7);
            border: 1px solid #333;
        }

        /* Gaya untuk Form Kata Sandi */
        .password-form {
            max-width: 350px;
            width: 80%;
            padding: 20px;
            background: #1e1e1e;
            border-radius: 10px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.5);
            margin-bottom: 20px;
        }
        .password-form input[type="password"] {
            width: 100%;
            padding: 10px;
            margin-top: 10px;
            border-radius: 5px;
            border: 1px solid #333;
            background: #333;
            color: #E0E0E0;
            box-sizing: border-box;
        }
        .password-form button {
            margin-top: 15px;
            padding: 10px 20px;
            background-color: #4CAF50;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .password-form button:hover {
            background-color: #439d48;
        }

        /* Gaya Konten Glowbox */
        #GlowboxContent {
            display: none; /* Default: Sembunyikan konten utama */
        }
        
        .header { margin-bottom: 30px; }
        .logo { font-size: 50px; display: block; margin-bottom: 10px; }
        .logo span { color: #FFC107; text-shadow: 0 0 15px rgba(255, 193, 7, 0.8); }
        h2 { font-size: 2.5rem; color: #4CAF50; margin-bottom: 5px; font-weight: 600; }
        .slogan { color: #A0A0A0; font-size: 0.9rem; margin-bottom: 20px; }
        .tombol-chat {
            color: white; text-decoration: none; text-transform: uppercase;
            font-weight: bold; letter-spacing: 1px; font-size: 1.2rem;
            display: block; width: 100%; padding: 14px;
            background-color: #4CAF50; border-radius: 8px; cursor: pointer;
            transition: background-color 0.3s, transform 0.1s; margin-top: 20px; 
        }
        .tombol-chat:hover { background-color: #439d48; transform: translateY(-2px); }
        .tagline {
            color: #A0A0A0; font-size: 0.9rem; margin-top: 25px;
            line-height: 1.5; font-style: italic;
        }

        /* Gaya Tambahan untuk Kontak Bantuan */
        .contact-section {
            text-align: left;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid #333; /* Pemisah visual */
        }
        .contact-section h4 {
            color: #E0E0E0;
            font-size: 1.1rem;
            margin-top: 15px;
            margin-bottom: 5px;
        }
        .contact-section p {
            font-size: 0.9rem;
            color: #A0A0A0;
            margin-bottom: 5px;
        }
        .contact-section .detail {
            font-weight: bold;
            color: #4CAF50; /* Warna hijau untuk detail kontak */
        }
        /* Style untuk link yang dapat diklik */
        .contact-section a.detail {
            text-decoration: none; /* Hapus garis bawah */
            color: #4CAF50; /* Pastikan link tetap hijau */
        }
        .contact-section a.detail:hover {
            color: #FFC107; /* Ubah warna saat di-hover */
        }
    </style>
</head>
<body>

<div class="password-form" id="PasswordForm">
    <p style="color: #E0E0E0;">Masukkan Kata Sandi Kelas untuk mengakses Glowbox:</p>
    <input type="password" id="passwordInput" placeholder="Kata Sandi">
    <button onclick="checkPassword()">Akses</button>
    <p id="errorMsg" style="color: #d9534f; margin-top: 10px; display: none;">Kata sandi salah. Coba lagi.</p>
</div>

<div id="GlowboxContent">
    
    <div class="top-alert-bar">
        Jika pesan Anda belum dibalas, silakan tunggu beberapa saat.
    </div>

    <div class="container">
        <div class="header">
            <span class="logo">💡</span>
            <h2>Glowbox</h2>
            <p class="slogan">Give light of wisdom bringing openness & xperience.</p>
            <p style="color: #A0A0A0; margin-bottom: 20px;">Bagikan Cerita Anda, Biarkan Cahayanya Bersinar.</p>
        </div>

        <a href="https://tawk.to/chat/6931b01cfc6441197ee01459/1jbl1ftgj" target="_blank" class="tombol-chat">
            KIRIM CERITA PRIBADI
        </a>

        <p class="tagline">Meskipun aku tak secepat AI, aku hadir untukmu, bukan kode, tapi partner curhatmu.</p>
        
        <div class="contact-section">
            <h3 style="color: #E0E0E0; text-align: center; margin-bottom: 20px;">Kontak Dukungan Resmi (Technical Support)</h3>
            
            <h4>1. Email (Dukungan Resmi)</h4>
            <p>Tujuan Penggunaan: Dukungan teknis tingkat lanjut, permintaan *reset* atau konfirmasi Kata Sandi Akses, dan pertanyaan mengenai kebijakan privasi atau *backup* data.</p>
            <p>Alamat Email: <a href="mailto:glowboxa@gmail.com" class="detail" style="text-decoration: none;">glowboxa@gmail.com</a></p>

            <h4>2. WhatsApp (Dukungan Cepat)</h4>
            <p>Tujuan Penggunaan: Pertanyaan singkat mengenai status aplikasi, masalah koneksi ke *live chat*, atau pertanyaan cepat lainnya yang memerlukan balasan instan.</p>
            <p>Nomor WhatsApp: <a href="https://wa.me/6285378079608" target="_blank" class="detail" style="text-decoration: none;">085378079608</a></p>

            <h4>3. Jam Operasional (Respons Administrator)</h4>
            <p>Jam Operasional ini menunjukkan kapan Administrator Glowbox aktif dan dapat memberikan respons melalui email atau WhatsApp. Waktu di luar jam ini tidak menjamin balasan yang cepat.</p>
            <p>Hari Operasional: <span class="detail">Sabtu - Minggu</span></p>
            <p>Waktu Operasional: <span class="detail">Pukul 17.00 - 20.00 WIB</span></p>
            <p style="font-style: italic; margin-top: 10px;">Catatan: Meskipun cerita dapat dikirimkan kapan saja (24/7), balasan personal dan respons dukungan teknis hanya akan diproses selama Jam Operasional yang tercantum di atas.</p>
        </div>
    </div>

</div> <script type="text/javascript">
var Tawk_API=Tawk_API||{}, Tawk_LoadStart=new Date();

Tawk_API.onLoad = function(){
    Tawk_API.setWelcomeMessage('Balasan admin akan dikirim ke EMAIL yang Anda masukkan. Pastikan email Anda benar, ya!');
};

(function(){
var s1=document.createElement("script"),s0=document.getElementsByTagName("script")[0];
s1.async=true;
s1.src='https://embed.tawk.to/6931b01cfc6441197ee01459/1jbl1ftgj'; 
s1.charset='UTF-8';
s1.setAttribute('crossorigin','*');
s0.parentNode.insertBefore(s1,s0);
})();
</script>
<script>
    function checkPassword() {
        const password = document.getElementById('passwordInput').value;
        const correctPassword = 'pkom2022'; // KATA SANDI SUDAH DISET KE 'pkom2022'

        if (password === correctPassword) {
            document.getElementById('PasswordForm').style.display = 'none'; 
            document.getElementById('GlowboxContent').style.display = 'block'; 
            
            // Atur padding-top agar konten tidak tertutup bilah merah
            document.body.style.paddingTop = '50px'; 
            
        } else {
            document.getElementById('errorMsg').style.display = 'block'; 
        }
    }
</script>

</body>
</html>
