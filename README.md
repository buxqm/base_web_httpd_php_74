# 基础镜像 WEB Httpd PHP 7.4

- L: Linux
- A: Apache Httpd
- P: PHP 7.4

## Example

TODO:

## Usage

### Conf

- apache /etc/apache2/
- php /usr/local/etc/php/php.ini

### ENV

- FLAG=ctfhub{httpd_php_74}

You should rewrite flag.sh when you use this image.
The `$FLAG` is not mandatory, but i hope you use it!

### Files

- src 网站源码
    + index.php
    + ...etc
- Dockerfile
- docker-compose.yml

### Dockerfile

```
FROM ctfhub/base_web_httpd_php_74

COPY src /var/www/html
COPY _files/flag.sh /flag.sh
```

