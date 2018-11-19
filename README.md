# Laravel com Docker

Ambiente de desenvolvimento Laravel com Docker

- PHP 7.2-fpm
- MariaDB 10.1
- Redis 5.0.1-alpine
- Nginx 1.15.6-alpine
- phpMyAdmin 4.8.3

**Atenção**: Você precisa instalar o Docker e logar em sua conta antes de iniciar o ambiente. Docker oferece suporte para os principais sistemas operacionais do mercado. Site oficial do Docker https://www.docker.com/get-started.

### Passo a passo
1. Instale o Docker e certifique de estar em execução. Digite o comando docker -v no terminal.
2. Clone o repositório tiagoandre/laravel-docker
3. Acesse a pasta do repositório e execute o comando cp .env.example .env
4. Abra o arquivo .env e defina todas configurações.
5. Abra o arquivo docker.conf em docker/nginx/vhosts e altere o domínio  em server_name. 
6. Abra o arquivo hosts e adiconar a linha 127.0.0.1 seguido pelo mesmo nome adicionado no passo anterior. 
7. Agora no terminal digite docker-compose up -d e os containers serão criados. Esse processo pode demorar um pouco dependendo da velocidade da sua internet. 
8. Acesse a pasta projects onde já possui uma instalação do Laravel 5.7 e execute o comando composer install.
