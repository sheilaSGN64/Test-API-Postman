sebelum menjalankan test api diperlukan diketahui kalau project ini berhasil di eksekusi di platform OS windows 10 x64, 
download Node.js(LTS) dan running instalasi nya seperti biasa 
beberapa requirementnya seperti berikut :
- Postman v11.69.1
- Node.js v22.21.0(LTS)

buka folder dimana file take_home_test.postman_environment.json dan Test_Case_02.postman_collection.json nya disimpan, perlu diperhatikan kalau kedua file ini harus dalam satu folder supaya bisa di eksekusi
buka command prompt (cmd) di folder tersebut, kemudian copy paste ini kalau Newman belum ada
.
-npm install -g newman
.
atau jika ingin hasil report HTML maka :
- npm install -g newman newman-reporter-htmlextra
.

masih di terminal folder yang sama, jalankan perintah ini untuk mengeksekusi test api dengan Newman :
- newman run Test_Case_02.postman_collection.json -e take_home_test.postman_environment.json 
