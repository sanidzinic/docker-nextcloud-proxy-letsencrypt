# docker-nextcloud-proxy-letsencrypt
This is a personal docker-compose.yml file that I use for the following components:

* Nextcloud (31.0.0-apache)
* Redis
* Nextcloud-DB
* Cron
* Web proxy (nginx-proxy:alpine)
* Let's Encrypt companion for automatic renewal of SSL certificates

The compose file creates six volumes to separate the web UI, database, and other components.
The main reason for using a web proxy is that I am running this Docker container on a Raspberry Pi and using multiple subdomains for the same Docker host.
