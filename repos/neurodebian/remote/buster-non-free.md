## `neurodebian:buster-non-free`

```console
$ docker pull neurodebian@sha256:dc6793856187c9c39c2b66375d0c1c937b962fc9b4763e6aef88513c6022b0a4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `neurodebian:buster-non-free` - linux; amd64

```console
$ docker pull neurodebian@sha256:328b5eade2581994ea8a93d00f30594ac1654d1f41755a825464613a109677dc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61306989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0384483cda04a7d15823f8140de13eef8410dc29c4509077931167c9a24b790b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:21:00 GMT
ADD file:e5e3f2fedf4fa6382f3bbf6203060ba68df1aadc7ebfa3350df20bf31b102f0e in / 
# Tue, 19 Dec 2023 01:21:01 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 17:25:27 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:29 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 17:25:29 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 17:25:33 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 17:25:38 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:30b73a2ffaab3c39355a8bcc5eae8ba1465bd7d9467f197b91f7635816b16bc9`  
		Last Modified: Tue, 19 Dec 2023 01:25:58 GMT  
		Size: 50.5 MB (50500409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ab53549f1d6f91ce1fcfb5a6ff812ebeca69b02bd07cbe6a1ae8df426ca90a4`  
		Last Modified: Tue, 19 Dec 2023 17:27:13 GMT  
		Size: 10.5 MB (10504778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e731abcc54cf5bcb086bc36b1e6f12ad7d73ca0f0139f4a0070a16d1bb6105a`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 1.8 KB (1766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9f5821293636913a5e5f156fde6c19fb62901cbcf38d66898b3154b4222b9e4`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d2c8d395609db22d85da949ac48af56210ff29e74765f2ae4f6f3dd8007e73c`  
		Last Modified: Tue, 19 Dec 2023 17:27:12 GMT  
		Size: 299.4 KB (299435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420d51671fd62d4e126c31d4831df03a8ab2acf080c8bc83a8eb772760dedd0b`  
		Last Modified: Tue, 19 Dec 2023 17:27:23 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; arm64 variant v8

```console
$ docker pull neurodebian@sha256:f764445ceab408a8b33ff6e0e70255f357997da4ad5c15da095c4619d3778441
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60101398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97bca1e9bfe9bfa37e72929b0e193a720d329783d7289784ea929d1b75eb5ac9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:41:31 GMT
ADD file:df5e5dd39efc6ae3cc9132f6ca6bb569731f7a37cf4b41f87bcb7aa1ba9771e8 in / 
# Tue, 19 Dec 2023 01:41:32 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:05:48 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:05:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:05:53 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:05:57 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:93507f9712ced9fbfd0d0f689cf7b55fb245cef88530c07ac5dc5cad20fa889d`  
		Last Modified: Tue, 19 Dec 2023 01:45:40 GMT  
		Size: 49.3 MB (49289026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c5fbc51c74a4f8750f148252ed129c0c57cc94d6e2b2f4ae83d5f1420fe9a2`  
		Last Modified: Tue, 19 Dec 2023 03:07:17 GMT  
		Size: 10.5 MB (10510551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7d0a1a828eff413800cec078c31256371b964ca8aa29198aea52bf930d8057`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 1.8 KB (1769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26dd41deea093d7e81d0007ed35420760c6cea45b552f575b45ee9e400eb7beb`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533e3cd401bcc7d93489b3ef17afb87ed22d96e3b19fb76fa2dfc90ee457c0c0`  
		Last Modified: Tue, 19 Dec 2023 03:07:16 GMT  
		Size: 299.4 KB (299449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134eef9048535ffd6796b146e362f4919bd2130d2183feda6ba05db3dcd4df96`  
		Last Modified: Tue, 19 Dec 2023 03:07:25 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `neurodebian:buster-non-free` - linux; 386

```console
$ docker pull neurodebian@sha256:8b36bd35183e06994e6a3ecff588a4906eca28d78ca5cb4e9f15047484150f83
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62425602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3995db1af7a67fbcd53860257fab3e0fcf305561c0d2bb8d86093d9000fcf4fe`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 19 Dec 2023 01:39:40 GMT
ADD file:4c009b0d408e3df297246382d87b0be68c34886e13ed79ba47feb8ff51acb863 in / 
# Tue, 19 Dec 2023 01:39:41 GMT
CMD ["bash"]
# Tue, 19 Dec 2023 03:50:47 GMT
RUN set -x 	&& apt-get update 	&& { 		which gpg 		|| apt-get install -y --no-install-recommends gnupg 	; } 	&& { 		gpg --version | grep -q '^gpg (GnuPG) 1\.' 		|| apt-get install -y --no-install-recommends dirmngr 	; } 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:50:49 GMT
RUN set -x 	&& export GNUPGHOME="$(mktemp -d)" 	&& gpg --batch --keyserver keyserver.ubuntu.com --recv-keys DD95CC430502E37EF840ACEEA5D32F012649A5A9 	&& gpg --batch --export DD95CC430502E37EF840ACEEA5D32F012649A5A9 > /etc/apt/trusted.gpg.d/neurodebian.gpg 	&& rm -rf "$GNUPGHOME" 	&& apt-key list | grep neurodebian
# Tue, 19 Dec 2023 03:50:50 GMT
RUN { 	echo 'deb http://neuro.debian.net/debian buster main'; 	echo 'deb http://neuro.debian.net/debian data main'; 	echo '#deb-src http://neuro.debian.net/debian-devel buster main'; } > /etc/apt/sources.list.d/neurodebian.sources.list
# Tue, 19 Dec 2023 03:50:54 GMT
RUN set -x 	&& apt-get update 	&& apt-get install -y --no-install-recommends neurodebian-freeze eatmydata 	&& ln -s /usr/bin/eatmydata /usr/local/bin/apt-get 	&& rm -rf /var/lib/apt/lists/*
# Tue, 19 Dec 2023 03:51:00 GMT
RUN [ -e /etc/apt/sources.list.d/debian.sources ] && srcs=/etc/apt/sources.list.d/debian.sources || srcs=/etc/apt/sources.list; sed -i -e 's,main *$,main contrib non-free,g' /etc/apt/sources.list.d/neurodebian.sources.list $srcs
```

-	Layers:
	-	`sha256:8d351f5ab6958b8ca5f2b8e463c49cba65be4285ead8bdbc1378b5ce2c8cd736`  
		Last Modified: Tue, 19 Dec 2023 01:44:53 GMT  
		Size: 51.3 MB (51255444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01ee695ce5b07c4aa0b90a93605547e631e728141c311b4bbf7c54fdac3be4`  
		Last Modified: Tue, 19 Dec 2023 03:52:23 GMT  
		Size: 10.9 MB (10868372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1379f0dec32e0488edb8bff0dcd0be9abb4c04675943257bc5c784bfd82fd870`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 1.8 KB (1768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f56e62a0bf8c627e0bfa8f075fdfdcabfd6fc8d4809a1ec507a91d81eec6c13a`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f016555c3e2050965be5f7aece4aa1a93943629cdaa4359707eb76a9fac47534`  
		Last Modified: Tue, 19 Dec 2023 03:52:21 GMT  
		Size: 299.4 KB (299418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956c541ecb88d435c686202fe372734189b393a6e7af060a508bd5cc94110ecf`  
		Last Modified: Tue, 19 Dec 2023 03:52:31 GMT  
		Size: 356.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
