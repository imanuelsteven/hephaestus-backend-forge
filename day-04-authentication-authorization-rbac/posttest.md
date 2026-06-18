# Posttest - Authentication, Authorization & RBAC

## Objective

Posttest ini digunakan untuk mengukur pemahaman peserta setelah mempelajari Authentication, Authorization, JWT, RBAC, dan resource-level authorization.

### 1. Apa itu authentication?

Jawaban:

```text
Authentication adalah proses memastikan identitas user, biasanya dengan login menggunakan username dan password.
```

### 2. Apa itu authorization?

Jawaban:

```text
Authorization adalah proses mengecek apakah user yang sudah dikenali boleh mengakses fitur atau data tertentu.
```

### 3. Apa perbedaan authentication dan authorization?

Jawaban:

```text
Authentication mengecek siapa usernya, sedangkan authorization mengecek apa saja yang boleh dilakukan user tersebut.
```

### 4. Kenapa user yang sudah login belum tentu boleh melakukan semua action?

Jawaban:

```text
Karena setiap user bisa memiliki role dan permission yang berbeda, jadi aksesnya harus dibatasi sesuai kebutuhannya.
```

### 5. Apa itu token-based authentication?

Jawaban:

```text
Token-based authentication adalah metode login yang memberikan token ke user setelah berhasil login untuk digunakan pada request berikutnya.
```

### 6. Apa fungsi Authorization header?

Jawaban:

```text
Authorization header berfungsi untuk mengirim token dari client ke server agar server bisa memvalidasi identitas user.
```

### 7. Apa arti Bearer token?

Jawaban:

```text
Bearer token berarti siapa pun yang membawa token valid tersebut dianggap sebagai user yang berhak mengakses request.
```

### 8. Apa itu JWT?

Jawaban:

```text
JWT adalah token berbentuk string yang berisi informasi user dan signature untuk membantu proses authentication dan authorization.
```

### 9. Apa itu claim pada JWT?

Jawaban:

```text
Claim pada JWT adalah data atau informasi yang disimpan di dalam payload token, seperti user id, role, atau waktu expired.
```

### 10. Sebutkan 4 claim yang umum ada pada JWT.

Jawaban:

```text
Empat claim yang umum ada pada JWT adalah sub, role, iat, dan exp.
```

### 11. Kenapa JWT payload tidak boleh dipercaya sebelum signature divalidasi?

Jawaban:

```text
Karena payload JWT bisa dibaca dan dimodifikasi, jadi server harus memvalidasi signature untuk memastikan token tidak dipalsukan.
```

### 12. Data apa saja yang tidak boleh disimpan di JWT?

Jawaban:

```text
Data sensitif seperti password, PIN, nomor kartu, NIK lengkap, dan data rahasia lain tidak boleh disimpan di JWT.
```

### 13. Kenapa token perlu expiry?

Jawaban:

```text
Token perlu expiry agar token yang bocor atau dicuri tidak bisa digunakan selamanya.
```

### 14. Apa perbedaan access token dan refresh token?

Jawaban:

```text
Access token digunakan untuk mengakses API dalam waktu singkat, sedangkan refresh token digunakan untuk mendapatkan access token baru.
```

### 15. Apa itu RBAC?

Jawaban:

```text
RBAC adalah sistem pengaturan akses berdasarkan role atau peran user dalam aplikasi.
```

### 16. Apa perbedaan role dan permission?

Jawaban:

```text
Role adalah jabatan atau kelompok user, sedangkan permission adalah izin spesifik untuk melakukan suatu action.
```

### 17. Berikan contoh role dalam loan system.

Jawaban:

```text
Contoh role dalam loan system adalah Customer, Agent, Risk Officer, dan Head Office.
```

### 18. Berikan contoh permission dalam loan system.

Jawaban:

```text
Contoh permission dalam loan system adalah create_application, view_application, review_application, dan approve_application.
```

### 19. Kenapa role check saja tidak cukup?

Jawaban:

```text
Role check saja tidak cukup karena user dengan role yang sama belum tentu boleh mengakses semua data atau resource.
```

