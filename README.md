sudo docker build -t devops-app .
sudo docker run -d \
  --name devops-app \
  -p 8001:3000 \
  devops-app
  docker compose up -d --build

  <!-- Install docker compose -->
  sudo mkdir -p /root/.docker/cli-plugins/
sudo cp ~/.docker/cli-plugins/docker-compose /root/.docker/cli-plugins/
sudo chmod +x /root/.docker/cli-plugins/docker-compose