# PLANETIFY
## 🚀 Proyek Visualisasi Tata Surya 3D Interaktif

### Pendahuluan

Proyek ini adalah aplikasi visualisasi tata surya 3D interaktif yang dibangun menggunakan pustaka **THREE.js**. Aplikasi ini menampilkan model planet yang realistis, simulasi orbit dan rotasi, serta fitur interaktif untuk mengeksplorasi dan membandingkan detail setiap planet.

### Fitur Utama

Aplikasi ini menawarkan beberapa fitur inti yang berfokus pada interaksi pengguna dan visualisasi data:

1.  **Visualisasi 3D Realistis:**
      * Model 3D planet-planet Tata Surya, termasuk Matahari dan Bulan.
      * Simulasi **rotasi** dan **orbit** planet yang dinamis (diatur dalam `animate()` di `script.js`).
      * Efek visual tingkat lanjut seperti **Bloom** (menggunakan `UnrealBloomPass`) pada Matahari dan **Outline** pada planet yang di-*hover* atau dipilih.
2.  **Interaksi Planet:**
      * **Klik untuk *Zoom In***: Menggunakan **Raycasting** (`onDocumentMouseDown`) untuk mendeteksi klik pada objek planet atau atmosfer. Kamera akan bergerak secara mulus (`camera.position.lerp`) ke posisi dekat planet yang dipilih.
      * **Panel Informasi:** Menampilkan detail spesifik planet (`planetInfo`) setelah *zoom in*.
3.  **Mode Komparasi (Perbandingan):**
      * Fitur unik yang memungkinkan pengguna memilih **dua planet** untuk dibandingkan secara berdampingan.
      * Pada mode ini, planet diatur ulang posisinya ke titik `(-30, 0, 0)` dan `(30, 0, 0)` dan seluruh *scene* utama disembunyikan (`planetSystem.visible = false`) untuk fokus pada perbandingan.
4.  **Kontrol Pengguna:**
      * Menggunakan **dat.GUI** untuk panel kontrol seperti mengubah kecepatan simulasi dan mengatur efek visual.
      * Kontrol navigasi bebas **Orbit Controls** (`OrbitControls.js`) yang dapat dinonaktifkan secara otomatis saat *zoom in* ke planet.

-----

### 💻 Teknologi yang Digunakan

Proyek ini sepenuhnya dibangun pada *front-end* menggunakan:

  * **THREE.js:** Pustaka JavaScript untuk menampilkan grafis 3D pada *browser*.
  * **HTML5 & CSS3:** Untuk struktur dan *styling* antarmuka pengguna (UI) seperti panel informasi (`planetInfo`) dan mode perbandingan (`comparisonView`).
  * **JavaScript (ES6 Modules):** Logika utama, perhitungan orbit, dan penanganan interaksi.

-----

### 🛠️ Cara Menjalankan Proyek

Untuk menjalankan proyek ini secara lokal, Anda perlu menyiapkan lingkungan Node.js dan menginstal dependensi.

1.  **Kloning Repositori:**

    ```bash
    git clone https://github.com/Jakij4ki/Planetify.git
    cd Planetify
    ```

2.  **Instal Dependensi:**
    Pastikan Anda memiliki **Node.js** dan **npm** terinstal, lalu jalankan perintah berikut untuk menginstal semua paket yang dibutuhkan (termasuk *server* pengembangan):

    ```bash
    npm install
    ```

3.  **Jalankan Aplikasi:**
    Gunakan perintah *script* yang telah dikonfigurasi dalam `package.json` Anda untuk memulai *server* pengembangan lokal:

    ```bash
    npm run dev
    ```

4.  **Akses Aplikasi:**
    Aplikasi akan terbuka secara otomatis di *browser* Anda pada alamat yang ditunjukkan oleh *server* (biasanya `http://localhost:5173` atau sejenisnya).

-----

### 👥 Kontributor

  * Dzaky Rezandi- (235150207111006)
  * Rifqi Cahyono - (235150201111002)
  * Catherine Nathania - (235150201111042)
  * Very Fachrurozi - (235150207111003)
  * I Made Deva Satria Wiguna Giri - (235150200111054)

