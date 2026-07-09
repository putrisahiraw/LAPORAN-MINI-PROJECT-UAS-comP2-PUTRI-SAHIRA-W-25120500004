# 📊 Analisis Network Observability pada Protokol Jaringan Terdistribusi

## 👤 Identitas Mahasiswa
* **Nama:** Putri Sahira Wulandari
* **Program Studi:** Data Science
* **Universitas:** Universitas Cakrawala
* **Materi:** Pertemuan 12 - Monitoring, Logging, Telemetry, & Observability

## 📦 Deskripsi Project
Project ini merupakan eksperimen mandiri untuk menguji aspek *Network Observability* pada aplikasi praktikum dosen dengan menggunakan **Postman** dan **Wireshark**.

## 🛠️ Lingkungan Pengujian
* **Demo App Target:** `http://127.0.0.1:8088`
* **Client:** Postman
* **Network Sniffer:** Wireshark

## 📈 Skenario Pengujian
### 1. Skenario Sukses (HTTP 200 OK)
Berhasil mengembalikan status `200 OK`. Wireshark berhasil menangkap paket JSON.

### 2. Skenario Gagal (HTTP 404 & 400)
- **404:** Rute salah `/metrics-salah` 
- **400:** Payload JSON cacat `"scenario": null`

### 3. Integrasi n8n
Dashboard mencatat **2 kali hit** pada rute n8n.

## 📷 Dokumentasi Bukti Eksperimen

### 1. Metrics 200 OK
![Metrics 200 OK](./matrics%20200ok.png)

### 2. Metrics Salah 404
![Metrics Salah](./matrics%20salah.png)

### 3. Observasi Log Null 400
![Observasi Log Null](./obsevasi%20log%20null.png)

### 4. Wireshark
![Wireshark](./wiresharks%20p12.png)

### 5. Capture Scenario
![Capture Scenario](./capture%20scenario.png)

### 6. n8n
![n8n](./n8n.png)

### 7. Custom Log
![Custom Log](./custome%20log.png)
