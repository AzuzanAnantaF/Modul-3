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
