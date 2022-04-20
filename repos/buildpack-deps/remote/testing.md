## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:49a85c90290edf8b255d06f43f3fe5a88a96ef3879efb8f1c5bd99feed3bed0f
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

### `buildpack-deps:testing` - linux; amd64

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

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:cd801be4153071d309d34f66f2f93f041d24bdd0633fbc3c1909e207c4e2894a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.7 MB (304731636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f96581379c833ab17714b6da642ea2f4bcc72619f1dad4f98bfea24ded84287`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:15:05 GMT
ADD file:e283a0d8ab69b94018679c485439a2b5700bcbd73218180b0a334a00df340093 in / 
# Wed, 20 Apr 2022 07:15:06 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 12:34:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:35:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 12:36:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 12:38:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7b4944a983e7a423568be713ae200d96e80ca1893c45b7758ec97be00ab710b`  
		Last Modified: Wed, 20 Apr 2022 07:30:20 GMT  
		Size: 53.0 MB (53001097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b73ce869fcfbdc3ffaeaa0d7d3b07f9fb196e529df28d7cce0d9976f8e0999`  
		Last Modified: Wed, 20 Apr 2022 12:58:01 GMT  
		Size: 5.1 MB (5105021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98c07b037b55f8ee9d1521c9f7f55cce527352418e84f9bb81e54017e02f8e9`  
		Last Modified: Wed, 20 Apr 2022 12:58:03 GMT  
		Size: 10.6 MB (10597592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f243a3e5566a2642f8bfdf039f8804b1a3f911af31cbec75d6e411433cca4a78`  
		Last Modified: Wed, 20 Apr 2022 12:58:54 GMT  
		Size: 55.1 MB (55071283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ddc68f6dbd4f8a7396d1ca21a4b7c719c6e9d66300c33c5e3d7567e07252a81`  
		Last Modified: Wed, 20 Apr 2022 13:00:55 GMT  
		Size: 181.0 MB (180956643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

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

### `buildpack-deps:testing` - linux; arm64 variant v8

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

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:afbb08f97e332511c3d9a0f6638e91144a3b6b29ed3e2087fcd781d8bb051dbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.9 MB (336885427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902ebdb6471753c34184f87efa7bf215458cf9d377a95a8ff6aa4be79dd89018`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:36:51 GMT
ADD file:469d404c80a1f5720a0a00e4cd116adfd490349ede3a368fae44c6409add4819 in / 
# Wed, 20 Apr 2022 07:36:52 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:13:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:13:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:14:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:16:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c3d3d77c2c71a18bcd4eead6143eb6d36f5096a31d00bfdb4cbd88058ba444c8`  
		Last Modified: Wed, 20 Apr 2022 07:43:35 GMT  
		Size: 56.6 MB (56624540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f37953affc719c71f109e570bbb539dc712570c50eafb76adeb6cd853aff96`  
		Last Modified: Wed, 20 Apr 2022 10:26:12 GMT  
		Size: 5.3 MB (5339609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f627a1c0c008ccb7b51d8adfc2441ea6d92182113c32697e7aaba9541bd9197e`  
		Last Modified: Wed, 20 Apr 2022 10:26:12 GMT  
		Size: 11.1 MB (11103895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc648d3f0a6e4b8565ccec828ba99bd5607463a76c6d7c449889b1d339277d3b`  
		Last Modified: Wed, 20 Apr 2022 10:26:32 GMT  
		Size: 58.9 MB (58856102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ce15e3a179cc4d5cc9ae747810989203d7e363ebc7699b0dd422faf28d978d`  
		Last Modified: Wed, 20 Apr 2022 10:27:06 GMT  
		Size: 205.0 MB (204961281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

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

### `buildpack-deps:testing` - linux; ppc64le

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

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab60654871cbf70637852b6e48f85997369446dcd9da21ad584e03a9414ae2bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **305.8 MB (305820836 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:645ad468159c7839b0b54fe7365fe585fc1859c22c57da79a06687d0799a0c2e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 08:37:57 GMT
ADD file:dd66488219818707ab57e2b9e87dcec876513326c64a733dcf95396ad5f22cd9 in / 
# Wed, 20 Apr 2022 08:38:03 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 11:09:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:09:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 11:10:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 11:13:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b24c47356e8597f2e75ec110237cb3350c6d41c44b019ed531f1d9069ab1a82`  
		Last Modified: Wed, 20 Apr 2022 08:48:48 GMT  
		Size: 53.8 MB (53813432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f80f6a4ee41ee80e5063d1d7d86ebb328ffa05ba98de6fe03109fafae44721`  
		Last Modified: Wed, 20 Apr 2022 11:27:14 GMT  
		Size: 5.2 MB (5185393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcd7e687f194e7ac60ded4e1bfd0eeacd9d22b2785dbbdf847eafa68e6a0058c`  
		Last Modified: Wed, 20 Apr 2022 11:27:14 GMT  
		Size: 10.8 MB (10817739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec5a65d3af6eca0c8714b06d93f4c226cbdca79f7d10b79ed6f964d5aca99e7`  
		Last Modified: Wed, 20 Apr 2022 11:27:29 GMT  
		Size: 56.8 MB (56769107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e4631b442ef0be01b1ef00fc9823a601fa5cec06ec8ffaf5afbdceebf2527ae`  
		Last Modified: Wed, 20 Apr 2022 11:27:56 GMT  
		Size: 179.2 MB (179235165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
