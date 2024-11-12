## **Dataset: Public Transportation Transaction Transjakarta** ##

## **Business Understanding** ##
Dataset yang disediakan berisi catatan transaksi dari sistem transportasi Transjakarta. Dataset terdiri dari variabel-variabel berikut:
1. Transaction ID (transID), Fare Collection ID (payCardID), Corridor ID (corridorID), and Payment Amount (payAmount).
2. Demografi Pengguna/Penumpang, seperti payee's bank, name, sex, dan birth date.
3. Rincian Perjalanan Penumpang, seperti corridor name, direction, tap-in and tap-out stops, and times.
Tujuan dari analisis ini adalah untuk mengetahui pendapatan Transjakarta dengan menganalisis transaksi dari berbagai koridor. Berikut hal-hal yang akan dianalisis:
1. Apa saja yang termasuk dalam top 10 koridor berdasarkan total pendapatan tertinggi?
2. Bagaimana distribusi dari jumlah pembayaran yang ada?
3. Bagaimana jumlah transaksi berdasarkan koridor untuk top 10 koridor berdasarkan total pendapatan tertinggi?

## **Data Understanding** ##
Dataset terkait terdiri dari 37.900 baris dan 22 kolom. Berikut adalah beberapa poin penting yang didapatkan dari overview data di atas:
### Key columns:
1. transID: ID transaksi unik.
2. payCardID, payCardBank, payCardName: Rincian kartu pembayaran.
3. tapInStops, tapInStopsName, tapOutStops, tapOutStopsName: ID dan nama pemberhentian untuk naik dan turun bus.
4. tapInTime, tapOutTime: Waktu untuk naik dan turun bus.
5. payAmount: Jumlah yang dibayar untuk perjalanan.
### Issue:
1. Terdapat missing values pada beberapa kolom seperti corridorName, corridorID,dan payAmount.

## **Conclusion** ##
Dari analisis, terdapat beberapa poin yang dapat disimpulkan dan menjawab rumusan masalah di awal:
### 1. High-Revenue Corridors 
Koridor dengan total pendapatan tertinggi menunjukkan banyak peminat/banyak digunakan penumpang dan dapat menjadi penyumbang utama pendapatan untuk sistem transportasi. Top 10 koridor dengan pendapatan tertinggi adalah               
1) Cibubur - Balai Kota               (7820000.0)    
2) Bekasi Barat - Kuningan            (4380000.0)    
3) Palem Semi - Bundaran Senayan      (3520000.0)  
4) Cinere - Bundaran Senayan          (3520000.0)       
5) Cibubur Junction - Blok M          (3120000.0)   
6) Bintaro - Fatmawati                (2920000.0)  
7) Bekasi Barat - Blok M              (2480000.0)   
8) BSD Serpong - Fatmawati            (1860000.0)  
9) Cibubur - Kuningan                 (1820000.0)      
10) Cinere - Kuningan                 (1680000.0)

### 2. Distribution of Payment Amounts
Dengan melihat payAmount, kita dapat mengetahui tarif yang dibayar di setiap koridor. Apabila tarif konsisten, berarti harganya standar. Apabila tarif berbeda-beda, kemungkinan karena jarak tempuh, jenis bus/armada, atau jenis tarif yang dipilih juga berbeda. Berdasarkan hasil yang disajikan, tarif cenderung berbeda-beda, namun perbedaan tidak terlalu banyak karena hanya tersedia 2 jenis tarif.

### 3. Total Transaction of High-Revenue Corridors
Koridor dengan jumlah transaksi tinggi menunjukkan rute yang sering dipakai. Biasanya, ini rute utama yang banyak dilalui penumpang atau area yang ramai. Berikut adalah jumlah transaksi dari top 10 koridor yang telah disebutkan:
1) Cibubur - Balai Kota                         (391)  
2) Bekasi Barat - Kuningan                      (219)  
3) Palem Semi - Bundaran Senayan                (176)  
4) Cinere - Bundaran Senayan                    (176)  
5) Cibubur Junction - Blok M                    (156)  
6) Bintaro - Fatmawati                          (146)  
7) Bekasi Barat - Blok M                        (124)  
8) BSD Serpong - Fatmawati                       (93)  
9) Cibubur - Kuningan                            (91)  
10) Cinere - Kuningan                            (84)

## **Recommendation** ##
### 1. Resource Allocation
Koridor dengan pendapatan tinggi dan volume tinggi harus diprioritaskan untuk alokasi sumber daya. Menambahkan lebih banyak bus/armada atau meningkatkan frekuensi layanan pada rute-rute ini dapat meningkatkan kepuasan penumpang dan mengurangi kepadatan.

### 2. Targeted Marketing and Promotions
Perlu dipertimbangkan strategi promosi untuk koridor dengan jumlah transaksi atau pendapatan rata-rata yang lebih rendah. Tarif yang lebih rendah selama jam-jam sepi dapat meningkatkan jumlah penumpang pada rute yang jarang digunakan.

### 3. Collaboration with External Parties
Meningkatkan kolaborasi dengan pihak eksternal (misal: sponsor) untuk koridor-koridor dengan volume tinggi, sehingga dapat menghasilkan pendapatan lain yang bisa digunakan untuk pembangunan koridor serta bus/armada transportasi itu sendiri.
