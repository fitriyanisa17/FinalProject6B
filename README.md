# FinalProject6B
Final Project Rakamin Data Science Batch 05 kelompok 6b

# Summary & Insight EDA
1. Terdapat kolom dengan tipe data kurang sesuai sehingga dilakukan perubahan
2. Terdapat 7 kolom yang memiliki nilai kosong
3. Terdapat variabel dengan value yang ambigu seperti Mobile Phone dengan Phone, CC dan Credit Card, COD dan Cash on Delivery. Perlu dilakukan preprocessing lebih lanjut.
4. Variabel Tenure menjadi perhatian karena banyaknya pelanggan churn pada tenure < 3 bulan.
5. Rata-rata pelanggan menghabiskan waktu selama 3 jam dalam menggunakan aplikasi.
6. Banyak pelanggan yang tidak menggunakan kupon saat belanja.
7. Rata-rata pembelian dari pelanggan dengan jarak <15 km dari ware house (gudang)
8. Jumlah pelanggan yang melakukan komplain dan churn terbilang cukup tinggi,mengindikasikan bahwa keluhan yang tidak teratasi dengan baik dapat memengaruhi keputusan pelanggan untuk melakukan churn.
9. Pelanggan yang menggunakan kupon < 3 cenderung akan churn
10. Satisfaction Scere yang baik belum tentu tidak melakukan churn
11. Pelanggan yang mengalami peningkatan signifikan dalam order amount mungkin lebih cenderung tetap setia, sedangkan pelanggan yang mengalami sedikit atau tidak ada peningkatan mungkin lebih cenderung melakukan churn.
12. Pelanggan yang aktif melakukan lebih banyak pesanan cenderung lebih setia, sedangkan pelanggan yang jarang melakukan pesanan mungkin lebih cenderung melakukan churn.
13. Pelanggan yang menerima tingkat cashback yang tinggi cenderung lebih setia, sedangkan pelanggan dengan tingkat cashback yang rendah atau sedang mungkin lebih cenderung melakukan churn.

Tindak Lanjut : Untuk mendapatkan perhitungan yang sesuai diperlukan data preprocessing dengan menghilangkan outlier, menentukan fitur yang sesuai dan metode correlation yang sesuai, menormalisasi fitur yang memiliki skew


# Summary dan insight Data Pre-prosesing
1. Pada handling data missing values kita menggunakan dropna karena dataset yang ada memiliki banyak data.
2. Pada saat mengecek duplikat data hasilnya adalah 0
3. Pada Feature Encoding kita menggunakan onehost, karena menghindari bias pada data.
4. Outlier yang kita hapus dari jumlah data yang ada sekitar 4.21 %. Alasan kita mengharapkan outlier yang ada karena outlier mempengaruhi proses untuk proses pemodelan.
5. Untuk feature transformation yang kita lakukan adalah mengecek distribusi setiap data.
6. Pada class imbalance kita melakukan klasifikasi pada pemodelan yang dilakukan dengan menggunakan kolom churn.
7. Pada feature selection kita menggunakan Selectkbest untuk melihat 6 feature terbaiknya
8. Pada feature extraction kita menambahkan kolom TotalSpanding, CustomerCatagory, MeanOrderAmountHikeFromlastYear, dan juga OrderAmountHike_Coupon_Interact.

Tindak Lanjut : Untuk Melakukan eksperimen feature yang nantinya akan dihapus atau tidak, mencari penyebab churn selain yang sudah didapatkan, mempertimbangkan feature lainnya, seperti daysincelastorder dan CashbackAmount, melakukan EDA dan membuat pre prosesing untuk feature yang baru ditambahkan. 

Hal-hal tersebut akan dilakukan untuk menunjang proses pada stage selanjutnya yaitu pemodelan.
