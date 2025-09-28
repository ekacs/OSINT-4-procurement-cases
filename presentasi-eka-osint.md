Berdasarkan penelitian yang ada, teknik Open Source Intelligence (OSINT) telah terbukti menjadi alat yang sangat efektif untuk menginvestigasi pelaksanaan dan kasus dalam pengadaan barang/jasa pemerintah di Indonesia. Pendekatannya bersifat sistematis dengan memanfaatkan data terbuka yang tersedia untuk publik seringkali digunakan oleh jurnalis investigasi dan detektif swasta.

**Pendahuluan - OSINT untuk Pengawasan Pengadaan**

* **Definisi OSINT Singkat:**
* **Mengapa Relevan?**
  * **Transparansi & Akuntabilitas:** Memperkuat pengawasan sosial (social auditing).
  * **Pencegahan Korupsi:** Mengidentifikasi indikasi markup, kolusi, dan conflict of interest sejak dini.
  * **Demokratisasi Pengawasan:** Setiap orang bisa menjadi pengawas mandiri dengan akses internet.

### 🛠️ Langkah-Langkah Praktis Investigasi OSINT untuk Pengadaan

Indonesia Corruption Watch (ICW) telah mengembangkan metodologi enam langkah yang dapat dijadikan panduan oleh masyarakat sipil, jurnalis, dan aparat pengawas internal pemerintah (APIP) .

1. **Temukan Proyek Mencurigakan:**
   Seorang investigator perlu peka terhadap pemberitaan yang sedang viral atau identifikasi masalah dari pengumuman pengadaan pemerintah.
   situs PBJ Pemerintah (**spse.inaproc**) dan e-commerce Pemerintah (**katalog.inaproc**)
