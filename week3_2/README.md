# Web Server dan load balancing

Web Server adalah sebuah software yang memberikan layanan berupa data. Berfungsi untuk menerima permintaan HTTP atau HTTPS dari client atau di kenal dengan web browser (chrome atau firefox). Kemudian web server akan mengirimkan respon atas permintaan tersebut dalam bentuk halaman web.

saya bikin proxy seperti ini

server {
    listen 80;
    server_name ramadhanhirmawan.xyz;

    location / {
        proxy_pass http://localhost:3000;
        proxy_set_header Host $host;
        proxy_set_header X-Real-IP $remote_addr;
        proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
    }
}

cd dumbways
sudo nano my.reverse-proxy.conf masukan konfigurasi diatas
cd ..
sudo nano nginx.conf tambahkan di ###virual hosts config tambahkan include /etc/nginx/dumbways/*
sudo nginx -t
sudo systemctl restart nginx
sudo nano /etc/hosts masukkan ip
git clone https://github.com/dumbwaysdev/dumbflix-frontend.git
lalu buka terminal baru
cd dumbflix-frontend
npm install
npm start


Load Balancing adalah suatu jaringan komputer yang menggunakan metode untuk mendistribusikan beban kerjaan pada dua atau bahkan lebih suatu koneksi jaringan secara seimbang agar pekerjaan dapat berjalan optimal dan tidak overload (kelebihan) beban pada salah satu jalur koneksi.
