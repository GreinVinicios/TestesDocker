Comandos docker

- Listar contineres rodando (asicionar -a para ver todos)
docker ps

- Limpar containeres que não estão rodando
docker container prune

- Listar imagens baixadas
docker images

- Remover imagens
/*
-f = forced
*/
rmi -f <id_container>

- Remover continer
/*
-f = forced
*/
rmi -f <id_container>

- Buildar uma imagem
/*
-f = file, nome do dockerfile
-t = tag, nome da tag
. = caminho onde está o dockerfile
*/
docker build -f books.dockerfile -t greinvinicios/books .

- Login no locker
docker login --username <user_name>

- Setar usuário do docker admin
sudo usermod -aG docker $USER

- Fazer upload de imagem
docker push greinvinicios/books


