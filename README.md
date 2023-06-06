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
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/503135d2-e4d2-4370-bae2-0e8e96030be8)


### Tabel KrsMahasiswa
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/764a3e4d-52da-47d3-aeda-6b81f1cb4c2a)

### Tabel JadwalMengajar
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/4518a687-6ddb-412c-891a-21e0b875f716)

### Tabel Matakuliah
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/d740a057-aabe-4b17-ac43-8d636f975741)


# LATIHAN

1 Lakukan join table Mahasiswa dan Dosen
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/72de578b-c05a-459e-9a57-85018595b85e)


2 Lakukan join tabel Matakuliah dan Dosen
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/365b67e3-2d0b-4173-ad7e-bdceb616b89a)

```
Pada kode ini hasilnya tabel dosen null karena kedua tabel tidak saling ber relasi
```


3 Lakukan join table JadwalMengajar, Dosen, dan Matakuluan
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/97819e83-8f76-497c-89b7-af66e53d5358)


4 Lakukan join tabel KrsMahasiswa, Mahasiswa, Matakuliah, dan Dosen
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/5acb7b13-f974-454f-ade7-ff31e6ca05c0)

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
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/63e233ee-f79b-4f7a-9312-ddff92fe489c)


3. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu'
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```

![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/4fba4278-5731-4941-a0f0-1332a75c1393)

4. JOIN table JadwalMengajar, Dosen, dan Matakuliah
```
SELECT jadwalMengajar.kd_mk, matakuliah.nama AS 'Mata kuliah', matakuliah.sks, Dosen.nama AS 'Dosen Pengampu', jadwalMengajar.hari, jadwalMengajar.jam, jadwalMengajar.ruang
FROM jadwalMengajar
JOIN Dosen ON jadwalMengajar.kd_ds = Dosen.kd_ds
JOIN matakuliah ON jadwalMengajar.kd_mk = matakuliah.kd_mk;
```
![image](https://github.com/riskibowo/PRAKTIKUM_5/assets/115862112/2752e027-1b86-46ef-8bf6-f7088656cc06)

[basisdata.pdf](https://github.com/riskibowo/PRAKTIKUM_5/files/11661245/basisdata.pdf)
