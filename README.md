🤖 Tanyain — Chatbot FAQ Multi-Klien Berbasis Flask

Tanyain adalah sistem **Chatbot FAQ berbasis AI** yang dirancang untuk membantu **UMKM, sekolah, dan klinik kecil** menjawab pertanyaan pelanggan secara otomatis.  
Platform ini mendukung **multi-klien** dengan dashboard admin modern, analitik chatbot, serta sistem approval dari superadmin.  

🚀 Fitur Utama

- 🔐 Sistem Login & Register Multi-Role
  - Role: Client (pemilik chatbot)` dan Admin (superadmin)
  - Client baru perlu approval dari admin sebelum bisa mengakses sistem.
  
- 💬 Chatbot FAQ Pintar
  - Menggunakan **TF-IDF + Cosine Similarity** untuk mencocokkan pertanyaan pengguna dengan jawaban paling relevan.
  - Setiap klien memiliki dataset FAQ sendiri (diunggah via CSV).

- 📈 Dashboard Analitik
  - Statistik total chat, pertanyaan populer, distribusi chat terjawab vs tidak.
  - Grafik aktivitas chat 30 hari terakhir.
  - Dashboard global untuk admin (opsional).

- 🧾 Upload & Kelola FAQ
  - Upload file CSV berisi pertanyaan dan jawaban.
  - Tambah, edit, dan hapus data langsung dari dashboard.

- 🕵️ Approval System
  - Admin dapat menyetujui atau menolak klien baru melalui panel superadmin.

- 🌙 UI Modern & Responsif
  - Dibangun dengan Tailwind CSS
  - Tersedia mode Dark/Light
  - Sidebar animatif dan tampilan dashboard profesional.

- 🧠Teknologi yang Digunakan
  -Backend : Python, Flask, SQLAlchemy
  -Frontend:Tailwind CSS, Chart.js, HTML
  -Database: SQLite (dapat diganti ke MySQL/PostgreSQL)
  -NLP TF-IDF + Cosine Similarity 
  -Deployment Replit 


⚙️Cara Instalasi & Menjalankan Proyek

1. Clone repository ini:
   bash
   git clone https://github.com/username/tanyain.git
   cd tanyain

2. Buat virtual environment dan aktifkan
  -python -m venv venv
  -source venv/bin/activate    # Linux/Mac
  -venv\Scripts\activate       # Windows

3.Install dependecies
  -pip install -r requirements.txt

4.Jalankan aplikasi
  -flask run

5.Akses di Akses di: http://localhost:5000

**Struktur Proyek**
  tanyain/
  │
  ├── app.py                    # Entry utama Flask
  ├── models.py                 # Model database (Client, ChatHistory, FAQ)
  ├── static/                   # Gambar, CSS, JS
  │   └── img/T-putih.png
  ├── templates/                # Semua halaman HTML
  │   ├── base_superadmin.html
  │   ├── superadmin.html
  │   ├── index.html
  │   ├── analytics.html
  │   ├── login.html
  │   └── register.html
  ├── requirements.txt
  └── README.md

  **Tampilan Aplikasi**
  


   
