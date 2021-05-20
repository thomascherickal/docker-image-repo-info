<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `teamspeak`

-	[`teamspeak:3.13`](#teamspeak313)
-	[`teamspeak:3.13.5`](#teamspeak3135)
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

## `teamspeak:3.13.5`

```console
$ docker pull teamspeak@sha256:83c4faf5d30732911ddc2d3e39bda41355937b3ba96770c8767d18ce0ce17269
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:3.13.5` - linux; amd64

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
