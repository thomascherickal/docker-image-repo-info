## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:93b2752362d6451cbf1d28e2599788c88b73c541f46c0ba84dc73c75a1e00e12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:1ffcc35dc1dfb9751e3339a92471844f54a1b2147c79b4e8a2f45a71137f768d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.1 MB (290073464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bad52367cc0f5c2f3115a8f96c1cb83c0c7bd5fb223d3ff41958867aceb72e3f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 26 Sep 2023 05:03:43 GMT
ARG RELEASE
# Tue, 26 Sep 2023 05:03:43 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 26 Sep 2023 05:03:43 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 26 Sep 2023 05:03:45 GMT
ADD file:5fb49f260a0c3bf404c0fe31d8f0f812e9c143bd48223c4f15a85168758eb880 in / 
# Tue, 26 Sep 2023 05:03:45 GMT
CMD ["/bin/bash"]
# Tue, 03 Oct 2023 05:02:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:03:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 03 Oct 2023 05:07:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:70c34fc37a9391a001a8d99c74b27823143398763bcd623c3402a790006947ea`  
		Last Modified: Tue, 03 Oct 2023 05:09:43 GMT  
		Size: 28.1 MB (28079281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13daebad235cc5fc75272df7a4cd22cd9e14040be8b10d9ec3764328c7be1ab`  
		Last Modified: Tue, 03 Oct 2023 05:09:41 GMT  
		Size: 13.9 MB (13886180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5024b0813f45b8c3c3d60316917bb453d13c81a8bab8316b17b30ac61156c6`  
		Last Modified: Tue, 03 Oct 2023 05:09:58 GMT  
		Size: 44.8 MB (44761138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd79646f814aefe34908af38903a3d5522c9455086876d9b84dda6633503c1d`  
		Last Modified: Tue, 03 Oct 2023 05:10:33 GMT  
		Size: 203.3 MB (203346865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f5236c278618d447f0d4a7ca6ddd91ed9c992bffce41d8e99bf93f1608ea7bcf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.2 MB (250247088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4753d6fb720fba84b8d15fcc9f50f7d25266e94e66b31eb4b7999eafc84a0a25`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:51 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:52 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:57 GMT
ADD file:3b10dde790011a91258183d8ef7e8ed5e24986b2296e00417509565fdfd45e31 in / 
# Tue, 12 Sep 2023 04:43:57 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:43:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:44:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:48:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:901b7210b5b59d80ecd06f3107fe68dbe84f1a47ffd468aa90dd8894057f62b7`  
		Last Modified: Sat, 16 Sep 2023 02:49:15 GMT  
		Size: 26.1 MB (26068467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d3b650c0e7bb6739dbe1082f6637079b42eebc467b66032c563599bf955dffe`  
		Last Modified: Sat, 16 Sep 2023 02:49:14 GMT  
		Size: 12.7 MB (12712685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908b46c2007ad413fc72abfff7e075713078a4875b6d49c60bc3f10db0f1111d`  
		Last Modified: Sat, 16 Sep 2023 02:49:32 GMT  
		Size: 48.9 MB (48948544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db7457b7529fcb766e3bb48db6c4ecaa2dc8e56392815e1267dd158a9953dc71`  
		Last Modified: Sat, 16 Sep 2023 02:50:04 GMT  
		Size: 162.5 MB (162517392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:857fd7d9fc8df6c0e1f1efd945ae48bf52866e87b047f282e82ead03adcf3dba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.1 MB (275141026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b60cdfa078bd6570128790ce5df9ef153c920ce5d1c6729408537148532bfc5c`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:46:07 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:46:08 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:46:08 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:46:15 GMT
ADD file:e7975e06b9483ac7786a825720e46167975054bca8b0679a3c001d143c325fbc in / 
# Tue, 12 Sep 2023 04:46:16 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:08:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:09:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:12:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8e30ad94028d16a73ba211f5c6c54cc5246b12575575b6c44c6c55b6f331994`  
		Last Modified: Sat, 16 Sep 2023 02:13:44 GMT  
		Size: 27.3 MB (27318189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb011cee5097836afefa9b1443d4ca56b7a28b4181bbba91dbe5f98c84c81a49`  
		Last Modified: Sat, 16 Sep 2023 02:13:43 GMT  
		Size: 13.4 MB (13393412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ce9808c41502adb5c86180f08ac4e060e6cbc9e4c1c827ee7806a31f97b48f`  
		Last Modified: Sat, 16 Sep 2023 02:14:00 GMT  
		Size: 44.6 MB (44648234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2928991d7f491a32605af1c80b8db761d5ecaa054fa985a3b7f0714bf0c73b8e`  
		Last Modified: Sat, 16 Sep 2023 02:14:29 GMT  
		Size: 189.8 MB (189781191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1f71bdd516a2efdc8643895e98a188e17280c2370806fafed6db6d5abb8bd229
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.9 MB (297888810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0794fecdbbf1f4e159770525909ef30876ad142c73cbbf4f3d551b2baf93e3b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:43:47 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:43:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:43:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:43:50 GMT
ADD file:56d58cbb4273b81f0c1a0b6eaede82f6a7e5d79c78d54525361f0537566dc9ec in / 
# Tue, 12 Sep 2023 04:43:50 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 02:42:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:43:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 02:49:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd229c9aa7cae185d030f835d891646d81b863cdb9cb773e41f12ee940228d28`  
		Last Modified: Sat, 16 Sep 2023 02:50:16 GMT  
		Size: 32.4 MB (32367087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec9bbd29feb8adb47adfbfa6309c9d863f2e8ec5f80cf30563f27da97167973`  
		Last Modified: Sat, 16 Sep 2023 02:50:12 GMT  
		Size: 15.9 MB (15938863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6f18bc37fc98bef3457686b1b305b6bc6178654b8998f68ee0fa0dcafcf065`  
		Last Modified: Sat, 16 Sep 2023 02:50:39 GMT  
		Size: 49.6 MB (49556244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1894b7a7f0e85a6e7c4c621db0d1f1c5013412f6a53c4eeee37bc1bdbae9268c`  
		Last Modified: Sat, 16 Sep 2023 02:51:39 GMT  
		Size: 200.0 MB (200026616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ec279543b53306f76d3387295112fc765a294b7391bf4bca270d3d7f60731b6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **261.2 MB (261219575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac91242935235eced867e080632d4cb409f2ed1a20edabdb1d955ac90fb12bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 12 Sep 2023 04:45:06 GMT
ARG RELEASE
# Tue, 12 Sep 2023 04:45:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 12 Sep 2023 04:45:06 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 12 Sep 2023 04:45:08 GMT
ADD file:6724cd2c23f7ec57f0524a81125b059327cf367ea1f3387b48c3f642bddc82b9 in / 
# Tue, 12 Sep 2023 04:45:09 GMT
CMD ["/bin/bash"]
# Sat, 16 Sep 2023 01:50:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 01:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 16 Sep 2023 01:53:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ac93ca815ee057f1083e81c9edcf7787c1047a557a07ded971abbb05fa515ca0`  
		Last Modified: Sat, 16 Sep 2023 01:55:18 GMT  
		Size: 27.5 MB (27458487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939194dd385d3eacfbb7f1bf5b9dcc18c16873f21f0cd06b02cceb11343c00ed`  
		Last Modified: Sat, 16 Sep 2023 01:55:16 GMT  
		Size: 14.3 MB (14252767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8e1239553e1d4214fc014d8343ebf58fdaec6f3d8c02336f867a7364d774ff`  
		Last Modified: Sat, 16 Sep 2023 01:55:31 GMT  
		Size: 45.0 MB (45012700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91d0943f80991078d4ba9f41386dc909335f602c9262f1c4c22823cce8e261ad`  
		Last Modified: Sat, 16 Sep 2023 01:55:58 GMT  
		Size: 174.5 MB (174495621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
