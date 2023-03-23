## `rethinkdb:bullseye-slim`

```console
$ docker pull rethinkdb@sha256:cbe93b22332076a16485a4c932035a561baa93eceefda2e5e2a1125ea0a36e9e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; s390x

### `rethinkdb:bullseye-slim` - linux; amd64

```console
$ docker pull rethinkdb@sha256:f2bab4f667cf39ee9577ca292bd85aa200bc58c102f0d6d599d8daf1a994f4b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47978749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a91f3e5a27e9a583b667e75827f9277713fbd67a8147dd1a22eb5f1fa6680384`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Wed, 01 Mar 2023 04:09:58 GMT
ADD file:493a5b0c8d2d63a1343258b3f9aa5fcd59a93f44fe26ad9e56b094c3a08fd3be in / 
# Wed, 01 Mar 2023 04:09:59 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 16:47:29 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:47:31 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Wed, 01 Mar 2023 16:47:31 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Wed, 01 Mar 2023 16:47:36 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 16:47:37 GMT
VOLUME [/data]
# Wed, 01 Mar 2023 16:47:37 GMT
WORKDIR /data
# Wed, 01 Mar 2023 16:47:37 GMT
CMD ["rethinkdb" "--bind" "all"]
# Wed, 01 Mar 2023 16:47:37 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:3f9582a2cbe7197f39185419c0ced2c986389f8fc6aa805e1f5c090eea6511e0`  
		Last Modified: Wed, 01 Mar 2023 04:14:23 GMT  
		Size: 31.4 MB (31411403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcdb5586b0fe92f1ed8dbddcd64dc35b4d59695d5d70acf9efd562e93521f05c`  
		Last Modified: Wed, 01 Mar 2023 16:47:52 GMT  
		Size: 6.3 MB (6328659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387899c9513e847717d1f3889e5f52eb106e5a607c9a0036dad051855b0d36ab`  
		Last Modified: Wed, 01 Mar 2023 16:47:51 GMT  
		Size: 2.7 KB (2689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76fd507bf127647bf96226177270c6158d50514db5f458d363b39fc9c3e953f3`  
		Last Modified: Wed, 01 Mar 2023 16:47:53 GMT  
		Size: 10.2 MB (10235871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01eab8e58b9a37fe9704ba3d5cfc2f2c6413e63f2addcadc9e459ffe94d3a18`  
		Last Modified: Wed, 01 Mar 2023 16:47:51 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; arm64 variant v8

```console
$ docker pull rethinkdb@sha256:d7a7862b005937d3d2ff3c47e9430616677f88e9c758fa087c9859b57251bd8d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45962971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89a07126fc874e8e37ba5041f3bf742198d9eb544d73aff3b8e0fbfd6475c2cb`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 13:33:05 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:33:07 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Thu, 23 Mar 2023 13:33:07 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Thu, 23 Mar 2023 13:33:11 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 13:33:11 GMT
VOLUME [/data]
# Thu, 23 Mar 2023 13:33:12 GMT
WORKDIR /data
# Thu, 23 Mar 2023 13:33:12 GMT
CMD ["rethinkdb" "--bind" "all"]
# Thu, 23 Mar 2023 13:33:12 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f3ec32e426cf36bfcb4aa57ed833ba9f346c7194cc3785f5b522a35cbe60f0`  
		Last Modified: Thu, 23 Mar 2023 13:33:22 GMT  
		Size: 6.3 MB (6309593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4906ad52735c52892ebb663d87553a4b7772f9578df91ce36b2aa018a3c5d5f9`  
		Last Modified: Thu, 23 Mar 2023 13:33:21 GMT  
		Size: 2.7 KB (2687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efee4e4091573c0d24619252d87dac1e07a863fedba2ffe85ebe9c3fb521f71`  
		Last Modified: Thu, 23 Mar 2023 13:33:23 GMT  
		Size: 9.6 MB (9587864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f679f5c7ecc00aad9c88535466daae9704a425c1254e515d59f987dd35f6bf7d`  
		Last Modified: Thu, 23 Mar 2023 13:33:21 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `rethinkdb:bullseye-slim` - linux; s390x

```console
$ docker pull rethinkdb@sha256:2306337e98d128151ee244a82fca676574875f4b8310b78db3acd51036ad5c56
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45427627 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb15e9f9db0a09b139d9655fb466e824e8a2e7a02f0a48e60ae830c4c3c20550`
-	Default Command: `["rethinkdb","--bind","all"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 10:58:43 GMT
RUN apt-get -qqy update     && apt-get install -y --no-install-recommends ca-certificates gnupg2 curl     && rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:58:45 GMT
RUN GNUPGHOME="$(mktemp -d)" && export GNUPGHOME     && gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F     && gpg --batch --export 539A3A8C6692E6E3F69B3FE81D85E93F801BB43F > /usr/share/keyrings/rethinkdb.gpg     && gpgconf --kill all && rm -rf "$GNUPGHOME"     && echo "deb [signed-by=/usr/share/keyrings/rethinkdb.gpg] https://download.rethinkdb.com/repository/debian-bullseye bullseye main" > /etc/apt/sources.list.d/rethinkdb.list
# Thu, 23 Mar 2023 10:58:45 GMT
ENV RETHINKDB_PACKAGE_VERSION=2.4.2~0bullseye
# Thu, 23 Mar 2023 10:58:50 GMT
RUN apt-get -qqy update 	&& apt-get install -y rethinkdb=$RETHINKDB_PACKAGE_VERSION 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 10:58:50 GMT
VOLUME [/data]
# Thu, 23 Mar 2023 10:58:51 GMT
WORKDIR /data
# Thu, 23 Mar 2023 10:58:51 GMT
CMD ["rethinkdb" "--bind" "all"]
# Thu, 23 Mar 2023 10:58:51 GMT
EXPOSE 28015 29015 8080
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3aed9d481c542a740b2c8e56ea676c8e36287662a1f86328f922a911d84aa04`  
		Last Modified: Thu, 23 Mar 2023 10:59:05 GMT  
		Size: 6.2 MB (6205551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614dd6e152fb9882a78a575b0b60b148686dd07492e8d112db9c9f7dd261cd0e`  
		Last Modified: Thu, 23 Mar 2023 10:59:04 GMT  
		Size: 2.7 KB (2688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1a42e543e089a5caa0189a342dd297fc5947383a1b18fc0b52913ef8147938`  
		Last Modified: Thu, 23 Mar 2023 10:59:05 GMT  
		Size: 9.6 MB (9572441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81c5650023f39967775c03498462d0614a8de6073e01cda8f6581f8d4e0a2cac`  
		Last Modified: Thu, 23 Mar 2023 10:59:04 GMT  
		Size: 127.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
