# Exercise 7: Impact of Resource Sharing on System Performance

## Tujuan
1. Menunjukkan bagaimana berbagi sumber daya dalam sistem multitasking dapat memengaruhi kinerja sistem.
2. Menganalisis dampak waktu akses sumber daya terhadap waktu penyelesaian tugas.

## Peralatan
1. STM32F1
2. STM32CubeIDE.
3. FreeRTOS library.
4. Tracealyzer (opsional).

## Langkah-langkah
**Persiapan Proyek**
1. Buat tugas HighPriorityTask dan LowPriorityTask di STM32CubeIDE.
2. Pastikan kedua tugas berbagi sumber daya bersama.

**Implementasi Kode**
1. Tanpa perlindungan, biarkan kedua tugas mengakses sumber daya bersama secara bebas.
2. Catat waktu penyelesaian tugas dengan dan tanpa proteksi.

**Uji Program**
1. Flash kode ke STM32F4 Discovery Board.
2. Gunakan Tracealyzer (opsional) untuk memvisualisasikan kinerja sistem.

## Hasil yang Diharapkan
1. Tanpa Perlindungan: Tugas berprioritas tinggi dapat terhambat oleh tugas berprioritas rendah, mengurangi performa sistem.
2. Dengan Proteksi: Menggunakan mekanisme seperti taskENTER_CRITICAL() memastikan tugas berprioritas tinggi tetap berjalan optimal

## Hasil Percobaan


https://github.com/user-attachments/assets/e7352ff9-c44c-42e2-bcef-3b741b5ac69c