### 20. Apa itu resource-level authorization?

Jawaban:

```text
Resource-level authorization adalah pengecekan apakah user boleh mengakses resource tertentu, misalnya data loan dengan id tertentu.
```

### 21. Apa itu ownership check?

Jawaban:

```text
Ownership check adalah pengecekan apakah data yang ingin diakses benar-benar milik user tersebut.
```

### 22. Apa itu IDOR?

Jawaban:

```text
IDOR adalah celah keamanan ketika user bisa mengakses data orang lain hanya dengan mengganti id pada request.
```

### 23. Bagaimana cara mencegah customer melihat data customer lain?

Jawaban:

```text
Caranya adalah dengan mengecek user id dari token dan memastikan data yang diminta memang milik customer tersebut.
```

### 24. Kapan menggunakan 401 Unauthorized?

Jawaban:

```text
401 Unauthorized digunakan ketika user belum login, token tidak ada, token salah, atau token sudah expired.
```

### 25. Kapan menggunakan 403 Forbidden?

Jawaban:

```text
403 Forbidden digunakan ketika user sudah login tetapi tidak punya izin untuk mengakses fitur atau data tersebut.
```

### 26. Apa perbedaan 401 dan 403?

Jawaban:

```text
401 berarti authentication gagal atau belum ada, sedangkan 403 berarti user sudah dikenali tetapi aksesnya ditolak.
```

### 27. Kenapa error message security tidak boleh terlalu detail?

Jawaban:

```text
Karena error yang terlalu detail bisa membantu attacker menebak sistem, token, user, atau kelemahan aplikasi.
```

### 28. Apa itu principle of least privilege?

Jawaban:

```text
Principle of least privilege adalah prinsip memberikan akses seminimal mungkin sesuai kebutuhan user.
```

### 29. Kenapa access log penting dalam finance backend?

Jawaban:

```text
Access log penting untuk audit, tracking aktivitas user, investigasi masalah, dan mendeteksi akses yang mencurigakan.
```

### 30. Sebutkan field penting dalam access log.

Jawaban:

```text
Field penting dalam access log adalah timestamp, user id, role, endpoint, method, status code, ip address, dan action.
```

### 31. Bagaimana auth requirement ditulis di API contract?

Jawaban:

```text
Auth requirement ditulis dengan menjelaskan endpoint mana yang butuh token, header yang digunakan, role atau permission yang dibutuhkan, dan kemungkinan response error.
```

### 32. Bagaimana Swagger/OpenAPI membantu dokumentasi endpoint yang protected?

Jawaban:

```text
Swagger/OpenAPI membantu menampilkan endpoint yang butuh authentication, cara memasukkan Bearer token, dan aturan aksesnya.
```

### 33. Apa risiko jika role dikirim dari client lalu langsung dipercaya?

Jawaban:

```text
Risikonya adalah user bisa memalsukan role dari client agar terlihat seperti admin atau role lain yang punya akses lebih besar.
```

### 34. Apa risiko token tanpa expiry?

Jawaban:

```text
Risikonya adalah token yang bocor bisa digunakan terus-menerus tanpa batas waktu.
```

### 35. Bagian mana yang paling sulit dari Day 4?

Jawaban:

```text
Implementasi Token Authorization manual, dan bikin role validator karena belum pernah buat jadi masih banyak searching dan ai, mengetahui apakah code saya sudah best practice atau tidak
```

## Reflection

Apa 3 hal utama yang kamu pahami hari ini?

```text
1. cara membuat RBAC
2. cara menggunakan anotasi yg baru terkait authorization seperti : requestheader, configuration, securityscheme dll
3. menambahkan config untuk open api dan iplemntasi security  barear
```

Apa 2 hal yang masih membingungkan?

```text
1. Proses pembuatan RBAC
2. Mengetahui apakah code saya sudah best pracitce atau belum, perlu di refactor atau tidak
```

Apa 1 pertanyaan untuk mentor?

```text
Apakah ada library yang memudahkan dalam pembuatan rbac, mungkin yang paling simpel?
```
