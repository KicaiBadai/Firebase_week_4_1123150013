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

## ✅ Selesai!
Project Firebase siap digunakan. Simpan API Key dengan aman! 🎉
