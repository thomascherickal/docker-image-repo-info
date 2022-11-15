## `rethinkdb:2-bullseye-slim`

```console
$ docker pull rethinkdb@sha256:aa68365c3137ef28b4a7f9a21e67fb2c15a149f3b005af78e52bc6d25f92e369
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:2-bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:47ce162da5b38ab925199f3fdd1afc3cf0f7d6b12d7afcac8d7192cdb9b7a056
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47982287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d316adf0b5e1da7359901f9a7130e119bc49803bdf917b5512065eac8aca1ee`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 14:07:48 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:07:51 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 15 Nov 2022 14:07:51 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 15 Nov 2022 14:07:56 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 14:07:56 GMT
VOLUME [/data]
# Tue, 15 Nov 2022 14:07:56 GMT
WORKDIR /data
# Tue, 15 Nov 2022 14:07:57 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 15 Nov 2022 14:07:57 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c3d907c81a02cec1310ced02ff0e21788dabfc822819b65c93801244172016`  
		Last Modified: Tue, 15 Nov 2022 14:08:13 GMT  
		Size: 6.3 MB (6330161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179f9af0a3d48bd5e3954f27a80863110e0492444666a0af357fba32b0d17c89`  
		Last Modified: Tue, 15 Nov 2022 14:08:12 GMT  
		Size: 2.7 KB (2685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c6640bd3d29e08a2fe912e138f71b54f6b9c8a21d1695240c784a9b2315ad2`  
		Last Modified: Tue, 15 Nov 2022 14:08:13 GMT  
		Size: 10.2 MB (10236684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85868eee933d701f1ebaa6f0ef0fe495a52191e06f12caf07a864ca2cd8cdf8`  
		Last Modified: Tue, 15 Nov 2022 14:08:12 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:b7a9d55b65e588c8cea5d1299d6c8288aea69ec12e98c346bc78beec13078430
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45962666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:593cb8c6863721682f6b1403d9b508371c3c73baa3863a385cc5f5e90936f97a`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:26:18 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:26:19 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 15 Nov 2022 13:26:19 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 15 Nov 2022 13:26:23 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:26:23 GMT
VOLUME [/data]
# Tue, 15 Nov 2022 13:26:24 GMT
WORKDIR /data
# Tue, 15 Nov 2022 13:26:24 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 15 Nov 2022 13:26:24 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28f080479308b0a99b5914a6598c168078a62ee662c43546d7e626551ca592d0`  
		Last Modified: Tue, 15 Nov 2022 13:26:41 GMT  
		Size: 6.3 MB (6310717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de88b0dd01aac73857e8b271674784b6fda7a2f7f75acbb8a0f6d6f11771c1da`  
		Last Modified: Tue, 15 Nov 2022 13:26:39 GMT  
		Size: 2.7 KB (2687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eeb7bd2ff7043cc43bf127e0c0c1c39b53b6e177f9751550b7c51c383ba6dc`  
		Last Modified: Tue, 15 Nov 2022 13:26:41 GMT  
		Size: 9.6 MB (9588532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6837886e49ed64583269d28e6d086a3fd1fcc90052754d650e442e96edfc40b5`  
		Last Modified: Tue, 15 Nov 2022 13:26:40 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:2-bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:8d61e6a04448636df6b008d67da49d31a5dd7b184c34d8933b3f0e8e22194978
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45427152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:920dcae207d248d886e46f471a1df45d38264b4b3d8bd7b8bd5698c4af5c7b72`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 13:12:57 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:13:01 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Tue, 15 Nov 2022 13:13:02 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Tue, 15 Nov 2022 13:13:17 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 13:13:19 GMT
VOLUME [/data]
# Tue, 15 Nov 2022 13:13:19 GMT
WORKDIR /data
# Tue, 15 Nov 2022 13:13:20 GMT
CMD ["rethinkdb" "--bind" "all"]
# Tue, 15 Nov 2022 13:13:21 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca82878636c1029042c47b781420f025156b77aa7453ddfbe5ebe1202674591`  
		Last Modified: Tue, 15 Nov 2022 13:14:03 GMT  
		Size: 6.2 MB (6207349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caeef5425cbe385d2c40f8c2893d1ad59a729991f1b77ec966fa41390476dc9b`  
		Last Modified: Tue, 15 Nov 2022 13:14:01 GMT  
		Size: 2.7 KB (2685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd95a0aec0d2a70d9339d2a6be55e9d11467d680a558e10d1bd7abf3346025d2`  
		Last Modified: Tue, 15 Nov 2022 13:14:04 GMT  
		Size: 9.6 MB (9573210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6479d73bdd6fde3e1987020ea8de9984f546718749c433c07c787043ff9cba9`  
		Last Modified: Tue, 15 Nov 2022 13:14:02 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
