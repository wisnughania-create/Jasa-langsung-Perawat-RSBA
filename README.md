# Jasa Langsung Perawat — online lewat GitHub Pages

## 1. Siapkan database (Supabase, gratis)
1. Daftar di supabase.com, buat project baru.
2. Buka **SQL Editor**, tempel isi `setup.sql`, klik **Run**.
3. Buka **Project Settings > API**, salin **Project URL** dan kunci **anon public**.
4. Tempel keduanya ke `config.js`.

## 2. Unggah ke GitHub
1. Buat repositori baru di github.com.
2. Unggah `index.html`, `config.js`, dan `README.md` (tombol **Add file > Upload files**).
3. **Settings > Pages**: Source = *Deploy from a branch*, branch `main`, folder `/ (root)`, Save.
4. Tunggu 1–2 menit. Alamatnya: `https://NAMAANDA.github.io/NAMA-REPO/`

## 3. Pertama kali dipakai
Buka alamatnya, masuk sebagai **admin** (password awal sama seperti di aplikasi), lalu di tab **Akun** klik **Buat akun kepala ruangan & perawat**. Segera ganti password admin.

## Keamanan (penting)
Kunci anon ada di file publik, dan aturan di `setup.sql` mengizinkan siapa pun yang tahu alamat + kunci membaca/menulis data, termasuk penghasilan tetap dan hash password. Login di aplikasi hanya membatasi tampilan, bukan akses ke database. Untuk data gaji yang sensitif, minta pengembang memasang Supabase Auth dan aturan akses per peran sebelum dipakai luas.
