# Modul: AI Code Humanizer (ai-code-tells)

Gunakan panduan ini saat menulis atau merapikan kode agar terlihat seperti ditulis oleh developer manusia yang berpengalaman, bukan hasil generate otomatis yang kaku.

## Ciri Kode "Khas AI" yang Harus Dihindari

### 1. Komentar Baris-per-Baris yang Redundan
*   **Hindari**: Menjelaskan hal yang sudah jelas terbaca dari kode (e.g., `// Menambahkan 1 ke nilai i` di atas `i++`).
*   **Ganti dengan**: Tulis komentar yang menjelaskan **mengapa (why)** keputusan desain itu diambil, atau untuk menjelaskan logika bisnis yang kompleks dan tidak langsung terlihat dari sintaksis.

### 2. Penamaan Variabel yang Terlalu Deskriptif atau Terlalu Generik
*   **Hindari**: Nama variabel super panjang yang berlebihan (e.g., `temporaryIntegerCounterForUserListLoop`) atau terlalu malas (e.g., `temp1`, `data`).
*   **Ganti dengan**: Nama yang ringkas namun informatif sesuai konvensi bahasa pemrogaman yang bersangkutan (e.g., `userCount`, `idx`, `isPending`).

### 3. Boilerplate & Over-Engineering Berlebih
*   **Hindari**: Membuat kelas, interface, pembungkus (wrapper), atau error handling berlapis-lapis untuk tugas sederhana yang sebenarnya bisa selesai dengan 10 baris kode bersih.
*   **Ganti dengan**: Prinsip KISS (Keep It Simple, Stupid) dan YAGNI (You Aren't Gonna Need It). Prioritaskan kesederhanaan dan keterbacaan.

### 4. Struktur & Layout Kode yang Terlalu Monoton
*   **Hindari**: Kode tanpa spasi pemisah logika, atau sebaliknya, spasi yang terlalu banyak secara acak.
*   **Ganti dengan**: Kelompokkan baris-baris kode yang berhubungan erat, dan pisahkan dengan satu baris kosong (blank line) untuk menunjukkan transisi alur logika (seperti paragraf dalam tulisan).
