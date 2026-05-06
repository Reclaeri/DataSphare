Nama Anggota Kelompok :
# Revan Oknanda
# Syahrul Haqqin Nazil
# Bilqis Rifat Safaa

# ⚙️ Database Trigger Documentation

Dokumentasi ini berisi trigger utama yang digunakan dalam sistem **Sistem Informasi Ekstrakurikuler** untuk menjaga konsistensi data.

---

## 🔒 1. Cegah Duplikasi Peserta

**Event:** `BEFORE INSERT ON peserta`

**Tujuan:**
Mencegah satu siswa terdaftar lebih dari satu kali pada ekskul yang sama.

**Logika:**

* Cek kombinasi `id_siswa` dan `id_ekskul`
* Jika sudah ada → batalkan insert

---



## 📅 2. Validasi Absensi

**Event:** `BEFORE INSERT ON absensi`

**Tujuan:**
Memastikan data absensi valid dan tidak kosong.

**Logika:**

* Cek apakah `id_peserta` valid
* Jika `status` kosong → set default `"Hadir"`

---

# ⚙️ Database Trigger Documentation

Dokumentasi ini berisi trigger utama yang digunakan dalam sistem **Sistem Informasi Ekstrakurikuler** untuk menjaga konsistensi data.

---

## 🔒 1. Cegah Duplikasi Peserta

**Event:** `BEFORE INSERT ON peserta`

**Tujuan:**
Mencegah satu siswa terdaftar lebih dari satu kali pada ekskul yang sama.

**Logika:**

* Cek kombinasi `id_siswa` dan `id_ekskul`
* Jika sudah ada → batalkan insert

---



## 📅 2. Validasi Absensi

**Event:** `BEFORE INSERT ON absensi`

**Tujuan:**
Memastikan data absensi valid dan tidak kosong.

**Logika:**

* Cek apakah `id_peserta` valid
* Jika `status` kosong → set default `"Hadir"`

---


<img width="1512" height="636" alt="erd pbo drawio" src="https://github.com/user-attachments/assets/1674966f-2656-4c26-9575-86a721f7844e" />
