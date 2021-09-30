# AWS Servidor PHP com Laravel Framework - http://54.94.195.88/LaravelSalaminha/public/   - will be www.salaminha.com
WebSite with Laravel Framework, PHP, CSS, HTML, JQuery - hosted in Cloud AWS with EC2(Webserver Apache Free), RDS (MySQL).
- Criada EC2 Micro Instance Linux Ubuntu  
- Srv http://54.94.195.88 
- LAravel OK Endereço http://54.94.195.88/LaravelSalaminha/public/
# TO install Laravel, PHP, Apache
```
sudo su
apt-get update
apt-get instal php7.4 apache2
apt install libapache2-mod-php php-mbstring php-xmlrpc php-soap php-gd php-xml php-cli php-zip php-bcmath php-tokenizer php-json php-pear
```

- Composer

```
cd ~
curl -sS https://getcomposer.org/installer | 
php
mv composer.phar /usr/local/bin/composer
ln -s /usr/local/bin/composer /usr/bin/composer
```

- Apos instalado ir para www e criar o Projeto Laravel
```
composer create-project laravel/laravel LaravelSalaminha --prefer-dist
```
- No projeto criado permit Storage
```
 chmod -R 777 storage
 a2enmod rewrite
 service apache2 restart
```
> SUCESSO !! 30/09/21

- Proximo passo subir os fontes do Site...
