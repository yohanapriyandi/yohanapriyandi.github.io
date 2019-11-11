---
layout: post
title:  "Beberapa perintah untuk melakukan clear cache dengan comman di Laravel 5"
date:   2019-11-11 15:31:02 +0700
categories: Laravel
---
Hai selamat siang, sambil menunggu proses chekcout ke repo yang lumayan besar saya coba selingi dengan menulis
pekerjaan yang saya lakukan sebagai memori, jaga-jaga kalau lupa tinggal buka blog pribadi [ini]:https://yohanapriyandi.github.io

Siang ini saya akan memeberi tahu teman teman coders beberapa perintah artisan yang ada di laravel yang berguna untuk membersihkan cache, langsung aja yah:

1. php artisan cache:clear
2. php artisan route:cache
3. php artisan config:clear
4. php artisan view:clear


teman teman juga bisa memanggil command-command di di atas di dalam route seperti contoh di bawah ini:

Route::get('/clear-cache', function() {
    Artisan::call('cache:clear');
    return "Cache is cleared";
});

Nah diatas merupakan perintah perintah yang sering saya gunakan untuk mengelola cache si laravel, jadi jangan bingung ketika ada error muncul mengenai cache coba jalankan perintah perintah di atas sesuia kebutuhan teman-teman coders. Oke cukup dulu kayaknya saya akan update artikel apabila ada trik baru mengenai cache di laravel. Terima kasih.

salam coding...

Sumber:
[laravel]:https://laravel.com/
