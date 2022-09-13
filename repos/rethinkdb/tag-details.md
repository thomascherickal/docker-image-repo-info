<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rethinkdb`

-	[`rethinkdb:2`](#rethinkdb2)
-	[`rethinkdb:2-bullseye-slim`](#rethinkdb2-bullseye-slim)
-	[`rethinkdb:2.4`](#rethinkdb24)
-	[`rethinkdb:2.4-bullseye-slim`](#rethinkdb24-bullseye-slim)
-	[`rethinkdb:2.4.2`](#rethinkdb242)
-	[`rethinkdb:2.4.2-bullseye-slim`](#rethinkdb242-bullseye-slim)
-	[`rethinkdb:bullseye-slim`](#rethinkdbbullseye-slim)
-	[`rethinkdb:latest`](#rethinkdblatest)

## `rethinkdb:2`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2.4-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.2`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2.4.2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4.2` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4.2` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.2-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2.4.2-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4.2-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4.2-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:bullseye-slim`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:57fad8ff4a2077d38ec2b505fa2b8e72242cf073f8d4cec437e92254b6bb1759
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:62ad7b76d1ea7ca8241d2696ad60db94a8c092a64e551cae594cb60b9ccd3e17
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47948570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb1b45d151c60ab012b1eb866efdfe55f962e08ea6ac45470c8cdd13b63ced64`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:50 GMT
ADD file:7726efb0e0eb5003dbcf2967ec29364479eec8b41f2569ff189372153115b54b in / 
# Tue, 23 Aug 2022 00:20:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 11:01:15 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:17 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 11:01:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 11:01:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 11:01:22 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 11:01:22 GMT
WORKDIR /data
# Tue, 23 Aug 2022 11:01:22 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 11:01:22 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:7a6db449b51b92eac5c81cdbd82917785343f1664b2be57b22337b0a40c5b29d`  
		Last Modified: Tue, 23 Aug 2022 00:24:59 GMT  
		Size: 31.4 MB (31381485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20181367ea9b1f32dbca4de165da7018b4f1083fd2186dcfe1a66fc9c187bbfb`  
		Last Modified: Tue, 23 Aug 2022 11:01:39 GMT  
		Size: 6.3 MB (6328500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4c59a6fbe9d585528f506c6bd650721f6806ff29c701ea89917408f6629bd40`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54db2c71fcb09eb030fab68d722b6066bc795ef92f2d30785dfae9d85fe9e602`  
		Last Modified: Tue, 23 Aug 2022 11:01:40 GMT  
		Size: 10.2 MB (10235769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96e4039912094f2cde75911c70a356bc43c14d89aacc1eafe7bae411a4c434`  
		Last Modified: Tue, 23 Aug 2022 11:01:38 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:latest` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f5b96489210618ed825621d9f01f8f0f0a59e1ecaaf0f92af54794a58c3f0bbb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993e852e4f6f9b06b18beebf599dd549a6fb1df90caac8208f1c3dbb55f02918`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:32 GMT
ADD file:90344130400909b0ad12bb54d439b0e4868fc5863f538f676e6fdfeaeb4dad51 in / 
# Tue, 23 Aug 2022 01:52:33 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 17:33:50 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:52 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 23 Aug 2022 17:33:53 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 23 Aug 2022 17:33:58 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:33:59 GMT
VOLUME [/data]
# Tue, 23 Aug 2022 17:34:00 GMT
WORKDIR /data
# Tue, 23 Aug 2022 17:34:01 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 23 Aug 2022 17:34:02 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:5b142346550416c75ea412d21741de5eaf3e76857affc12fab789277f81f53b3`  
		Last Modified: Tue, 23 Aug 2022 01:58:00 GMT  
		Size: 30.1 MB (30063788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df3b4e10490fe18d4cefcfd0ac879109eb8f61fa40ccf2feb966491eb8d6071`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 6.1 MB (6103355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed0200c2fa6764d4ea192e8eae6a4fdc68b21f3c32ee7c0709d0f82c862e92c`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d66e99d4413325381a48b676addb6a154edb71813b3cc53d721b6a464a492d`  
		Last Modified: Tue, 23 Aug 2022 17:34:28 GMT  
		Size: 9.4 MB (9372153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed012e5dff886545941674b755fa01f56eac483d0c2df92153abdd91b711645`  
		Last Modified: Tue, 23 Aug 2022 17:34:27 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:latest` - linux; s390x

```console
$ docker pull rethinkdb@sha256:78d2f2b9ef9c7b5acb9d1f0c067c1f20eb126512caf9583122cd207083711b2b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45416018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82757c2a85810b65f1a192806a47b28b3a382f84cbd099ef75b730a341459221`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 00:48:07 GMT
ADD file:e8a6c2e8be5d9d1f83c1e280419014489438391a9feb7c77b6c21adbf0ec062b in / 
# Tue, 13 Sep 2022 00:48:08 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 06:52:33 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:36 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 06:52:36 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 06:52:42 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 06:52:42 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 06:52:42 GMT
WORKDIR /data
# Tue, 13 Sep 2022 06:52:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 06:52:43 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:c64715e5ebd39975a39b5cf2535772544c27713cbed678b0a21e73680fffaf72`  
		Last Modified: Tue, 13 Sep 2022 00:52:39 GMT  
		Size: 29.6 MB (29635080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d90ae81aa48a6524de47405ccda60aa21c6019a0e5ce06910111a253b10947`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 6.2 MB (6205669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e9f0b2c76f6722904687acef1569fd85c4ed9fdbcd3c1f2a641379141fe0274`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad2716a6c3e2534cf18ef82bf9b1adf79d3060548e805457f70f55b96b1c98`  
		Last Modified: Tue, 13 Sep 2022 06:53:10 GMT  
		Size: 9.6 MB (9572453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6fd9d26d856864d33ffb44a1773a1c20ee8209228bcdff1186241bbabf10a6`  
		Last Modified: Tue, 13 Sep 2022 06:53:09 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
