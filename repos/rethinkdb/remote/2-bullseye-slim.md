## `rethinkdb:2-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:4d8bfbe82ff8a3c64a09d2a43a0ed5a7adb748fe5d25bfdfb115d33e2dd3da00
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:98bc75062292f876b2069d7a6a0f9cdd5af626c2535ba850f58e045d06301855
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47944463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d38c1f4893fe2610dcdb417b168f3f629d710b983d37731571bc695b008ef94`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 28 May 2022 01:20:23 GMT
ADD file:134f25aec8adf83cb940ba073a3409ca85dbb5ae592b704f95193e7d2539a3bc in / 
# Sat, 28 May 2022 01:20:23 GMT
CMD ["bash"]
# Sat, 28 May 2022 15:20:04 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:20:06 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 28 May 2022 15:20:06 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Sat, 28 May 2022 15:20:11 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 15:20:11 GMT
VOLUME [/data]
# Sat, 28 May 2022 15:20:11 GMT
WORKDIR /data
# Sat, 28 May 2022 15:20:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 28 May 2022 15:20:12 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:42c077c10790d51b6f75c4eb895cbd4da37558f7215b39cbf64c46b288f89bda`  
		Last Modified: Sat, 28 May 2022 01:25:19 GMT  
		Size: 31.4 MB (31379276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51a48596cf85051f8e5acf65ce98358206ce7582b2463a15d9f0560a8e3baec1`  
		Last Modified: Sat, 28 May 2022 15:20:27 GMT  
		Size: 6.3 MB (6326609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68d56169b735e58217129664da91446ac147824270bfd018d9750afeed95038b`  
		Last Modified: Sat, 28 May 2022 15:20:26 GMT  
		Size: 2.7 KB (2686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7831c6bf8e18069a117919ad2b5c0e08ebfdd6abe15b8aa5de306b82a04fe052`  
		Last Modified: Sat, 28 May 2022 15:20:28 GMT  
		Size: 10.2 MB (10235765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db79c318e6afdd9d916c3d4af8ec101b44ada6dfb1b8c51f83387f34b2024af`  
		Last Modified: Sat, 28 May 2022 15:20:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:a954878f552e5f047b9f1a49857ebef0795435297735e46c665e5caab4318c53
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45543960 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b86ae2a0a34801ba4ea44048a01025fd5437d38951c4cc82b2135db10d52c069`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 28 May 2022 00:40:39 GMT
ADD file:55b4fe3115c684f545e4e4148c93745f12192976a08c37d090fcac708fb709a7 in / 
# Sat, 28 May 2022 00:40:39 GMT
CMD ["bash"]
# Sat, 28 May 2022 09:29:43 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:29:46 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 28 May 2022 09:29:46 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Sat, 28 May 2022 09:29:52 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 09:29:52 GMT
VOLUME [/data]
# Sat, 28 May 2022 09:29:53 GMT
WORKDIR /data
# Sat, 28 May 2022 09:29:54 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 28 May 2022 09:29:55 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:dc1f00a5d701e86e2cd2568b860c61b393d66be1341e7267d07e6e57448ceeba`  
		Last Modified: Sat, 28 May 2022 00:47:35 GMT  
		Size: 30.1 MB (30065728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b59bde64cef75e6f3b25cad2b815ecef10e7cbfaff8ffca2c0a4bbb56c3c9f`  
		Last Modified: Sat, 28 May 2022 09:30:22 GMT  
		Size: 6.1 MB (6103294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac6f5f167561e97fd27e8a4f20f857e6cb9a4ada30937ff941aec443f9204c0a`  
		Last Modified: Sat, 28 May 2022 09:30:21 GMT  
		Size: 2.7 KB (2665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4391f153d9e2a3fe5f0d92b26db5043423b897aec22ce1c2214c3acca77fa0ca`  
		Last Modified: Sat, 28 May 2022 09:30:23 GMT  
		Size: 9.4 MB (9372180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca29a2e42d8068c963f682a33a6bcf06d98d5369e0d2db696ff05e0889d23005`  
		Last Modified: Sat, 28 May 2022 09:30:21 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:898bd8fdb50a658d5c8fbf8c4a88b76371680332bb76994adb4b783579365f08
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45434866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd4c605915d46d9d83c58117ce0750ce066ee156aadc240231c36838b7c3d073`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Sat, 28 May 2022 00:43:00 GMT
ADD file:95dc6dcd4ebd15b42beaf935d91adafb0ea44a443bb44597bc1ff236e831ce18 in / 
# Sat, 28 May 2022 00:43:03 GMT
CMD ["bash"]
# Sat, 28 May 2022 14:26:00 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:26:03 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Sat, 28 May 2022 14:26:04 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Sat, 28 May 2022 14:26:16 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 14:26:17 GMT
VOLUME [/data]
# Sat, 28 May 2022 14:26:18 GMT
WORKDIR /data
# Sat, 28 May 2022 14:26:18 GMT
CMD ["rethinkdb" "--bind" "all"]
# Sat, 28 May 2022 14:26:19 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f7bb6d2d11c3060ba2e66ba762e2aa10a0d1d361cfa6a806bcf26a64cc3a79aa`  
		Last Modified: Sat, 28 May 2022 00:49:46 GMT  
		Size: 29.7 MB (29655258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d0acf5b0f6f498cc428f777e1cc15aaf87502450856b3e2b6488a46bbfc3d6`  
		Last Modified: Sat, 28 May 2022 14:26:52 GMT  
		Size: 6.2 MB (6204229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:655dd14d4ea5664899154a1707336ae8eca4f35e28a9efce796ebd66e7e19dd8`  
		Last Modified: Sat, 28 May 2022 14:26:51 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11961d1a71d77214eec493331fbe97a741f516c61aabdc54c7e8ba67bf7f73cc`  
		Last Modified: Sat, 28 May 2022 14:26:52 GMT  
		Size: 9.6 MB (9572563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2fe2db49d5cce642c571edaec4e910461e9a948f7c6a46bb35ff998d116bdb0`  
		Last Modified: Sat, 28 May 2022 14:26:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
