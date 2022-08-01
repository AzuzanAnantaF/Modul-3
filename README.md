###### Nama : Azuzan Ananta F
###### Kelas : XIII RPL 1
###### No Absen : 17 

# Modul 3

###### Route dengan aksi controller
Route seperti ini ketika dijalankan akan mengakses controller yang disebutkan pada 
parameter kedua. Jika ingin mengakses method atau function tertentu pada controller, maka 
antara nama controller dengan nama fungsi dipisahkan dengan tanda @. Untuk 
mempraktekan route ini buatlah satu controller dengan menggunakan perintah artisan sebagai 
berikut:
```
php artisan make:controller BarangController
```

Perintah artisan diatas 
akan menghasilkan satu file baru bernama ProdukController.php yang terletak di folder 
app\Http\Controller. Bukalah file controller tersebut dan tambahkan satu fungsi bernama 
index seperti pada controh skrip dibawah:
```
<?php

namespace App\Http\Controllers;

use Illuminate\Http\Request;

class BarangController extends Controller
{
    Public function index()
    {
        return 'Mengakses Fungsi di controller menggunakan route';
    }
}
```

Kemudian buka file web.php yang ada pada folder routes/web.php tambahkan satu route baru 
dengen bentuk seperti berikut:
```
<?php

use Illuminate\Support\Facades\Route;
use App\Http\Controllers\BarangController;

Route::get('/barang', [BarangController::class, 'index']);
```

Tapi sebelum membuat itu semua kita harus memasukkan code pemograman dicmd, dengan code seperti dibawah ini. Agar website kita berjalan.

![image](https://user-images.githubusercontent.com/109930500/182089881-6126a9b1-a89f-498c-a577-14ce26ea008c.png)

![image](https://user-images.githubusercontent.com/109930500/182091014-e9e347ad-d65c-4650-97b8-8c1c4db62093.png)

SOAL
1. Buatlah Route yang menuju kehalaman Kategori
2. Buatlah halaman tambah data di setiap route

Jawaban:

1. Langkah pertama masukkan code pemograman dicmd, dengan code seperti dibawah ini.

![image](https://user-images.githubusercontent.com/109930500/182089881-6126a9b1-a89f-498c-a577-14ce26ea008c.png)

Langkah kedua
