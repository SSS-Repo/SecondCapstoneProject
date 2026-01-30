# SecondCapstoneProject

Link Tableau Dashboard: https://public.tableau.com/app/profile/sultan.sulaiman.said/viz/AirbnbListingsBangkok_17697909269710/Dashboard1?publish=yes

## Latar Belakang

Dalam project ini, data booking Airbnb, yaitu aplikasi yang digunakan untuk melakukan booking akomodasi sementara, akan di analisa. Dataset yang digunakan adalah data listing Airbnb di kota Bangkok. Dokumen analisa ini ditulis dalam Bahasa Inggris.

## Studi Kasus

Analisa ini diperuntukkan utamanya untuk seseorang yang ingin memulai usaha listing akomodasi dengan menggunakan AirBNB. Dengan analisa ini,pengguna akan mencari strategi harga dan kebijakan lainnya terbaik untuk memaksimalkan keuntungan yang diperoleh. Sebagai acuan, pertanyaan berikut akan dijawab dalam analisa ini: 

- Bagaimana perbandingan harga listing di berbagai lingkungan (neighborhood) dan tipe kamar dibandingkan dengan kompetitor?
- Apakah terdapat pola harga musiman atau terkait acara tertentu yang dapat dimanfaatkan untuk meningkatkan pendapatan?
- Apakah persyaratan minimum malam menginap dapat disesuaikan secara dinamis untuk memaksimalkan tingkat hunian tanpa mengorbankan pendapatan?
- Apakah ada fitur tertentu yang bersedia dibayar lebih mahal oleh tamu?

## Data Understanding, cleaning dan EDA

Berikut adalah variabel yang di analisa di dalam dokumen ini. 

- **name**: Nama listing sebagaimana terdaftar di dalam database Airbnb.
- **host_name**: Nama pemilik properti (host) yang sesuai dengan `host_id`.
- **neighborhood**: Lokasi lingkungan atau kawasan tempat listing berada.
- **latitude/longitude**: Koordinat lokasi akomodasi yang dapat ditampilkan pada peta.
- **room_type**: Jenis akomodasi yang ditawarkan.
- **price**: Harga sewa harian dari akomodasi yang terdaftar.
- **minimum_nights**: Durasi minimum penyewaan dalam satuan malam.
- **number_of_reviews**: Jumlah total ulasan yang diterima oleh listing.
- **last_review**: Tanggal terakhir listing menerima ulasan.
- **reviews_per_month**: Rata-rata jumlah ulasan yang diterima per bulan.
- **calculated_host_listings_count**: Jumlah total properti yang dimiliki dan didaftarkan oleh satu host di kota tersebut.
- **availability_365**: Jumlah hari dalam satu tahun di mana akomodasi tersedia untuk dipesan.
- **number_of_reviews_ltm**: Jumlah total ulasan yang diterima oleh suatu listing dalam satu tahun terakhir.

Sebelum analisa, data yang diatas melewati proses cleaning untuk mengubah semua nilai yang hilang. 

Setelah melakukan analisa persebaran dan uji normalitas, telah ditemukan kalau variabel2 yang diatas tidak ada yang mengikuti distribusi normal. Oleh karena itu, *Median* akan dipakai sebagai parameter dalam analisa. 

## Data Analysis

### Metode yang tertera dibawah ini digunakan sebagai bagian dari proses analisa. 

- Analisa persebaran geospatial dengan menggunakan Folium.
- Pemetaan harga median, jumlah listing, rata-rata durasi minimum dengan daerah tempat sewa
- Trend bulanan dan tahunan harga sewa akomodasi
- Plot antara durasi booking minimum dengan harga, ketersediaan dan jumlah review median

## Kesimpulan

Berdasarkan hasil analisis data listing Airbnb di Bangkok, dapat disimpulkan bahwa harga, tipe kamar, dan lokasi merupakan faktor utama yang mempengaruhi performa suatu listing. Listing yang berada di lokasi strategis dan menawarkan tipe kamar tertentu cenderung memiliki tingkat popularitas dan harga sewa yang lebih tinggi. Selain itu, variabel seperti ketersediaan tahunan dan jumlah ulasan juga memberikan gambaran penting mengenai tingkat permintaan dan daya tarik suatu properti.

Analisis ini menunjukkan bahwa strategi penetapan harga dan pengelolaan listing perlu disesuaikan dengan karakteristik pasar, perilaku tamu, serta kondisi persaingan di setiap wilayah.

## Rekomendasi

Berdasarkan kesimpulan yang diperoleh, berikut beberapa rekomendasi yang dapat dipertimbangkan:

1. Pemilik properti disarankan untuk menyesuaikan harga berdasarkan lokasi dan tipe kamar agar tetap kompetitif di pasar.
2. Strategi harga musiman dapat diterapkan dengan memanfaatkan periode permintaan tinggi untuk meningkatkan pendapatan.
3. Fitur dan fasilitas yang memiliki nilai tambah bagi tamu sebaiknya ditonjolkan karena berpotensi meningkatkan kesediaan tamu untuk membayar harga yang lebih tinggi.
4. Penyesuaian kebijakan minimum malam menginap dapat dilakukan secara fleksibel untuk meningkatkan tingkat hunian tanpa mengurangi pendapatan secara signifikan.
5. Host dengan banyak listing disarankan untuk memantau performa masing-masing properti secara berkala guna memastikan strategi pengelolaan yang optimal.
