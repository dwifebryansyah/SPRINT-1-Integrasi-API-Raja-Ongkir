Cara Install:
    1. Clone terlebih dahulu repository ini
    2. Composer Update di Command Prompt
    3. Nyalakan Apache sama Mysql XAMPP
    4. Buat Database:
            4.1 Buka pada Browser localhost/phpmyadmin
            4.2 Buka SQL Lalu perintahkan : Create database namadatabase
    5. Masuk ke folder yang sudah di clone tadi, terus buka file .env
    6. isi DB_DATABASE dengan database yang sudah dibikin tadi
        contoh DB_DATABASE=DOT_Sprint_Dwi
    7. Untuk username sama password isi apabila saat masuk mysql memang ada username sama passwordnya , kalo tidak ada biarkan saja
    8. Apabila sudah semua, buka Command Prompt dan arahkan ke folder yang sudah diclone tadi lalu jalankan
        php artisan migrate
    9. Otomatis nanti table sudah terbuat dengan migrate
    10. Setelah itu buka file RunApi tunggu sampai ada tulisan started, dan biarkan jangan di close
    11. Untuk melakukan fetching data Province , klik RunFetchingProvince , pastikan sudah jalan RunApinya
    12. Untuk melakukan fetching data City, klik RunFetchingCities , pastikan sudah jalan RunApinya pastikan setelah RunFetchingProvince
    13. Lihat di database yang sudah dibikin tadi , otomatis table Province sama City sudah terisi
        atau bisa dilihat dengan membuka browser , lalu ketik:
        Untuk Melihat Province keseluruhan  : http://localhost:8000/api/search/province
        Untuk Melihat Province satuan       : http://localhost:8000/api/search/province?id=5
        Untuk Melihat City keseluruhan      : http://localhost:8000/api/search/cities
        Untuk Melihat City satuan           : http://localhost:8000/api/search/cities?id=5
    14. Cukup sekian tutorial yang bisa saya sampaikan , apabila ada pertanyaan bisa hubungi saya 
        email: dwifebryansyah5@gmail.com
        notelp: 082258130886