<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `teamspeak`

-	[`teamspeak:3.13`](#teamspeak313)
-	[`teamspeak:3.13.3`](#teamspeak3133)
-	[`teamspeak:latest`](#teamspeaklatest)

## `teamspeak:3.13`

```console
$ docker pull teamspeak@sha256:83c4faf5d30732911ddc2d3e39bda41355937b3ba96770c8767d18ce0ce17269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:3.13` - linux; amd64

```console
$ docker pull teamspeak@sha256:148a9b628f72251818057b7def7e3a14de482fa3a9df3a3c25f8751c75df0325
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13481531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e2ede28f4f9d6ce17e6dcfed62e1e84bdc2ff8f4c5744859a63fd35038d06`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 19 May 2021 19:43:42 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Wed, 19 May 2021 19:43:43 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Wed, 19 May 2021 19:43:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Wed, 19 May 2021 19:43:43 GMT
ARG TEAMSPEAK_CHECKSUM=db70478d8b2d6358c0005504f1673e490ec0220b7ab93bdb418f0b051f4940aa
# Wed, 19 May 2021 19:43:44 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.5/teamspeak3-server_linux_alpine-3.13.5.tar.bz2
# Wed, 19 May 2021 19:43:46 GMT
# ARGS: TEAMSPEAK_CHECKSUM=db70478d8b2d6358c0005504f1673e490ec0220b7ab93bdb418f0b051f4940aa TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.5/teamspeak3-server_linux_alpine-3.13.5.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Wed, 19 May 2021 19:43:47 GMT
VOLUME [/var/ts3server/]
# Wed, 19 May 2021 19:43:47 GMT
WORKDIR /var/ts3server/
# Wed, 19 May 2021 19:43:47 GMT
EXPOSE 10011 30033 9987/udp
# Wed, 19 May 2021 19:43:47 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Wed, 19 May 2021 19:43:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 19 May 2021 19:43:48 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7233f76dfed8c4fa76c114eb1d6d47449b91bc6b5b7fda5acd707072e4a23`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.4 MB (1433301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e65b71b4286f1cebc0934f416d5a9b52ead3472a1fa6b19b3051886ba8c72`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9283f9c5ce87aade67744f1cd30d3b373845be9be328c2d4834c8aa986e28`  
		Last Modified: Wed, 19 May 2021 19:44:00 GMT  
		Size: 9.2 MB (9233376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cf66db51385a82e67ba5311fe3a6bd1512afdc00687f0ad5f5db1c7ea43c8`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:3.13.3`

```console
$ docker pull teamspeak@sha256:7a2acc19b86efa5f046c336a10c4e3085a1a1b42686ab2008927db6653549dca
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:3.13.3` - linux; amd64

```console
$ docker pull teamspeak@sha256:87effe781734e3b1989e90ea67ca493dbc6d6706cdc58307c463897c28fa2a9b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12788782 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ffb254ca337dbe23212ec04210d653736fa3e6ad9d10433df3a76498072a071`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Wed, 14 Apr 2021 19:20:04 GMT
ADD file:c5377eaa926bf412dd8d4a08b0a1f2399cfd708743533b0aa03b53d14cb4bb4e in / 
# Wed, 14 Apr 2021 19:20:05 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:31:33 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Wed, 14 Apr 2021 23:31:34 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Wed, 14 Apr 2021 23:31:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Wed, 14 Apr 2021 23:31:35 GMT
ARG TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498
# Wed, 14 Apr 2021 23:31:35 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
# Wed, 14 Apr 2021 23:31:37 GMT
# ARGS: TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Wed, 14 Apr 2021 23:31:37 GMT
VOLUME [/var/ts3server/]
# Wed, 14 Apr 2021 23:31:38 GMT
WORKDIR /var/ts3server/
# Wed, 14 Apr 2021 23:31:38 GMT
EXPOSE 10011 30033 9987/udp
# Wed, 14 Apr 2021 23:31:38 GMT
COPY file:6f38f0bdd32398bda0227797278f67250720c9ff535447f0c53ae8d42a8789d0 in /opt/ts3server 
# Wed, 14 Apr 2021 23:31:38 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 14 Apr 2021 23:31:38 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:396c31837116ac290458afcb928f68b6cc1c7bdd6963fc72f52f365a2a89c1b5`  
		Last Modified: Wed, 14 Apr 2021 19:21:14 GMT  
		Size: 2.8 MB (2798338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f10e8bac6a3791415a86d19944f0bf8cb190a38f8b85f2eca4af2d2ee65038`  
		Last Modified: Wed, 14 Apr 2021 23:31:49 GMT  
		Size: 760.5 KB (760474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a78863af2998f92432d1fa139da4bab8a877daa8f72f7cba11ef39927de346d`  
		Last Modified: Wed, 14 Apr 2021 23:31:49 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ed4f07c9c263f9e17c6def992417eec806c58a85eb06d3715df405769d74c0`  
		Last Modified: Wed, 14 Apr 2021 23:31:51 GMT  
		Size: 9.2 MB (9227058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e3bf7e36b7e000f231a4fd3e4dff481a15d4769dd29672aa740bdb15edcd39`  
		Last Modified: Wed, 14 Apr 2021 23:31:49 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:83c4faf5d30732911ddc2d3e39bda41355937b3ba96770c8767d18ce0ce17269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:148a9b628f72251818057b7def7e3a14de482fa3a9df3a3c25f8751c75df0325
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13481531 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b18e2ede28f4f9d6ce17e6dcfed62e1e84bdc2ff8f4c5744859a63fd35038d06`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 19 May 2021 19:43:42 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Wed, 19 May 2021 19:43:43 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Wed, 19 May 2021 19:43:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Wed, 19 May 2021 19:43:43 GMT
ARG TEAMSPEAK_CHECKSUM=db70478d8b2d6358c0005504f1673e490ec0220b7ab93bdb418f0b051f4940aa
# Wed, 19 May 2021 19:43:44 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.5/teamspeak3-server_linux_alpine-3.13.5.tar.bz2
# Wed, 19 May 2021 19:43:46 GMT
# ARGS: TEAMSPEAK_CHECKSUM=db70478d8b2d6358c0005504f1673e490ec0220b7ab93bdb418f0b051f4940aa TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.5/teamspeak3-server_linux_alpine-3.13.5.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Wed, 19 May 2021 19:43:47 GMT
VOLUME [/var/ts3server/]
# Wed, 19 May 2021 19:43:47 GMT
WORKDIR /var/ts3server/
# Wed, 19 May 2021 19:43:47 GMT
EXPOSE 10011 30033 9987/udp
# Wed, 19 May 2021 19:43:47 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Wed, 19 May 2021 19:43:47 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 19 May 2021 19:43:48 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4e7233f76dfed8c4fa76c114eb1d6d47449b91bc6b5b7fda5acd707072e4a23`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.4 MB (1433301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a0e65b71b4286f1cebc0934f416d5a9b52ead3472a1fa6b19b3051886ba8c72`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9283f9c5ce87aade67744f1cd30d3b373845be9be328c2d4834c8aa986e28`  
		Last Modified: Wed, 19 May 2021 19:44:00 GMT  
		Size: 9.2 MB (9233376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15cf66db51385a82e67ba5311fe3a6bd1512afdc00687f0ad5f5db1c7ea43c8`  
		Last Modified: Wed, 19 May 2021 19:43:58 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
