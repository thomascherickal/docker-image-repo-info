## `rethinkdb:bullseye-slim`

```console
$ docker pull rethinkdb@sha256:c663e4c337c9ba330a6d7eb50326be8fbc1b50a84c310f11b0ab447f5c546893
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:27e9c3a782e6d495ed711b415376379b4f8fc607a76a0f31816fcb4f48621921
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47987244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c45625405a54293f3e5c2058eedf15b3eaaf74f608fce816af8f50a03565e00`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:39 GMT
ADD file:b78b777208be08edd8f297035cdfbacddb45170ad778fd643c792ee045187e39 in / 
# Tue, 04 Oct 2022 23:26:39 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 09:40:04 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:40:06 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 05 Oct 2022 09:40:06 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Wed, 05 Oct 2022 09:40:11 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 09:40:11 GMT
VOLUME [/data]
# Wed, 05 Oct 2022 09:40:11 GMT
WORKDIR /data
# Wed, 05 Oct 2022 09:40:11 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 05 Oct 2022 09:40:12 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:bd159e379b3b1bc0134341e4ffdeab5f966ec422ae04818bb69ecef08a823b05`  
		Last Modified: Tue, 04 Oct 2022 23:30:54 GMT  
		Size: 31.4 MB (31420102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea58a078abbc55fc9c3e0a8e883dc94c73768b587a95fa51224f0223e2a3413f`  
		Last Modified: Wed, 05 Oct 2022 09:40:27 GMT  
		Size: 6.3 MB (6328556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6d6fdaf40d39b7f2bf5cbc5a9758a8e8cbf60de69a99a96fa4716ae8662f13`  
		Last Modified: Wed, 05 Oct 2022 09:40:26 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6790a92fc92e0973a2bccae17b187bb329b1f000e0de6fb7680294a8da2fc47c`  
		Last Modified: Wed, 05 Oct 2022 09:40:27 GMT  
		Size: 10.2 MB (10235771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:730ba5fc5211a146121af1efeb844ad7bface0d7af6b98b45cf4c5e723bd1403`  
		Last Modified: Wed, 05 Oct 2022 09:40:26 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:355c19f28b5fc4eb72f5d495c97fd2f0eea5012e48ba0effbaaf2e7d13ed707f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45542742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e0efbd66412264da89013149e353f922cf475851dafb5b94f85621762f3ef5`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 04 Oct 2022 23:44:42 GMT
ADD file:dcb96c5906228cc8195f87d079b2a65ab49cde56edd7f0ccd238cdc65f9b693c in / 
# Tue, 04 Oct 2022 23:44:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 12:36:32 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:36:34 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 05 Oct 2022 12:36:35 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Wed, 05 Oct 2022 12:36:40 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 12:36:41 GMT
VOLUME [/data]
# Wed, 05 Oct 2022 12:36:42 GMT
WORKDIR /data
# Wed, 05 Oct 2022 12:36:43 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 05 Oct 2022 12:36:44 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:df8e44b0463f16c791d040e02e9c3ef8ec2a84245d365f088a80a22a455c71e8`  
		Last Modified: Tue, 04 Oct 2022 23:50:23 GMT  
		Size: 30.1 MB (30064395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed79aac93557e9b55770aad54a891fd1666e169eb2a2ed770c736dd1f8df876`  
		Last Modified: Wed, 05 Oct 2022 12:37:10 GMT  
		Size: 6.1 MB (6103415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9274c11730e508fb1ef4682a1d2f3de17f27359ff783053c4d7d889be7e9e21d`  
		Last Modified: Wed, 05 Oct 2022 12:37:09 GMT  
		Size: 2.7 KB (2668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463fa5e0d416837d8ee970ec2cef33a4764d788bd3cffd0df1fdc1d8935a5b8c`  
		Last Modified: Wed, 05 Oct 2022 12:37:10 GMT  
		Size: 9.4 MB (9372171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b426e47aa5c6bbc1a8126940f4541f0cae8f7aaf64f34f7c7818fb7a7037949d`  
		Last Modified: Wed, 05 Oct 2022 12:37:08 GMT  
		Size: 93.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:3fa83f5d08d58b4c8fe160235ebb90669e28a2449eaf0efb67297ede804a4d54
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45431537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:040ed421c217d3d47ae79aa5363e15f48b9ff442f56b7405b9da26b9f2a8ddb8`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 04 Oct 2022 23:42:42 GMT
ADD file:7acfe92be51da9cffeb5b063cc87926d1ce457729e3080de340603a38216a708 in / 
# Tue, 04 Oct 2022 23:42:43 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 03:02:28 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:02:30 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 05 Oct 2022 03:02:30 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Wed, 05 Oct 2022 03:02:36 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 03:02:36 GMT
VOLUME [/data]
# Wed, 05 Oct 2022 03:02:36 GMT
WORKDIR /data
# Wed, 05 Oct 2022 03:02:37 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 05 Oct 2022 03:02:37 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:62990b94a520bfcf718ec711f8444f83c536af2c83c8e53fdfe1f89fdcb79826`  
		Last Modified: Tue, 04 Oct 2022 23:47:16 GMT  
		Size: 29.7 MB (29650719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e844052b0e573d959a29635a4e114263dc81d516b25fcf80581d7780425f06f`  
		Last Modified: Wed, 05 Oct 2022 03:03:04 GMT  
		Size: 6.2 MB (6205607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd4ea1a131080425a363ecdfbf94864ab4f989718bc2171110c018b35ad6d0b3`  
		Last Modified: Wed, 05 Oct 2022 03:03:04 GMT  
		Size: 2.7 KB (2686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:769d8be98bc28b967cb27671647323e71a8eaee486bf5193f57f1037712ca583`  
		Last Modified: Wed, 05 Oct 2022 03:03:05 GMT  
		Size: 9.6 MB (9572402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f595e22b8386d30f0fada7cb45d01604bbee26d9d5316a4773e52a672a6bb84`  
		Last Modified: Wed, 05 Oct 2022 03:03:04 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
