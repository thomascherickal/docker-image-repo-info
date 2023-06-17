## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:b56d7340cb3b6fd842e7f4c0d11ee03b9f162872f879ff54300012adc838d772
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:2f4e9d3f72d606f771c9802db9a0050c171903dbb877df6758f2d4ec407d26de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262679015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562a717e0775af1594514720e96eaab6ef8d92ed71375f11868402c17bee8a51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:32 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:32 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:32 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:34 GMT
ADD file:f8bb312bf73c62343d91c9988d58945c5d0fced3f559b95c4dd21a19183d933d in / 
# Mon, 05 Jun 2023 17:02:34 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:42:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:43:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:46:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6cee4c55bd500a2c4a00a5b79538d4485726955d83a652dd23d53199e149efe2`  
		Last Modified: Fri, 16 Jun 2023 01:55:57 GMT  
		Size: 27.5 MB (27488513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6b0fb7f48d56947f4fb88d70beb688a4862300af9ea9a03aa6ebadbbe71f7e`  
		Last Modified: Fri, 16 Jun 2023 01:55:54 GMT  
		Size: 14.2 MB (14189181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ba1ce9eba0b87729fedba113ddd4bdfd7d207c68be455662273a0474087524`  
		Last Modified: Fri, 16 Jun 2023 01:56:11 GMT  
		Size: 39.8 MB (39826083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2be209e7f6d8da4f469613de2615cbbb9eec09d725bec6820e7e2ea07b686cd`  
		Last Modified: Fri, 16 Jun 2023 01:56:42 GMT  
		Size: 181.2 MB (181175238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5a0e3190f4797c653b64a5ada58cca4c7d7c51393da330657b42a57be361c758
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **225.6 MB (225643211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c971316c51d84b7629d0ee714201e00fd8badf236989425ebe8a8652dca019e9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:04:06 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:04:06 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:04:06 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:04:07 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:04:15 GMT
ADD file:615be72e62c21704af356d6cfd4e32a7df8dd4b93d0c3ee3ea2e1641127c54ea in / 
# Mon, 05 Jun 2023 17:04:16 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 00:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:46:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 00:48:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4bf34fad731c68e9e2b3f1ab9be267f88256224d876e0b36cd63ff42fe27225a`  
		Last Modified: Fri, 16 Jun 2023 00:58:56 GMT  
		Size: 25.9 MB (25914047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d88eb5459ee9fba90e6dc257e7e3002bdb40e23d679a15bf566ec317a366bb`  
		Last Modified: Fri, 16 Jun 2023 00:58:55 GMT  
		Size: 13.1 MB (13141250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1ff3680907d768021e43095ea76751da3011e63414be63b980806f2ce05d85`  
		Last Modified: Fri, 16 Jun 2023 00:59:12 GMT  
		Size: 42.9 MB (42939688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6670329fbb184599c497ba2d8d363a214cabaa75b7a5a5e42f9ccedce6f890c`  
		Last Modified: Fri, 16 Jun 2023 00:59:40 GMT  
		Size: 143.6 MB (143648226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:6450ff70dcc21517fbc43c36e1403f23201fc063bfb31ddd4ae29d7145bcabdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.4 MB (250437571 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c2da83b8414125b33d5003d9771ce420145e2fd5585f640167dc976a13b1ff0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:02:45 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:02:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:02:45 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:02:46 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:02:50 GMT
ADD file:b85182b4593c262faef116755e01baa608e8090e1cb697d735485ff0bd5b353e in / 
# Mon, 05 Jun 2023 17:02:50 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 02:20:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:21:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 02:24:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d08ab8ea3b2755ec06aa9ce6972e64da08c79b30281c9416cac92b6aa23a7d8`  
		Last Modified: Fri, 16 Jun 2023 02:34:35 GMT  
		Size: 26.7 MB (26727371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11fa3a4a444d42bc471027a78d4e890bb44584c98f6160625eb80e66f566049`  
		Last Modified: Fri, 16 Jun 2023 02:34:32 GMT  
		Size: 13.7 MB (13727198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b51bbb1bce4e9d99daf88e47964d3e6228a1af3e8c83e9aa282d385788830cfa`  
		Last Modified: Fri, 16 Jun 2023 02:34:48 GMT  
		Size: 39.6 MB (39635989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78020169d5bc399fc192babbe604c93257a5d2b7bc02c0acdbdc705dadc1a8ed`  
		Last Modified: Fri, 16 Jun 2023 02:35:12 GMT  
		Size: 170.3 MB (170347013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:560b753c45abb5240352793e87c207f2b7e7df112cc1a485e0dd61eafb4e0165
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **285.6 MB (285554093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35c7c5998bfdf0245d01fccce28b49135ec0c9882da781f51876d06f8c9349c5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:48 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:48 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:48 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:52 GMT
ADD file:48c30fe281554302bb6533dd33a43a0877851ac5ba59dc3aff3d3d9ceae6f8a9 in / 
# Mon, 05 Jun 2023 17:10:52 GMT
CMD ["/bin/bash"]
# Fri, 16 Jun 2023 01:04:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:05:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 16 Jun 2023 01:10:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e97b48410348d002f0aaa3d5e7df14543cadcf78a962c446f311040094d1348`  
		Last Modified: Fri, 16 Jun 2023 01:27:17 GMT  
		Size: 32.1 MB (32102208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf4d9ebe87a9f4a30cb3454f9146c64bf5f745c3afc33b5ef9066928de29bc3`  
		Last Modified: Fri, 16 Jun 2023 01:27:13 GMT  
		Size: 16.2 MB (16234116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb051abeb64dceef5e8138c11b37546238818695904b8b144a607f81964871d4`  
		Last Modified: Fri, 16 Jun 2023 01:27:38 GMT  
		Size: 44.2 MB (44231490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b846c5134e1fa6226c7da97a84a2a2bf1a9aa146e918f292b298821c487aa8`  
		Last Modified: Fri, 16 Jun 2023 01:28:33 GMT  
		Size: 193.0 MB (192986279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b122cbd93966173e324bed10b46003a1499a6fa1f099086cb4514d10db4dd748
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **233.1 MB (233062462 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2471e1864b14d7637a2a024b934f1ef936d7f8d40a147e9141f5da52deafe111`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 05 Jun 2023 17:10:49 GMT
ARG RELEASE
# Mon, 05 Jun 2023 17:10:49 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 05 Jun 2023 17:10:49 GMT
LABEL org.opencontainers.image.version=22.10
# Mon, 05 Jun 2023 17:10:51 GMT
ADD file:2390e4c5ac4f862cf5fb266c70962a01f271fa692b74af886f18911482025825 in / 
# Mon, 05 Jun 2023 17:10:51 GMT
CMD ["/bin/bash"]
# Sat, 17 Jun 2023 09:50:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:50:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 17 Jun 2023 09:52:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45d37589c642f2585803ed2ba24d2b897920c885c7a913bb399e12a2410d5503`  
		Last Modified: Sat, 17 Jun 2023 10:01:25 GMT  
		Size: 26.0 MB (26034488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d10ce8336984e795efd05d14a13611a92ef77b199d749859036bd37fbbf18040`  
		Last Modified: Sat, 17 Jun 2023 10:01:24 GMT  
		Size: 14.3 MB (14344562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f89ec5257613dfb7e6ac3731cf008ae93397126d7d27b80d7d9e63428331cd`  
		Last Modified: Sat, 17 Jun 2023 10:01:38 GMT  
		Size: 39.7 MB (39678007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df5e09768f30946e642c4ccc2ba209f76e0f517c84c6302d60380391c1fb4c86`  
		Last Modified: Sat, 17 Jun 2023 10:02:02 GMT  
		Size: 153.0 MB (153005405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
