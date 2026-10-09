Doorprize PRO — V3 Copyright 2026 noorhasanudin email : noor.hasanudin@gmail.com WA : +6285652070654

# Overview Aplikasi Doorprize PRO — V3
<img width="200" height="200" alt="image" src="https://github.com/user-attachments/assets/41c64bb5-8c3c-4a1f-9c26-9d43d7455721" />

Aplikasi Doorprize PRO — V3 adalah aplikasi untuk undian Doorprize berbasis Web, yang dapat melakukan pengundian hadiah Doorprize secara otomatis dijalankan oleh sistem, yang cepat, dan transparan, tanpa rekayasa, karena sistem akan secara acak memilih pemenang undian dari daftar peserta yang sudah terverifikasi, dan hanya Peserta yang bestatus "HADIR" yang masuk dalam proses Undian Doorprize.

Aplikasi secara otomatis membuat Kartu QR (File PDF) yang dapat digunakan untuk melakukan Konfirmasi Kehadiran Peserta, dan Konfirmasi Kehadiran Peserta menggunakan Scanner QR Peserta (Hanya terdapat Pada Aplikasi Doorprize Pro - V3 Plus). 

 
# Keunggulan Aplikasi Doorprize PRO — V3

- Aplikasi dibuat menggunakan Framework `Flask Python` yang fleksibel, sangat ringan dan cepat.
- Database menggunakan `SQLite3`, tanpa perlu menginstall MySQL
- Cocok digunakan untuk acara besar
- Data Peserta Tidak Terbatas
- Branding acara: Nama acara, subtitle, logo
- Fullscreen / LED mode
- Dashboard statistik
- Manajemen data dan pengaturan dilindungi login admin.
- Import Excel (.xlsx/.xlsm)
- Manajemen hadiah + quantity
- Status Peserta
- Animasi Roda keberuntungan
- Animasi Rolling peserta
- Suara drumroll dan fanfare berbasis Web Audio API
- Peserta pemenang otomatis dikeluarkan dari undian berikutnya
- Riwayat pemenang
- Reset hasil atau reset seluruh data
- Konfirmasi Kehadiran Manual
- Otomatis membuat QR Peserta untuk Konfirmasi Kehadiran** -> Opsional pada Aplikasi Doorprize Versi PRO V3 Plus 
- Download QR Peserta Per Peserta (.pdf) atau Semua Peserta** (.zip) -> Opsional pada Aplikasi Doorprize Versi PRO V3 Plus
- Konfirmasi Kehadiran Otomatis Menggunakan Scanner QR Peserta** -> Opsional pada Aplikasi Doorprize Versi PRO V3 Plus

## Source files
	- /static
	- /static/app.js
	- /static/attendance.png
	- /static/draw.png
	- /static/doorprice_pro.ico
	- /static/doorprice_pro.png	
	- /static/register_and_setting.png
	- /static/state.png
	- /static/register_and_setting.png
	- /static/style.css
	- /templates
	- /templates/admin_login.html
	- /templates/attendance.html
	- /templates/draw.html
	- /templates/index.html
	- /templates/register_and_setting.html
	- /templates/state.html
	- app.py
	- doorprize_pro.db
	- Doorprize_PRO_V3.bat
	- Template_Upload_Hadiah_Doorprize.xlsx
	- Template_Upload_Peserta_Doorprize.xlsx
	- README.md
	- requirements.txt

## Menjalankan Aplikasi
	Klik `Doorprize_PRO_V3.bat` akan otomatis menjalankan `DOS/Windows Powershell` yang terdiri dari:
	- Menginstall tools Library `Python`: `pip install -r requirements.txt`.
	- Menjalankan Aplikasi `Flask Python`: `python app.py`
	- Memjalankan `Chrome` Localhost `http://127.0.0.1:5000/`
	- Menampilkan Dashboard Aplikasi `Doorprize PRO V3`

## Membuat Shortcut Aplikasi + Icon Desktop
	- Klik Kanan pada `Doorprize_PRO_V3.bat` -> Send to `Desktop (Create Shortcut)`
	- Klik Kanan pada Shortcut Desktop `Doorprize__PRO_V3.bat - Shortcut` `Rename` menjadi `Doorprize_PRO_V3`
	- Klik Kanan Pada Shortcut Desktop `Doorprize_PRO_V3` -> `Properties` -> `Change Icon` -> `Browse` Cari file `/static/doorprice_pro.ico` -> `Open`
	
## Dashboard
	Terdapat 5 Menu Utama pada Dashboard Doorprize PRO — V3:
	- `📝 Registrasi & Pengaturan`
	- `📷 Konfirmasi Kehadiran`
	- `📰 Status Peserta`
	- `🎡 Putar Undian`

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/06a0de46-9c8c-49e4-adc9-0e1fec9bdd22" />
Dashboard Doorprize PRO V3


## Menu `📝 Registrasi & Pengaturan`

### Login Admin
	- Login Admin — `📝 Registrasi & Pengaturan`
		Menu `📝 Registrasi & Pengaturan` dilindungi login admin.
		Kredensial awal:
		Username: `admin`
		Password: `admin123`
	- Klik Tombol `🔑 Masuk Sebagai Admin`
	- Password disimpan sebagai hash di SQLite.
	- Endpoint input data, upload Excel, logo, pengaturan, dan hapus semua data juga dilindungi session admin.
	- Setelah masuk, Klik Tombol `🔑 Ubah Password` untuk mengganti password.
	- Password baru minimal 8 karakter dan disimpan sebagai hash di SQLite.
	- Logout: Klik Tombol `🔒 Logout Admin`
	- Klik Tombol `← Kembali ke Dashboard`untuk kembali ke Halaman Dashboard.
