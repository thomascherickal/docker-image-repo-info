## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:70a41805e9c17aa45ee4d9f0101ec7cbd77b2cc17f8629c1fb4676bf1243c176
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:1d9018ee451b62c20e8c7b83ad4f41e0ed2d717cf3ebe410e0f7e77a9aff85fb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.8 MB (12787626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8eb9c21ad2a9f87d1f0abf8e4cab1f671075637edbec43446f947f84b322220`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:25 GMT
ADD file:e944b37facf29902a466ebf545744be882c811e9501a8d2926393bd81a09b12a in / 
# Wed, 31 Mar 2021 20:10:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:48:23 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Thu, 01 Apr 2021 17:48:24 GMT
RUN set -eux;     addgroup -g 9987 ts3server;     adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;     install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Thu, 01 Apr 2021 17:48:24 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Thu, 01 Apr 2021 17:48:24 GMT
ARG TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498
# Thu, 01 Apr 2021 17:48:25 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
# Thu, 01 Apr 2021 17:48:27 GMT
# ARGS: TEAMSPEAK_CHECKSUM=b4134aeba964782e10c22dcb96b6de4c96e558965e9d5ed9b0db47e648ad1498 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.13.3/teamspeak3-server_linux_alpine-3.13.3.tar.bz2
RUN set -eux;     apk add --no-cache --virtual .fetch-deps tar;     wget "${TEAMSPEAK_URL}" -O server.tar.bz2;     echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;     mkdir -p /opt/ts3server;     tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;     rm server.tar.bz2;     apk del .fetch-deps;     mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;     ldconfig /usr/local/lib
# Thu, 01 Apr 2021 17:48:27 GMT
VOLUME [/var/ts3server/]
# Thu, 01 Apr 2021 17:48:28 GMT
WORKDIR /var/ts3server/
# Thu, 01 Apr 2021 17:48:28 GMT
EXPOSE 10011 30033 9987/udp
# Thu, 01 Apr 2021 17:48:28 GMT
COPY file:6f38f0bdd32398bda0227797278f67250720c9ff535447f0c53ae8d42a8789d0 in /opt/ts3server 
# Thu, 01 Apr 2021 17:48:28 GMT
ENTRYPOINT ["entrypoint.sh"]
# Thu, 01 Apr 2021 17:48:28 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:bfdacc68c91b7e6d1aed01fb1262c6f752e85c932bd632e6bd62263818905ff9`  
		Last Modified: Wed, 31 Mar 2021 20:11:27 GMT  
		Size: 2.8 MB (2797176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f572110021d2df52716bef7b52d28e7b9adf0ccd2e37257eb68d64edf1ba5cc0`  
		Last Modified: Thu, 01 Apr 2021 17:48:41 GMT  
		Size: 760.5 KB (760469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5b0148dd53e3639766457c5966618212fe73a75a826b5742df09a35fb8b795`  
		Last Modified: Thu, 01 Apr 2021 17:48:41 GMT  
		Size: 1.3 KB (1348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3d9606becb20e202e4af7d258e45c11970433acf7c8e094a15104136813dade`  
		Last Modified: Thu, 01 Apr 2021 17:48:43 GMT  
		Size: 9.2 MB (9227071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d4fbe883fb077c56e600ff8c39264f63adf5c9b6f08152f0ed4e49ed7c0a11c`  
		Last Modified: Thu, 01 Apr 2021 17:48:43 GMT  
		Size: 1.6 KB (1562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
