## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:e38ab57fffe4dee26911d7b0803ea647e23d3a85b270a1f294751dc8559bc78e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:984c082123cf26ca78121b524a1bd801266af1862f2d16dbfd32968792dc79ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333789698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:073c35ab07cb52fa3461329088ee7d6474bdb641a5fe65430389fbe83ed2e3c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:42:54 GMT
ADD file:b5180fc4d45b984afa69f3cdfa95980bcdfd76d75f704f74f1aa60e416272f1a in / 
# Wed, 20 Apr 2022 04:42:54 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:56:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:56:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:56:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8cb01d170a54a4c7fd7c1969e79df0a453468ebabfe1d860b863f7a3b6fbbc2f`  
		Last Modified: Wed, 20 Apr 2022 04:47:18 GMT  
		Size: 55.6 MB (55578729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec411cc74e7329b4aa762298d902d14025f16214d6dfccffc28adffa29c655c`  
		Last Modified: Wed, 20 Apr 2022 07:04:37 GMT  
		Size: 5.2 MB (5208374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3518a73a45d857ec3136592d439326badcede35952ad723c33e4148b5e83d9`  
		Last Modified: Wed, 20 Apr 2022 07:04:37 GMT  
		Size: 10.9 MB (10924132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fee26143ae45bb521ee21c064678ca5bf451d9c940e15c92b78ccd693581c0c`  
		Last Modified: Wed, 20 Apr 2022 07:04:56 GMT  
		Size: 57.5 MB (57452359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c12737e059d2baad01cea5e9c0e89f08aeb135a33295702b3db7f65ef32208`  
		Last Modified: Wed, 20 Apr 2022 07:05:32 GMT  
		Size: 204.6 MB (204626104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:7e5308e1944fc1787dfd450bacba7bbe9859856f745a6e7aaa0ceddd6582b423
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.9 MB (303917448 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec4962b715d6e6bda7ec5550500040d73d5b3745a205d6f23532db0d1f089452`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:07 GMT
ADD file:6b5b5c095508b777a2c8b2633d97d6143bfab0320bed58e8e335179bfd681fc9 in / 
# Tue, 29 Mar 2022 00:49:08 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:38:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:38:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:39:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:42:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b209f6efb315c2c09d16e50d6077a10a401191c741a83c3c6c0767fe202d69d`  
		Last Modified: Tue, 29 Mar 2022 01:03:30 GMT  
		Size: 53.0 MB (52995524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bc9d490149e4bcb11fe298e2c5a923c08cc31f08662f9f7637aca6473309b73`  
		Last Modified: Tue, 29 Mar 2022 08:02:54 GMT  
		Size: 5.2 MB (5163931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1132e128b11ccea17e38c248a34ec3142776903dcca038a3e7789c9e8f52f6a1`  
		Last Modified: Tue, 29 Mar 2022 08:02:56 GMT  
		Size: 10.6 MB (10597029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bea4cefcae02c237fe7371ca4d568c1f51b28d10f874dfcdd78ad48b4b5234f`  
		Last Modified: Tue, 29 Mar 2022 08:03:39 GMT  
		Size: 54.8 MB (54809370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5598b39f93060be7cdb0eb78efa2a5db7f9bb86aaee7fe02bb691c1b74c8938b`  
		Last Modified: Tue, 29 Mar 2022 08:05:28 GMT  
		Size: 180.4 MB (180351594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1b7f006eb3a57bab345054192acd054f943cf3cfd7bb6b115c103509d1e19365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **290.9 MB (290939687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85b20281cfcd48c8a697a638e28485625d00ccb49f6dd5663dad8efe495e27b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:16:59 GMT
ADD file:5ab9a8a4847f677425562eebef8854e58592bb57501d4bc6f521315d90815c3c in / 
# Tue, 29 Mar 2022 02:17:01 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:02:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:03:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:03:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:05:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c7c8b286eb908a262d0005e4560150fabc15db4a3531f7e00f77b76643457e6c`  
		Last Modified: Tue, 29 Mar 2022 02:32:14 GMT  
		Size: 50.6 MB (50609802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d739161e2986c208982baa48eed3572da3097ebf10a7f4e51faf03c0273ea371`  
		Last Modified: Wed, 30 Mar 2022 20:27:35 GMT  
		Size: 5.0 MB (5023298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94e98cfbaf9038f43192a4328368893d374a691bbc690dd7b94222d51e41dfd`  
		Last Modified: Wed, 30 Mar 2022 20:27:37 GMT  
		Size: 10.2 MB (10244161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99ff68e3ac47baa10b1f98b0d5f14dbfc37964e7a2b10b452927f86c64fd0f84`  
		Last Modified: Wed, 30 Mar 2022 20:28:25 GMT  
		Size: 52.8 MB (52780274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:634e25a466b6069d9f5828e16523e475d6d14db70495b310c406383c5070ebff`  
		Last Modified: Wed, 30 Mar 2022 20:30:14 GMT  
		Size: 172.3 MB (172282152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b9a1b51c0dae84a5b1bb148088431a81dc347bb1352a2f8a41e08ce62023ee4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.4 MB (326431607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:150acef53969ff5ef532e519cf93f84adace07117e4b4195d456e98d2756ff45`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:29 GMT
ADD file:23397ad30e34521aa2c0881ab09c9c75f58316594a1c14f01cfcb212161c32fc in / 
# Wed, 20 Apr 2022 04:28:30 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:42:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:42:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:42:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:43:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c6d996fb7c2fde9d95056213e2cc0a2ea025cc86ce1ceeac46b8c51b2d458d84`  
		Last Modified: Wed, 20 Apr 2022 04:34:39 GMT  
		Size: 54.5 MB (54493289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ee691ff28baa681054135ac8fa72e16199a7024e056d33c427338a21e4dc9a`  
		Last Modified: Wed, 20 Apr 2022 06:53:00 GMT  
		Size: 5.2 MB (5195219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b23bcd2aa6bcebcec9157dcb6c0fecb23e91f1255c588550180d6cd7f9fc26`  
		Last Modified: Wed, 20 Apr 2022 06:53:02 GMT  
		Size: 10.7 MB (10691123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e004e1e477153d2e7cdf23a84ae9b22b0d4d1493b45f04c0e19e20d1ad88f9b`  
		Last Modified: Wed, 20 Apr 2022 06:53:22 GMT  
		Size: 57.5 MB (57484900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b650220d5c49781bed9b83bd215958e748d86bddd92476767e8635524833c29`  
		Last Modified: Wed, 20 Apr 2022 06:53:58 GMT  
		Size: 198.6 MB (198567076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8851d1e8a77483566b82195c9eaffceea6b155944274e3e51755a7776a38983f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.1 MB (336094169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03d22e95f6da9cb5a3ef8107bf0dca8187b7f438b41ea53d8c835986af951337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:20 GMT
ADD file:828aa883b729cb9e3bbc9efef043626425a2803461bd7b07862d746e2df08c10 in / 
# Tue, 29 Mar 2022 00:41:21 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:53:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:53:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:54:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:55:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e0acfe1e9e31a265994eee72788e1a0b4b33edc5c9d6fc978fd65d87aa94b53`  
		Last Modified: Tue, 29 Mar 2022 00:47:47 GMT  
		Size: 56.6 MB (56628219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e1b01718568970f8976ea798ed333d8acb22b4cdc57a341b078bb0a7e4e4dc`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 5.4 MB (5400088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296971f2bacc0edb451554653b20751f9adfa0cbce82cb5e06a78c72076b036a`  
		Last Modified: Tue, 29 Mar 2022 18:13:41 GMT  
		Size: 11.1 MB (11103529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f03b11aedb9bbc81a6111cf72e7c011c9682d79ce42ad6dba4bac5f1a2340`  
		Last Modified: Tue, 29 Mar 2022 18:14:03 GMT  
		Size: 58.6 MB (58613121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c72142fbc612ab497e789e0cf317e15155ad755a807c55a5e0c33308079666`  
		Last Modified: Tue, 29 Mar 2022 18:14:42 GMT  
		Size: 204.3 MB (204349212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:4b96719aa342c4bfd8465cef5960ac34e4b1ef74915e068e1f157ce0adc065d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.3 MB (313279863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94cb436aa3e4b96d1b765561aadd9908d0b900046f7c6612823f0e3d0b33198a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:40:39 GMT
ADD file:88e75745fdbfd0784c1c18134a0a52a5534df18201a6f49555a5c618b4531804 in / 
# Tue, 29 Mar 2022 07:40:44 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:16:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:17:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:19:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:26:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bdc3f4c024aea887030bcf477ee808da6aa3e6683fb111845d94ab4f2480ff24`  
		Last Modified: Tue, 29 Mar 2022 07:50:58 GMT  
		Size: 54.2 MB (54240334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e94f68f0d96094b4bd1aa9ba6f4465ec7d6879ed28f910b949ffb165eef3fe`  
		Last Modified: Tue, 29 Mar 2022 08:54:21 GMT  
		Size: 5.2 MB (5221857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd581c56a027feec68bb7a881cac731bca045297cd76398414512c34351a063d`  
		Last Modified: Tue, 29 Mar 2022 08:54:24 GMT  
		Size: 10.7 MB (10672471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3631eb84b5e85d4e37526f1ae6b1259a7a43e8e02c45f72f851783117629e90a`  
		Last Modified: Tue, 29 Mar 2022 08:55:13 GMT  
		Size: 56.0 MB (55951132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365030772f8d919db49c949fdcb31ab34f90afe192c43a10bf522b2eab07e743`  
		Last Modified: Tue, 29 Mar 2022 08:57:20 GMT  
		Size: 187.2 MB (187194069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c4855f28939a48ab04ab5f76613221e545d77574a55093a1d35f9962b8090178
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.0 MB (343007252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2228008410bf32c4d9e0c92ea8554a5b00edc3adf2961ee56b1a178140459b1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:20:10 GMT
ADD file:c9ff325b9fe680d344c36e7e25729f90711bdf646908892ebdc0f3a53d92bc50 in / 
# Tue, 29 Mar 2022 00:20:29 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 05:30:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:32:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 05:34:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 05:46:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fc5522fc3ca5c5e9e4af133a35ed8a4e104c9366b7ab66c3cc5601aef68f175a`  
		Last Modified: Tue, 29 Mar 2022 00:30:15 GMT  
		Size: 60.0 MB (59999423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31127088a5022a99c9c420931875f462b30887ac8cdd2b9832e9a48833053641`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 5.5 MB (5543257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20e81de5da1931ed0a987d558ca1844e91b01be66fe4fa9f9a11ab9c2e851f7`  
		Last Modified: Wed, 30 Mar 2022 06:23:56 GMT  
		Size: 11.7 MB (11702051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9353b28a9fb4647d78b62d393fd6fe5b2983eee962f4429ab69b8baedb393997`  
		Last Modified: Wed, 30 Mar 2022 06:24:21 GMT  
		Size: 61.9 MB (61868324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106c7924170a6bd732149f34c47aa890e48efc66345e9b7ec167a89ff84a0b28`  
		Last Modified: Wed, 30 Mar 2022 06:25:15 GMT  
		Size: 203.9 MB (203894197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f2b1c8403f6418a76d9bef105f436be2751f3613a86216f798d87cfb0786ed5f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.1 MB (305122699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13fcd55951d8207b56f341adf6c714d7b2dd0f7e86de9688df0c8abb30a642c6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:05 GMT
ADD file:9a99e896abdfac4163e20511778572abbec89bf317a3c3dad1f6fe0c63b126b1 in / 
# Tue, 29 Mar 2022 00:51:11 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 02:23:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:23:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 02:24:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 02:24:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4c231abb22533340c714e28363f98b83f5da88a6702fdfc7d06ed65b8f2e70e1`  
		Last Modified: Tue, 29 Mar 2022 00:57:13 GMT  
		Size: 53.8 MB (53839067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1f72f77effa39a86785d5e5242154a329664927615884293ae53de3228e345`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 5.2 MB (5245181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a40794a51d7ee7ef5a9c0175be5b9245646cf0f2703acbb34ea8e72c731272f5`  
		Last Modified: Wed, 30 Mar 2022 02:32:53 GMT  
		Size: 10.8 MB (10819318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c986ac3bb53ec5a4892c250c435a3e59ee79ddb71f265aa5d083d3f87a1faf3b`  
		Last Modified: Wed, 30 Mar 2022 02:33:07 GMT  
		Size: 56.6 MB (56559391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812bc5decd96fca156a3b3458545508f1eb911d930b7b7f77799022ee544d126`  
		Last Modified: Wed, 30 Mar 2022 02:33:32 GMT  
		Size: 178.7 MB (178659742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
