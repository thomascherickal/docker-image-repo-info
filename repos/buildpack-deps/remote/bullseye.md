## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:c56964ed4528ca9408806beab642c79c86706b22f120ea3b8e3fc4b887e0e66e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:241ecdcb478abc4f2df5fba0866f4b401899fe36959c49e6991708500f614ad5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.4 MB (323376265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8cc63fa7004f98324a899e30d62315cfd16ca8ef9168df78752117a0ef958ac`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 06:27:09 GMT
ADD file:3feae44a900d0e1e835d12f1ea607313fe008d55842495a8cc533e7cfa75064f in / 
# Fri, 15 May 2020 06:27:09 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:30:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:30:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:31:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:31:57 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5acaaf333e788954dc63603194f262baba7644709169c9584c92237472fe3a9a`  
		Last Modified: Fri, 15 May 2020 06:36:49 GMT  
		Size: 51.4 MB (51391128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86454c7eb0ea041d8338f7821ab10f9501b14d3021a4d5f2dce05ba946d9188`  
		Last Modified: Fri, 15 May 2020 17:47:09 GMT  
		Size: 7.9 MB (7934302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31dd76374a13b2aafe8574e44d4bb42e142c3abe4fe7b7f1f82ce19cdad51311`  
		Last Modified: Fri, 15 May 2020 17:47:09 GMT  
		Size: 10.5 MB (10463054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19105d4e0710b44c9c203f25e1cd393cfadb8e9d1b33855aa6641533d625c4f7`  
		Last Modified: Fri, 15 May 2020 17:47:30 GMT  
		Size: 55.7 MB (55658572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b290975b76921db3ebeba3f6486e6ddf083a8f32d2491b3f4b6e89fc60c4e1ff`  
		Last Modified: Fri, 15 May 2020 17:50:36 GMT  
		Size: 197.9 MB (197929209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:6da39f0cd933a48328cef9880b17006ecb9e503ad4297e063dc1a1df4adcfc59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294830272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17b3b23805fc6f0562d9117ee225906f22c4412dd842048c55deb1eaccd3b3cf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 22:36:28 GMT
ADD file:099743a0547d5c892b4a3daaa3fc0f05d8317cd4946a0e9508d130ee56db63bb in / 
# Thu, 14 May 2020 22:36:31 GMT
CMD ["bash"]
# Fri, 15 May 2020 03:38:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:38:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 03:39:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 03:41:38 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0238daf30887e241cdd1334fa6bd5883d06738c7ff61cea1b32a3361de098564`  
		Last Modified: Thu, 14 May 2020 22:45:51 GMT  
		Size: 49.4 MB (49359451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f1dbc2de2b0cbdbc9ae5411e2efb20958587e0c8691a15a5755669fe35e467`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 7.5 MB (7514224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a4b62e0336252e727cea159b040a0ef9263bc7ec15d9411459056795050f87`  
		Last Modified: Fri, 15 May 2020 04:00:22 GMT  
		Size: 10.2 MB (10157685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fa5c09a3e017a2b7a2b6e53f1c3afa3978189e8bbe966b83cfc29251b56616`  
		Last Modified: Fri, 15 May 2020 04:00:47 GMT  
		Size: 53.3 MB (53295430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f21bf3c739738d10894b2138317eba223e86a5c538187fff73a6872d1982e88`  
		Last Modified: Fri, 15 May 2020 04:01:46 GMT  
		Size: 174.5 MB (174503482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:23d7d0524a4ba7a3020d7ecc24ca0385ecb5599d2104d19123d1dba50300287e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.3 MB (289268331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1935628252dc0769fa4950d3183777596ecbcdee64849345e75a330981c3abb6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 00:58:28 GMT
ADD file:c0d2fe9468c0056452ba2eba677a3cfb1318edf3174c0106a65ec1c5608f130f in / 
# Fri, 15 May 2020 00:58:30 GMT
CMD ["bash"]
# Fri, 15 May 2020 10:28:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:29:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 10:30:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 10:33:06 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:add59fdfc3a148d6f3bc80c671fa82b62aebfbe6f2ed783df08b083fb9497d23`  
		Last Modified: Fri, 15 May 2020 01:10:22 GMT  
		Size: 47.2 MB (47161514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ed350c74909d45b8bbadbed0841a0212e60d10edb4e0fc351433b86807c174`  
		Last Modified: Fri, 15 May 2020 10:55:58 GMT  
		Size: 7.3 MB (7256985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef0fe0276714c46bcc2d93dd77955362fe60814e5ec6b075e68a97b34da7f34`  
		Last Modified: Fri, 15 May 2020 10:55:59 GMT  
		Size: 9.8 MB (9804735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15989d6fd8c30478f6d030c5c9aa82929f5467d22588698401d7bed07a35e74`  
		Last Modified: Fri, 15 May 2020 10:56:22 GMT  
		Size: 51.1 MB (51080530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:472c5fbf1f6fe08660f9571cad333d7b2ae2a46b7aec8e9179526940f1c03bf2`  
		Last Modified: Fri, 15 May 2020 10:57:14 GMT  
		Size: 174.0 MB (173964567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:94dd6086f3e030cb12d6846bba24bc42d6dc5cc174a63e6a8913a7a80a4fb2ce
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.3 MB (315335648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85f8094068c8e3ded50d491f7720ca56e447bd20b3a0450fa69f102b11a9412`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:41:55 GMT
ADD file:47e352caa545ab1122a3a9df6a86296796c3b1633a1a8151d6fb438f88b47d5d in / 
# Fri, 15 May 2020 12:41:58 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:02:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:02:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 20:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:05:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:523842c45f03b461bd15f8ec65b3e2670cde3c595006ef67af2d46f30e971812`  
		Last Modified: Fri, 15 May 2020 12:52:36 GMT  
		Size: 50.3 MB (50328985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e57198818fd11918588ce78d9cd056305b237e52e37463ed090e08379da0ff`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 7.8 MB (7809462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822a6e14baacb6f567947c7991213c158c4924519e3e8e989752bb8ff12813c7`  
		Last Modified: Fri, 15 May 2020 20:17:55 GMT  
		Size: 10.5 MB (10459841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbb68fda96e6d2109cadb2b094a5f3b64b213595b13f3f88bf43deb6e56b33d`  
		Last Modified: Fri, 15 May 2020 20:18:16 GMT  
		Size: 55.8 MB (55803169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d1f3aeb6e612b7e04e4bfac4445b4e6cd018bf3bd7ea7b1dff2b23e6f93b95b`  
		Last Modified: Fri, 15 May 2020 20:19:05 GMT  
		Size: 190.9 MB (190934191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:76a7314bbfc8791fc043a8ece5e14d0d80738e93de494dbf0534e683b70213ff
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.2 MB (333165047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d499f36997e9dfe26c8c580dff2a4c404dc3ba2e7278c0031d016047364cda4e`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 07:06:18 GMT
ADD file:7290df675cbf34dadbbbb441b1c875c896d0027e51ef4f0322ea750d256dc1d7 in / 
# Fri, 15 May 2020 07:06:18 GMT
CMD ["bash"]
# Fri, 15 May 2020 17:05:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:05:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 17:05:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 17:06:52 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c978edbcc0f43d7a702a8796ed2e5dd9443fd302b396d9b20d4472b6152672f8`  
		Last Modified: Fri, 15 May 2020 07:16:58 GMT  
		Size: 52.5 MB (52481343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51518769fedac128b59ec5b081ca9002aa4c0af29f5a7a0c8ec1b3d02d8c4bbb`  
		Last Modified: Fri, 15 May 2020 17:25:02 GMT  
		Size: 8.1 MB (8112069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e20b512a546a13c02057a9f7978b41d29d8e7c70a91f8c2d9d6b09db8f5c1e`  
		Last Modified: Fri, 15 May 2020 17:25:07 GMT  
		Size: 10.8 MB (10841246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a629d631fe32949e213eb3eea28481d067b67bc40e33f20f2bddd5076a09c189`  
		Last Modified: Fri, 15 May 2020 17:25:30 GMT  
		Size: 57.5 MB (57518069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80728c1c165a654e799cc154e568d386c3b60155f11fb15d3693f74f5585a392`  
		Last Modified: Fri, 15 May 2020 17:26:21 GMT  
		Size: 204.2 MB (204212320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6214e8acc1569cd006314e792b701e888d6640aa44dfa6b365b517eca6b7ee39
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.1 MB (315075994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd8479c1b2611e7c8f662f04e1213be210f2a17f4637f234881fe4003bb40aed`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 04:46:53 GMT
ADD file:fcf688b002e58dbfd2392e8a30b0ad1975c59c068b68c9d846430ce0f63eb390 in / 
# Fri, 15 May 2020 04:46:54 GMT
CMD ["bash"]
# Fri, 05 Jun 2020 21:38:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 21:38:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 05 Jun 2020 21:39:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 05 Jun 2020 21:43:26 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dcbeba28f7aa4ae28ec4e38f90ddc68bb34f71bf49e3361203df2f569876774f`  
		Last Modified: Fri, 15 May 2020 04:55:03 GMT  
		Size: 50.1 MB (50131847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46d0ed8dc6e716f36dc92c5111b99ac84ac31e108fa46c6a77978317ff5c8d6`  
		Last Modified: Fri, 05 Jun 2020 21:44:34 GMT  
		Size: 7.5 MB (7460933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a86a877eb6ead7b0031c439d2b52cdad0273b54b9dfdf91f3106609216b07be`  
		Last Modified: Fri, 05 Jun 2020 21:44:34 GMT  
		Size: 10.5 MB (10505299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1cd9875fc44b4d1139ab8940bd044d55e24d13f5438c0980e4dc0e4b348c05`  
		Last Modified: Fri, 05 Jun 2020 21:45:30 GMT  
		Size: 56.9 MB (56868332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec5bf1476da986aebef3b90cfe8b16c81e0084d3b2a161fd3e450e2c2d2d1711`  
		Last Modified: Fri, 05 Jun 2020 21:47:59 GMT  
		Size: 190.1 MB (190109583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eb8b0234f630adc76ecdbf65aa9b9f45e295f8a111ec6e1932197ba88e65a1eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343128137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf9fc05e4f527f8a86883252cf6e199ee9e6cdd5a17ef6ce16fef352abe567`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:32:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:42:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e43969f6c0ff55aa4240214980deed196b68292106e0144d8d1290495d9b7`  
		Last Modified: Thu, 14 May 2020 00:25:02 GMT  
		Size: 8.4 MB (8356860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eacce9e1d274d8f139e9d384ceb5e66a86ca1857d025523765b1b099330719b`  
		Last Modified: Thu, 14 May 2020 00:24:57 GMT  
		Size: 11.2 MB (11176806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12dd448830e6ab4491686ac42b85cc8f50e9b182a8b19722842140e7e06c1af`  
		Last Modified: Thu, 14 May 2020 00:25:53 GMT  
		Size: 61.0 MB (61049897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e509d495da37eb010696bb333af1093f653da43115bc762475c7d7b145b1e`  
		Last Modified: Thu, 14 May 2020 00:28:34 GMT  
		Size: 207.4 MB (207434267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:adf6adad36597f5df2877dba54ea17cd1deb7136bc608ab3037e04c23ef81fe3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.1 MB (304142487 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0daf2998b97097bc3ed7d59ceef4cdb580246ca6faa7d92ae3b50e9f5ffbfc41`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 14 May 2020 23:05:50 GMT
ADD file:56a2d8bf46ec4edd3d768966ad8e9b4c86561cbcd482ae49fc18cc34306d54fb in / 
# Thu, 14 May 2020 23:05:53 GMT
CMD ["bash"]
# Fri, 15 May 2020 04:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 04:58:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 04:58:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 05:00:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f0cbd757e4d594cf3793c18e1f7d5d6f3fd983ea05bd2edeac4774c47e85b763`  
		Last Modified: Thu, 14 May 2020 23:10:41 GMT  
		Size: 50.0 MB (50002620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb69a5809930b7b8812ae832cb600c60afe5387c53903bf422ae0e80ff086583`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 7.6 MB (7600625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd25c680ce576408f8c9a5e8891ea37ac21483e932a4bacc4b744cad80a975e`  
		Last Modified: Fri, 15 May 2020 05:07:54 GMT  
		Size: 10.3 MB (10347742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775b4e20d2d0e51cbdce841c11938b1192f017a82d06190796de1bbfabcc12bf`  
		Last Modified: Fri, 15 May 2020 05:08:08 GMT  
		Size: 54.9 MB (54899878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:278ae126eb2e17613e7b56db2c840af94916facdc3d1054b2cfd7e0a84d173af`  
		Last Modified: Fri, 15 May 2020 05:08:46 GMT  
		Size: 181.3 MB (181291622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
