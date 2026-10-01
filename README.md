# Cek Kesehatan Awal KAI

Halaman statis satu file untuk calon pelamar rekrutmen KAI Group 2026:

- **Kalkulator BMI/IMT** dengan tiga ambang: WHO dewasa, Kemenkes Asia-Pasifik, dan IMT/U (WHO 2007, usia 15–18 tahun).
- **Cek tinggi badan** terhadap syarat minimal per formasi KAI, plus pembanding Polri/TNI/sekolah kedinasan.
- **Rencana sampai hari tes** — berat sasaran, waktu tersisa, laju yang dibutuhkan, dengan peringatan terhadap jalan pintas sebelum rikkes.
- **Checklist 10 komponen kesehatan awal** beserta persiapannya, tersimpan di `localStorage`.
- **Timeline tahapan rekrutmen 2026** (tanggal registrasi & apply resmi; tahap setelahnya estimasi).

Catatan penting yang juga tertulis di halaman: rentang BMI 18,5–24,9 adalah klasifikasi WHO, **bukan** ambang kelulusan yang diterbitkan KAI. Pengumuman KAI hanya menyebut "berat badan ideal sesuai formasi" tanpa angka.

## Menjalankan

Tidak ada build step dan tidak ada dependency. Buka `index.html` langsung di browser, atau serve folder ini sebagai situs statis:

```sh
python3 -m http.server 8000
```

## Deploy

Repo ini punya workflow GitHub Pages di `.github/workflows/pages.yml`.

Sekali saja, aktifkan dulu Pages-nya: **Settings → Pages → Build and deployment → Source: GitHub Actions**. `GITHUB_TOKEN` tidak punya izin membuat Pages site sendiri, jadi langkah ini tidak bisa diotomatiskan dari workflow.

Setelah itu setiap push ke branch ini akan men-deploy ulang ke:

<https://marselcerebrum-jpg.github.io/BMI-TES-KESEHATAN-KAI/>
