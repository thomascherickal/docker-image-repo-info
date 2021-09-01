## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:a88d61887cbfa78012ce8bf69e6fad5988d853b7b72a9483000b1af8a6083ff8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:ff7a92727ffbf05925b54bb12e65bfee311d4193fc68e175dacd63a0048c28bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13483800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24a912ec13c6a1763fbed99f9a42a833782f1850869c8b9e0bdf8cafe87cb1eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 00:29:27 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Wed, 01 Sep 2021 00:29:28 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Wed, 01 Sep 2021 00:29:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Wed, 01 Sep 2021 00:29:29 GMT
ARG TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0
# Wed, 01 Sep 2021 00:29:29 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
# Wed, 01 Sep 2021 00:29:34 GMT
# ARGS: TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Wed, 01 Sep 2021 00:29:35 GMT
VOLUME [/var/ts3server/]
# Wed, 01 Sep 2021 00:29:35 GMT
WORKDIR /var/ts3server/
# Wed, 01 Sep 2021 00:29:36 GMT
EXPOSE 10011 30033 9987/udp
# Wed, 01 Sep 2021 00:29:36 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Wed, 01 Sep 2021 00:29:36 GMT
ENTRYPOINT ["entrypoint.sh"]
# Wed, 01 Sep 2021 00:29:37 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c8c8b6e9f75e2398c156fc8f421aae8bc2af5bd77ce63b6a92e50e2296284`  
		Last Modified: Wed, 01 Sep 2021 00:29:50 GMT  
		Size: 1.4 MB (1433645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac2d40443b5efa40d019f41c8e1fded6141fdc293535b9a615c5087f8428c88`  
		Last Modified: Wed, 01 Sep 2021 00:29:49 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4289c459c08713a0baccdbf70568b59a2ccb88ea83e8e5611d65f706fa7b3f37`  
		Last Modified: Wed, 01 Sep 2021 00:29:51 GMT  
		Size: 9.2 MB (9233195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dcdc4e930be497164a7f30cdb766b9b2c8e618a1808c23bb34b63084bbdc20c`  
		Last Modified: Wed, 01 Sep 2021 00:29:49 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
