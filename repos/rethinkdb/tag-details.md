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
$ docker pull rethinkdb@sha256:e29ed132b1931baa60505543dd1b12531626702447184ea1d09f2d658e1fc0ae
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
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
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
$ docker pull rethinkdb@sha256:4a5f1b5209f6ce2cacd3e695f3da6f4f153de10ab51c4db5ad87334f6134f4a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `rethinkdb:2-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4`

```console
$ docker pull rethinkdb@sha256:e29ed132b1931baa60505543dd1b12531626702447184ea1d09f2d658e1fc0ae
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
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
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
$ docker pull rethinkdb@sha256:4a5f1b5209f6ce2cacd3e695f3da6f4f153de10ab51c4db5ad87334f6134f4a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `rethinkdb:2.4-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.3`

```console
$ docker pull rethinkdb@sha256:4a5f1b5209f6ce2cacd3e695f3da6f4f153de10ab51c4db5ad87334f6134f4a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `rethinkdb:2.4.3` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:2.4.4-bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4a5f1b5209f6ce2cacd3e695f3da6f4f153de10ab51c4db5ad87334f6134f4a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `rethinkdb:2.4.4-bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:bookworm-slim`

```console
$ docker pull rethinkdb@sha256:4a5f1b5209f6ce2cacd3e695f3da6f4f153de10ab51c4db5ad87334f6134f4a3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

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

### `rethinkdb:bookworm-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `rethinkdb:latest`

```console
$ docker pull rethinkdb@sha256:e29ed132b1931baa60505543dd1b12531626702447184ea1d09f2d658e1fc0ae
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
$ docker pull rethinkdb@sha256:f85dc716c4972b9bb61c97e490a8817cdb88dd0925843f1ef2072670ef9d76a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48336901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ff85603eb84c64c3a5c88879e1dabf7bc242dd559bd141686ccf911d820a56`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Tue, 12 Dec 2023 18:58:39 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 12 Dec 2023 18:58:41 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bookworm bookworm main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 13 Dec 2023 23:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.4~0bookworm
# Wed, 13 Dec 2023 23:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 Dec 2023 23:54:49 GMT
VOLUME [/data]
# Wed, 13 Dec 2023 23:54:49 GMT
WORKDIR /data
# Wed, 13 Dec 2023 23:54:49 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 13 Dec 2023 23:54:49 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c9135c3915c6365fef3780e67e564c24edf19b0c1218bf60d1cde501e1f427`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9586130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e301a7defddc5c4579d99f4805faa531b084dc7af58b8f4547f3d3bfff51b3b`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf605ac1f12920a5d09f4e42786654bf4916f67c9bcd2b9c4493c78a7e91979`  
		Last Modified: Wed, 13 Dec 2023 23:55:03 GMT  
		Size: 9.6 MB (9568679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ceb8a7a135f8c51d5cdc2503be85c4e1bd5657b7f5bf85a771ef0e00aff88f3`  
		Last Modified: Wed, 13 Dec 2023 23:55:02 GMT  
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
