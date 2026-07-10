# 📊 Analisis Network Observability pada Protokol Jaringan Terdistribusi

## 👤 Identitas Mahasiswa
* **Nama:** Putri Sahira Wulandari
* **Program Studi:** Data Science
* **Universitas:** Universitas Cakrawala
* **Materi:** Pertemuan 12 - Monitoring, Logging, Telemetry, & Observability

## 📦 Deskripsi Project
Project ini eksperimen menguji *Network Observability* menggunakan **Postman** dan **Wireshark**.

> **Analogi:** Kayak cek resi paket online. Status "Terkirim" di aplikasi harus dibuktikan dengan cek di gudang/log. Di sini kita cek sampai level paket jaringan.

## 🛠️ Lingkungan Pengujian
* **Demo App:** `http://127.0.0.1:8088`
* **Client:** Postman
* **Sniffer:** Wireshark

## 📈 Hasil Pengujian
1. **200 OK:** Request berhasil, Wireshark tangkap JSON
2. **404 Not Found:** Rute `/metrics-salah` ditolak
3. **400 Bad Request:** Payload `"scenario": null` ditolak
4. **n8n:** 2 hit tercatat di `/api/automation/inbox`

## 📷 Dokumentasi Bukti Eksperimen

### 1. HTTP 200 OK
![Screenshots/Metrics 200 OK](./matrics%20200ok.png)

### 2. HTTP 404 Not Found
![Metrics Salah](./matrics%20salah.png)

### 3. HTTP 400 Bad Request
![Observasi Log Null](./obsevasi%20log%20null.png)

### 4. Wireshark Capture
![Wireshark](./wiresharks%20p12.png)

### 5. Capture Scenario
![Capture Scenario](./capture%20scenario.png)

### 6. Integrasi n8n
![n8n](./n8n.png)

### 7. Custom Log
![Custom Log](./custome%20log.png)
