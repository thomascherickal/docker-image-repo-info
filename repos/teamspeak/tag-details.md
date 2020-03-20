<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `teamspeak`

-	[`teamspeak:3.12`](#teamspeak312)
-	[`teamspeak:3.12.0`](#teamspeak3120)
-	[`teamspeak:latest`](#teamspeaklatest)

## `teamspeak:3.12`

```console
$ docker pull teamspeak@sha256:0e0caf85de6360c0c6599e8c469ed6d83c05c4b8de38623138ef80ad5839be0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:3.12` - linux; amd64

```console
$ docker pull teamspeak@sha256:375e34c23ed0edabdce38fc06d2444f43968192795985f33a398e78d8a7e77fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12535574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59090e9a17eaa5a23384fc90568c9aae0fb4588aa67271e3ecbc0a8b53cc49c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:17:27 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Fri, 24 Jan 2020 06:17:29 GMT
RUN set -eux;  addgroup -g 9987 ts3server;  adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;  install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Fri, 24 Jan 2020 06:17:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
# Fri, 20 Mar 2020 18:22:54 GMT
# ARGS: TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
RUN set -eux;  apk add --no-cache --virtual .fetch-deps tar;  wget "${TEAMSPEAK_URL}" -O server.tar.bz2;  echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;  mkdir -p /opt/ts3server;  tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;  rm server.tar.bz2;  apk del .fetch-deps;  mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;  ldconfig /usr/local/lib
# Fri, 20 Mar 2020 18:22:54 GMT
VOLUME [/var/ts3server/]
# Fri, 20 Mar 2020 18:22:55 GMT
WORKDIR /var/ts3server/
# Fri, 20 Mar 2020 18:22:55 GMT
EXPOSE 10011 30033 9987/udp
# Fri, 20 Mar 2020 18:22:55 GMT
COPY file:6d1cf26aa3141617a27d9a975d3a4ef216e03df89fc20159d5734f178aab0e88 in /opt/ts3server 
# Fri, 20 Mar 2020 18:22:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 20 Mar 2020 18:22:55 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65962c5b1376b9f8d20fccf94b290a5db6367840b0099f950bcd993e72ca15`  
		Last Modified: Fri, 24 Jan 2020 06:17:42 GMT  
		Size: 763.2 KB (763183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ffb8a772b5344af21dc94647378ef35cc748bad680751544446bfd2aaaf5a1`  
		Last Modified: Fri, 24 Jan 2020 06:17:40 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7282e2b33168c7c02735149c99de5764d550bad5fbef15b362d841004175b58d`  
		Last Modified: Fri, 20 Mar 2020 18:23:03 GMT  
		Size: 9.0 MB (8982561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b217b6ece05c00dc962a55afe93bc7b6f030dbd19dbf9ee6f1f513d964d8652`  
		Last Modified: Fri, 20 Mar 2020 18:23:02 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:3.12.0`

```console
$ docker pull teamspeak@sha256:0e0caf85de6360c0c6599e8c469ed6d83c05c4b8de38623138ef80ad5839be0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:3.12.0` - linux; amd64

```console
$ docker pull teamspeak@sha256:375e34c23ed0edabdce38fc06d2444f43968192795985f33a398e78d8a7e77fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12535574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59090e9a17eaa5a23384fc90568c9aae0fb4588aa67271e3ecbc0a8b53cc49c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:17:27 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Fri, 24 Jan 2020 06:17:29 GMT
RUN set -eux;  addgroup -g 9987 ts3server;  adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;  install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Fri, 24 Jan 2020 06:17:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
# Fri, 20 Mar 2020 18:22:54 GMT
# ARGS: TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
RUN set -eux;  apk add --no-cache --virtual .fetch-deps tar;  wget "${TEAMSPEAK_URL}" -O server.tar.bz2;  echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;  mkdir -p /opt/ts3server;  tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;  rm server.tar.bz2;  apk del .fetch-deps;  mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;  ldconfig /usr/local/lib
# Fri, 20 Mar 2020 18:22:54 GMT
VOLUME [/var/ts3server/]
# Fri, 20 Mar 2020 18:22:55 GMT
WORKDIR /var/ts3server/
# Fri, 20 Mar 2020 18:22:55 GMT
EXPOSE 10011 30033 9987/udp
# Fri, 20 Mar 2020 18:22:55 GMT
COPY file:6d1cf26aa3141617a27d9a975d3a4ef216e03df89fc20159d5734f178aab0e88 in /opt/ts3server 
# Fri, 20 Mar 2020 18:22:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 20 Mar 2020 18:22:55 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65962c5b1376b9f8d20fccf94b290a5db6367840b0099f950bcd993e72ca15`  
		Last Modified: Fri, 24 Jan 2020 06:17:42 GMT  
		Size: 763.2 KB (763183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ffb8a772b5344af21dc94647378ef35cc748bad680751544446bfd2aaaf5a1`  
		Last Modified: Fri, 24 Jan 2020 06:17:40 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7282e2b33168c7c02735149c99de5764d550bad5fbef15b362d841004175b58d`  
		Last Modified: Fri, 20 Mar 2020 18:23:03 GMT  
		Size: 9.0 MB (8982561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b217b6ece05c00dc962a55afe93bc7b6f030dbd19dbf9ee6f1f513d964d8652`  
		Last Modified: Fri, 20 Mar 2020 18:23:02 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `teamspeak:latest`

```console
$ docker pull teamspeak@sha256:0e0caf85de6360c0c6599e8c469ed6d83c05c4b8de38623138ef80ad5839be0c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `teamspeak:latest` - linux; amd64

```console
$ docker pull teamspeak@sha256:375e34c23ed0edabdce38fc06d2444f43968192795985f33a398e78d8a7e77fa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **12.5 MB (12535574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c59090e9a17eaa5a23384fc90568c9aae0fb4588aa67271e3ecbc0a8b53cc49c`
-	Entrypoint: `["entrypoint.sh"]`
-	Default Command: `["ts3server"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:17:27 GMT
RUN apk add --no-cache ca-certificates libstdc++ su-exec
# Fri, 24 Jan 2020 06:17:29 GMT
RUN set -eux;  addgroup -g 9987 ts3server;  adduser -u 9987 -Hh /var/ts3server -G ts3server -s /sbin/nologin -D ts3server;  install -d -o ts3server -g ts3server -m 775 /var/ts3server /var/run/ts3server /opt/ts3server
# Fri, 24 Jan 2020 06:17:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/ts3server
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066
# Fri, 20 Mar 2020 18:22:52 GMT
ARG TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
# Fri, 20 Mar 2020 18:22:54 GMT
# ARGS: TEAMSPEAK_CHECKSUM=6f414b427f43aef5a0ab95e0b996b7ba9620ad7b0017fff8c9bdb2855beef066 TEAMSPEAK_URL=https://files.teamspeak-services.com/releases/server/3.12.0/teamspeak3-server_linux_alpine-3.12.0.tar.bz2
RUN set -eux;  apk add --no-cache --virtual .fetch-deps tar;  wget "${TEAMSPEAK_URL}" -O server.tar.bz2;  echo "${TEAMSPEAK_CHECKSUM} *server.tar.bz2" | sha256sum -c -;  mkdir -p /opt/ts3server;  tar -xf server.tar.bz2 --strip-components=1 -C /opt/ts3server;  rm server.tar.bz2;  apk del .fetch-deps;  mv /opt/ts3server/*.so /opt/ts3server/redist/* /usr/local/lib;  ldconfig /usr/local/lib
# Fri, 20 Mar 2020 18:22:54 GMT
VOLUME [/var/ts3server/]
# Fri, 20 Mar 2020 18:22:55 GMT
WORKDIR /var/ts3server/
# Fri, 20 Mar 2020 18:22:55 GMT
EXPOSE 10011 30033 9987/udp
# Fri, 20 Mar 2020 18:22:55 GMT
COPY file:6d1cf26aa3141617a27d9a975d3a4ef216e03df89fc20159d5734f178aab0e88 in /opt/ts3server 
# Fri, 20 Mar 2020 18:22:55 GMT
ENTRYPOINT ["entrypoint.sh"]
# Fri, 20 Mar 2020 18:22:55 GMT
CMD ["ts3server"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c65962c5b1376b9f8d20fccf94b290a5db6367840b0099f950bcd993e72ca15`  
		Last Modified: Fri, 24 Jan 2020 06:17:42 GMT  
		Size: 763.2 KB (763183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ffb8a772b5344af21dc94647378ef35cc748bad680751544446bfd2aaaf5a1`  
		Last Modified: Fri, 24 Jan 2020 06:17:40 GMT  
		Size: 1.3 KB (1299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7282e2b33168c7c02735149c99de5764d550bad5fbef15b362d841004175b58d`  
		Last Modified: Fri, 20 Mar 2020 18:23:03 GMT  
		Size: 9.0 MB (8982561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b217b6ece05c00dc962a55afe93bc7b6f030dbd19dbf9ee6f1f513d964d8652`  
		Last Modified: Fri, 20 Mar 2020 18:23:02 GMT  
		Size: 1.6 KB (1569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
