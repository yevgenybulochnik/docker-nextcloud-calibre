# Docker Nextcloud Calibre

This repository is a docker-compose setup for nextcloud and calibre using traefik as a proxy. It uses both calibre and calibre-web to manage books. The setup is completely local intended to be used with a VPN (wireguard).

## Env Vars

```
MYSQL_ROOT_PASSWORD    = nextcloudpass
MYSQL_PASSWORD         = nextcloudpass
MYSQL_DATABASE         = nextcloud
MYSQL_USER             = nextcloud
MYSQL_DATA             = /var/lib/mysql

NEXTCLOUD_URL          = local.nextcloud
NEXTCLOUD_STORAGE_PATH = /var/www/html

CALIBRE_URL            = local.calibre
CALIBRE_LIBRARY

CALIBRE_WEB_URL        = local.calibre-web
CALIBRE_WEB_CONFIG     = ./calibre-web-config
CALIBRE_WEB_LIBRARY
```

## References

### Docker Images
- [Traefik](https://hub.docker.com/_/traefik)
- [Docker-Socket-Proxy](https://hub.docker.com/r/tecnativa/docker-socket-proxy)
- [MariaDB](https://hub.docker.com/_/mariadb)
- [Nextcloud](https://hub.docker.com/_/nextcloud)
- [Calibre](https://hub.docker.com/r/linuxserver/calibre)
- [Calibre-Web](https://hub.docker.com/r/linuxserver/calibre-web)

### Documentation
- [Traefik]()
- [Docker-Socket-Proxy]()

### Articles
- [Nextcloud, Calibre, Moon Reader](https://itnext.io/calibre-web-home-in-browser-online-library-with-nextcloud-storage-and-moon-reader-on-android-bee6a30c15b9)
