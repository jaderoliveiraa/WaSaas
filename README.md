# WaSaas
Wha Saas

- Atualizar dependencias do linux
	
	apt update && apt upgrade

- Instalar o NodeJs

	curl -fsSL https://deb.nodesource.com/setup_14.x | sudo -E bash - &&\
sudo apt-get install -y nodejs

- Instalar o Docker

	apt install docker.io

- Instalar o Redis (docker)
	
	sudo docker run --name redis-container --restart always -d redis

- Instalar o Postgresql (docker)

	sudo docker run --name database -e POSTGRES_PASSWORD=45597ac534d8c5c35749bbe5dab551 -p 5432:5432 --restart always -d postgres

- Criar o Banco de Dados (Postgresql)

	docker exec -it database /bin/bash
	su postgres
	psql
	CREATE DATABASE whatsapp;

- Configurar a conexão com o banco no arquivo .env, seguir o .env-example como referência
- Configurar conexão com Redis
- Rodar as Migrations
- Rodar os Seeds
- Subir o Sistema


--- Adicionais Vps --

- Configurar o Nginx Proxy
	apt install nginx
- Configurar o Let's Encrypt Ssl
- Configurar o Pm2


---------------------------------
