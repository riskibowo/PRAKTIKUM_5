# PRAKTIKUM_5
```
Latihan
1 Lakukan join table Mahasiswa dan Dosen
2 Lakukan join tabel Matakuliah dan Dosen
3 Lakukan join table JadwalMengajar, Dosen, dan Matakuluan
4 Lakukan join tabel KrsMahasiswa, Mahasiswa, Matakuliah, dan Dosen
```
### Tabel Mahasiswa
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/b1a74894-13fa-46af-a25f-aad99267fa41)


### Tabel Dosen
![dosen](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/e73130cc-78b6-4b2d-ac9b-8c3c08590d13)

### Tabel KrsMahasiswa
![krs](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/9ada5183-534f-4f6e-8f5f-0cc3e7a98058)

### Tabel JadwalMengajar
![jadwal](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/56c3847c-cc7a-4372-9fa1-6957ebb49c89)

### Tabel Matakuliah
![matkul](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/798ba69c-0376-4049-a8c8-b2d7c393faf4)

# LATIHAN

1 Lakukan join table Mahasiswa dan Dosen
![tg1](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/2014b9f4-5535-46a6-bb23-13092d4dc9c8)


2 Lakukan join tabel Matakuliah dan Dosen
![tg2](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/1ee85568-d73c-4571-8797-02df3bd907a2)
```
Pada kode ini hasilnya tabel dosen null karena kedua tabel tidak saling ber relasi
```


3 Lakukan join table JadwalMengajar, Dosen, dan Matakuluan
![tg3](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/2abdbb33-7af2-4631-a508-b1c1d65bfde2)


4 Lakukan join tabel KrsMahasiswa, Mahasiswa, Matakuliah, dan Dosen
![tg4](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/7b5a1c72-176d-46e7-b63f-7c6d29d74972)

# LATIHAN

1. JOIN table Mahasiswa dan Dosen
```
SELECT Mahasiswa.nim, Mahasiswa.nama, Mahasiswa.jenis_kelamin, Dosen.nama AS 'Dosen' 
FROM Mahasiswa 
JOIN Dosen ON Dosen.kd_ds=Mahasiswa.kd_ds;
```
![vs1](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/7ae17c02-9129-43ac-85ae-789e08268952)


2. LEFT JOIN table Mahasiswa dan Dosen
```
SELECT Mahasiswa.nim, Mahasiswa.nama, Mahasiswa.jenis_kelamin, Dosen.nama AS 'Dosen'
FROM Mahasiswa
LEFT JOIN Dosen ON Dosen.kd_ds=Mahasiswa.kd_ds;
```
![vs2](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/d85a9a75-cbe1-4b7f-98da-f8305ac007a8)


3. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu'
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```
![vs3](https://github.com/DimasF3009/Basis-Data-Praktikum-5/assets/115356128/cc7cddcb-85fe-460d-b3af-91e00c6bcdf4)


4. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu', jadwalMengajar.hari, jadwalMengajar.jam, jadwalMengajar.ruang
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```
[basisdata.pdf](https://github.com/riskibowo/PRAKTIKUM_5/files/11661245/basisdata.pdf)
