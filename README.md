# KOMENTAR BLOG POST PLUGIN
Deskripsi :
Plugin untuk menayangkan komentar yang diinput oleh visitor pada halaman web blog post.

Kebergantungan :
Plugin ini bergantung kepada Plugin RainLab.Blog.

Implementasi pada Halaman Front End :
Plugin ini memiliki 2 component : formKomentar dan postKomentar.

formKomentar menyediakan form dimana visitor bisa menginputkan komentar pada halaman tertentu. Form field terdiri dari Nama, Email dan Komentar.

postKomentar menampilkan semua data komentar yang diinputkan oleh visitor pada halaman tertentu diurut turun berdasarkan tanggal dan waktu input.

Implementasi pada Halaman Back End :
Menu Utama Komentar, menampilkan semua komentar yang sudah diinputkan oleh visitor dari semua halaman blog post. Menu ini memiliki fitur untuk menghapus komentar tertentu.


INTEGRASI COMPONENT KEPADA HALAMAN BLOG POST
 1. Buka Menu Utama CMS
 2. Pada layout tambahkan markup {% framework extras %} setelah tag script core jquery.
 3. Pemasangan component dipisahkan satu tingkat lebih tinggi terhadap markupnya. Misalkan jika markup {% component 'postKomentar' %} ditaruh pada tingkat partials maka component postKomentar diletakkan pada tingkat pages. Atau jika markup {% component 'formKomentar' %} ditaruh pada tingkat pages maka component formKomentar diletakkan pada tingkat layouts 
