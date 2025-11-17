# Repository Latihan dan Tugas Praktikum Python

Repository ini berisi kode dan dokumentasi untuk latihan dasar manipulasi list Python serta implementasi program input nilai mahasiswa sebagai tugas praktikum.

---

## 📝 Latihan Dasar List Python

Bagian ini mencakup latihan dasar untuk memahami dan memanipulasi struktur data `list` di Python.

### Tujuan Latihan

* Membuat dan menginisialisasi list.
* Mengakses elemen list menggunakan indeks tunggal dan slicing.
* Mengubah (update) elemen list.
* Menambahkan elemen ke dalam list.
* Menggabungkan beberapa list.

### Implementasi Latihan

Berikut adalah contoh operasi list yang dilakukan:

1.  **Membuat List:**
    ```python
    A = [10, "Apel", 3.14, True, 25]
    ```

2.  **Mengakses List:**
    * Elemen ke-3: `A[2]`
    * Elemen ke-2 sampai ke-4: `A[1:4]`
    * Elemen terakhir: `A[-1]`

3.  **Mengubah Elemen List:**
    * Ubah elemen ke-4: `A[3] = "Jeruk"`
    * Ubah elemen ke-4 sampai terakhir: `A[3:] = [False, 50]`

4.  **Menambah Elemen List:**
    * Membuat list baru `B` dari bagian `A`: `B = A[:2]`
    * Menambah string ke `B`: `B.append("Mangga")`
    * Menambah 3 nilai ke `B`: `B.extend([100, 200, 300])`
    * Menggabungkan `B` dengan `A`: `C = B + A`

---

## 💻 Tugas Praktikum: Program Input Nilai Mahasiswa

Bagian ini adalah implementasi program sederhana untuk mengelola data nilai mahasiswa dengan fitur input berulang dan perhitungan Nilai Akhir.

### 📌 Fitur Program

* **Input Data Berulang:** Program meminta pengguna untuk memasukkan data mahasiswa (Nama, NIM, Nilai Tugas, UTS, UAS) secara berulang.
* **Konfirmasi Penambahan Data:** Pengguna dapat memilih untuk menambah data lagi (`y`) atau mengakhiri input (`t`).
* **Perhitungan Nilai Akhir:** Setelah semua data dimasukkan, program secara otomatis menghitung Nilai Akhir (NA) untuk setiap mahasiswa.
* **Tampilan Data Tabel:** Semua data mahasiswa beserta Nilai Akhir ditampilkan dalam format tabel yang rapi.

### 📐 Ketentuan Perhitungan Nilai Akhir

Nilai Akhir dihitung dari 3 komponen nilai dengan bobot sebagai berikut:

* **Nilai Tugas:** 30% (0.30)
* **Nilai UTS:** 35% (0.35)
* **Nilai UAS:** 35% (0.35)

Rumus yang digunakan adalah:
$$ \text{NA} = (\text{Nilai Tugas} \times 0.30) + (\text{Nilai UTS} \times 0.35) + (\text{Nilai UAS} \times 0.35) $$

### ⚙️ Alur Program

Berikut adalah alur kerja program input nilai mahasiswa:

1.  **Inisialisasi:** Program membuat list kosong `daftar_nilai` untuk menyimpan data dan menetapkan bobot persentase untuk Tugas, UTS, dan UAS.
2.  **Input Berulang:** Program masuk ke mode perulangan.
    * Pengguna diminta memasukkan Nama, NIM, Nilai Tugas, Nilai UTS, dan Nilai UAS.
    * Validasi input angka sederhana dilakukan dengan blok `try-except`.
3.  **Perhitungan & Penyimpanan:** Setelah input valid, Nilai Akhir dihitung. Data mahasiswa (termasuk NA) disimpan sebagai sebuah *dictionary* dan ditambahkan ke dalam `daftar_nilai`.
4.  **Konfirmasi:** Program menanyakan **"Tambah data(y/t)?"**.
    * Jika pengguna menjawab `y` (ya), perulangan berlanjut untuk input data berikutnya.
    * Jika pengguna menjawab `t` (tidak), perulangan berhenti.
5.  **Tampilan Output:** Setelah perulangan berakhir, program menampilkan seluruh data mahasiswa yang telah tersimpan dalam `daftar_nilai` dalam format tabel yang terstruktur.

### 📊 Flowchart Program

Berikut adalah representasi visual alur program dalam bentuk flowchart:

![WhatsApp Image 2025-11-17 at 7 00 12 AM](https://github.com/user-attachments/assets/62a863fc-906f-4265-bf31-93e5172f6361)
