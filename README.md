sudo docker build -t devops-app .
sudo docker run -d \
  --name devops-app \
  -p 8001:3000 \
  devops-app
  docker compose up -d --build