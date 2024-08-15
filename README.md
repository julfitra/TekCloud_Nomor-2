# Praktikkan Menggunakan Containerd

## Instalasi containerd

1. Menggunakan ubuntu:
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
