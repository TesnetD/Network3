node Network 3 di VPS dengan spesifikasi minimal 1CPU/2GB RAM/60GB SSD menggunakan Ubuntu 22.04:

1. Persiapan VPS
Update dan upgrade sistem:

sudo apt update && sudo apt upgrade -y
Install tools yang dibutuhkan:

sudo apt install -y screen net-tools
Catatan: Jika diminta untuk restart proses, pilih opsi terakhir: "No of them."
2. Instalasi Network 3 Node
Unduh file instalasi:

wget https://network3.io/ubuntu-node-v2.1.0.tar
Ekstrak file dan masuk ke folder:

tar -xvf ubuntu-node-v2.1.0.tar
rm -rf ubuntu-node-v2.1.0.tar
cd ubuntu-node
3. Menjalankan Node
Buat session baru di screen:

screen -S network3
Jalankan node:

sudo bash manager.sh up
Salin API Key:

sudo bash manager.sh key
4. Hubungkan Node dengan Browser
Buka URL yang muncul setelah menjalankan node:

https://account.network3.ai/main?o=xx.xx.xx.xx:8080
(Ganti xx.xx.xx.xx dengan IP server VPS Anda).
Klik tombol “+”, tempelkan API Key, lalu klik OK.
5. Jika Tombol + Tidak Muncul
Stop instalasi:

sudo bash manager.sh down
Buka port 8080:

sudo ufw allow 8080/tcp
Jalankan kembali node:

sudo bash manager.sh up
6. Screen Management
Keluar dari screen tanpa menghentikan proses:

CTRL+A, D
Kembali ke screen:

screen -r network3
Selesai. Node sudah siap berjalan!
