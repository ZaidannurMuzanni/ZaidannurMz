# Praktikum 3 – Web Service Architecture  
Mata Kuliah: Web Service Engineering  

## 📌 Identitas
- Nama   : Zaidannur Muzanni
- NIM    : 230104040225
- Kelas  : TI23a
- Dosen  : Muhayat, M.IT

---

## 📖 Deskripsi Praktikum
Praktikum ini bertujuan untuk memahami dan membandingkan tiga arsitektur utama
dalam Web Service, yaitu **Client–Server**, **Service Oriented Architecture (SOA)**,
dan **Microservices**.  
Pada praktikum ini mahasiswa membangun layanan sederhana menggunakan **Node.js
dan Express**, lalu menguji komunikasi antar service menggunakan **Postman dan Browser**.

---

## 🎯 Tujuan
1. Memahami konsep Client–Server, SOA, dan Microservices  
2. Membangun web service sederhana sesuai arsitektur  
3. Menguji request–response menggunakan HTTP  
4. Menganalisis kelebihan dan kekurangan tiap arsitektur  

---

## 🛠️ Tools & Teknologi
- Node.js (LTS)
- Express.js
- Postman
- Browser (Chrome)
- Visual Studio Code

---

## 🧩 Arsitektur yang Diimplementasikan

### 1️⃣ Client–Server
Client mengirim request langsung ke satu server utama dan menerima response.

Endpoint:
- `GET /hello`
- `POST /mahasiswa`
- `GET /mahasiswa`
- `PUT /mahasiswa/:nim`
- `DELETE /mahasiswa/:nim`

---

### 2️⃣ Service Oriented Architecture (SOA)
Aplikasi dibagi menjadi dua service terpisah:
- **Authentication Service** (Login & JWT)
- **Data Service** (Akses data dengan token)

Alur:
1. Client login ke Auth Service
2. Auth Service mengembalikan JWT
3. Client mengakses Data Service menggunakan token

---

### 3️⃣ Microservices
Aplikasi mini dibagi menjadi beberapa service independen:
- API Gateway
- Authentication Service
- Product Service
- Order Service
- Notification Service

Setiap service berjalan di port berbeda dan berkomunikasi melalui HTTP API.

---

## ▶️ Cara Menjalankan Project

### Client–Server
```bash
npm install
node server.js

