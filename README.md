# Dummy Kalkulator PNBP - Izin Penerapan CPPOB

Prototipe/wireframe interaktif untuk kalkulator estimasi PNBP Izin Penerapan Cara Produksi Pangan Olahan yang Baik (CPPOB), mengacu pada PP 15/2026.

**Status: dummy / data uji coba** - bukan halaman resmi, belum terhubung ke data atau API produksi.

## Isi halaman

- Data izin: tipe permohonan, skala usaha, jenis permohonan
- Baris lokasi + proses produksi (bisa ditambah lebih dari satu, kombinasi unik lokasi + proses dihitung sebagai unit biaya terpisah)
- Pencarian kategori pangan per lokasi (multi, dengan catatan bebas)
- Estimasi PNBP otomatis berdasarkan kombinasi skala usaha x jenis permohonan
- Panel UPT/unit pemeriksa (khusus tipe pendaftaran mengikuti lokasi pabrik, tipe ekspor tetap ke Direktorat Pengawasan Produksi Pangan Olahan)
- Panel informasi (komponen biaya, variabel yang memengaruhi, acuan regulasi) - saat ini masih lorem ipsum

## Data dummy yang dipakai

| Item | Nilai contoh |
|---|---|
| Lokasi | Bandung, Surabaya, Jakarta, Bekasi |
| UPT | BBPOM di Bandung, BBPOM di Surabaya, BBPOM di Jakarta (Bekasi ikut BBPOM di Bandung) |
| Proses produksi | Sterilisasi, Pasteurisasi, Pemanggangan, Mixing |
| Kategori pangan | Susu, Daging Olahan, Biskuit |

## Tabel tarif (dummy, skala x jenis permohonan)

| Skala usaha | Baru | Perpanjangan | Perubahan teknis | Perubahan administrasi |
|---|---|---|---|---|
| Besar | Rp 3.000.000 | Rp 2.000.000 | Rp 1.000.000 | Rp 0 |
| Menengah | Rp 1.000.000 | Rp 750.000 | Rp 500.000 | Rp 0 |
| Kecil | Rp 0 | Rp 0 | Rp 0 | Rp 0 |
| Mikro | Rp 0 | Rp 0 | Rp 0 | Rp 0 |

## Cara akses

Halaman ini di-hosting via GitHub Pages: `https://<username>.github.io/<nama-repo>/`

## Catatan

Seluruh data pada halaman ini (lokasi, UPT, proses produksi, kategori pangan, tarif, dan teks panel informasi) adalah data sementara untuk keperluan uji coba alur dan tampilan, bukan data final.