<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/e4377ea8-1720-4957-aa07-6a82e41d9480" />
Login Admin

### Pengaturan
	- Klik Tombol `⚙️ Pengaturan`
	- Pada Row Pertama isikan Nama Acara
	  Default : `GRAND DOORPRIZE`
	- Pada row kedua isikan Subtitle.
	  Default : `Annual Gathering & Celebration`
	- Untuk Mengubah Logo Klik `🖼️ Upload Logo` -> Pilih File Gambar (.png/.jpg/.webp) -> `Open`
	- Klik Tombol `Simpan`atau Tombol `Batal` untuk membatalkan perubahan pengaturan.
	- Klik Tombol `⚠️ Hapus Semua Data` untuk menghapus semua database yang tersimpan di SQLite (Data Peserta, Hadiah, Pemenang dan Pengaturan).
	- Klik Tombol `← Dashboard`untuk kembali ke Halaman Dashboard.

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/de930235-c286-4b12-b4ae-2454f7dadf34" />
Pengaturan

### Input Data Peserta
	- Isikan Nomor Tiket pada row input `Tiket` (*Wajib diisi).
	- Isikan Nama peserta pada row input `Nama peserta` (*Opsional).
	- Isikan Departemen / Instansi pada row input `Departemen / Instansi` (*Opsional).
	- Isikan Nomor HP / WA pada row input `Nomor HP / WA` (*Opsional).
	- Klik Tombol `➕ Tambah Peserta`.
	- Urutan Kolom Tabel Excel `Upload Excel Peserta` : |No|Nomor Tiket|Nama Peserta|Departemen|No HP|Status| atau bisa juga menggunakan Template file Excel yang tersedia.
	- Untuk Upload data Peserta menggunakan Template file Excel Klik `📊 Upload Excel Peserta` -> Pilih File Excel Peserta (.xlxs) -> `Open`
	- Untuk menghapus data Peserta satu per satu klik tommbol `❌` pada sisi kanan data Peserta.

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/2001f68f-3a29-41ba-91ed-413d62f483c6" />
Input Data Peserta Manual

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/e7fb95e0-b28d-448e-a651-224c156e0000" />
Template Impor Excel Data Peserta	

### Input Data Hadiah
	- Isikan Nama hadiah pada row input `Nama hadiah` (*Wajib diisi).
	- Isikan Jumlah pada row input `Jumlah` (*Wajib diisi dengan angka minimal `1`).
	- Klik Tombol `➕ Tambah Hadiah`.
	- Urutan Kolom Tabel Excel `Upload Hadiah` : |No|Nama Hadiah|Jumlah|Keterangan| atau bisa juga menggunakan Template file Excel yang tersedia.
	- Untuk Upload data Hadiah menggunakan Template file Excel Klik `📊 Upload Excel Hadiah` -> Pilih File Excel Peserta (.xlxs) -> `Open`
	- Untuk menghapus data Hadiah satu per satu klik tommbol `❌` pada sisi kanan data Hadiah.
	- Klik Tombol `← Dashboard`untuk kembali ke Halaman Dashboard.

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/73362251-0452-4735-a672-a759fcb924df" />
Input Data Hadiah Manual

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/1448c282-8e07-47ad-8821-3868f6da4fe2" />
Template Impor Excel Data Hadiah	

### Reset Riwayat Pemenang
	- Klik Tombol `Reset Hasil` untuk mengembalikan semua data pemenang.

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/e50c69d5-d692-4dfc-87d1-b02dcaab9fa1" />
Reset Riwayat Pemenang

## Menu `📝 Konfirmasi Kehadiran`
### Konfirmasi kehadiran manual
	- Isikan `Nomor Tiket` pada row input `Nomor Tiket` sebagai alternatif jika scanner tidak tersedia
	- Klik Tombol `✓ Konfirmasi Hadir` sampai tampil pesan `Kehadiran berhasil dikonfirmasi`, dan pada Status Kehadiran  yang sebelumnya `⏳Belum Hadir` menjadi `Hadir`.
	- Klik Tombol `← Dashboard` untuk kembali ke Halaman Dashboard.

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/5ac7474a-b154-492c-abb0-e6090da8464a" />
Konfirmasi kehadiran manual	
	
## Menu `📰 Status Peserta`
	- Pada menu Status Peserta digunakan untuk menampilkan status kehadiran peserta `⏳Belum Hadir` / `Hadir`/ `Hadir` `🏆 Sudah Menang`

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/a3496f43-6787-4e08-8c83-168a79899899" />
Status Peserta

## Menu `🎡 Putar Undian`

### Pengaturan Tampilan Undian
	- Klik Tombol `▣ LED / Fullscreen` untuk mengubah ke mode Fullscreen
	- tekan `ESC` untuk keluar dari mode Fullscreen

### Memulai undian
	- Pilih Hadiah salah satu jenis hadiah yang terdapat pada row Pilihan hadiah.
	- Klik Tombol `🔊 Suara ON` untuk mode suara aktif, atau `🔇 Suara OFF` untuk mode suara senyap.
	- Pastikan terdapat status `SIAP`
	- Klik Tombol `🎡 Putar Undian` untuk menentukan Pemenang Undian, tunggu sampai putaran undian berhenti dan pemenang tampil pada layar.
	- Seluruh Pemenang akan tampil pada bagian sisi bawah.
	- Klik Tombol `← Dashboard` untuk kembali ke Halaman Dashboard.	

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/13b038eb-889d-4bb3-8ad6-4e35eb460355" />
Melakukan Pengundian Doorprize

<img width="100%" height="Auto" alt="image" src="https://github.com/user-attachments/assets/aee70bf3-c061-4956-9a86-9b4dd2dd116a" />
Hasil Pemenang Undian Doorprize




	
