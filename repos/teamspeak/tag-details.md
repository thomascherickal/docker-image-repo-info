<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `teamspeak`

-	[`teamspeak:3.13`](#teamspeak313)
-	[`teamspeak:3.13.7`](#teamspeak3137)
-	[`teamspeak:latest`](#teamspeaklatest)

## `teamspeak:3.13`

```console
$ docker pull teamspeak@sha256:9bf4b1bd2b2bd507edb977be30a80d2f23b41ba190186c91cd2289f844444008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:3.13` - linux; amd64

```console
$ docker pull teamspeak@sha256:adb97ff3b3df49b50b728a33b82e91a415148fd05adbfba129bc75f58a7992cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13481650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad17fc34e34d87d4120a2e034e6d9d4600adfecce0d6026c07852a49206a9528`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:43:51 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Tue, 05 Apr 2022 09:43:51 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Tue, 05 Apr 2022 09:43:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Tue, 05 Apr 2022 09:43:51 GMT
ARG TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0
# Tue, 05 Apr 2022 09:43:52 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
# Tue, 05 Apr 2022 09:43:54 GMT
# ARGS: TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Tue, 05 Apr 2022 09:43:54 GMT
VOLUME [/var/ts3server/]
# Tue, 05 Apr 2022 09:43:54 GMT
WORKDIR /var/ts3server/
# Tue, 05 Apr 2022 09:43:54 GMT
EXPOSE 10011 30033 9987/udp
# Tue, 05 Apr 2022 09:43:54 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Tue, 05 Apr 2022 09:43:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 09:43:55 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e2a3e53f7b63d3b584a2f90666a9bf53058b5909fe8d100b2fdd33af737fd3`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.4 MB (1425643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94580f7d0016c73ceb27fa192cc5db03b877381b0cdf079fb1b31df3a769e34b`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c23001009309c3c4d6b4dcc691439edb1b30116f78a3ce9f713e0828c5b6e3`  
		Last Modified: Tue, 05 Apr 2022 09:44:06 GMT  
		Size: 9.2 MB (9233816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d995af928ab6d75278a09427e32898e4b9c8f3cb38c1561e3cf707922f880`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:3.13.7`

```console
$ docker pull teamspeak@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 0

## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:9bf4b1bd2b2bd507edb977be30a80d2f23b41ba190186c91cd2289f844444008
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:adb97ff3b3df49b50b728a33b82e91a415148fd05adbfba129bc75f58a7992cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13481650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad17fc34e34d87d4120a2e034e6d9d4600adfecce0d6026c07852a49206a9528`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:14 GMT
ADD file:0f80c1db9ba5535d5020662b1c880624848316637bf3f9c189f459ab31f365d0 in / 
# Tue, 05 Apr 2022 00:20:14 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 09:43:51 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Tue, 05 Apr 2022 09:43:51 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Tue, 05 Apr 2022 09:43:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Tue, 05 Apr 2022 09:43:51 GMT
ARG TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0
# Tue, 05 Apr 2022 09:43:52 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
# Tue, 05 Apr 2022 09:43:54 GMT
# ARGS: TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Tue, 05 Apr 2022 09:43:54 GMT
VOLUME [/var/ts3server/]
# Tue, 05 Apr 2022 09:43:54 GMT
WORKDIR /var/ts3server/
# Tue, 05 Apr 2022 09:43:54 GMT
EXPOSE 10011 30033 9987/udp
# Tue, 05 Apr 2022 09:43:54 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Tue, 05 Apr 2022 09:43:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Tue, 05 Apr 2022 09:43:55 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:6097bfa160c13665f946cea95b206a812a795d2517d7690a0a0796d64ec5f817`  
		Last Modified: Tue, 05 Apr 2022 00:21:00 GMT  
		Size: 2.8 MB (2819312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e2a3e53f7b63d3b584a2f90666a9bf53058b5909fe8d100b2fdd33af737fd3`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.4 MB (1425643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94580f7d0016c73ceb27fa192cc5db03b877381b0cdf079fb1b31df3a769e34b`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c23001009309c3c4d6b4dcc691439edb1b30116f78a3ce9f713e0828c5b6e3`  
		Last Modified: Tue, 05 Apr 2022 09:44:06 GMT  
		Size: 9.2 MB (9233816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867d995af928ab6d75278a09427e32898e4b9c8f3cb38c1561e3cf707922f880`  
		Last Modified: Tue, 05 Apr 2022 09:44:05 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
