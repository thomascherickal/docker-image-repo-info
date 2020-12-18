## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:068b42adcfbc07c236dbcaa95bc70f8f7fe680e4cba403b830f9fe91be046c48
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:c7ad687252ffaf779c72904d55fe1a527df186b7a39193139f6f63c28f182f97
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12787363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a115284467257e4d8d69c6b58cd15bea0d72f2cd1a27fcef9972db3badd8459`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 16:44:39 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Fri, 24 Apr 2020 16:44:40 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Fri, 24 Apr 2020 16:44:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Fri, 18 Dec 2020 06:54:15 GMT
ARG TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498
# Fri, 18 Dec 2020 06:54:15 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
# Fri, 18 Dec 2020 06:54:18 GMT
# ARGS: TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Fri, 18 Dec 2020 06:54:18 GMT
VOLUME [/var/ts3server/]
# Fri, 18 Dec 2020 06:54:18 GMT
WORKDIR /var/ts3server/
# Fri, 18 Dec 2020 06:54:18 GMT
EXPOSE 10011 30033 9987/udp
# Fri, 18 Dec 2020 06:54:19 GMT
COPY file:6f38f0bdd32398bda0227797278f67250720c9ff535447f0c53ae8d42a8789d0 in /opt/ts3server 
# Fri, 18 Dec 2020 06:54:19 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 18 Dec 2020 06:54:19 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a197d17e92a5c619f3c7a35bc157d4372aa57930455deaebe45c5f89f70e8a`  
		Last Modified: Fri, 24 Apr 2020 16:44:50 GMT  
		Size: 761.9 KB (761868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793f8f0f64a0bb76b2f05d88d886672db4fff7b804ee19ebfdbb99a4b692efdf`  
		Last Modified: Fri, 24 Apr 2020 16:44:51 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bff8daffce8ca9b0babf0e2a726ec3d0d8c864231bbb909f516ef2b5e451e84`  
		Last Modified: Fri, 18 Dec 2020 06:54:29 GMT  
		Size: 9.2 MB (9227044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a86e6884f27c91faa2c1cda6c7acb31c683b2549ea6a93c4bdd4fb96c14b96a`  
		Last Modified: Fri, 18 Dec 2020 06:54:28 GMT  
		Size: 1.6 KB (1571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
