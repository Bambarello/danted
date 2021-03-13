Dante SOCKS proxy server
====================

Usage
----
```sh
sudo apt-get remove -y docker docker-engine docker.io docker-compose && \
sudo apt install docker.io docker-compose -y && \
sudo systemctl start docker && \
sudo systemctl enable docker; \
git clone https://github.com/bambarello/danted.git; \
cd danted; \
nano Dockerfile; \
docker-compose build; \
docker-compose up -d; \
docker-compose logs -f
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
