<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `rethinkdb`

-	[`rethinkdb:2`](#rethinkdb2)
-	[`rethinkdb:2-bookworm-slim`](#rethinkdb2-bookworm-slim)
-	[`rethinkdb:2.4`](#rethinkdb24)
-	[`rethinkdb:2.4-bookworm-slim`](#rethinkdb24-bookworm-slim)
-	[`rethinkdb:2.4.3`](#rethinkdb243)
-	[`rethinkdb:2.4.4-bookworm-slim`](#rethinkdb244-bookworm-slim)
-	[`rethinkdb:bookworm-slim`](#rethinkdbbookworm-slim)
-	[`rethinkdb:latest`](#rethinkdblatest)

## `rethinkdb:2`

```console
$ docker pull rethinkdb@sha256:14ac991d686d62311ea8c07cb6332918e81da2436cd4b00550939cbf15f6702e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:9205ce12c46f79bf10b255b3aa63e0e7016966a849ad9e153a2da62225c241d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45968634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84dd82db07596ee88231d5be3e39ded85c31c26d7a5978611e52aa64483be848`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:50:28 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:29 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 20:50:29 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 20:50:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:33 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 20:50:34 GMT
WORKDIR /data
# Tue, 21 Nov 2023 20:50:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 20:50:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8731fcd86b256f3df11487e0a3c2a3ba68620e3a2eef1f0687d433ad9da592`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 6.3 MB (6312122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2f46d60705e1eb1c171b4f2e8350f349941b3ca38f83fa216c5bb0a5b3711`  
		Last Modified: Tue, 21 Nov 2023 20:50:44 GMT  
		Size: 2.7 KB (2685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c4b847aeed78cd1e493ca2cfe410ead07ead1b27dc9fcd618ce6dd1be8c172`  
		Last Modified: Tue, 21 Nov 2023 20:50:46 GMT  
		Size: 9.6 MB (9589577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff047367a05c0d7e589b69c73b840557b139764daf7c5da09b2b13f49d89301`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2` - linux; s390x

```console
$ docker pull rethinkdb@sha256:ef42784c4b0c031ea9900eee08f254ea40e46cb907d343db9460e426350a2fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45441901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb8011b6f9f1c4f69934b8f787581f1697054fefafc1cf3a184e149d56c7a1f9`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:53:22 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:23 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 05:53:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 05:53:29 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:30 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 05:53:30 GMT
WORKDIR /data
# Tue, 21 Nov 2023 05:53:30 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 05:53:30 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51a24b94a3e321435de17e4c84c747ce43bdb7ad7b804ca86d8185c7c3b0a2`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 6.2 MB (6207534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162fe5c2b50cd7212eec042bdbae1ddf0c03b5fbb29acc0a0e499224024e1182`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0736f53418415403d8f5908ecfad7fade9c50069b98887f8e202826d81431`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 9.6 MB (9574613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f4603e964cad3c1645ac52d7efccefdcc4af0a988a5c7019bf266ca1c163ce`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2-bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2-bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:14ac991d686d62311ea8c07cb6332918e81da2436cd4b00550939cbf15f6702e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2.4` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:9205ce12c46f79bf10b255b3aa63e0e7016966a849ad9e153a2da62225c241d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45968634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84dd82db07596ee88231d5be3e39ded85c31c26d7a5978611e52aa64483be848`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:50:28 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:29 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 20:50:29 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 20:50:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:33 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 20:50:34 GMT
WORKDIR /data
# Tue, 21 Nov 2023 20:50:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 20:50:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8731fcd86b256f3df11487e0a3c2a3ba68620e3a2eef1f0687d433ad9da592`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 6.3 MB (6312122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2f46d60705e1eb1c171b4f2e8350f349941b3ca38f83fa216c5bb0a5b3711`  
		Last Modified: Tue, 21 Nov 2023 20:50:44 GMT  
		Size: 2.7 KB (2685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c4b847aeed78cd1e493ca2cfe410ead07ead1b27dc9fcd618ce6dd1be8c172`  
		Last Modified: Tue, 21 Nov 2023 20:50:46 GMT  
		Size: 9.6 MB (9589577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff047367a05c0d7e589b69c73b840557b139764daf7c5da09b2b13f49d89301`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2.4` - linux; s390x

```console
$ docker pull rethinkdb@sha256:ef42784c4b0c031ea9900eee08f254ea40e46cb907d343db9460e426350a2fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45441901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb8011b6f9f1c4f69934b8f787581f1697054fefafc1cf3a184e149d56c7a1f9`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:53:22 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:23 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 05:53:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 05:53:29 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:30 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 05:53:30 GMT
WORKDIR /data
# Tue, 21 Nov 2023 05:53:30 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 05:53:30 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51a24b94a3e321435de17e4c84c747ce43bdb7ad7b804ca86d8185c7c3b0a2`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 6.2 MB (6207534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162fe5c2b50cd7212eec042bdbae1ddf0c03b5fbb29acc0a0e499224024e1182`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0736f53418415403d8f5908ecfad7fade9c50069b98887f8e202826d81431`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 9.6 MB (9574613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f4603e964cad3c1645ac52d7efccefdcc4af0a988a5c7019bf266ca1c163ce`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4-bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4-bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.3`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.3` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.4-bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:2.4.4-bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4687d87f45675d704804b1b188ce895eecdf368d058d17b46e3949ccc7468f68
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `rethinkdb:bookworm-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:14ac991d686d62311ea8c07cb6332918e81da2436cd4b00550939cbf15f6702e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:latest` - linux; amd64

```console
$ docker pull rethinkdb@sha256:8a41211b67e0a9ad1a6f9678f2da1440cb6d2b09bc2931b46c94d3fe7411f393
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49140319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:425c04783e91453d2ffc48d0d4e28fbe415515b0c79ca46da83a7424d6ad5acf`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:20:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:20:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:20:17 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:20:22 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:20:23 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:20:23 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:20:23 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:20:23 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e27c4b9f3d90f10afbdf95273f1c0bd904c1fc11c5588546bf19d597f47a5c9`  
		Last Modified: Tue, 12 Dec 2023 18:20:55 GMT  
		Size: 9.8 MB (9789060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1a8fa566039e71b2179938f635faaf0ed681a373ad3a3eeb27e64a0dfce4abc`  
		Last Modified: Tue, 12 Dec 2023 18:20:54 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5941bb608cbc6aa331c60524e5aeee41e8d6b337da2feefa9aaae1e9098139eb`  
		Last Modified: Wed, 13 Dec 2023 23:20:35 GMT  
		Size: 10.2 MB (10198535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:161eaac0e185db0872164cdb4f7ea3b9e36d6cbf5b8056cffe787b03bfe2c226`  
		Last Modified: Wed, 13 Dec 2023 23:20:33 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:latest` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:9205ce12c46f79bf10b255b3aa63e0e7016966a849ad9e153a2da62225c241d0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45968634 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84dd82db07596ee88231d5be3e39ded85c31c26d7a5978611e52aa64483be848`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 20:50:28 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:29 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 20:50:29 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 20:50:33 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 20:50:33 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 20:50:34 GMT
WORKDIR /data
# Tue, 21 Nov 2023 20:50:34 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 20:50:34 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8731fcd86b256f3df11487e0a3c2a3ba68620e3a2eef1f0687d433ad9da592`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 6.3 MB (6312122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b2f46d60705e1eb1c171b4f2e8350f349941b3ca38f83fa216c5bb0a5b3711`  
		Last Modified: Tue, 21 Nov 2023 20:50:44 GMT  
		Size: 2.7 KB (2685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c4b847aeed78cd1e493ca2cfe410ead07ead1b27dc9fcd618ce6dd1be8c172`  
		Last Modified: Tue, 21 Nov 2023 20:50:46 GMT  
		Size: 9.6 MB (9589577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff047367a05c0d7e589b69c73b840557b139764daf7c5da09b2b13f49d89301`  
		Last Modified: Tue, 21 Nov 2023 20:50:45 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:latest` - linux; s390x

```console
$ docker pull rethinkdb@sha256:ef42784c4b0c031ea9900eee08f254ea40e46cb907d343db9460e426350a2fd1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45441901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb8011b6f9f1c4f69934b8f787581f1697054fefafc1cf3a184e149d56c7a1f9`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:53:22 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:23 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 21 Nov 2023 05:53:24 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 21 Nov 2023 05:53:29 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Nov 2023 05:53:30 GMT
VOLUME [/data]
# Tue, 21 Nov 2023 05:53:30 GMT
WORKDIR /data
# Tue, 21 Nov 2023 05:53:30 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 21 Nov 2023 05:53:30 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c51a24b94a3e321435de17e4c84c747ce43bdb7ad7b804ca86d8185c7c3b0a2`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 6.2 MB (6207534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162fe5c2b50cd7212eec042bdbae1ddf0c03b5fbb29acc0a0e499224024e1182`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a0736f53418415403d8f5908ecfad7fade9c50069b98887f8e202826d81431`  
		Last Modified: Tue, 21 Nov 2023 05:53:45 GMT  
		Size: 9.6 MB (9574613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f4603e964cad3c1645ac52d7efccefdcc4af0a988a5c7019bf266ca1c163ce`  
		Last Modified: Tue, 21 Nov 2023 05:53:44 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
