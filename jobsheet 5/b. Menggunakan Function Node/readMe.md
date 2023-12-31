# B. Menggunakan Function Node

### a. Langkah Kerja
  1. Buatlah flow fungsi output tunggal seperti pada gambar berikut
     ![job5b](https://github.com/iamanisaamalia/sistemembedded/assets/147674408/7ada2874-b23d-42f8-a2c6-58a117d6f1ae)
  2. Konfigurasikan node Input1. Isikan payload dengan “Hello World”, dan topic berupa “test1”.
  3. Deploy program dan dokumentasikan hasilnya.
  4. Buatlah flow fungsi output berganda yang berfungsi memisahkan pesan seperti gambar di bawah ini.
     ![langkah-2](https://github.com/iamanisaamalia/sistemembedded/assets/147674408/77990891-a4ad-4bd0-bdbc-dc79ad012823)
  5. Konfigurasikan node Input2. Isikan payload dengan “Expeliarmus”, dan topic berupa “test2”.
  6. Konfigurasikan node fungsi seperti gambar berikut ini.

     ![job5bjuga](https://github.com/iamanisaamalia/sistemembedded/assets/147674408/479dc948-0a22-43ce-af94-8f00bb52b988)
     
  8. Deploy program dan dokumentasikan hasilnya.
### b. Hasil dan Pembahasan
Pada percobaan pertama, function node dimulai dengan membuat flow fungsi output tunggal dan menkonfigurasi node input1 lalu mengisi payload dengan ”Hello World” dan topik berupa ”test1”. Deploy program dan hasil akan muncul pada debug, yaitu "Hello World"

![hasil-2-1](https://github.com/iamanisaamalia/sistemembedded/assets/147674408/c0c74118-8f01-4281-9c20-9c1ebb244c6f)


Kemudian dilanjutkan dengan membuat flow fungsi output berganda yang berfungsi memisahkan pesan lalu konfigurasikan node Input2. Isikan payload dengan “Expeliarmus”, dan topic berupa “test2”. 
Function node pada Node-RED adalah elemen yang memungkinkan penulisan kode JavaScript khusus untuk memproses dan memanipulasi data yang mengalir melalui alur kerja. Dengan function node, hasil yang muncul adalah
- Jika msg.topic adalah "test1", maka node output pertama akan menerima [msg, null], yang berarti pesan "Hello World" akan dikirim ke output pertama, sedangkan output kedua akan tetap kosong (null).
- Jika msg.topic adalah "test2", maka node output kedua akan menerima [msg, null], yang berarti pesan "Expeliarmus" akan dikirim ke output kedua, sedangkan output pertama akan tetap kosong (null).

![hasil-2-2](https://github.com/iamanisaamalia/sistemembedded/assets/147674408/d1073605-391d-4f6e-a007-8dea1b14c577)
