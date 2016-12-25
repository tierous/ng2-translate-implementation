# ng2-translate-implementation
Mengimplementasikan ng-2translate ke seed webpack-starter

## Kesimpulan
* ng2-translate bisa diimplementasikan pada seed angular2-webpack-starter
* Belum support menggunakan file bahasa.json yang berbeda untuk setiap module dengan alasan karena pendeklarasian TranslateModule milik ng2-translate harus dilakukan di root module dimana tempat untuk menentukan letak file bahasa.json dideklarasikan di TranslateModule.forRoot() yang mana .forRoot() tidak boleh dideklarasikan di child module.
* Untuk setiap child module yang akan menggunakan TranslateModule mesti mengimport TranslateModule lagi walaupun sudah diimport di AppModule
* Bisa digunakan di dalam attribute tag HTML

## Cara Implementasi
* Baca dokumentasi di https://github.com/ocombe/ng2-translate
