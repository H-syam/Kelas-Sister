melakukan instalasi microservice 3 debian 10 , microservice 4 debian 10 , microservice 5 debian 10


sudo lxc-create -n microservice3 -t download -- --dist "debian" --release "buster" –arch amd64

sudo lxc-create -n microservice4 -t download -- --dist "debian" --release "buster" –arch amd64

sudo lxc-create -n microservice5 -t download -- --dist "debian" --release "buster" –arch amd64

dengan mengisi Architecture : amd64

![1](https://github.com/H-syam/Kelas-Sister/assets/148841928/dfbb4aab-27c1-4377-a1dc-9aaebc1af3ab)

Setelah itu , menjalankan ketiga microservice yang baru di isntall 

lxc-start -n microservice3

lxc-start -n microservice4

lxc-start -n microservice5

![2](https://github.com/H-syam/Kelas-Sister/assets/148841928/438c39c1-5ede-4810-b843-c761e888b7c6)

Setelah berhasil dijalankan, sekarang pindah ke nano /etc/nginx/sites-enabled  untuk menambahkan ip baru yang bernama microservice3.dev

![3](https://github.com/H-syam/Kelas-Sister/assets/148841928/c53f6bfe-35ee-4b76-bf97-b678014eb6d6)

Lakukan hal yang sama  ke semua microservice yang baru 

![9](https://github.com/H-syam/Kelas-Sister/assets/148841928/1a9c9ebc-7579-475c-8c1e-e74cafd7cdbd)
![10](https://github.com/H-syam/Kelas-Sister/assets/148841928/8cb779c8-6a97-404f-896e-39bd4e79cacb)

melakukan konfig ke sudo nano /etc/nginx/sites-available/syam.local

![11](https://github.com/H-syam/Kelas-Sister/assets/148841928/e4030a33-6d91-4e38-8d74-4a511468b174)

setelah selesai,selanjutnya melakukan curl -i app syam.local untuk melihat konektivitas 

![8](https://github.com/H-syam/Kelas-Sister/assets/148841928/37ee4100-37ef-4344-a356-06f5ae3c0272)






