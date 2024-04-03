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




