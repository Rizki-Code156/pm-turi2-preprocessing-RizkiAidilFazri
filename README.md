# Pertemuan 4

[svg](https://github.com/Rizki-Code156/pm-turi2-preprocessing-RizkiAidilFazri/tree/main#pertemuan-4)

**Mata Kuliah:** Pembelajaran Mesin (INF62325)  
**Nama:** Rizki Aidil Fazri  
**NIM:** 2488010021

## Ringkasan

[svg](https://github.com/Rizki-Code156/pm-turi2-preprocessing-RizkiAidilFazri/tree/main#ringkasan)

Praktikum Pertemuan 4 membahas **Preprocessing & Feature Engineering** sebagai tahap persiapan data sebelum digunakan dalam proses pembelajaran mesin. Praktikum ini mencakup penanganan nilai yang hilang, encoding data kategorikal, pembagian data latih dan data uji, serta scaling pada fitur numerik untuk mencegah terjadinya data leakage.

## Isi Repositori

[svg](https://github.com/Rizki-Code156/pm-turi2-preprocessing-RizkiAidilFazri/tree/main#isi-repositori)

`PM_P4_Rizki Aidil Fazri_2488010021.ipynb` : Notebook praktikum Preprocessing & Feature Engineering menggunakan dataset karyawan buatan.

## Temuan Utama

[svg](https://github.com/Rizki-Code156/pm-turi2-preprocessing-RizkiAidilFazri/tree/main#temuan-utama)

1. Nilai yang hilang pada kolom `usia` dan `pendapatan` berhasil ditangani menggunakan metode imputasi median.

2. Metode imputasi median pada kolom `usia` dibandingkan dengan metode mean untuk melihat perbedaan hasil pengisian nilai yang hilang.

3. Data kategorikal `pendidikan` diubah menggunakan ordinal encoding karena memiliki tingkatan, yaitu `SMA`, `S1`, dan `S2`.

4. Data kategorikal `kota` dan `status` diubah menggunakan one-hot encoding karena kategorinya tidak memiliki tingkatan.

5. Dataset dibagi menjadi data latih dan data uji sebelum proses scaling dilakukan untuk mencegah terjadinya data leakage.

6. `StandardScaler` digunakan untuk melakukan standardisasi pada fitur numerik, sedangkan `MinMaxScaler` digunakan sebagai perbandingan untuk mengubah nilai fitur ke rentang 0 sampai 1.

7. Penggunaan `fit_transform` dilakukan pada data latih, sedangkan pada data uji hanya menggunakan `transform` agar parameter scaling tidak dipelajari dari data uji.

8. Setelah proses preprocessing, data tidak memiliki nilai yang hilang dan seluruh fitur yang digunakan dalam proses pembelajaran mesin telah berada dalam bentuk numerik.

## Kesimpulan

[svg](https://github.com/Rizki-Code156/pm-turi2-preprocessing-RizkiAidilFazri/tree/main#kesimpulan)

Preprocessing merupakan tahap penting dalam mempersiapkan data sebelum digunakan dalam pembelajaran mesin. Pada praktikum ini, data berhasil diproses melalui imputasi nilai yang hilang, encoding data kategorikal, pembagian data, dan scaling. Urutan preprocessing yang tepat diperlukan agar tidak terjadi data leakage dan hasil pengolahan data dapat digunakan dengan baik pada tahap pembelajaran mesin.
