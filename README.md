sudo docker build -t devops-app .
sudo docker run -d \
  --name devops-app \
  -p 8001:3000 \
  devops-app
    sudo docker compose down --remove-orphans
  docker compose up -d --build



  <!-- Install docker compose -->
  sudo mkdir -p /root/.docker/cli-plugins/
sudo cp ~/.docker/cli-plugins/docker-compose /root/.docker/cli-plugins/
sudo chmod +x /root/.docker/cli-plugins/docker-compose


<!-- SSL -->
sudo yum update -y
sudo yum install -y certbot
sudo systemctl stop nginx
sudo certbot certonly --standalone \
-d api.baobui.click \
-d baobui.click

sudo systemctl start nginx