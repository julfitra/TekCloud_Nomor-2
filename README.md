# Praktikkan Menggunakan Containerd

## Langkah-Langkah Praktikum Containerd

1. Instalasi containerd:
   **Di Ubuntu/Debian:**
   - sudo apt-get update

     ![alt](images/image-1.png)  

   - sudo apt-get install -y containerd

     ![alt](images/image-2.png)  

3. Konfigurasi containerd
   **Untuk membuat konfigurasi default, jalankan**
   
   - containerd config default > /etc/containerd/config.toml

     ![alt](images/image-3.png)  

5. Mulai dan Aktifkan containerd
   **Jalankan dan aktifkan layanan containerd:**
   - sudo systemctl start containerd
  
     ![alt](images/image-4.png)  
     
   - sudo systemctl enable containerd

     ![alt](images/image-5.png)

6. Menjalankan dan Mengelola Container
   **Gunakan perintah ctr untuk menarik image dari Docker Hub sebelum menjalankannya**
   - sudo ctr image pull docker.io/library/alpine:latest

     ![alt](images/image-6.png)

   **Setelah image berhasil di-pull, coba jalankan container kembali:**
   - sudo ctr run --rm -t docker.io/library/alpine:latest mycontainer /bin/sh

     ![alt](images/image-7.png)

7. Verifikasi Containerd
   **Untuk memeriksa status containerd dan container yang berjalan**
   - sudo ctr containers list dan sudo ctr tasks list

     ![alt](images/image-8.png)
