<details>
  <summary> Commit 1 Reflection Notes </summary>

  Method `handle_connection` memiliki input stream berupa `TcpStream`. Method ini membaca HTTP Request dengan membuat `BufReader` untuk membaca buffer dari stream, lalu menggunakan `.lines()` untuk mereturn iterator baris dari `BufReader`. Selanjutnya, menggunakan `.map` untuk mengubah `Result` menjadi String dan menggunakan `.take_while()` untuk mengambil baris hingga akhir headers HTTP. Method ini juga akan mengumpulkan baris-baris tersebut ke dalam sebuah vektor `http_request`. Dari proses tersebut, akan ada output yang dicetak pada perintah `println!`.
</details>

<details>
  <summary> Commit 2 Reflection Notes </summary>

  Text seperti Content-Length adalah HTTP response yang dikirimkan setelah kita menerima request HTTP, dalam hal ini adalah `hello.html`. Dari kode yang ada, dapat dilihat bahwa response yang ingin diberikan adalah `"{status_line}\r\nContent-Length: {length}\r\n\r\n{contents}"`. Di situ, `status_line` akan berisi status dari requestnya (misal berhasil atau tidak), lalu, `\r` menandakan carriage return, dan `\n` menandakan new line. Lalu, `Content-length` yang diisi dengan `{length}` adalah panjang dari body http responsenya (dalam konteks ini, `hello.html`), sedangkan `{contents}` berisi konten dari response itu sendiri. Hal ini diperlukan untuk memastikan bahwa HTTP responsenya valid

  ![Commit 2 screen capture](assets/images/Commit2.png)
</details>
<details>
  <summary> Commit 3 Reflection Notes </summary>

  ![Commit 3 screen capture](assets/images/Commit3.png)
</details>
<details>
  <summary> Commit 4 Reflection Notes </summary>
</details>
<details>
  <summary> Commit 5 Reflection Notes </summary>
</details>
