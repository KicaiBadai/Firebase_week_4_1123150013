## README.md yang sudah dirapikan:

# Firebase_week_4_1123150013

### Cara Login Firebase & Buat Project Baru

---

## 📌 Langkah-langkah

**1. Login ke Firebase Console**
- Buka [firebase.google.com](https://firebase.google.com/)
- Klik **"Go to console"** (pojok kanan atas)
- Pilih akun Google Anda

**2. Buat Project Baru**
- Klik **"Create a project"** atau **"Add project"**
- Masukkan **nama project** → Klik **"Continue"**
- **Google Analytics**: Pilih "Enable" atau "Disable" (jika tidak perlu, matikan saja)
- Klik **"Create project"**
- Tunggu proses selesai → Klik **"Continue"**

---

## 📸 Screenshot Tutorial

| No | Langkah | Gambar |
|:--:|---------|--------|
| **1** | Klik **"Go to console"** | <img src="https://github.com/user-attachments/assets/08695cd2-45ae-42a7-9e42-2d94200ac1da" width="400"> |
| **2** | Klik **"Create project"** | <img src="https://github.com/user-attachments/assets/d1548006-2b2b-49c0-895f-0140d345172a" width="400"> |
| **3** | Tampilan project selesai | <img src="https://github.com/user-attachments/assets/94c8468b-6681-4008-b914-ae3e2e140bfd" width="400"> |

---

## 🔑 Mendapatkan API Key

**3. Ambil API Key**
- Masuk ke halaman **Project Overview**
- Klik ikon **⚙️ Settings** (roda gigi) → pilih **"Project settings"**
- Di menu **"General"**, scroll ke bawah ke bagian **"Your apps"**
- Pilih ikon **Web** `</>` (jika belum ada, tambahkan app web dulu)
- Copy **`apiKey`** yang ada di dalam konfigurasi Firebase

**Contoh tampilan:**
<img src="https://github.com/user-attachments/assets/5574a963-aa1b-43b8-a9c7-74b260cf62a3" width="600">

---

## 🔐 Mengaktifkan Authentication

**4. Aktifkan Sign-in Method**
- Di Firebase Console, klik menu **"Authentication"** di sidebar kiri
- Pilih tab **"Sign-in method"**
- Klik **"Email/Password"**
- Aktifkan dengan mengklik toggle **"Enable"**
- Klik **"Save"**

**Tampilan Authentication:**
<img src="https://github.com/user-attachments/assets/fc221cd6-6018-4be3-bd94-5478a5597a22" width="600">

---

## 🚀 Setup Environment di Postman

**5. Buat Environment Baru di Postman**
- Buka **Postman**
- Klik **"Environments"** (sidebar kiri)
- Klik **"New Environment"**
- Beri nama: **`firebase auth dev`**
- Tambahkan variable berikut:

| Variable | Value | Keterangan |
|----------|-------|------------|
| `FIREBASE_API_KEY` | `AIzaSyB_xxx...` | Web API Key dari Firebase Console |
| `FIREBASE_ID_TOKEN` | (diisi otomatis) | Diisi otomatis setelah login (via Test script) |
| `BACKEND_BASE_URL` | `http://localhost:8080/v1` | Base URL backend kamu |
| `BACKEND_TOKEN` | (diisi setelah verify) | Token JWT dari backend |
| `USER_EMAIL` | `test@example.com` | Email untuk testing |
| `USER_PASSWORD` | `Test@12345` | Password untuk testing |

**Tampilan Environment:**
<img src="https://github.com/user-attachments/assets/ec83e65b-3cbf-4d1f-aecc-82f68dafeee1" width="600">

---

## 📬 Testing API dengan Postman

**6. Konfigurasi Request**

**Endpoint:**
<img src="https://github.com/user-attachments/assets/d9b67698-17df-4091-b737-6e0d27d56836" width="600">

**Headers:**
<img src="https://github.com/user-attachments/assets/8c40c4ca-2fe2-4ca9-9883-ee0cc5f77296" width="600">

**Body (Raw JSON):**
<img src="https://github.com/user-attachments/assets/2fcd2b38-997b-40a1-a8e6-d5ee30d292c6" width="600">

**Response (200 OK):**
<img src="https://github.com/user-attachments/assets/8b2e4751-3026-40d3-94e8-e7401cecdbe6" width="600">

---

## 📝 Membuat Script

**7. Tambahkan Script**
<img src="https://github.com/user-attachments/assets/cb8a061f-a104-4480-9593-902a7c04ee88" width="600">

---

## 📧 Verifikasi Email

**8. Kirim Email Verifikasi**

**Endpoint (POST):**
<img src="https://github.com/user-attachments/assets/b617fac0-8224-46a9-9812-873e5eb2a508" width="600">

**Headers:**
<img src="https://github.com/user-attachments/assets/7870c325-bf91-4679-b286-f180f8459396" width="600">

**Body (Raw JSON):**
<img src="https://github.com/user-attachments/assets/d9eafb69-237b-48a4-b2c1-bf265bb27c49" width="600">

**Pastikan Response 200 OK:**
<img src="https://github.com/user-attachments/assets/17425093-c7d6-4d5c-8764-79d140370e4d" width="600">

**9. Cek Email untuk Verifikasi**
- Buka kotak masuk email yang digunakan
- Jika tidak ada, periksa folder **Spam**
- Klik tautan verifikasi yang dikirim

**Contoh Email Verifikasi:**
<img src="https://github.com/user-attachments/assets/8c4a9d37-20f9-414f-8f3d-d0907f1ba67c" width="600">

---

## ✅ Selesai!
Project Firebase siap digunakan. Simpan API Key dengan aman! 🎉

---

### Catatan:
- Pastikan `FIREBASE_API_KEY` diisi dengan benar
- Untuk pengujian, gunakan email yang benar-benar dapat diakses
- Simpan semua credential dengan aman
