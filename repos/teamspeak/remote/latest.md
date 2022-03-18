## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:ae80b94aa922c6b08790755a75e2760953f4026380a6e6c969cf00e6b773dde8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:71e8638b201d596ada0bf7d611ee65fd3c6157db4662ed2fe0aa4b487816acda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **13.5 MB (13479624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b592cea3c0af4fd718ddf4428a24f69d22e19edf642b76099d710af2b96769eb`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:36 GMT
ADD file:51c08645923aa2d3513f66571f0c598a727dd5805e4f2bb87fb660b2f789348d in / 
# Thu, 17 Mar 2022 15:19:36 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 15:55:02 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec libpq
# Thu, 17 Mar 2022 15:55:03 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Thu, 17 Mar 2022 15:55:03 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Thu, 17 Mar 2022 15:55:03 GMT
ARG TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0
# Thu, 17 Mar 2022 15:55:03 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
# Thu, 17 Mar 2022 15:55:12 GMT
# ARGS: TEAMSPEAK_CHECKSUM=f30a5366f12b0c5b00476652ebc06d9b5bc4754c4cb386c086758cceb620a8d0 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.6/teamspeak3-server_linux_alpine-3.13.6.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Thu, 17 Mar 2022 15:55:12 GMT
VOLUME [/var/ts3server/]
# Thu, 17 Mar 2022 15:55:12 GMT
WORKDIR /var/ts3server/
# Thu, 17 Mar 2022 15:55:12 GMT
EXPOSE 10011 30033 9987/udp
# Thu, 17 Mar 2022 15:55:13 GMT
COPY file:d9f653f53e40ea33be02ca61f8194eb1a4147066050f721a3172007f06bb834c in /opt/ts3server 
# Thu, 17 Mar 2022 15:55:13 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 17 Mar 2022 15:55:13 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:e1096b72685a2366348e697f5b57e3b8feb41660e3dbe68447e168381515111a`  
		Last Modified: Thu, 17 Mar 2022 15:20:24 GMT  
		Size: 2.8 MB (2817181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51fe4498854b138321aaf2216f162bafc7d6b79d7793bed26165701ac481886`  
		Last Modified: Thu, 17 Mar 2022 15:55:25 GMT  
		Size: 1.4 MB (1425752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b000c2423a0eff5bef70268a17d0b4545cd971bd34b9efb825077abdd4d571a`  
		Last Modified: Thu, 17 Mar 2022 15:55:25 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857a362ce8180809f7798b12da6fe10fa77608b1db62cc9c988a84382fff4305`  
		Last Modified: Thu, 17 Mar 2022 15:55:26 GMT  
		Size: 9.2 MB (9233809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54bc1461aabcffd381e6f712efb05473f8c80f29b0b74867349b267745249e8`  
		Last Modified: Thu, 17 Mar 2022 15:55:25 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
