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
