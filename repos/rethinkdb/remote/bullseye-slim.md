## `rethinkdb:bullseye-slim`

```console
$ docker pull rethinkdb@sha256:ba11265be5459da6e6008df91f6992e8409527e2e937d631bae2a373eba8c5bf
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
$ docker pull rethinkdb@sha256:88342bf62ee52b14e3aacd16cd0836248d72be34df78bc7510d97a3ff50152d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45737528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87d1b48df760e17172198b76562bf7892eb7c008e03e8619f0d6d9ea70062ff0`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 13 Sep 2022 02:10:56 GMT
ADD file:e8f00260a993aacae732bef51e6074b6c064d50a8ce1f0c44d53fe9e3c868e43 in / 
# Tue, 13 Sep 2022 02:10:56 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 12:54:41 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:54:43 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 13 Sep 2022 12:54:44 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 13 Sep 2022 12:54:49 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 12:54:49 GMT
VOLUME [/data]
# Tue, 13 Sep 2022 12:54:50 GMT
WORKDIR /data
# Tue, 13 Sep 2022 12:54:51 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 13 Sep 2022 12:54:52 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3d898485473e3507374cea2e09f019c2ff5728f0911aa36c70b7a7235e9bc8ac`  
		Last Modified: Tue, 13 Sep 2022 02:16:19 GMT  
		Size: 30.1 MB (30054239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdb798efcdcaae74f91bcb0ace60426a35282030913bf7275c3deca829dffaaa`  
		Last Modified: Tue, 13 Sep 2022 12:55:18 GMT  
		Size: 6.3 MB (6308354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf5428c08948c61a4e31a351f288b3c521e35ff08c841b2c366d6d532769e70`  
		Last Modified: Tue, 13 Sep 2022 12:55:17 GMT  
		Size: 2.7 KB (2670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a37601cf141f7fabbd2762548457a870c51364e5e3fc245e992f820ef90ecc`  
		Last Modified: Tue, 13 Sep 2022 12:55:18 GMT  
		Size: 9.4 MB (9372172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0f90a8ee3ced5331433eb37004438abfdfcf41fd0bbad320481c56aabf909c`  
		Last Modified: Tue, 13 Sep 2022 12:55:17 GMT  
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
