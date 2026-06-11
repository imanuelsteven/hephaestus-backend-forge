# Posttest - Java Fundamental

Jawab pertanyaan berikut setelah membaca materi dan mengerjakan exercise Java Fundamental.

### 1. Apa itu variable?

Jawaban:

```text
tempat untuk menyimpan data dan bisa digunakan untuk menjalankan program tertentu, misal saya punya variabel :
String nama; -> artinya `nama` adalah sebuah variabel yang bertipe string dan variabel ini bisa digunakan untuk kebutuhan membuat suatu program nantinya
```

### 2. Apa perbedaan String, int, Long, dan boolean?

Jawaban:

```text
String digunakan untuk data bersifat huruf dan angka
-> namun tidak bisa di gunakan untuk numerical operation

int digunakan untuk data yang bersifat angka namun hanya bilangang bulat dan bisa digunakan untuk numerical operation

Long digunakan untuk untuk data yang bersifat angka/bilangan bulat namun kapasitasnya dapat menyimpan angka yang jauh lebih besar dari integer.
```

### 3. Kenapa Java menggunakan camelCase untuk variable?

Jawaban:

```text
kareana sudah menjadi kesepakatan komunitas java pada saat itu, tujuannya untuk menjaga readability/kemudahan membaca dan juga  membuat standar/keseragaman.

```

### 4. Apa perbedaan class dan object?

Jawaban:

```text
Class adalah sebuah bluprint yang bisa berisikan field, method, constructor dll, sedangkan object adalah wujud nyata atau hasil instance dari class. object sendiri bisa berbeda beda isinya walupun dihasilkan dari class yang sama.
```

### 5. Apa itu field?

Jawaban:

```text
Variabel/atribut/karakteristik/data yang terdapat di dalam kelas yang nantinya akan dijadikan sebuah objek.
```

### 6. Apa itu method?

Jawaban:

```text
Method adalah kumpulan kode yang dieksuksi dan digabungkan untuk melakukan suatu hal tertentu, jika didalam class method berfungsi sebagai tindakan yang bisa dilakukan oleh class tersebut.
```

### 7. Apa itu parameter?

Jawaban:

```text
Masukan yang diterima oleh method agar method bisa dieksekusi dan dijalankan.
```

### 8. Apa itu return value?

Jawaban:

```text
Value yang menjadi hasil/keluaran yang diberikan oleh suatu method
```

### 9. Apa fungsi constructor?

Jawaban:

```text
method khusus yang akan di eksekusi terlebih dahulu dalam membuat sebuah objek, jadi jika kita akan membuat objek field akan di assign ke constructor dan baru akan di assign ke kelasnya.
```

### 10. Apa fungsi `this`?

Jawaban:

```text
this menjadi pananda bahwa field yang di ambil berasal dari kelas yang dibuat konstruktornya. this juga menjawab abiguitas ketika nama field asli class == parameter constructor yang dibuat.
```

### 11. Kenapa field dibuat private?

Jawaban:

```text
Agar class lain dan folder lain tidak dapat mengaksesnuya secara sembarangan dan hanya bisa melalui setter dan getter saja. intinya keamanan dan biar ga eror jika sewaktu waktu field tidak sengaja keisi dengan nilai yang sembarangan.
```

### 12. Apa fungsi getter dan setter?

Jawaban:

```text
getter dan setter digunakan untuk mengakses field yang di set private. Getter digunakan untuk mengambil/menarik field, sedangkan setter digunakan untuk mengedit field.
```

### 13. Apa itu encapsulation?

Jawaban:

```text
Salah satu prinsip data oop yang menekankan keamanan data : contohnya adlalh penerapan akses modiefier dan juga setter getter.
```

### 14. Apa perbedaan List dan Map?

Jawaban:

```text
list  berisikan banyak nilai namun tidak ada key dan value  didalam nya sedangkan map berisikan key dan values.
```

### 15. Kenapa CustomerService menggunakan Map<Long, Customer>?

Jawaban:

```text
karene customer storage membutuhkan id unik yang bertipe long dan juga Customer yang berinalai objek untuk menyimpan data lengkap pelangan yang dibangun dengan class Customer(blueprint yang sudah kita buat sebelumnya)
```

### 16. Kenapa getAllCustomers mengembalikan List<Customer>?

Jawaban:

```text
karena di awal kita membuat method dengan `public List<Customer>` artinya kita wajib return list objek customer, selain itu di dalam getallcustomer kita memberikan return semua objek customer yang sudah dibuat dengan arraylist sehingga output dari method tersebut berupa list.
```

### 17. Apa itu interface?

Jawaban:

```text
interface adalah sekumpulan method yang dijadikan sebuah kontrak, dan ketika suatu class mengimplementasikannya maka method yang ada di interface harus dan wajib hukumnya untuk di tulis/digunakan dalam class tersebut.
```

### 18. Apa perbedaan interface dan abstract class?

Jawaban:

```text
Interface lebih ke kontrak yang harus diimplentasikan methodnya sedangkan abstract adalah rancangan yang masih abstract sehingga bebas jika tidak digunakan, abstrak juga bersifat general misal abstracy hewan -> nanti baru bikin class kucing untuk di extend dari abstraknya. keduanya sama sama tidak bisa dijadikan objek dan harus di extend (kalo abstract) dan implement(kalo interface).
```

### 19. Dari exercise, jelaskan flow createCustomer.

Jawaban:

```text
- Menyiapkan long sequence = 0 sebagai id dari objek yg akan dibuat
- membuat method create customer yang berisikan parameter
    - nama
    - email
    - phonnumber
    - ini akan digunakan dalam membuat objek -> assign ke constructor.
- melakukan validasi apakah nilai nama tidak kosong, jika kosong maka akan throw eror handling
- membuat objek yang bernama 'customer' dan memasukan paramater fungsi ke konstruktor sehingga terciptalah objek
- menambah nilai variabel sequence sehingga idnya menjadi inrement bertambah
- menyimpan id/sequence dan value/objek customer didalam variabel customerStorage yg bertipe hashmap
- menghasilkan output objek customer.
```

### 20. Bagian mana yang paling sulit?

Jawaban:

```text
penggunaan abstract dan juga upcasting downcasting (kalo dimateri), tidak hafal sintaks dan kadang bingung  mau nulis apa. (yang di exercise )
```
