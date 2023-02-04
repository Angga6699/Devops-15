![Screenshot from 2023-02-04 15-55-13](https://user-images.githubusercontent.com/111972023/216759730-d92513dd-4ae9-4360-94ed-9fb3d5613aea.png)



![Screenshot from 2023-02-04 15-55-14](https://user-images.githubusercontent.com/111972023/216759735-3ed9dc15-b59f-4f7d-ab16-afbb42c4562f.png)



![Screenshot from 2023-02-04 15-55-15](https://user-images.githubusercontent.com/111972023/216759739-f47a6d00-c9b4-454e-9be3-dfb49e96b055.png)



sudo apt install mysql-server


![34](https://user-images.githubusercontent.com/111972023/216759780-d691f42a-1353-44cc-8608-6a6d447af2c6.png)


sudo mysql -u root


![35](https://user-images.githubusercontent.com/111972023/216759792-8ac4f9f9-591a-4fe1-840c-a990a3b92381.png)


Memberikan Password Kepada User Sudo Atau Root


![36](https://user-images.githubusercontent.com/111972023/216759825-92050af0-7704-4382-97fd-eef5a26ed2b6.png)

Membuat User Baru Dan Password




![37](https://user-images.githubusercontent.com/111972023/216759869-59314c54-1426-4bfb-a6c5-44240e555870.png)



Memberikan Semua Akses Ke User Baru Yang Tadi Dibuat



![38](https://user-images.githubusercontent.com/111972023/216759905-5f5290c2-05bf-4666-b528-c389a9791e66.png)



sudo mysql -u angga -p

Dan Buat Database Baru Namakan Dengan dbwayshub



![39](https://user-images.githubusercontent.com/111972023/216759948-b0458eb5-5055-4533-804f-eb445baa5e0a.png)


Melihat Databases

show databases;


![40](https://user-images.githubusercontent.com/111972023/216759981-05b03458-498c-4da9-9604-1df927ff275c.png)




Masuk Ke Database dbwayshub Dan Melihat isi Databasenya

use dbwayshub;

show tables;



![41](https://user-images.githubusercontent.com/111972023/216760050-08f995b3-b763-4d40-b4b4-8157ff1e108d.png)




Set Up Backend



Git Clone wayshub-backend


![42](https://user-images.githubusercontent.com/111972023/216760123-cc8f5176-7db2-46c1-8ddc-0c0219b5b3b6.png)




Untuk Migrasi Database Dari Backend Ke Database Mysql



![43](https://user-images.githubusercontent.com/111972023/216760181-1bd0956e-5e64-495b-86f5-d8dcd52796aa.png)



![44](https://user-images.githubusercontent.com/111972023/216760190-907c95c2-c42e-4d0d-8ac2-e44b95c5fd4f.png)


Untuk Bisa Migrasi Database Dari Backend Ke Database Mysql Harus Menggunakan sequelize


npm install -g sequelize-cli



![45](https://user-images.githubusercontent.com/111972023/216760270-6802a37d-026f-4f9d-a3db-79103776da82.png)





sequelize db:migrate




![46](https://user-images.githubusercontent.com/111972023/216760288-a41560ed-7559-4d4f-902f-a3e073d4fd19.png)



Melihat Hasil Migrasi Dari Backend Ke Mysql, Menggunakan sequelize-cli



![47](https://user-images.githubusercontent.com/111972023/216760344-1e1a3cf7-b4ff-4f5e-b738-cc11e82f59a6.png)



Menjalankan Backend Wayshub Dengan Menggunakan PM2



![48](https://user-images.githubusercontent.com/111972023/216760393-e2eddf0b-221f-4ff3-a832-a0c54d27f117.png)




![49](https://user-images.githubusercontent.com/111972023/216760401-e1de1304-3dfa-4d26-9a2b-64f016eed35a.png)




Challange : UFW Enable





![50](https://user-images.githubusercontent.com/111972023/216760423-d3e76ffd-635e-4e88-b699-d65afd2268ea.png)





Supaya Website Tadi Menjadi Lebih Aman Dan Menjadi https, Menggunakan Certbot


sudo apt-get update



![51](https://user-images.githubusercontent.com/111972023/216760478-e2c3c672-1b6b-47aa-bf7f-56fae32f42f6.png)


Set Up Certbot



![52](https://user-images.githubusercontent.com/111972023/216760513-30310436-02d8-46a3-b948-2fe541bc2572.png)




![53](https://user-images.githubusercontent.com/111972023/216760527-19ea8283-f750-41b2-b0ad-9e5156e7de30.png)





![54](https://user-images.githubusercontent.com/111972023/216760539-a04ee216-a7f4-412b-9d13-3cff2ae52909.png)






![55](https://user-images.githubusercontent.com/111972023/216760551-394be5fc-aa95-46e8-8fcf-d84a765f7b58.png)

