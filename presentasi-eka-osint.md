# **OSINT untuk Pengawasan Pengadaan**

 Saat ini teknik Open Source Intelligence (OSINT) telah terbukti menjadi alat yang sangat efektif untuk menginvestigasi pelaksanaan dan kasus dalam pengadaan barang/jasa pemerintah di Indonesia. Pendekatannya bersifat sistematis dengan memanfaatkan data terbuka yang tersedia untuk publik seringkali digunakan oleh jurnalis investigasi dan detektif swasta.

### **Definisi OSINT Singkat**

   **OSINT (Open Source Intelligence)** adalah proses mengumpulkan dan menganalisis informasi dari sumber terbuka yang legal dan tersedia untuk publik, seperti media online, dokumen pemerintah, laporan akademik, media sosial, dan data publik lainnya, untuk tujuan intelijen atau investigasi.
   Dulu dikenal eksklusif di dunia CyberSecurity tapi sekarang diperuntukkan untuk kegiatan jurnalis.

### **Mengapa Relevan?**

* **Transparansi & Akuntabilitas:** Memperkuat pengawasan sosial (social auditing).
* **Pencegahan Korupsi:** Mengidentifikasi indikasi markup, kolusi, dan conflict of interest sejak dini.
* **Demokratisasi Pengawasan:** Setiap orang bisa menjadi pengawas mandiri dengan akses internet.

### **Syarat dan Kemampuan yang dibutuhkan**

#### 🧠 **Kemampuan Utama**

**Kemampuan riset dan analisis**
Mampu menelusuri data, dokumen, dan sumber informasi secara mendalam, termasuk wawancara dan observasi lapangan.

- Kemampuan menulis dan menyusun narasi
  Mampu menyampaikan temuan secara sistematis, menarik, dan mudah dipahami, termasuk menyederhanakan isu kompleks.
- Kemampuan komunikasi interpersonal
  Penting untuk membangun kepercayaan dengan narasumber, menggali informasi sensitif, dan menjaga etika wawancara.
- Pemahaman hukum dan etika jurnalistik
  Mengetahui batasan hukum, hak privasi, dan prinsip-prinsip etika agar tidak melanggar hak individu atau institusi.

#### 🔍 Karakteristik Investigatif

- Rasa ingin tahu yang tinggi dan skeptisisme sehat
  Tidak mudah puas dengan jawaban permukaan; selalu bertanya “mengapa”, “siapa lagi yang terlibat”, dan “apa dampaknya”.
- Ketekunan dan kesabaran
  Investigasi bisa memakan waktu lama dan menghadapi banyak hambatan. Jurnalis harus tahan banting dan tidak mudah menyerah.
- Keberanian dan integritas
  Siap menghadapi risiko, tekanan, atau intimidasi, terutama saat mengungkap skandal atau pelanggaran besar.

#### 🛠️ Teknik dan Metodologi

- Menguasai teknik penelusuran fakta
  Termasuk rekonstruksi peristiwa, analisis pola, dan pemetaan aktor yang terlibat dalam isu.
- Kemampuan digital dan teknologi
  Mampu menggunakan alat bantu digital untuk riset, verifikasi data, dan keamanan informasi.
- Kreativitas dalam memilih angle liputan
  Liputan investigasi bukan hanya soal data, tapi juga bagaimana menyajikan “story behind the news” secara menarik dan berdampak.
- Teknik dan aplikasi yang biasa saya gunakan, [cekidot](OSINT-tools-(frequently%20used)-PoC.md)

## 🛠️ Langkah-Langkah Praktis Investigasi OSINT untuk Pengadaan

1. **Temukan Proyek Mencurigakan:**
   Seorang investigator perlu peka terhadap pemberitaan yang sedang viral atau identifikasi masalah dari pengumuman pengadaan pemerintah.
   situs PBJ Pemerintah (**spse.inaproc**), e-commerce Pemerintah (**katalog.inaproc**) dan/atau pengadaan di BUMN,
2. **Identifikasi Pengadaan Pemerintah yang berisiko terjadi fraud**:
   Langkah pertama adalah memilih pengadaan yang akan dipantau,dari sumber informasi primer terbuka
   [(cekidot **sumber yang sering saya kunjungi**)](github%20OSINT%20source%204%20national%20eprocurement.md)

   Anda dapat menggunakan platform seperti **opentender.net** yang memberikan peringkat risiko (tinggi, menengah, rendah) pada setiap prosedur pengadaan berdasarkan metode analisis PFA(*Potential Fraud Analysis*) dari Indonesia Corruption Watch (ICW). Namun saat basis data **opentender.net** tidak update (data terbaru biasanya setahun sebelumnya dan hanya khusus tender saja) sehingga perlu mengetahui cara mengidentifikasi pengadaan bermasalah secara mandiri.
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
4. **Identifikasi Pengadaan Serupa**: Cari tahu apakah ada pengadaan yang serupa di lokasi yang sama dalam kurun waktu tertentu. Pengadaan berulang untuk pekerjaan yang sama (misalnya, perbaikan jalan yang berulang dengan spesifikasi berbeda dan/atau perbedaan harga yang tidak wajar) dapat menjadi tanda pemborosan atau kecurangan.
5. **Tinjau Rekam Jejak Perusahaan**: Periksa latar belakang perusahaan pemenang tender. Anda perlu melakukan:

   - **Identifikasi Perusahaan Pemenang:** Dapatkan NAma Perusahaan dan NPWP-nya dari SPSE.
   - Memeriksa **track record** perusahaan dalam mengerjakan proyek pemerintah melalui opentender.net.
   - **Putusan Pengadilan**: Mengecek melalui website **Mahkamah Agung** atau **Komisi Pengawas Persaiangan Usaha (KPPU)** apakah perusahaan pernah terlibat dalam perkara pidana atau perdata.
   - Mengecek dokumen legal perusahaan seperti akta pendirian dan kepemilikan saham melalui website **Direktorat Jenderal Administrasi Hukum Umum (AHU) Kementerian Hukum dan HAM** untuk mendeteksi kemungkinan conflict of interest atau perusahaan shell (cangkang) .
   - Memverifikasi kualifikasi perusahaan di sistem **SIKaP LKPP** dan memeriksa apakah perusahaan pernah masuk daftar hitam (**blacklist**) di **inaproc.lkpp.go.id** .
   - Telusuri di OSS:** Cek latar belakang perusahaan (kapan berdiri, modal, **pemegang saham, dan pengurus/direksi**).
