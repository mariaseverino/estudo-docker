sudo docker run -ti ubuntu:22.04 - pra executar comandos no terminal
docker rmi hello-world - remove image
docker rmi hello-world -f - remove image
docker rm id && docker rmi hello-world - remove image
docker run -d nginx:1.19.10-alpine - nao prende terminal
docker logs id
docker run -d -p 8000:80 -v $(pwd):/usr/share/nginx/html nginx:1.19.10-alpine
docker run -d -v $(pwd):/home/node/app -p 8000:3000 imagem-node
docker exec -it a33 /bin/bash
docker image ls | grep imagem-node
docker build -t imagem-node-prod -f Dockerfile.prod .
docker build -t mariaseverino/imagem-node-prod -f Dockerfile.prod . - se eu tivese conta no docker hub pra subir a imagem **faz novo build se quiser atualizar**
docker push mariaseverino/imagem-node-prod - pegar minha imagem criada
docker run -p 8000:3000 mariaseverino/imagem-node-prod - roda minha aplicação

docker compose --biuld

<!-- ter um arquivo dockerfile -->

sudo docker build -t meu-ubuntu .
sudo docker run -ti meu-ubuntu

<!-- ter um arquivo Dockerfile_nginx -->

sudo docker build -t meu-app -f Dockerfile_nginx .
sudo docker run -d -p 8080:80 meu-app

sudo docker ps
sudo docker ps -a - nap precisa do sudo
sudo docker stop [id]

sudo service docker start - deu erro no daemon

docker image ls - lista as minha imagens

---

google cloud run
