# SnapSpends - AI-Powered Receipt Tracker

<div align="center">
  <p><em>Proyek Matakuliah Rekayasa Perangkat Lunak (RPL)</em></p>
</div>

## 📖 Deskripsi Proyek
SnapSpends adalah aplikasi manajemen pengeluaran cerdas yang memungkinkan pengguna untuk memantau keuangan mereka cukup dengan memotret atau mengunggah foto struk belanja. Dengan memanfaatkan kecerdasan buatan dan OCR, sistem secara otomatis mengekstrak informasi penting seperti total belanja, tanggal, dan nama *merchant* untuk kemudian dicatat ke dalam database.

## ✨ Fitur Utama
- **Smart Receipt Scanning:** Ekstraksi teks dan data finansial dari gambar struk secara otomatis.
- **Expense Management:** Sistem CRUD untuk mencatat, mengedit, dan menghapus riwayat pengeluaran.
- **Interactive Interface:** Antarmuka responsif yang dirancang untuk kenyamanan pengguna (UX-focused).
- **RESTful API Architecture:** Pemisahan *backend* dan *frontend* yang jelas untuk skalabilitas kode.

## 🛠️ Tech Stack
- **Frontend:** Vue.js
- **Backend:** Python (FastAPI)
- **Database:** PostgreSQL / MySQL
- **AI / OCR Engine:** Google Cloud Vision API
- **Prototyping & Design:** Figma

## 🚀 Prasyarat (Prerequisites)
Pastikan perangkat lunak berikut sudah terinstal di sistem Anda:
- [Python 3.9+](https://www.python.org/)
- [Node.js & npm](https://nodejs.org/)
- [MySQL](https://www.mysql.com/) atau PostgreSQL
- Akun Google Cloud Platform (untuk file *credential key* JSON)

## ⚙️ Instalasi dan Setup

### 1. Setup Backend (FastAPI)
```bash
# Clone repository
git clone https://github.com/username/snapspends.git
cd snapspends/backend

# Buat virtual environment
python -m venv venv

# Aktivasi virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Konfigurasi Environment Variables
# Buat file .env dan isi dengan:
# DB_URL=mysql+pymysql://user:password@localhost:3306/snapspends
# GOOGLE_APPLICATION_CREDENTIALS="path/to/your/gcp-service-account-key.json"

# Jalankan server
uvicorn main:app --reload
```

### 2. Setup Frontend (Vue.js)
```bash
cd ../frontend

# Install node modules
npm install

# Jalankan development server
npm run dev
```

## 👨‍💻 Penulis
- **Daniel Abner** - Mahasiswa Informatika, Universitas Pradita
