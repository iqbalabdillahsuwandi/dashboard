Analisis Data Bike Sharing
=========================================
Proyek ini menganalisis data Bike Sharing berdasarkan data historis yang mencakup informasi seperti waktu, kondisi cuaca, dan jumlah pengguna. Dashboard interaktif dibangun menggunakan Streamlit untuk memvisualisasikan dan mengeksplorasi data secara dinamis.

=========================================
Persyaratan
=========================================
Sebelum menjalankan dashboard, pastikan Anda telah menginstal perangkat lunak berikut:

- Python (versi 3.6 atau lebih tinggi)
- Pip (Package Installer for Python)
- Numpy
- Streamlit
- Pandas
- Matplotlib
- Seaborn
- Babel

Anda dapat menginstal semua pustaka yang diperlukan dengan menjalankan perintah berikut:
bash
`pip install numpy streamlit pandas matplotlib seaborn babel`

=========================================
Menjalankan dashbord
=========================================
Menyalin repositori
  `git clone https://github.com/iqbalabdillahsuwandi/submission.git`
  `cd submission`

Menjalankan streamlit
  Setelah mengkloning repositori, buka terminal (atau command prompt) dan navigasikan ke direktori tempat repositori dikloning. Jalankan perintah berikut untuk memulai aplikasi Streamlit:
  `streamlit run dashboard.py`


=========================================
Metode Analisis Data
=========================================
Dalam analisis data ini, menggunakan beberapa metode dan teknik analisis yang berbeda untuk memahami pola yang ada. Berikut metode yang digunakan:

=========================================
1. Analisis Deskriptif
=========================================
Analisis deskriptif digunakan untuk memahami karakteristik dasar data. Metode ini melibatkan penggunaan statistik dasar seperti rata-rata (mean), median, modus, maksimum, minimum, dan standar deviasi. Dalam dataset ini, kita menggunakan analisis deskriptif untuk memahami distribusi data pengguna berdasarkan waktu (jam, hari, musim) dan variabel lainnya seperti suhu, kelembaban, kecepatan angin, dll.

=========================================
2. Pengelompokan (Grouping) dan Agregasi
=========================================
Pengelompokan dan agregasi digunakan untuk mengelompokkan data berdasarkan satu atau lebih variabel dan kemudian menghitung agregat seperti jumlah (sum), rata-rata (mean), dan lainnya. Dalam konteks ini, kita menggunakan teknik ini untuk:
- Mengelompokkan data berdasarkan musim (`season`) dan menghitung rata-rata pengguna terdaftar (`registered`).
- Mengelompokkan data berdasarkan jam (`hr`) dan menghitung jumlah total pengguna (`cnt`).

=========================================
3. Visualisasi Data
=========================================
Visualisasi data digunakan untuk menyajikan data dalam bentuk grafik untuk memudahkan pemahaman dan interpretasi. Beberapa visualisasi yang digunakan dalam analisis ini meliputi:
- Diagram Batang : Digunakan untuk menampilkan rata-rata pengguna terdaftar berdasarkan musim. Visualisasi ini membantu dalam memahami bagaimana penggunaan bervariasi sepanjang musim.
- Diagram Garis : Digunakan untuk menampilkan perubahan jumlah pengguna berdasarkan jam dalam satu hari. Ini membantu dalam mengidentifikasi jam-jam puncak penggunaan.

=========================================
4. Teknik Penyaringan Data
=========================================
Teknik penyaringan (filtering) digunakan untuk mengekstrak subset data berdasarkan kondisi tertentu. Misalnya, kami dapat memfilter data untuk hanya menampilkan hari kerja atau akhir pekan, atau hari dengan cuaca tertentu, untuk melihat bagaimana faktor-faktor ini mempengaruhi jumlah pengguna.

=========================================
5. Analisis Korelasi
=========================================
Analisis korelasi membantu dalam mengidentifikasi hubungan antara variabel yang berbeda. Dalam dataset ini, kita dapat melakukan analisis korelasi untuk memahami bagaimana variabel seperti musim (`season`), kelembaban (`hum`), kecepatan angin (`windspeed`), dan cuaca (`weathersit`) mempengaruhi jumlah pengguna.
