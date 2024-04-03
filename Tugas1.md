# Kelas-Sister

# Sebelumnya kita sudah melakukan instalasi Instalasi vm https://ciperx.com/install-ubuntu-server/ storage 35GB 
# Dan juga melakukan persiapan Persiapan Server host 

 setelah itu kita memulai melakukan Install lxc sesuai dari record dan referensi yang telah diberikan 

  sudo apt-get install lxc lxctl lxc-templates net-tools  
![1 St](https://github.com/H-syam/Kelas-Sister/assets/148841928/9b82c127-ac58-411d-abde-7b9fee14d558)

Selanjutnya untuk menampilkan  template container yang tersedia

sudo ls /usr/share/lxc/templates/
![2st](https://github.com/H-syam/Kelas-Sister/assets/148841928/0ac67a78-731c-441c-a3a2-b4bd85474666)

Setelah itu melakukan berbagai langkah yang diberikan melalui records , mulai dari menginstall nginx extras 
![3st](https://github.com/H-syam/Kelas-Sister/assets/148841928/a90371c5-f811-4d9a-9753-cbf6c2a14cef)

Melakukan konfig server di etc/nginx/sites-enabled 
![5](https://github.com/H-syam/Kelas-Sister/assets/148841928/2e57d971-5211-4bbc-b94f-b840ab636dd3)

Melakukan konfig pada index 
![6](https://github.com/H-syam/Kelas-Sister/assets/148841928/569abe6c-0184-4818-a903-82442f1daffd)

Setelah itu menambahkan server local baru (127.0.0.1 syam.local) melalui notepad dan menjalankan nya di browser 
![7](https://github.com/H-syam/Kelas-Sister/assets/148841928/099bfead-1048-42d3-ae63-07cd7fd80de4)


tugas selanjutnya melakukan instalasi microservice . dimulai dari 

sudo lxc-create -n microservice1 -t download -- --dist ubuntu --release focal --arch amd64 --force-cache --no-validate --server images.linuxcontainers.org 

sudo lxc-create -n microservice2 -t download -- --dist ubuntu --release bionic --arch amd64 --force-cache --no-validate --server images.linuxcontainers.org
![1](https://github.com/H-syam/Kelas-Sister/assets/148841928/99ee3c9a-ad4b-49d9-a663-3cc2e98b99a3)

melakukan install nano dan nginx di kedua mcsv 
![nano mv1-2](https://github.com/H-syam/Kelas-Sister/assets/148841928/1daecd73-9443-4c6a-b4c3-9fcb7692f64c)
![nginxsd1-2](https://github.com/H-syam/Kelas-Sister/assets/148841928/5e95fd65-8ce6-4316-a9fa-cbcc4d0fea55)

melakukan konfig index di setiap mcsv 
![index1-2](https://github.com/H-syam/Kelas-Sister/assets/148841928/8d75ab40-6111-40c8-bcc5-4b2ae5916e6a)

setelah mengatur ,dicek menggunakan curl 
![curl localhost1-2](https://github.com/H-syam/Kelas-Sister/assets/148841928/5dd28b95-d3bd-4625-9927-8293831c9184)

masuk ke dalam sudo nano /etc/netplan/10-lxc.yaml untuk mengatur ip dengan mengantikan sesuai ip setiap mcsv 
![mic2-1](https://github.com/H-syam/Kelas-Sister/assets/148841928/9aaac686-1ee0-4613-80f8-62a9ed9499e1)

setelah itu masuk ke nano /ect/hosts/ untuk menambahkan ip baru yaitu ip dari kedua mcsv 
![mcsv+](https://github.com/H-syam/Kelas-Sister/assets/148841928/f646351e-9a45-41ae-9462-e022611e009b)

melakukan test ping terhadap setiap ip mcsv untuk mengetahui konektivitas 
![testping 1-2](https://github.com/H-syam/Kelas-Sister/assets/148841928/ccdd7beb-69bd-44ce-bb63-031586ef96e5)

setelah ping terkoneksi,maka langsung bisa menggunakan syam.local/blog dan syam.local/aboutus di browser 
![mcsv1=](https://github.com/H-syam/Kelas-Sister/assets/148841928/4a1e8e31-41ec-4763-ba23-c82108140811)

![mcsv2=](https://github.com/H-syam/Kelas-Sister/assets/148841928/f8a563f4-d652-41b7-a0e3-7550e87d0e8a)












