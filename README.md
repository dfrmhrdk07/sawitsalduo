# SAWIT — SAL Web-based Integrated Tracking
### Versi SATU BERKAS (paling aman untuk Vercel)

Dashboard operasional PKS **PT Sari Aditya Loka 2**.

Seluruh CSS, JavaScript, dan logo sudah **tertanam di dalam `index.html`**.
Tidak ada folder `js/`, `css/`, atau `assets/` yang bisa tertinggal saat upload —
inilah penyebab layar putih pada versi terpisah.

## Cara Deploy

1. **GitHub** → buat repository baru (disarankan Private) →
   **Add file** → **Upload files** → seret **3 berkas** ini:
   `index.html`, `vercel.json`, `robots.txt` → **Commit changes**.

   ⚠️ `index.html` harus berada di **akar repository**, bukan di dalam folder.
   Setelah upload, halaman depan repo harus langsung memperlihatkan `index.html`.

2. **Vercel** → **Add New… → Project** → Import repository →
   Framework Preset **Other**, semua kolom Build/Output/Install **dikosongkan** → **Deploy**.

3. **Disarankan:** Project Settings → **Deployment Protection** →
   aktifkan **Password Protection** agar dashboard tidak terbuka untuk umum.

## Akun Demo

| Peran | Username | Password |
|---|---|---|
| Administrator | `krani.admin` | `krani2026` |
| Staff | `asisten.proses` | `proses2026` |
| Management | `mill.manager` | `manager2026` |

Ubah pada konstanta `USERS` di dalam `index.html`.

## Peringatan

- Autentikasi diperiksa di browser — **bukan keamanan**. Jangan pakai password asli karyawan.
- Data tersimpan di `localStorage`, **per-perangkat**. Data di komputer Krani tidak terlihat di HP Manajer.
- Hapus data contoh 5 tahun lewat **Settings → Data & Sistem → Reset** sebelum pemakaian nyata.
- Total Losses menampilkan "belum dikonfigurasi" sampai faktor konversi ke %TBS diisi
  pada **Settings → Faktor Losses**.
