# php
# Setup Docker Para Projetos com PHP, MySQL, Nginx e PHPMyadmin

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
DB_DATABASE=nome_que_desejar_db
DB_ROOT_USERNAME=root
DB_USERNAME=root
DB_PASSWORD=root
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
