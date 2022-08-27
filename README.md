## JavaScript Intermdiate - Asynchronous - Async Await
Penjelasan penggunaan Async Await
- Async/Await adalah salah satu cara untuk mengatasai masalah asynchronous pada Javascript selain menggunakan callback dan promise.
- Pada implementasi Async/Await, kita menggunakan kata kunci async sebelum fungsi. Await sendiri hanya bisa digunakan pada fungsi yang menggunakan async.
- Untuk menggunakan Async/Await, kembalian dari suatu fungsi harus merupakan suatu Promise. Async/Await tidak dapat berdiri tanpa adanya Promise.
- Tidak seperti Promise, dengan Async/Await maka suatu baris kode dapat tersusun rapi mirip dengan kode yang sifatnya synchronous.
- Setiap baris yang menggunakan await, akan ditunggu sampai Asynchronous Promise tersebut di resolve.
Contoh Array sebagai berikut:
``` 
    const getAllUser = async ()=> {
	const data = await getUser()
	console.log(data)
    }
```

## Responsive WEb Design
Responsive web design atau desain web responsif adalah sebuah teknik atau metode bagi web designer untuk membuat suatu layout website yang dapat menyesuaikan diri sesuai dengan ukuran layar pengguna.
> Chrome Dev Tools - browser chrome
 
Untuk mengakses Chrome Dev Tools: 
  > ctrl + shift + j

## Mengenal Flexbox Pada CSS
Flexbox atau Flexible Box  merupakan sebuah mode pengaturan atau konsep layout pada CSS yang digunakan untuk mengatur elemen atau container beserta item didalamnya pada halaman web.

### Property Flex pada Container
1. display

Langkah pertama untuk membuat sebuah container menjadi flex, adalah menambahkan “flex” pada property “display”. Hal ini akan membuat container yang kita punya menjadi flex dan dapat memakai property flex.
``` 
    .container {
     display: flex;
    }
```
2. flex-direction

dengan menggunakan property “flex-direction”, maka kita dapat menentukan arahnya item-item yang ada didalam container.

![display1](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2021.png?1628228538451)

![display2](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2022.png?1628228559883)

- Row (default) : item akan berurutan dari kiri ke kanan
- Row-reverse : kebalikan dari row, item berurutan dari kanan ke kiri
- Column : sama seperti row, tetapi akan berurutan dari atas ke bawah
- Column-reverse : sama seperti row-reverse. Tetapi berurutan dari bawah ke atas
``` 
    .container {
      flex-direction: row | row-reverse | column | column-reverse;
    }
```

3. flex-wrap

defaultnya, item pada flex akan mencoba masuk atau fit ke dalam satu baris atau row. Kita bisa membuat item yang berlebihan untuk lanjut ke baris atau kolom berikutnya.

![wrap1](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2023.png?1628228598739)

![wrap2](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2024.png?1628228613938)

- Nowrap (default): semua item akan berada di satu baris
- Wrap: item flex akan pindah ke baris selanjutnya apabila tidak muat, dari atas ke bawah
- Wrap-reverse: sama seperti wrap, tetapi arah nya dari bawah ke atas.
``` 
    .container {
      flex-wrap: nowrap | wrap | wrap-reverse;
    }
```
4. Justify-content

property ini memungkinkan kita mengkontrol atas penyelarasan (alignment) item flex yang berada di dalam container.

![J1](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2025.png?1628228669251)

![J2](https://www.gamelab.id/uploads/modules/NEWS/817/Group%2026.png?1628228677875)
- Flex- start: posisi item akan dikemas pada bagian awal “flex-direction”
- Flex-end: posisi item akan dikemas pada bagian akhir “flex-direction”
- Center: posisi item akan dikemas ke bagian tengah baris
- Space-between: letak item akan didistribusikan secara merata, item pertama ada pada bagian start dan item terakhir pada bagian end.
- Space-around: letak item akan didistribusikan secara merata dengan space/ruang yang ada diantara item.
``` 
    .container{
     justify-content: flex-start | flex-end | center | space-between | space-around;
    }
```
## Bootstrap
Bootstrap adalah framework web development gratis dan open-source yang dirancang untuk memudahkan proses pengembangan web responsif dan mobile-first (memprioritaskan perangkat seluler), dengan menyediakan berbagai syntax untuk desain template.

Mengapa menggunakan bootstrap?
- Mudah Digunakan
- Responsive Grid
- Kompatibel dengan Banyak Browser
- Dokumentasi Bootstrap yang Lengkap

3 File Utama Bootstrap
- **Bootstrap.css**, framework CSS yang mengatur dan mengelola tata letak website.
- **Bootstrap.js**, Ini adalah bagian inti Bootstrap, terdiri dari file JavaScript yang bertugas untuk menangani interaktivitas website.
- **Glyphicons**,  Bootstrap menggunakan ikon yang disebut Glyphicons, yang mencakup set Halflings Glyphicons. Untuk mengubah ukuran Glyphicons, Anda perlu menimpa gaya default dengan properti font-size (ukuran font) CSS.
### Cara Menggunakan Bootstrap
``` 
 <html lang="en">
    <head>
     <meta charset="utf-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge"/>
     <meta name="viewport" content="width=device-width, initial-scale=1" /> 
     <title>Bootstrap 101 Template</title>
     <link href="css/bootstrap.min.css" rel="stylesheet" />
    </head>
    <body>
     <h1>Hello, world!</h1>
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.3/jquery.min.js"></script>
     <script src="js/bootstrap.min.js"></script>
    </body>
 </html>
```
