# VO-Otomatis — AUDIT V14

Otomatisasi pengisian narasi VO1–VO30 melalui 5 batch menggunakan Windows PowerShell dan Google AI Studio (text-to-speech).

## Cara memakai
1. Simpan berkas Part berformat `.txt`, `.md`, atau `.docx` ke folder `INPUT PART`, dengan nama mengandung **Part** diikuti nomor (misalnya `Part1.txt`).
2. Jalankan salah satu dari lima berkas `.bat` di folder utama sesuai kelompok VO.
3. Skrip membaca nomor Part yang tersedia secara berurutan, menutup jendela batch sebelumnya, membuka hingga 6 jendela VO, lalu memasukkan narasi.
4. Skrip berhenti setelah narasi terisi; **tidak** memilih suara, menekan tombol Generate, memeriksa kualitas/durasi, atau mengunduh audio.

Lihat [PETUNJUK V14.txt](PETUNJUK%20V14.txt) untuk pemetaan VO dan contoh.

## Isi
- `AutoPartKeVO_IsiNarasi_V14.ps1`, `ChromeVO_AIStudio_Zoom67_V14.ps1`, `TutupSemuaVOBatch_V14.ps1`: skrip utama.
- `1 - ... .bat` sampai `5 - ... .bat`: tombol batch VO1–VO30.
- `AUDIT V14.json`: parameter proyek.
- `INPUT PART/`: tiga contoh narasi. Di repository ini contoh dari dokumen `.docx` pada ZIP diubah menjadi `.txt` dengan teks narasi tetap sama, sehingga tetap dapat dibaca skrip dan mudah ditinjau di GitHub.
- `LOG/`: log uji dari arsip yang diberikan.

**Catatan:** Repo publik. Jangan menyimpan token akun, sandi, atau data narasi rahasia di sini.

Sumber: unggahan pengguna `AUDIT V14 5 BATCH VO1-30 - PART BERURUTAN OTOMATIS(1).zip`.
