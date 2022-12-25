Nguyễn Minh Nhựt - 20110534


Nguyễn Thị Thu Hoài - 2011091


Dương Tôn Phát  - 20110486

# Hướng Dẫn Cài Đặt

truy cập vào terminal của ec2


![image](https://user-images.githubusercontent.com/118672271/209454318-a0e2771e-1040-4e28-aa60-662133323d7d.png)

chạy các lệnh sau để cài đặt môi trường

sudo apt-get update

sudo apt-get upgrade

sudo apt-get install \

  apt-transport-https \
  
 	ca-certificates \
  
 	curl \
  
 	gnupg-agent \
  
 	software-properties-common

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -

sudo apt-get install docker-ce docker-ce-cli containerd.io

apt-cache madison docker-ce

sudo apt-get install docker-ce docker-ce-cli containerd.io

sudo apt install docker.io

sudo apt install docker-compose

# sau khi cài đặt môi trường xong ta clone code từ github về

git clone	https://github.com/Luciferidabet/web-code_DTDM

# truy cập vào thư mục

cd web-code_DTDM

# chạy lệnh docker để build images

docker build -t cd web-code_DTDM .

# chạy docker images vừa tạo

docker run -p 8080:80 web-code_DTDM

# sau đó ta mở web với port 8080

![image](https://user-images.githubusercontent.com/118672271/209454420-46a1a419-0968-42ea-bc8d-621901e865d8.png)


