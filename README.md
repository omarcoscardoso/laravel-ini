# Laravel Docker Linux

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