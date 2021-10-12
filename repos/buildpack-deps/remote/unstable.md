## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:cd1267f36a74ad2cf883585b8c4952aaad6e261e4a2e92fd84afa26625aa05e3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ac086300ddd307bf8d8dbc2c861f4f5b07bd621a0e49275b4c7dea1e9d02297f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **490.7 MB (490675845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5ec41b4e074440558fb7be1e3339957ea686fcb7916ca004c0590be9b145680`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:21:58 GMT
ADD file:2d684471f088173801ff86eaf94c1d858b74220b84642d73b02bd1bfe0d54b60 in / 
# Tue, 12 Oct 2021 01:21:58 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 15:46:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:46:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 15:47:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 15:48:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ba87283d9c312600aafb7f4149986884d524aae42e0701a90d2fc23c85e977b1`  
		Last Modified: Tue, 12 Oct 2021 01:28:21 GMT  
		Size: 55.7 MB (55687470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bcf62d5f60a89ffe69fdffb6f89c02e782fc35bf8d5766b9e4d46ebc82278a`  
		Last Modified: Tue, 12 Oct 2021 15:55:24 GMT  
		Size: 5.2 MB (5216552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:669cb549c6380d94ce53b7413b60cfab218aebd91bdcfc6c970d908b333925a8`  
		Last Modified: Tue, 12 Oct 2021 15:55:25 GMT  
		Size: 10.9 MB (10900892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a4cbc1206c2266ee34ccdeb1d5e8209dbeeff0f65a52a3af81a6c46546f37a0`  
		Last Modified: Tue, 12 Oct 2021 15:55:44 GMT  
		Size: 55.7 MB (55734443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99b8abfbeaa8e98eed9751a16720fc738ed4d9326a9ca215d6d43089aeef9301`  
		Last Modified: Tue, 12 Oct 2021 15:56:56 GMT  
		Size: 363.1 MB (363136488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:215a46aa6f638cf9e220fab73f63e86e8bfab8c61cfd70685dbda87356f34fa8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **474.9 MB (474871327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd2a73342dfad8a3515950c7aab1d759d8165ed5f42f656523b75f8e7b6ef43a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:53:53 GMT
ADD file:2918872df07d47b9a7862abf3b22f39600ab45587fcd02466bdefa775a3fc2dd in / 
# Tue, 12 Oct 2021 00:53:54 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:49:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:49:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 05:50:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:53:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8f73c109c91bd2f18faab4d6862ba33d940956d6457aaaaeeda5e8f72281edcc`  
		Last Modified: Tue, 12 Oct 2021 01:11:00 GMT  
		Size: 53.2 MB (53186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd99c7b364b1329f3fc27bcb8d50810c30d8a7928b7518c93f2d538a1124daa0`  
		Last Modified: Tue, 12 Oct 2021 06:07:28 GMT  
		Size: 5.1 MB (5122384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8779df359e844ab400aaeab5d2001cf6d805ff10af17660fd4577296ecbf7f9`  
		Last Modified: Tue, 12 Oct 2021 06:07:30 GMT  
		Size: 10.6 MB (10606788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83014d4ab58f54e38e974b2de48f1a41a6bee268a7b6ebb1050582b1d782db1b`  
		Last Modified: Tue, 12 Oct 2021 06:08:20 GMT  
		Size: 53.4 MB (53442505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4af54fd52817c8dff8e7fb1fb4b62845da3ed7da902c46ad93c9210945460647`  
		Last Modified: Tue, 12 Oct 2021 06:11:57 GMT  
		Size: 352.5 MB (352513298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1b627f4c0635c1c28c94a70b9966a8f78641fa3cc43e12f8a5e8242198ceb835
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **446.1 MB (446050738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2b6e007ca966f71cc422f797443fe2df3a46134f168b554625ada0823ab2c72`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:32:13 GMT
ADD file:defbc06b1cc21db01a673f118d34d129435486fcb83814c5c987ff566c61360a in / 
# Tue, 12 Oct 2021 01:32:14 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 18:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:43:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 18:44:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 18:47:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:153dc8e6452cda134a8143d2ac887e7ebfa01c8568115d6b3172ca0008ef4838`  
		Last Modified: Tue, 12 Oct 2021 01:49:06 GMT  
		Size: 50.8 MB (50797066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58bc8cfd03a1c715f9702494a8f0c4599bf04e51f4a7094befc758068725b5db`  
		Last Modified: Tue, 12 Oct 2021 19:02:43 GMT  
		Size: 5.0 MB (4984307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7905528e1493cb4119aa69a5a20f43d64dc225128ef6308ed4a2ea77a1684b7d`  
		Last Modified: Tue, 12 Oct 2021 19:02:45 GMT  
		Size: 10.2 MB (10249876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87677333086e2dfb5a81ca8e8c60b5923e629e363255c0419e6b467f805c4500`  
		Last Modified: Tue, 12 Oct 2021 19:03:18 GMT  
		Size: 51.4 MB (51378224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bd6a1fc0c89aa5d1c3ed4391182e8317a5dd70d987225ceb8e6a79ee690a7b`  
		Last Modified: Tue, 12 Oct 2021 19:06:32 GMT  
		Size: 328.6 MB (328641265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7c2154de1988c62f561d9d754cfb077450d5ce27728dfcb6f8d60732e14f6515
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **484.0 MB (483966477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc267e57c84623f4c55b1ce856ec59fdd97c994bec2168ec3276a3d19c58932a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:36 GMT
ADD file:830671e1709a0164ca60ad1012d3d0202e7e63c74bdbec7df54f308a4d4c8b11 in / 
# Tue, 12 Oct 2021 01:42:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:12:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:13:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:13:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:14:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ed37bc205e0aad196bfd6ba235a1a5fba10e02175afd192c816df6457d06c75`  
		Last Modified: Tue, 12 Oct 2021 01:50:51 GMT  
		Size: 54.7 MB (54702895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9e12eb84409ba3f2dbf96f9e720e1db75055189af4f9c412b3be39768c371b5`  
		Last Modified: Tue, 12 Oct 2021 02:21:19 GMT  
		Size: 5.2 MB (5205920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39f86ea1fa7d211d3c24d9f11b0ad622d344241f5f4288b575d09a0e038e903`  
		Last Modified: Tue, 12 Oct 2021 02:21:19 GMT  
		Size: 10.9 MB (10899227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82855758df584636866eabeef61f652a1b64eb39037aa2155d68f7d9cfb5dae4`  
		Last Modified: Tue, 12 Oct 2021 02:21:40 GMT  
		Size: 55.9 MB (55881502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5074f546e2f5bb7f1e16ccafd4aaee5a6240a7e26d7a9dad19e6d213377fa897`  
		Last Modified: Tue, 12 Oct 2021 02:22:41 GMT  
		Size: 357.3 MB (357276933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4ea2edd31669732d12dce321d6928127ffbe9073c24d96085b9ca44c2933bfab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.4 MB (332367435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ea23a81b9c83e610134b648dd92aba29502de7ae1aa419876e7ab76976e253a2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:27 GMT
ADD file:9ab0c16547aac0a32292246b35737ca5260c5942d5e26ca1381be39c9e321ee5 in / 
# Tue, 12 Oct 2021 01:41:27 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:40:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:40:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:42:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c36fe1aa4217cf0326227a0bdcadc16e85d2670bd6485518167903dfc6934c65`  
		Last Modified: Tue, 12 Oct 2021 01:50:33 GMT  
		Size: 56.7 MB (56716103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1cefa3abf3c8d9687bfe164fbd73be6245f1e0c523603077cfcffd5881a3778`  
		Last Modified: Tue, 12 Oct 2021 04:51:12 GMT  
		Size: 5.3 MB (5346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902f94685b9ef6228bbe2d7c552fb6d02ea5e723469df5c9e980d102fd9c6aa2`  
		Last Modified: Tue, 12 Oct 2021 04:51:13 GMT  
		Size: 11.3 MB (11281973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802e1fd067f1198f877ff5bc97afd5870c21a28609a1919a09063ff8aacf5fd4`  
		Last Modified: Tue, 12 Oct 2021 04:51:37 GMT  
		Size: 57.2 MB (57159249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ecb28b33acfca8e5784c5c3b85c0efb3eeb8d08971fe4e1e1dee2cc768ee8d`  
		Last Modified: Tue, 12 Oct 2021 04:52:26 GMT  
		Size: 201.9 MB (201863866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e6343e56bba09935f72a10d828c77a50eeffe9aac2e36e94fb151fde5e8717d9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.5 MB (547497141 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0d641cbbca8576a6e14aaa72bb411e2c5ec8d1ec56e6586a2b51767dd8dbaa5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:13:27 GMT
ADD file:27e1d46380432bbd287bef3c049b6707a409fa2f49f07e76f4826c6ee57cfca9 in / 
# Tue, 12 Oct 2021 01:13:28 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:58:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 01:59:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:04:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7afe2e09744237d99a12c5f86f33ba55800e5acee482662abac2c64c64a7824`  
		Last Modified: Tue, 12 Oct 2021 01:23:41 GMT  
		Size: 54.3 MB (54313468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f8be3dfdc1ee7ccf4465ff4d91c782f9ad2d795bd9ea4965953382190a5626`  
		Last Modified: Tue, 12 Oct 2021 02:11:44 GMT  
		Size: 5.2 MB (5177464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f028726b389731d6d9e30d4ef26719ac3a44889d1bd0681ebbf11f085178373`  
		Last Modified: Tue, 12 Oct 2021 02:11:46 GMT  
		Size: 10.9 MB (10904218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2076aaf953f38208fdacaa4098bb05224c1ede12a74b5ecee28db74cfd04ac8`  
		Last Modified: Tue, 12 Oct 2021 02:12:36 GMT  
		Size: 54.5 MB (54529853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14acf8037da3046701b0f2294ae0913b78f9605322ccffcd438b1dc7cef1fc2e`  
		Last Modified: Tue, 12 Oct 2021 02:17:01 GMT  
		Size: 422.6 MB (422572138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e60b1558dd3a10adab3fad32c228cdf1431263d739fd550a5e143f77f21ac418
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.7 MB (488667599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95c92c445909404fef5ff33ea7b1175f6633df51002d7d090cc4d6549e44ba1c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:27:58 GMT
ADD file:975422ef5390ff94fc050a84a9840e39188158f1c74f7b6dfde93829787b7c8d in / 
# Tue, 12 Oct 2021 01:28:07 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 04:23:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:24:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 04:26:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 04:38:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3794e49fdef56187e1a7ffe8a3c0d0dda8a5b5c159e370831000df5e5f638479`  
		Last Modified: Tue, 12 Oct 2021 01:41:02 GMT  
		Size: 59.9 MB (59889168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3a771c64c6b854d6abde14ad239e8808ef66674301b6a066df68b719b9ef04`  
		Last Modified: Tue, 12 Oct 2021 04:44:22 GMT  
		Size: 5.5 MB (5468996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c1a4272fe59063922ad53af8014c08c537807fbc8a6fe125f51be34de8ffc53`  
		Last Modified: Tue, 12 Oct 2021 04:44:23 GMT  
		Size: 11.7 MB (11654490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97493787213daeca4485b87abed722776481493a73f647e2d70fc24c1d0efd7`  
		Last Modified: Tue, 12 Oct 2021 04:44:45 GMT  
		Size: 60.2 MB (60156002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e1fc7af67bffe540cb01493036e43dc24e5f55cbc25d530a9124d1cd2885a8a`  
		Last Modified: Tue, 12 Oct 2021 04:45:55 GMT  
		Size: 351.5 MB (351498943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:63c49a2c53224cab678ffc29c6ee17d58a43db77a7e66f7a6bc8b7626de435a4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.8 MB (341833159 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52b2d003ab60510328227198c5d40fb77f205c48512887e672d581d6ed58e139`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 01:14:22 GMT
ADD file:bd71d5680d1006cf090b0a295547cb405dc17469df91f3492267dbd5019f25c5 in / 
# Tue, 12 Oct 2021 01:14:25 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 01:56:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 01:57:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:01:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:10:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6f088a81a8bb9ab030ef8f6d37a5e280f5ad79eaf2817310f6498ffe43ca2dac`  
		Last Modified: Tue, 12 Oct 2021 01:30:29 GMT  
		Size: 51.5 MB (51516608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f3fde059905204e836dc3ffbe360b638f58c8c7dc954c038d591b1859643368`  
		Last Modified: Tue, 12 Oct 2021 02:34:36 GMT  
		Size: 5.0 MB (5032271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1ba22ae6fbd86a3c7aed8e1c6ec2a2f1af7f4893efe5133d85c145066a77f8`  
		Last Modified: Tue, 12 Oct 2021 02:34:39 GMT  
		Size: 10.3 MB (10314713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173a27bd17e1f1571ed8f4073a4e420529a44ded0e627650b24d0a2cefa08d6f`  
		Last Modified: Tue, 12 Oct 2021 02:36:46 GMT  
		Size: 51.8 MB (51789956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002ea648c32057975389dfba877c4f59f3ad6fa847aa6071ff79509b20a93458`  
		Last Modified: Tue, 12 Oct 2021 02:42:43 GMT  
		Size: 223.2 MB (223179611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f0ec22f2499a2116aba4b111588f864f83581251e3ee8f1d43805723e7027576
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **444.8 MB (444786780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:725fd78f16a2dafb018507e091a464c2cfa0213df23fd1b7b2db32dc08e43338`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 12 Oct 2021 00:43:35 GMT
ADD file:d0d1a83115052a10810bdba27eb855359796f604b655de31492b0699abf1d546 in / 
# Tue, 12 Oct 2021 00:43:38 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:43:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:43:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 07:43:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 07:44:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:979a8d8677c5949943057dfc51bfa612e3d365d71df4150210296bec00f04cf2`  
		Last Modified: Tue, 12 Oct 2021 00:49:29 GMT  
		Size: 53.9 MB (53940740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b2ee0930fe303c9ea2baf728cca61c84ba351c6472da4fd5385e62530f6673`  
		Last Modified: Tue, 12 Oct 2021 07:50:03 GMT  
		Size: 5.2 MB (5199342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92727346c90e0492705828b0c21131c81b3b275773725847689d7cb0a15efa57`  
		Last Modified: Tue, 12 Oct 2021 07:50:03 GMT  
		Size: 10.8 MB (10793861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe0ed031f749a2507ced21f398da3825f07398298d2a33454410b1e09d37b82`  
		Last Modified: Tue, 12 Oct 2021 07:50:19 GMT  
		Size: 55.2 MB (55166037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c40fe887960fd64e2ab3b8de4a6869a4754bc634e4c331ef041a3068a6ab7aa`  
		Last Modified: Tue, 12 Oct 2021 07:51:00 GMT  
		Size: 319.7 MB (319686800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
