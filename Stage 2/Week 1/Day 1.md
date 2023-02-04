![Screenshot from 2023-02-04 15-55-02](https://user-images.githubusercontent.com/111972023/216758453-1b866ec3-8066-45c0-b14f-0127f030e205.png)


![Screenshot from 2023-02-04 15-55-11](https://user-images.githubusercontent.com/111972023/216758496-52ae8f98-0c7c-48d9-9ac2-f06c8ea6855e.png)



<br>
<br>
<br>


# Set Up Wayshub

Sudo apt-get update

![](https://github.com/Angga6699/Devops-15/blob/main/Stage%202/Week%201/Poto%20Day%201%20Dan%20Day%202/1.png)


curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.1/install.sh | bash

![2](https://user-images.githubusercontent.com/111972023/216758753-ac6abdf6-1a93-41b8-b961-8b05823fd198.png)

exec bash

![3](https://user-images.githubusercontent.com/111972023/216758773-8b3c778d-d6f5-48f0-9cf8-3764b657364d.png)

nvm install 10

![4](https://user-images.githubusercontent.com/111972023/216758791-0a5b2906-8502-4133-bfa5-cf2480379866.png)


# Set Up pm2

1.npm install -g pm2


![5](https://user-images.githubusercontent.com/111972023/216758826-9dd8f51f-c02e-40fb-b92d-a27354c497f8.png)


2.git clone https://github.com/dumbwaysdev/wayshub-frontend.git


![6](https://user-images.githubusercontent.com/111972023/216758912-1a97722d-afab-40d6-b9cb-7f047b0a5f3e.png)

3.Masuk ke direktori lalu jalankan npm install
cd wayshub-frontend/
npm install


![7](https://user-images.githubusercontent.com/111972023/216758975-82a0c067-163a-445f-a654-4fb711d5c513.png)


4.Jalankan Perintah Berikut :
pm2 init simple



![8](https://user-images.githubusercontent.com/111972023/216758997-1d3cc6ec-4a47-4e01-b91a-992341b10cb8.png)


5.Edit file ecosystem lalu rubah bagian script menjadi npm start


![9](https://user-images.githubusercontent.com/111972023/216759024-398cabea-33dc-4bf4-aad5-8ac3ed4d8bc3.png)


5.Jalankan script dengan pm2
pm2 start ecosystem.config.js


![10](https://user-images.githubusercontent.com/111972023/216759059-61538c48-c675-495c-b254-aae791c52b45.png)


![11](https://user-images.githubusercontent.com/111972023/216759067-a8643fab-889e-4738-bded-54e8ff1bac69.png)


6.Akses Di Web Browser Menggunakan ip:3000(portnya)



![12](https://user-images.githubusercontent.com/111972023/216759089-d958069c-5236-4a3d-9db5-0bb1aec0f1e2.png)


Setup DNS Cloudflare


sudo apt-get update


![14](https://user-images.githubusercontent.com/111972023/216759163-d63e1366-e0f5-4bbc-a98d-ab0498bd9dee.png)



Buat file konfigurasi baru di folder /etc/nginx/appserver
sudo nano /etc/nginx/appserver/appserver.conf
Lalu isikan berikut


![15](https://user-images.githubusercontent.com/111972023/216759238-ed9854fb-fce1-4e06-b562-22e239750fd6.png)


![16](https://user-images.githubusercontent.com/111972023/216759252-2f71f5c0-afa8-40d6-a6f9-74bc75a633ed.png)


![17](https://user-images.githubusercontent.com/111972023/216759260-38a00eca-ee09-42e6-8f98-e6421c660c77.png)


sudo nginx -t


![18](https://user-images.githubusercontent.com/111972023/216759287-8be14f2f-1afe-4908-a003-80666d00b59c.png)

sudo systemctl reload nginx


![19](https://user-images.githubusercontent.com/111972023/216759333-9972d161-689c-4125-8c9c-64952ae7c93b.png)

