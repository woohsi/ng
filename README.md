docker pull nginx
docker run -p 443:443 -p 80:80 -v ./nginx.conf:/etc/nginx/nginx.conf -v ./html:/usr/share/nginx/html -v ./log:/var/log/nginx --name ng -d nginx
