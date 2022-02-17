# How to run a docker nodejs app and host it
## Installation
1. First run `sudo groupadd docker`.
2. Then run `sudo usermod -aG docker $USER`
3. Go to [Docker](https://docs.docker.com/engine/install/ubuntu/) and install docker.
4. Go to [Caddy](https://caddyserver.com/docs/install#debian-ubuntu-raspbian) and install the webserver.
5. Create a nodeJS app.
6. Create and upload the image to docker hub or an other repo.
7. Now pull the image on your server.
	1. Might have to run `docker login`
8. Now `docker run -p yourport:containerport yourimage`.
9. Go to `/etc/caddy` and edit the `Caddyfile`.
10. Comment out the default config and add the following:
```
YOURDOMAIN.com {
	reverse_proxy localhost:YOURPORTNUMBER
}
```
11. Now run `caddy start`.
12. Now run `caddy reload`.