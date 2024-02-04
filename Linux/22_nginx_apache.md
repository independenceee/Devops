## Deploy web cơ bản với nginx

# install nginx

- sudo apt update
- sudo apt install nginx
- sudo ufw app list
- sudo ufw allow 'Nginx HTTP'
- sudo ufw status
- systemctl status nginx

# on off nginx service

- sudo service nginx restart
- sudo service nginx start
- sudo service nginx stop

# manager service

- sudo mkdir -p /var/www/demarket/html
- sudo chown -R $USER:$USER /var/www/demarket/html
- sudo chmod -R 755 /var/www/demarket
- sudo vim /var/www/demarket/html/index.html -> <h1>Hello</h1>

# create nginx 
- vim /etc/nginx/nginx.conf => Xem cấu hình 
- sudo vim /etc/nginx/sites-available/demarket
- sudo vim /etc/nginx/sites-enabled/demarket

```bash
server {
        listen 80;
        listen [::]:80;

        root /var/www/demarket/html;
        index index.html index.htm index.nginx-debian.html;

        server_name demarket.vn;

        location / {
                try_files $uri $uri/ =404;
        }
}
```



sudo cp /etc/nginx/sites-enabled/demarket  /etc/nginx/sites-enabled/demarket

sudo vi /etc/nginx/sites-enabled/demarket
```bash
server {
        listen 80;
        listen [::]:80;

        root /var/www/demarket/html;
        index index.html index.htm index.nginx-debian.html;

        server_name f8unbuntu.online;

        location / {
                try_files $uri $uri/ =404;
        }
}
```
- sudo nginx -t
- sudo service nginx reload



