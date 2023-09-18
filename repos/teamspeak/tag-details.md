<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `teamspeak`

-	[`teamspeak:3.13`](#teamspeak313)
-	[`teamspeak:3.13.7`](#teamspeak3137)
-	[`teamspeak:latest`](#teamspeaklatest)

## `teamspeak:3.13`

```console
$ docker pull teamspeak@sha256:6abfca45862b69884b5a06b3ea118c58991790b57859a9aa1f44e7b5e4195ac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:3.13` - linux; amd64

```console
$ docker pull teamspeak@sha256:796b8d14b82b4d4768f65088c219f946f62496a398b4fcda33d62edaa3b4b351
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13970383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65abe2c015a966d727ed01915b2afbe89df18b58cfd29a2a42353f13d823244d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:21:50 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Mon, 18 Sep 2023 19:21:50 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
# Mon, 18 Sep 2023 19:21:53 GMT
# ARGS: TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Mon, 18 Sep 2023 19:21:53 GMT
VOLUME [/var/ts3server/]
# Mon, 18 Sep 2023 19:21:54 GMT
WORKDIR /var/ts3server/
# Mon, 18 Sep 2023 19:21:54 GMT
EXPOSE 10011 30033 9987/udp
# Mon, 18 Sep 2023 19:21:54 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Mon, 18 Sep 2023 19:21:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 18 Sep 2023 19:21:54 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377287b3e48277a20800ff7699f0e732b5050d9864e6e9bd93edb7d8a293ed50`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 MB (1316517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ceafc35bdd9a814760e29b1f7fa7b9697136fe02e0974516bb4813f32b5b6`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee766c1a8d91386bddb2e1e47495a75e71a9794d6fe8569340d84988c61a9ee1`  
		Last Modified: Mon, 18 Sep 2023 19:22:04 GMT  
		Size: 9.2 MB (9249357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e781a1defe6ef09012fda39546ad20e939f26173677d78d3ce9bd918bd0597`  
		Last Modified: Mon, 18 Sep 2023 19:22:02 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:3.13.7`

```console
$ docker pull teamspeak@sha256:6abfca45862b69884b5a06b3ea118c58991790b57859a9aa1f44e7b5e4195ac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:3.13.7` - linux; amd64

```console
$ docker pull teamspeak@sha256:796b8d14b82b4d4768f65088c219f946f62496a398b4fcda33d62edaa3b4b351
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13970383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65abe2c015a966d727ed01915b2afbe89df18b58cfd29a2a42353f13d823244d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:21:50 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Mon, 18 Sep 2023 19:21:50 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
# Mon, 18 Sep 2023 19:21:53 GMT
# ARGS: TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Mon, 18 Sep 2023 19:21:53 GMT
VOLUME [/var/ts3server/]
# Mon, 18 Sep 2023 19:21:54 GMT
WORKDIR /var/ts3server/
# Mon, 18 Sep 2023 19:21:54 GMT
EXPOSE 10011 30033 9987/udp
# Mon, 18 Sep 2023 19:21:54 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Mon, 18 Sep 2023 19:21:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 18 Sep 2023 19:21:54 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377287b3e48277a20800ff7699f0e732b5050d9864e6e9bd93edb7d8a293ed50`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 MB (1316517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ceafc35bdd9a814760e29b1f7fa7b9697136fe02e0974516bb4813f32b5b6`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee766c1a8d91386bddb2e1e47495a75e71a9794d6fe8569340d84988c61a9ee1`  
		Last Modified: Mon, 18 Sep 2023 19:22:04 GMT  
		Size: 9.2 MB (9249357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e781a1defe6ef09012fda39546ad20e939f26173677d78d3ce9bd918bd0597`  
		Last Modified: Mon, 18 Sep 2023 19:22:02 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:6abfca45862b69884b5a06b3ea118c58991790b57859a9aa1f44e7b5e4195ac0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:796b8d14b82b4d4768f65088c219f946f62496a398b4fcda33d62edaa3b4b351
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **14.0 MB (13970383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65abe2c015a966d727ed01915b2afbe89df18b58cfd29a2a42353f13d823244d`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:20 GMT
ADD file:32ff5e7a78b890996ee4681cc0a26185d3e9acdb4eb1e2aaccb2411f922fed6b in / 
# Mon, 07 Aug 2023 19:20:20 GMT
CMD ["/bin/sh"]
# Mon, 18 Sep 2023 19:21:50 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Mon, 18 Sep 2023 19:21:50 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e
# Mon, 18 Sep 2023 19:21:51 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
# Mon, 18 Sep 2023 19:21:53 GMT
# ARGS: TEAMSPEAK_CHECKSUM=359aac972679cfd98d62af51ddaf80e674cab166e13c6a835e81759097f9ba2e TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.7/teamspeak3-server_linux_alpine-3.13.7.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Mon, 18 Sep 2023 19:21:53 GMT
VOLUME [/var/ts3server/]
# Mon, 18 Sep 2023 19:21:54 GMT
WORKDIR /var/ts3server/
# Mon, 18 Sep 2023 19:21:54 GMT
EXPOSE 10011 30033 9987/udp
# Mon, 18 Sep 2023 19:21:54 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Mon, 18 Sep 2023 19:21:54 GMT
ENTRYPOINT ["entrypoint.sh"]
# Mon, 18 Sep 2023 19:21:54 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:7264a8db6415046d36d16ba98b79778e18accee6ffa71850405994cffa9be7de`  
		Last Modified: Mon, 07 Aug 2023 19:20:54 GMT  
		Size: 3.4 MB (3401613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377287b3e48277a20800ff7699f0e732b5050d9864e6e9bd93edb7d8a293ed50`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 MB (1316517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c58ceafc35bdd9a814760e29b1f7fa7b9697136fe02e0974516bb4813f32b5b6`  
		Last Modified: Mon, 18 Sep 2023 19:22:03 GMT  
		Size: 1.3 KB (1334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee766c1a8d91386bddb2e1e47495a75e71a9794d6fe8569340d84988c61a9ee1`  
		Last Modified: Mon, 18 Sep 2023 19:22:04 GMT  
		Size: 9.2 MB (9249357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e781a1defe6ef09012fda39546ad20e939f26173677d78d3ce9bd918bd0597`  
		Last Modified: Mon, 18 Sep 2023 19:22:02 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
