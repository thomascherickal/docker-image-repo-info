## `rethinkdb:2-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:3798254817e5e8e0ee4e060feb9dea53d3fe55001ef140c0d3e9a0abc2bca538
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:4452aadba3e99771ff3559735dab16279c5a352359d79f38737c6fdca941c6e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47944705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce59549f0c046540e10788de1be822f1710568ed76111c0eb0aaaebc4cd8f906`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Thu, 23 Jun 2022 00:20:27 GMT
ADD file:8adbbab04d6f84cd83b5f4205b89b0acb7ecbf27a1bb2dc181d0a629479039fe in / 
# Thu, 23 Jun 2022 00:20:27 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 12:37:17 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:37:19 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Thu, 23 Jun 2022 12:37:19 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Thu, 23 Jun 2022 12:37:24 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 12:37:25 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 12:37:25 GMT
WORKDIR /data
# Thu, 23 Jun 2022 12:37:25 GMT
CMD ["rethinkdb" "--bind" "all"]
# Thu, 23 Jun 2022 12:37:25 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:b85a868b505ffd0342a37e6a3b1c49f7c71878afe569a807e6238ef08252fcb7`  
		Last Modified: Thu, 23 Jun 2022 00:25:18 GMT  
		Size: 31.4 MB (31379408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bb28ba7e8a6993983fcb329c610b2469a7fb49a6241638ea2e1af37415a7801`  
		Last Modified: Thu, 23 Jun 2022 12:37:43 GMT  
		Size: 6.3 MB (6326725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a4883e6561248c4b0375999c2b4e5d20c94f95967b2afed1231c996934d3c8`  
		Last Modified: Thu, 23 Jun 2022 12:37:42 GMT  
		Size: 2.7 KB (2687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dcc411eaabeb6a5b64e7a77bfbe4fe752628b91658918f6081a8ff30e8525ef`  
		Last Modified: Thu, 23 Jun 2022 12:37:43 GMT  
		Size: 10.2 MB (10235758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b39921d5de33afe5df6605776c61e7c2a2e213fa08f63b06808d3778fa663c`  
		Last Modified: Thu, 23 Jun 2022 12:37:42 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:17d7c9cde5375503e4d61ff9019b33e6521fe0e59ce921ba96f4c68bf707ba7b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45736592 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61a85a60426b38b58b0447a563ace957c33cd16e38ec2f010be09a69c03be2a1`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 12 Jul 2022 00:40:34 GMT
ADD file:f3a33075f4c3324c6a634ef37a1965ddd5606b4449c0f5909ce18eeb8268b612 in / 
# Tue, 12 Jul 2022 00:40:35 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 12:58:49 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 12:58:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 12 Jul 2022 12:58:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 12 Jul 2022 12:58:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 12:58:58 GMT
VOLUME [/data]
# Tue, 12 Jul 2022 12:58:59 GMT
WORKDIR /data
# Tue, 12 Jul 2022 12:59:00 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 12 Jul 2022 12:59:01 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:60197a4c18d4b386d371cf39d01c48e98c357bba06da0b070a3c1f75006fd838`  
		Last Modified: Tue, 12 Jul 2022 00:46:13 GMT  
		Size: 30.1 MB (30054226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd64d21079be01bfbfc2e3c03b980dae2555e3cde8f67989d6548e0a0c4b9e1`  
		Last Modified: Tue, 12 Jul 2022 12:59:28 GMT  
		Size: 6.3 MB (6307438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4867547263d5c578be8d148bf9a3b99b196f59f9627d30c077b367aceb822369`  
		Last Modified: Tue, 12 Jul 2022 12:59:27 GMT  
		Size: 2.7 KB (2669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6caa23d65e5714906e1c7785d47a85e8dbff934bdcce0d4c02133f88182274`  
		Last Modified: Tue, 12 Jul 2022 12:59:28 GMT  
		Size: 9.4 MB (9372166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f74bd782c64b26192fdef2ea0fce33f70798cf991501e67b01d016173cf896`  
		Last Modified: Tue, 12 Jul 2022 12:59:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:66daaf46cd34cfd771b7c160e00601fd2d5fa6804eccffe5a0e6119edc6e8b33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45434585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f619841234da6caacf1ea14be636d8388ca6ed121836b19b912d981537e4244`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Thu, 23 Jun 2022 00:43:10 GMT
ADD file:0b511e3efd87267fb27161eae56c4d08f0fed733697da6ffe6ea96a4cb68e938 in / 
# Thu, 23 Jun 2022 00:43:15 GMT
CMD ["bash"]
# Thu, 23 Jun 2022 13:00:41 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:00:43 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Thu, 23 Jun 2022 13:00:43 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Thu, 23 Jun 2022 13:00:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jun 2022 13:00:49 GMT
VOLUME [/data]
# Thu, 23 Jun 2022 13:00:49 GMT
WORKDIR /data
# Thu, 23 Jun 2022 13:00:50 GMT
CMD ["rethinkdb" "--bind" "all"]
# Thu, 23 Jun 2022 13:00:50 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c547f465e0c8708ad0c57cf09caa52f4c2b5b295bf10ab1ce71ca17ff81ea36a`  
		Last Modified: Thu, 23 Jun 2022 00:51:59 GMT  
		Size: 29.7 MB (29655262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3104fccb3513ac4a04f15b186f4f8d3c88580133df6e3be8e523a60b53cd30`  
		Last Modified: Thu, 23 Jun 2022 13:01:19 GMT  
		Size: 6.2 MB (6204050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40b7b28887b426c1db0eb36aa2e1269750469e3ebfd5b6b294c39373df45b306`  
		Last Modified: Thu, 23 Jun 2022 13:01:17 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead49101fb2b2b324995f8cc7b670e5cb0b5ae554add6609c673d99e4212f6fc`  
		Last Modified: Thu, 23 Jun 2022 13:01:18 GMT  
		Size: 9.6 MB (9572457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a211e0c69fd205999d25be28d81b21ad4b6e8ac3ba021df2239830ca084d8c0`  
		Last Modified: Thu, 23 Jun 2022 13:01:17 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
