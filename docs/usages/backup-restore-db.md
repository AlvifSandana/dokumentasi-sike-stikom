# Backup / Restore DB
Fitur ini memungkinkan aplikasi dapat meng-***backup*** maupun ***restore*** database yang digunakan. Saat ini fitur dalam masa pengembangan untuk versi yang berjalan pada ***Docker Container***.

> Catatan: File hasil proses backup tersimpan di direktori `public/backupdb`.

## Backup
1. Klik tombol `Backup` berwarna hijau pada card `Backup Database`.
2. Tunggu hingga muncul `alert` berwarna hijau di atas card dan klik link **Download** untuk mengunduh file `.sql`
<img src="_media/images/br.png" alt="show_backup_restore"></img>

## Restore
1. Pilih file `.sql` dengan meng-klik tombol `Browse`.
2. Klik tombol `Restore` berwarna biru untuk meng-upload file `.sql` dan melakukan proses **restore** database. 
<img src="_media/images/br-1.png" alt="show_restore"></img>


