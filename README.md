## Readme for tutorial8 subscriber repository
a. what is amqp? <br>
Jawab: AMQP atau Advanced Message Queuing Protocol merupakan standard protokol layer suatu aplikasi yang diimplementasikan sebagai
message-oriented middleware atau suatu infrasturktur yang mendukung pengiriman dan penerimaan pesan antar sistem terdistribusi. Tujuan utama dari penggunaan AMQP 
yakni memungkinkannya penyampaian pesan yang dapat disampaikan antar organisasi di seluruh platform yang terdistribusi secara beragam. AMQP memudahkan aplikasi perangkat lunak 
yang berbeda, ditulis dalam bahasa pemrograman yang berbeda dan berjalan pada platform yang berbeda untuk berkomunikasi satu sama lain secara andal dan efisien. <br>
<br>
b. what it means? guest:guest@localhost:5672, what is the first quest, and what is the second guest, and what is localhost:5672 is for? <br>
Jawab: Pada AMQP, `guest:guest@localhost:5672` digunakan sebagai koneksi url yang terhubung pada server AMQP <br>
- guest:guest = Bagian ini mengacu pada nama pengguna dan kata sandi yang digunakan untuk otentikasi saat menghubungkan ke RabbitMQ. Di RabbitMQ, secara default akan terdapat
akun pengguna default dengan nama pengguna "guest" dan kata sandi "guest"
- localhost:5672 = Bagian ini menunjukkan host dan port server RabbitMQ. "localhost" menunjukkan bahwa server RabbitMQ berjalan di mesin yang sama dengan kode yang menghubungkannya.Sementara itu,
port 5672 adalah port default untuk koneksi AMQP <br>
Artinya, ketika kode yang saya buat membuat koneksi ke url amqp://guest:guest@localhost:5672, kode tersebut akan terhubung ke server RabbitMQ yang berjalan di localhost menggunakan kredensial
"guest" secara default untuk proses otentikasi
