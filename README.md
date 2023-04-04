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

## 1. Membuat Data Base Lathian1

![image](https://user-images.githubusercontent.com/115771479/229927909-f167b637-2226-41c0-80ce-e802998dc382.png)

## 2. Membuat Tabel
- ``CREATE TABLE siswa (nama VARCHAR(100),alamat TEXT);``
 
![image](https://user-images.githubusercontent.com/115771479/229928072-d756fe74-cc49-46ac-b96b-2800e1bfdc05.png)

## 3. Menambahkan Kolom Di Awal
- ``ALTER TABLE siswa ADD COLUMN id INT FIRST;``
 
![image](https://user-images.githubusercontent.com/115771479/229929010-a24d5d02-8e78-4757-8d0b-c57901582c6d.png)

## 4. Mengubah Nama Kolom
- ``ALTER TABLE siswa CHANGE keterangan kelas VARCHAR(10);``
 
![image](https://user-images.githubusercontent.com/115771479/229929193-ed8f6bd3-9cf0-4487-916a-eaed4b66e454.png)

## 5. Mengubah Tipe Data
- ``VARCHAR(10) menjadi VARCHAR(11)``
  
![image](https://user-images.githubusercontent.com/115771479/229929345-d0561a80-8933-4aec-8542-ecdc855aefda.png)

## 6. Menghapus Kolom
- ``ALTER TABLE siswa DROP COLUMN kelas;``
 
![image](https://user-images.githubusercontent.com/115771479/229929478-5b4f1e01-b7fd-41fc-8146-963d3e4fadbf.png)

## 7. Menambahkan Primary Key Id
- ``ALTER TABLE siswa ADD PRIMARY KEY(id);``
 
![image](https://user-images.githubusercontent.com/115771479/229929640-f838078a-a4e7-4aaa-8e50-aaf984c144f6.png)

## 8. Menghapus Primary Key
- ``ALTER TABLE siswa DROP PRIMARY KEY;``
 
![image](https://user-images.githubusercontent.com/115771479/229930034-34a80d69-63b8-4cc5-87fb-7fabfaef4c9b.png)

## 9. Menambahkan Constraint
- ``ALTER TABLE siswa ADD CONSTRAINT PK_siswa PRIMARY KEY(id);``
 
![image](https://user-images.githubusercontent.com/115771479/229930080-0dd58949-f2fe-4daf-861e-ecb635edb46e.png)

## 10. Menghapus Constraint Primary Key juga Bisa Seperti Ini:
- ``ALTER TABLE siswa DROP PRIMARY KEY;``
 
![image](https://user-images.githubusercontent.com/115771479/229930346-04e3844a-4a2e-4b16-a341-0033fcbf862f.png)