2. **Identifikasi Pengadaan Pemerintah yang berisiko terjadi fraud**:
   Langkah pertama adalah memilih pengadaan yang akan dipantau,dari sumber informasi primer terbuka
   [(cek **Github saya**)](github%20OSINT%20source%204%20national%20eprocurement.md)

   Anda dapat menggunakan platform seperti **opentender.net** yang memberikan peringkat risiko (tinggi, menengah, rendah) pada setiap prosedur pengadaan khusus pelelangan berdasarkan metode analisis PFA(*Potential Fraud Analysis*) dari Indonesia Corruption Watch (ICW). Namun dikarenakan basis data **opentender.net** tidak update (data terbaru biasanya setahun sebelumnya) sehingga perlu mengetahui cara mengidentifikasi secara mandiri.
   Berikut 7 redflags pengadaan yang perlu dicermati:([metode PFA](https://www.opentender.net/method))
   a. Durasi antara tanggal pengumuman dengan penetapan pemenang
   b. Perbandingan Nilai Kontrak dan HPS
   c. Nilai Kontrak Tinggi
   d. Tender dengan judul kurang dari 20
   e. Tender dengan deskripsi kurang dari 60 karater
   f. Pengadaan di kuartal 4
   g. Pemenang berulang
   Tambahan baru dari saya:
   h. Pengadaan Multiyears (lewat tahun anggaran)
   i. Pengadaan tidak mengikat (berada di akhir tahun atau awal tahun)
   j. Pengadaan yang ber-episode (cirinya judul pengadaan diberikan kata tahap dari apa)
3. **Tinjau Proses Perencanaan**:
   Pastikan proyek yang akan dilaksanakan sudah tercantum dalam rencana umum pengadaan (**SIRUP** dan **AMEL Perencanaan**). Proyek yang tidak ada dalam perencanaan keduanya atau perbedaan keduanya dapat mengindikasikan permasalahan.
4. **Identifikasi Pengadaan Serupa**: Cari tahu apakah ada pengadaan yang serupa di lokasi yang sama dalam kurun waktu tertentu. Pengadaan berulang untuk pekerjaan yang sama (misalnya, perbaikan jalan yang berulang dengan spesifikasi berbeda) dapat menjadi tanda pemborosan atau kecurangan.
5. **Tinjau Rekam Jejak Perusahaan**: Periksa latar belakang perusahaan pemenang tender. Anda dapat:

   - Memeriksa **track record** perusahaan dalam mengerjakan proyek pemerintah melalui opentender.net .
   - Mengecek dokumen legal perusahaan seperti akta pendirian dan kepemilikan saham melalui website **Direktorat Jenderal Administrasi Hukum Umum (AHU) Kementerian Hukum dan HAM** untuk mendeteksi kemungkinan conflict of interest atau perusahaan shell .
   - Memverifikasi kualifikasi perusahaan di sistem **SIKaP LKPP** dan memeriksa apakah perusahaan pernah masuk daftar hitam (**blacklist**) di **inaproc.lkpp.go.id** .
   - Telusuri di OSS:** Cek latar belakang perusahaan (kapan berdiri, modal, **pemegang saham, dan pengurus/direksi**).
   - .  **Identifikasi Perusahaan Pemenang:** Dapatkan nama dan NPWP-nya dari LPSE.

**Slide 4: Peta Sumber Data Kunci Indonesia (The "Gold Mine")** >> buat di github

* **Kategorikan sumber-sumber primer yang WAJIB diketahui:**
  * **Sumber Resmi Pengadaan:**
    * **LPSE (Layanan Pengadaan Secara Elektronik):** `lpse.kemenkeu.go.id` - Sumber utama informasi lelang (pengumuman, hasil, HPS, dll).
    * **SIRUP (Sistem Rencana Umum Pengadaan):** `sirup.lkpp.go.id` - Untuk melihat perencanaan pengadaan dari awal.
  * **Sumber Data Perusahaan & Keuangan:**
    * **OSS (Online Single Submission):** `oss.go.id` - Mengecek legalitas, pemegang saham, dan pengurus perusahaan.
    * **Data Indonesia:** `data.id` - Portal data terbuka pemerintah.
  * **Sumber Pendukung:**
    * **Laporan Keuangan Perusahaan Publik:** Untuk membandingkan kinerja.
    * **Google Maps/Street View:** Memverifikasi lokasi proyek fisik.
    * **Media Sosial & Berita Online:** Melacak reputasi dan koneksi perusahaan.

5. **Tinjau Pelaksanaan Proyek**: Untuk proyek konstruksi, Anda dapat menggunakan teknik OSINT untuk memverifikasi realisasi di lapangan .

   - **Google Maps/Street View**: Memeriksa kemajuan fisik proyek.
   - **Berita Online**: Melacak apakah ada pemberitaan tentang masalah pada proyek, seperti jembatan yang runtuh tak lama setelah dibangun.
   - **Putusan Pengadilan**: Mengecek melalui website Mahkamah Agung apakah perusahaan pernah terlibat dalam perkara pidana atau perdata.
6. **Analisis Koneksi & Jejak Kepemilikan (Mencari "Benyamin")**
   **Ini inti dari investigasi.**

   * **Conflict of Interest:** Bandingkan nama pengurus perusahaan pemenang dengan nama pejabat di instansi yang mengadakan. Gunakan mesin pencari untuk mencocokkan.
   * **Perusahaan "Benyamin":** Apakah perusahaan pemenang adalah UKM baru dengan modal kecil yang memenangkan proyek miliaran? Cek di OSS.
   * **Kluster Perusahaan:** Apakah satu orang atau alamat yang sama memiliki banyak perusahaan yang sering ikut lelang yang sama? (Gunakan fitur pencarian lanjutan di OSS/SIRUP).
   * **Visualisasi Koneksi:** Gunakan diagram sederhana untuk menunjukkan hubungan antara Pejabat -> Perusahaan A -> Perusahaan B.
     **Analisis dan Pelaporan**: Kumpulkan semua bukti dan lakukan analisis mendalam untuk mengidentifikasi kemungkinan pelanggaran. Pada tahap ini, laporan audit dari **Badan Pemeriksa Keuangan (BPK)** dapat menjadi sumber verifikasi yang penting .
7. 

### 💡 Contoh Kasus: Investigasi Tirai DPR RI

Pada 2022, ICW menggunakan OSINT untuk menginvestigasi pengadaan tirai untuk kediaman anggota DPR RI yang bernilai sangat tinggi, mencapai Rp 43,5 miliar .

- **Identifikasi Risiko**: Proyek ini teridentifikasi memiliki **potensi risiko kecurangan yang tinggi** di platform opentender.net .
- **Analisis Proses**: Meski ada 49 peserta yang mendaftar, hanya **3 perusahaan** yang memasukkan penawaran. Dari ketiganya, dua perusahaan dinyatakan tidak lulus kualifikasi .
- **Temuan**: Investigasi lebih lanjut menunjukkan bahwa hanya satu perusahaan yang memenuhi kualifikasi yang diminta. Hal ini menimbulkan kecurigaan kuat bahwa proses tender hanyalah formalitas dan kompetisi bisnis tidak berlangsung sehat . Kasus ini menunjukkan bagaimana data terbuka dapat mengungkap kejanggalan dalam proses pengadaan.

### ⚠️ Tantangan dan Kendala yang Dihadapi

Meski powerful, penerapan OSINT dalam investigasi pengadaan di Indonesia menghadapi beberapa tantangan :

- **Integrasi Data**: Tidak semua data, terutama dari Badan Usaha Milik Negara (BUMN), terintegrasi penuh dengan sistem pengadaan nasional .
- **Keterbatasan Akses Informasi**: Meski diatur hukum, permintaan informasi publik terkait pengadaan tertentu masih sering ditolak .
- **Beban Pembuktian yang Tinggi**: Laporan dari masyarakat kepada LKPP harus disertai dengan bukti awal yang substansial, dan banyak laporan ditolak karena dianggap buktinya belum lengkap .

Semoga informasi ini memberikan Anda kerangka yang jelas untuk menyusun materi presentasi. Jika ada aspek tertentu yang ingin Anda gali lebih dalam, seperti tools teknis OSINT atau studi kasus lainnya, silakan ditanyakan.
