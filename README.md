# Realestica Machine Learning

Repository ini berfokus pada pengembangan model machine learning untuk memprediksi harga rumah di wilayah Jakarta dengan menggunakan fitur properti lengkap, termasuk spesifikasi rumah, fasilitas, dan lingkungan sekitar.

## Tahapan Tahapan Melakukan Cleaning Data
1. Import Library
2. Gathering Data
3. Rename Feature
4. Extract Facilities
5. Extract Specification
6. Clear Monthly Installment Format
7. Extract POI
8. Extract Location
9. Extract Estimated Savings
10. Menyimpan Data yang Sudah di Cleaning
11. Exploratory Data Analysis

## Tahapan Tahapan Membuat Model
1. Import Library
2. Gathering Data yang Sudah di Cleaning
3. Melakukan Encoding
4. Menghapus Kolom yang Tidak Digunakan Untuk Model
5. Menhapus Nilai Null
6. Menetukan variabel dependen dan independen
7. Melakukan Train Test Split Dataset
8. Membuat Model
9. Melakukan Tuning Model
10. Melakukan Feature Selection
11. Evaluasi
12. Menyimpan Model

## Profile Data yang Sudab di Cleaning
Dataset ini terdiri dari 50464 baris dan 57 kolom fitur yang berisi informasi properti, fasilitas, spesifikasi dan lingkungan sekitar di wilayah Jakarta. 

## Dictionary Data yang sudah di cleaning
- `description` : Deskripsi properti dalam bentuk teks, bisa berupa highlight atau ringkasan.
- `facilities` : Fasilitas yang tersedia yang belum di extract/dipisahkan.
- `monthly_installment_info` : Informasi tentang cicilan bulanan (jika ada skema cicilan).
- `location` : Lokasi properti, biasanya berupa string alamat atau nama wilayah.
- `nearby_points_of_interest` : Tempat-tempat penting yang dekat properti, seperti sekolah, pasar, dsb.
- `posted_by` : Identitas atau peran pengiklan (misalnya: agen, developer, individu).
- `price_display` : Harga dalam format teks (bisa mengandung simbol atau satuan).
- `price_numeric` : Harga dalam format numerik (tanpa simbol).
- `property_type` : Jenis properti (contoh: rumah, apartemen, ruko, dll).
- `estimated_savings` : Estimasi penghematan jika membeli properti ini (misalnya diskon).
- `specifications` : Spesifikasi properti, biasanya dalam bentuk ringkasan atau teks gabungan.
- `title` : Judul iklan properti.
- `updatedAt` : Tanggal atau waktu terakhir data diperbarui.
- `source_url` : URL sumber data/iklan properti.
- `error` : Indikator error saat crawling atau memproses data.

- `f_taman` : Taman umum atau hijau di area properti.
- `f_jogging_track` : Jalur jogging atau lari.
- `f_cctv` : Kamera pengawas (CCTV).
- `f_lapangan_voli` : Lapangan untuk bermain voli.
- `f_lapangan_bola` : Lapangan sepak bola.
- `f_lapangan_basket` : Lapangan bola basket.
- `f_lapangan_bulu_tangkis` : Lapangan bulu tangkis.
- `f_tempat_jemuran` : Area untuk menjemur pakaian.
- `f_kulkas` : Tersedia kulkas di properti.
- `f_telepon` : Fasilitas sambungan telepon.
- `f_tempat_cuci` : Area mencuci pakaian (terpisah dari laundry).
- `f_laundry` : Fasilitas laundry (umumnya laundry bersama di apartemen).
- `f_masjid` : Terdapat masjid di sekitar area.
- `f_taman_bermain` : Area bermain anak-anak.
- `f_kolam_renang` : Kolam renang.
- `f_mesin_cuci` : Tersedia mesin cuci.
- `f_kompor` : Kompor disediakan.
- `f_keamanan_24_jam` : Keamanan 24 jam.
- `f_kolam_ikan` : Kolam ikan hias.
- `f_backyard` : Halaman belakang.
- `f_kitchen_set` : Dapur sudah dilengkapi kitchen set.
- `f_teras` : Terdapat teras.
- `f_wastafel` : Wastafel dapur atau kamar mandi.
- `f_akses_parkir` : Akses parkir untuk kendaraan.
- `f_lapangan_tenis` : Lapangan tenis.
- `f_tempat_gym` : Tempat gym/fitness.
- `f_ac` : Pendingin ruangan (AC).
- `f_water_heater` : Pemanas air.
- `f_one_gate_system` : Sistem keamanan satu pintu masuk.

- `s_carport` : Kapasitas atau keberadaan carport (tempat parkir mobil terbuka).
- `s_daya_listrik` : Besaran daya listrik (dalam VA/Watt).
- `s_garasi` : Kapasitas atau keberadaan garasi tertutup.
- `s_jumlah_lantai` : Jumlah lantai bangunan.
- `s_kamar_mandi` : Jumlah kamar mandi.
- `s_kamar_mandi_pembantu` : Jumlah kamar mandi khusus pembantu.
- `s_kamar_tidur` : Jumlah kamar tidur utama/penghuni.
- `s_kamar_tidur_pembantu` : Jumlah kamar tidur untuk pembantu.
- `s_kondisi_properti` : Kondisi properti (baru, second, renovasi, dll).
- `s_luas_bangunan` : Luas bangunan (m²).
- `s_luas_tanah` : Luas tanah (m²).
- `s_sertifikat` : Jenis sertifikat (SHM, HGB, AJB, dll).

- `poi_perbelanjaan` : Titik perbelanjaan terdekat (mall, pasar, supermarket).
- `poi_sekolah` : Sekolah atau institusi pendidikan terdekat.
- `poi_transportasi` : Akses ke transportasi publik (stasiun, halte, bandara, dsb).
- `kabupaten` : Nama kabupaten atau kota administratif properti tersebut.
