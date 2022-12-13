# Setup Docker para projetos com: PHP, MySQL, Nginx e phpMyAdmin.

Clone Repositório
```sh
git clone https://github.com/wwanzeller/php.git php
```

```sh
cd php/
```

Remova o versionamento
```sh
rm -rf .git/
```


Crie o Arquivo .env
```sh
cp .env.example .env
```


Atualize as variáveis de ambiente do arquivo .env
```dosini
DB_DATABASE=nome_que_desejar
DB_ROOT_PASSWORD=root
DB_PASSWORD=sua_senha
DB_USERNAME=seu_nome
```


Suba os containers do projeto
```sh
docker-compose up -d
```


Acessar o container
```sh
docker-compose exec app bash
```


Instalar as dependências do projeto
```sh
composer install
```


Acesse o projeto
[http://localhost](http://localhost)

Acesse o phpMyAdmin:
[http://localhost:8080](http://localhost:8080)
```dosini
servidor=mysql
Utilizador=root
Senha=root
```
ou

```dosini
servidor=mysql
Utilizador=seu_nome
Senha=sua_senha
```
