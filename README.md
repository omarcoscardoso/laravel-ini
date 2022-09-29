<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center"> 

![license](https://img.shields.io/github/license/omarcoscardoso/eleicao-simples)
![license](https://img.shields.io/badge/LINUX-free-green)
![docker](https://img.shields.io/badge/Docker-dev-blue)

</p>

# Laravel Docker Linux

Pequeno projeto para facilitar o desenvolvimento inicial com Laravel usando docker. ​

## 🔨 Funcionalidades

- `Laravel`: Escolha a versão do Laravel que deseja usar
- `MySQL`: Já temos uma instância para banco de dados
- `Docker`: Sem comentários :-)

## Composer Install

```shell
cd www && \
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');" && \
php composer-setup.php && \
php -r "unlink('composer-setup.php');" && \
sudo mv composer.phar /usr/local/bin/composer
```

## Create Project Laravel

```shell
composer create-project --prefer-dist laravel/laravel:^8.0 laravel && \
chmod -R 777 laravel/storage && \
cd ..
```

## Docker up

```docker compose up -d```

## Finally Running in Browser

http://127.0.0.1:8080/
