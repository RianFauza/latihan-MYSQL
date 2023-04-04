# latihan-MYSQL 

## 1. Membuat database latihan2:
# ``CREATE DATABASE latihan2;``
![image](https://user-images.githubusercontent.com/115771479/229921958-ec728715-f149-4ad0-b5d6-94b1a350ae8d.png)

## MENAMPILKAN DAFTAR BASIS DATA
![image](https://user-images.githubusercontent.com/115771479/229925566-5c0bf285-a66c-47d7-9984-51ee130fd8d0.png)

## 2. Membuat tabel biodata di dalam database latihan2:
# ``USE latihan2; CREATE TABLE biodata (nama VARCHAR(15),alamat VARCHAR(15));``
![image](https://user-images.githubusercontent.com/115771479/229922967-70538c57-9704-4e7e-bd5f-d22461a41036.png)

## 3. Menambahkan kolom keterangan:
# ``ALTER TABLE biodata ADD keterangan VARCHAR(15);``
![image](https://user-images.githubusercontent.com/115771479/229923774-aafc34d6-1d18-4739-ab69-d0216d5387ee.png)

## 4. Menambahkan kolom id di awal:
# ``ALTER TABLE biodata ADD id INT(11) FIRST;``
![image](https://user-images.githubusercontent.com/115771479/229924635-f622f0ac-7525-4aa3-9d5e-c40585641669.png)

## 5. Menambahkan kolom phone setelah kolom alamat:
# ``ALTER TABLE biodata ADD phone VARCHAR(15) AFTER alamat;``
![image](https://user-images.githubusercontent.com/115771479/229924689-57741e36-0215-4408-a0d3-e3a5429f353b.png)

## 6. Mengubah tipe data kolom id menjadi char(11):
# ``ALTER TABLE biodata MODIFY id CHAR(11);``
![image](https://user-images.githubusercontent.com/115771479/229924736-dad897cd-0d6c-444d-bf89-7eeebb86fba9.png)

## 7. Mengubah nama kolom phone menjadi hp (varchar 20):
# ``ALTER TABLE biodata CHANGE phone hp VARCHAR(20);``
![image](https://user-images.githubusercontent.com/115771479/229924778-52bf91d2-c177-4fc8-8f06-ce6d9a0e33ab.png)

## 8. Menambahkan kolom email setelah kolom hp:
# ``ALTER TABLE biodata ADD email VARCHAR(15) AFTER hp;``
![image](https://user-images.githubusercontent.com/115771479/229924840-fc208b6d-1b76-4ea2-bdbf-3b96d30c5aa6.png)

## 9. Menghapus kolom keterangan:
# ``ALTER TABLE biodata DROP COLUMN keterangan;``
![image](https://user-images.githubusercontent.com/115771479/229924870-98e06689-9b9f-4463-ad65-97c58daf071f.png)

## 10. Mengganti nama tabel menjadi data_mahasiswa:
# ``ALTER TABLE biodata RENAME TO data_mahasiswa;``
![image](https://user-images.githubusercontent.com/115771479/229924911-17f9d966-0c72-4a76-9cce-7b10ffe01844.png)

## 11. Mengganti nama field id menjadi nim:
# ``ALTER TABLE data_mahasiswa CHANGE id nim CHAR(11);``
![image](https://user-images.githubusercontent.com/115771479/229924957-0196bda8-ad3a-4d8f-9e02-3a4d7a1ef278.png)

## 12. Menjadikan nim sebagai PRIMARY KEY:
# ``ALTER TABLE data_mahasiswa ADD PRIMARY KEY (nim);``
![image](https://user-images.githubusercontent.com/115771479/229924997-bff61b23-f7d0-40b8-9275-2d2a481017bd.png)

## 13. Menjadikan kolom email sebagai UNIQUE KEY:
# ``ALTER TABLE data_mahasiswa ADD UNIQUE KEY (email);``
![image](https://user-images.githubusercontent.com/115771479/229925043-3a28d5c6-c33a-47a9-8e8e-ebf423ef29e3.png)

## HASIL OUTPUT AKHIR
![Screenshot (67)](https://user-images.githubusercontent.com/115771479/228744899-3b91276a-ea63-494e-bc00-396e3c11b5a0.png)


- ## Apa maksud dari int (11)? Yang dimaksud int(11) artinya suatu data yang dipakai atau digunakan menggunakan tipe data int atau integer dengan length atau panjang karakter 11.

- ## Ketika kita melihat struktur tabel dengan perintah desc, ada kolom Null yang berisi Yes dan No. Apa maksudnya?  Apabila Null berisi no, maka data tersebut nantinya akan dilakukan pengisian atau penginputan. Sedangkan apabila Null berisi yes, maka artinya data tersebut akan dikosongkan atau tidak dilakukan penginputan.
