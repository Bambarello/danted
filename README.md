Dante SOCKS proxy server
====================

Usage
----
```sh
$ git clone https://github.com/bambarello/danted.git
$ cd danted
$ nano Dockerfile
$ docker-compose build
$ docker-compose up
```

You can change username and password in docker-compose.yml

```sh
$ nano docker-compose.yml
```

Test
----
```sh
$ curl -x socks5://my_user:my_password@localhost:55555 ipinfo.io/ip
```