6. **Tinjau Realisasi Pelaksanaan Proyek**: Untuk proyek konstruksi, apabila memungkinkan Anda perlu memverifikasi realisasi di lapangan.
   Terkadang pemeriksaan kemajuan fisik proyek bisa diketahui dari  **Google-Earth/ Google-Maps/Street View**: Memeriksa kemajuan fisik proyek atau pemberitaan di media online, bahkan terdapat kemungkinan juga video/foto yang diupload di platform social media, anda perlu mencermati tanggal uploadnya
7. **Analisis potensi kecurangan**

   * **Telusuri data orang penting** Cari tahu orang-orang yang berada di perusahaan (pemilik/pengurus/keluarga), melalui situs perusahaan, alamat email yang terhubung, linKedIn, dan semua platform social media
   * **Conflict of Interest:** Bandingkan nama pengurus perusahaan pemenang dengan nama pejabat di instansi yang mengadakan. Gunakan mesin pencari untuk mencocokkan.
   * **Keuangan Perusahaan "Benyamin":** Apakah perusahaan pemenang adalah UKM baru dengan modal kecil yang memenangkan proyek miliaran? Cek di OSS.
   * **Kluster Perusahaan:** Apakah satu orang atau alamat yang sama memiliki banyak perusahaan yang sering ikut lelang yang sama? (Gunakan fitur pencarian lanjutan di OSS/SIRUP).
   * **Visualisasi Koneksi:** Gunakan diagram sederhana untuk menunjukkan hubungan antara Pejabat -> Perusahaan A -> Perusahaan B.
     **Analisis dan Pelaporan**: Kumpulkan semua bukti dan lakukan analisis mendalam untuk mengidentifikasi kemungkinan pelanggaran. Pada tahap ini, laporan audit dari **Badan Pemeriksa Keuangan (BPK)** dapat menjadi sumber verifikasi yang penting .

### 💡 Contoh Kasus: Investigasi Tirai DPR RI

Pada 2022, ICW menggunakan OSINT untuk menginvestigasi pengadaan tirai untuk kediaman anggota DPR RI yang bernilai sangat tinggi, mencapai Rp 43,5 miliar .

- **Identifikasi Risiko**: Proyek ini teridentifikasi memiliki **potensi risiko kecurangan yang tinggi** di platform opentender.net .
- **Analisis Proses**: Meski ada 49 peserta yang mendaftar, hanya **3 perusahaan** yang memasukkan penawaran. Dari ketiganya, dua perusahaan dinyatakan tidak lulus kualifikasi .
- **Temuan**: Investigasi lebih lanjut menunjukkan bahwa hanya satu perusahaan yang memenuhi kualifikasi yang diminta. Hal ini menimbulkan kecurigaan kuat bahwa proses tender hanyalah formalitas dan kompetisi bisnis tidak berlangsung sehat . Kasus ini menunjukkan bagaimana data terbuka dapat mengungkap kejanggalan dalam proses pengadaan.

### 💡 Contoh Kasus: Pengadaan Senjata Penanganan Demonstran

lihat video berikut yang berjudul [Janggal Pengadaan Senjata Polri, Ada Driver Ojol Jadi Pemenang Tender](https://www.youtube.com/watch?v=Yys81jvvEio)

### ⚠️ Tantangan dan Kendala yang Dihadapi

Meski powerful, penerapan OSINT dalam investigasi pengadaan di Indonesia menghadapi beberapa tantangan :

- **Integrasi Data**: Tidak semua data, terutama dari Badan Usaha Milik Negara (BUMN), terintegrasi penuh dengan sistem pengadaan nasional .
- **Keterbatasan Akses Informasi**: Meski diatur hukum, permintaan informasi publik terkait pengadaan tertentu masih sering ditolak .
- **Beban Pembuktian yang Tinggi**: Laporan dari masyarakat kepada LKPP harus disertai dengan bukti awal yang substansial, dan banyak laporan ditolak karena dianggap buktinya belum lengkap .

Semoga informasi ini memberikan Anda kerangka yang jelas untuk menyusun materi presentasi. Jika ada aspek tertentu yang ingin Anda gali lebih dalam, seperti tools teknis OSINT atau studi kasus lainnya, silakan ditanyakan.
