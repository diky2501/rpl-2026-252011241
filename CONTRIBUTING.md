# Panduan Kontribusi Repository

Dokumen ini dibuat sebagai acuan kerja agar setiap perubahan file dan penambahan tugas di repositori ini teratur, rapi, dan mudah ditelusuri riwayat perubahannya oleh dosen maupun anggota tim.

### 1. Ketentuan Kontribusi
Seluruh perubahan yang dimasukkan ke dalam repositori ini harus berkaitan dengan tugas dan dokumentasi mata kuliah Rekayasa Perangkat Lunak. Sebelum melakukan commit atau penggabungan kode, pastikan berkas sudah diperiksa secara mandiri agar tidak ada eror, penulisan yang salah, atau informasi pribadi/sensitif yang belum disamarkan.

### 2. Alur Penggunaan Branch
Untuk menjaga agar cabang utama (`main`) selalu stabil dan bersih, hindari mengedit file secara langsung di cabang `main`. Buatlah *branch* baru sesuai dengan jenis pekerjaan yang sedang dilakukan:

| Nama Branch | Kegunaan / Perubahan |
| :--- | :--- |
| `main` | Cabang utama yang berisi dokumen/tugas versi stabil |
| `feature/nama-fitur` | Untuk menambahkan tugas, laporan PDF, atau materi baru |
| `docs/nama-dokumen` | Untuk memperbarui atau merapikan file dokumentasi (`.md`) |
| `fix/nama-perbaikan` | Untuk membenahi kesalahan ketik, format, atau eror |

Contoh perintah Git untuk membuat branch baru:

git checkout main
git pull origin main
git checkout -b feature/tugas-01-laporan

### 3. Standar Pesan Commit
Setiap perubahan wajib dicatat menggunakan pesan commit yang singkat, jelas, dan menggambarkan perbaikan yang dilakukan. Gunakan awalan (prefix) standar berikut:

feat: penambahan berkas, laporan, atau fitur baru
Contoh: feat: tambah pdf laporan tugas 01

docs: pembaruan isi file dokumentasi Markdown
Contoh: docs: perbarui profil dan decision log di readme

fix: perbaikan kesalahan penulisan, format, atau eror
Contoh: fix: perbaiki format tabel di ai policy

refactor: penataan ulang struktur atau posisi file/folder tanpa mengubah isi utama
Contoh: refactor: rapikan struktur folder tugas-01

Contoh perintah menyimpan perubahan:
git add .
git commit -m "docs: tambah panduan kontribusi"

### 4. Alur Pull Request & Review
Jika pengerjaan di branch sudah selesai, ikuti alur penggabungan berikut:

* Unggah branch kamu ke GitHub: 
* git push -u origin feature/tugas-01-laporan
* Buka halaman repositori di GitHub, lalu klik Compare & pull request.
* Tuliskan deskripsi singkat mengenai apa saja yang diubah atau ditambahkan pada Pull Request (PR) tersebut.
* Lakukan peninjauan mandiri (self-review) untuk memastikan tidak ada berkas yang salah atau informasi rahasia yang terunggah.
* Jika semua kriteria sudah sesuai, lakukan Merge pull request ke cabang main.

5. Hal yang Wajib Diperiksa Sebelum Merge
Sebelum menggabungkan PR ke main, pastikan poin-poin berikut sudah terpenuhi:
[ ] File yang diubah sudah sesuai dengan instruksi tugas.
[ ] Data pribadi atau informasi sensitif pada bukti screenshot sudah disamarkan.
[ ] Pesan commit ditulis secara jelas dan menggunakan awalan yang tepat.
[ ] Tampilan format Markdown (.md) rapi dan dapat terbaca dengan baik di GitHub.


Apabila ditemukan masalah, lakukan perbaikan terlebih dahulu sebelum perubahan digabungkan.

6. Etika Kontribusi
Setiap kontributor diharapkan untuk tetap menjaga integritas akademik, menghargai hasil karya orang lain, serta menyampaikan masukan secara sopan. 
Seluruh referensi dari luar wajib dicantumkan sumbernya, dan penggunaan AI harus tetap mematuhi aturan yang tertera pada file AI_POLICY.md.
