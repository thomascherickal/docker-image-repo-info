<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `buildpack-deps`

-	[`buildpack-deps:20.04`](#buildpack-deps2004)
-	[`buildpack-deps:20.04-curl`](#buildpack-deps2004-curl)
-	[`buildpack-deps:20.04-scm`](#buildpack-deps2004-scm)
-	[`buildpack-deps:22.04`](#buildpack-deps2204)
-	[`buildpack-deps:22.04-curl`](#buildpack-deps2204-curl)
-	[`buildpack-deps:22.04-scm`](#buildpack-deps2204-scm)
-	[`buildpack-deps:23.04`](#buildpack-deps2304)
-	[`buildpack-deps:23.04-curl`](#buildpack-deps2304-curl)
-	[`buildpack-deps:23.04-scm`](#buildpack-deps2304-scm)
-	[`buildpack-deps:23.10`](#buildpack-deps2310)
-	[`buildpack-deps:23.10-curl`](#buildpack-deps2310-curl)
-	[`buildpack-deps:23.10-scm`](#buildpack-deps2310-scm)
-	[`buildpack-deps:bookworm`](#buildpack-depsbookworm)
-	[`buildpack-deps:bookworm-curl`](#buildpack-depsbookworm-curl)
-	[`buildpack-deps:bookworm-scm`](#buildpack-depsbookworm-scm)
-	[`buildpack-deps:bullseye`](#buildpack-depsbullseye)
-	[`buildpack-deps:bullseye-curl`](#buildpack-depsbullseye-curl)
-	[`buildpack-deps:bullseye-scm`](#buildpack-depsbullseye-scm)
-	[`buildpack-deps:buster`](#buildpack-depsbuster)
-	[`buildpack-deps:buster-curl`](#buildpack-depsbuster-curl)
-	[`buildpack-deps:buster-scm`](#buildpack-depsbuster-scm)
-	[`buildpack-deps:curl`](#buildpack-depscurl)
-	[`buildpack-deps:focal`](#buildpack-depsfocal)
-	[`buildpack-deps:focal-curl`](#buildpack-depsfocal-curl)
-	[`buildpack-deps:focal-scm`](#buildpack-depsfocal-scm)
-	[`buildpack-deps:jammy`](#buildpack-depsjammy)
-	[`buildpack-deps:jammy-curl`](#buildpack-depsjammy-curl)
-	[`buildpack-deps:jammy-scm`](#buildpack-depsjammy-scm)
-	[`buildpack-deps:latest`](#buildpack-depslatest)
-	[`buildpack-deps:lunar`](#buildpack-depslunar)
-	[`buildpack-deps:lunar-curl`](#buildpack-depslunar-curl)
-	[`buildpack-deps:lunar-scm`](#buildpack-depslunar-scm)
-	[`buildpack-deps:mantic`](#buildpack-depsmantic)
-	[`buildpack-deps:mantic-curl`](#buildpack-depsmantic-curl)
-	[`buildpack-deps:mantic-scm`](#buildpack-depsmantic-scm)
-	[`buildpack-deps:oldoldstable`](#buildpack-depsoldoldstable)
-	[`buildpack-deps:oldoldstable-curl`](#buildpack-depsoldoldstable-curl)
-	[`buildpack-deps:oldoldstable-scm`](#buildpack-depsoldoldstable-scm)
-	[`buildpack-deps:oldstable`](#buildpack-depsoldstable)
-	[`buildpack-deps:oldstable-curl`](#buildpack-depsoldstable-curl)
-	[`buildpack-deps:oldstable-scm`](#buildpack-depsoldstable-scm)
-	[`buildpack-deps:scm`](#buildpack-depsscm)
-	[`buildpack-deps:sid`](#buildpack-depssid)
-	[`buildpack-deps:sid-curl`](#buildpack-depssid-curl)
-	[`buildpack-deps:sid-scm`](#buildpack-depssid-scm)
-	[`buildpack-deps:stable`](#buildpack-depsstable)
-	[`buildpack-deps:stable-curl`](#buildpack-depsstable-curl)
-	[`buildpack-deps:stable-scm`](#buildpack-depsstable-scm)
-	[`buildpack-deps:unstable`](#buildpack-depsunstable)
-	[`buildpack-deps:unstable-curl`](#buildpack-depsunstable-curl)
-	[`buildpack-deps:unstable-scm`](#buildpack-depsunstable-scm)

## `buildpack-deps:20.04`

```console
$ docker pull buildpack-deps@sha256:4012d4c808c46a9a637840bbdd390b6c376567bd757dd7f9e3f220cb6acb0172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:acd56f331b33212692b155f660b552b4c88f58d5ff8872826cf7776d8254e736
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245803354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fda0fc31b0a48175e7336ca929f7ae5db6d6b985ec61f1eb2e34e09e47c0fd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:27:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e934f6d128d65c709d47ca01bccaae13c479a8306ec18c7fcd2b492f16089c4`  
		Last Modified: Thu, 03 Aug 2023 03:38:43 GMT  
		Size: 60.9 MB (60923971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d83c40e01065bb197fcf80fb04dacbe13913dfdd9d8f9536fc4585b63af296`  
		Last Modified: Thu, 03 Aug 2023 03:39:10 GMT  
		Size: 145.2 MB (145169180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:583ccef8d57e8083fb49465862f1d91a72c4c354463b55d48b40981af478232d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212026855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae217cb1499d44d0503a7acb9635a9ef089e3a054c66d3496428a9f59f7eadf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:09:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:11:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab787541d8bd910e22e242d890b591088a8056ebe44d8f49093e22e780fefa7`  
		Last Modified: Thu, 03 Aug 2023 01:24:28 GMT  
		Size: 55.8 MB (55824728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b16044bcb697f6b7460deb249f147af14046beb812b7673eb8c7b42ddb89cb`  
		Last Modified: Thu, 03 Aug 2023 01:24:54 GMT  
		Size: 122.0 MB (122010037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4561f7a165e00049e2fd0d22f71bd39b9c943b958ffddf108fc8cb0c2d3352c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236070832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e168e1909b18bfb49feb06a8f81249f49a2b79eeb8afffdef29e96cb40d03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:33:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:36:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7d1a175de684642bf290a3882b913844851fa5b7582e492e466ed74035f035`  
		Last Modified: Thu, 03 Aug 2023 00:50:08 GMT  
		Size: 61.0 MB (61014742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257b81580f56d0fdcedfd9d17039d8c6225cadba4d0173a78cc30a3a8ba87562`  
		Last Modified: Thu, 03 Aug 2023 00:50:31 GMT  
		Size: 136.9 MB (136872285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:455def3ef4d52747cdbaab828e783a0881efde84a4f41064e8223ff241bc624d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269569036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b53b87cd5bed2144465a3b4f663a78abeed0b756f44e4adaf79bae8e7cfd6d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726e55a0f98534a51453930e4c0788ba5f9425af2106a0f632242d22add5e029`  
		Last Modified: Thu, 03 Aug 2023 03:50:26 GMT  
		Size: 69.6 MB (69644291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec136ee45fd038a87eceb7f9940509dbe2343c5dd06ad15175b2c74454a0520`  
		Last Modified: Thu, 03 Aug 2023 03:51:18 GMT  
		Size: 153.7 MB (153680155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:146a4f8c725380eec620a5f6d2f018386dc774ce13692cc79159c2f120c7137a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226607654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed94ac912c0ed9895b3abef8896dee8e605f2bc4e578bb2b29f23932a7ba0bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:11:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c95e4e206b384145bd8128e74027e092da89c7654f4aebfd616735756a6f9`  
		Last Modified: Thu, 03 Aug 2023 00:21:42 GMT  
		Size: 128.6 MB (128593276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-curl`

```console
$ docker pull buildpack-deps@sha256:18e96a2da642503b6b1dd2a822a6f08a04573f3641cb18ab50b7cae0a00648ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:25f7002f1f22788abd523a869097b453d18139ad76634090717fcaadd420c8c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39710203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0bf7833fb8ea45c517e7a264f113dd4ad0750a8ca080acdbe8175645371016`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:277a8c3f670eebf90abb7d136c5a7f7bbea2ba47c638604a7c3fde09b5a73623
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34192090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a4d7cc90e6e8e793f1b97cccf70c09f05538a4936ab7f69f3cf7297b7da660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf755867f779cd7d3788c2c3c8c6825ab43fb5487616afda3928d832cf0e7af2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38183805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a79375418b299d399ca410b47922d62003dde194891a752b910e8982ce198a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ff870a684265eb22a3502debb0824422af014d8a4dc397696f8a589d12246045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46244590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d6b65f4dbad88c0c655d3477312f05d99ba5d188ca0fb47c6caffc0a44050b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:028f59f497fa2c8e7f3a358182ef00c601e83780a8c7f9b0fd4e4f0f735ef4cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37702848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674186b606991aba08faede7dbb56393ab45900ba8c3e92969a9030076dba1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:20.04-scm`

```console
$ docker pull buildpack-deps@sha256:6777277d166b7084754912e6fa30b35bc6e37a817429346aacaf3c99b544b60f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:20.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:adfac55a5e84f9a71a4011f19ff1f92d9dd15e59dc30bd400dde2b3bc506a95a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100634174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdb4a6f59d3ac3f984df2be0978789f608389a147873c4fd36ac32be18a0fd5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e934f6d128d65c709d47ca01bccaae13c479a8306ec18c7fcd2b492f16089c4`  
		Last Modified: Thu, 03 Aug 2023 03:38:43 GMT  
		Size: 60.9 MB (60923971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9d44afa60dd5fb0db64fb915f1251f44e3ebf76b47981d309412e717fdfe3419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90016818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8254924c1588feb35db2643cade83e5af7f78c7e94ef3a02c420fd8d5bce794`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:09:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab787541d8bd910e22e242d890b591088a8056ebe44d8f49093e22e780fefa7`  
		Last Modified: Thu, 03 Aug 2023 01:24:28 GMT  
		Size: 55.8 MB (55824728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a42388d0c67c42187cf6e82f611a70a45a4db4ab48b0282b7f8e420f4b8d0087
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99198547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f01d02871cdea6466854b6ebf99bb53d48314df82755480b0a7df3158700688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:33:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7d1a175de684642bf290a3882b913844851fa5b7582e492e466ed74035f035`  
		Last Modified: Thu, 03 Aug 2023 00:50:08 GMT  
		Size: 61.0 MB (61014742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ed245924e86e7281a3885a36bfffa044077c144dd55db087aafa03f503c8248e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12179e95e3e7c1da6373ed192b5977cea19225ea0c9e1e468ee59b5bd566c345`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726e55a0f98534a51453930e4c0788ba5f9425af2106a0f632242d22add5e029`  
		Last Modified: Thu, 03 Aug 2023 03:50:26 GMT  
		Size: 69.6 MB (69644291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:20.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:079f48635b01d56e2478857b7e0c5fb6212336f9e594e783bbf19cb9dda8b0f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98014378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2522830f5bbe1d8ea3e120ce6ff28c07dbc6f1a8b7f24c17fbb61b252bbab549`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04`

```console
$ docker pull buildpack-deps@sha256:70272962f14206151d3f524e9a2cb91913d4d36ff7109ccd76356c1600f5fd15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8f28bd087741849791b564aea220968c88f2cace4063336681cd238858e05a79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249847907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442a35809fbea57170756e05e1a3bbb375ae8094fe1dbba784e092fd2935b0d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13d40b1da6010e8c9c1adb56fc6fb577c2db289f338cac71cc1c97fd28e6bdb`  
		Last Modified: Tue, 04 Jul 2023 03:56:35 GMT  
		Size: 172.9 MB (172868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:82dc71eec7f734241614d16b3a4eb66ebfef9c7a6ad60a3fcb9fe8819fad561c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216815905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a668d45893320321a9b7d361c43ba1aae9afad349f124144018c6aff67fd9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:41:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcf856a6334dae4b42fc54fea2a58544fa35961851c6d1e3007586c1e0917f`  
		Last Modified: Wed, 16 Aug 2023 05:52:13 GMT  
		Size: 42.2 MB (42244900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b51d420affa83085eaf6a3e84b9fc5325fde73b64976b53d13bc996be9f681`  
		Last Modified: Wed, 16 Aug 2023 05:52:42 GMT  
		Size: 140.5 MB (140522119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:25554a1e81affd0a7148f3363ded7ad133e915712366dda969f4db3cba8dd0c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241336078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff063c8c03b0f010bed01ee0a96a37316ca6c1433490497ba5b53bc2f78a7494`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:32:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6bfccc5cc58c82f10e31821cddd5b985299b78e91935c891542b24f2c62f3b`  
		Last Modified: Wed, 16 Aug 2023 01:42:14 GMT  
		Size: 39.4 MB (39368139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4614e2cec4ab0ddfa81eb3ced0780c45cdeece6b214d12aabf70908c95cfb9`  
		Last Modified: Wed, 16 Aug 2023 01:42:38 GMT  
		Size: 166.5 MB (166509502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d66a2fc9c52dd6d4f07d37dafb2ef3749f915a796dc77f6a928ae2246e368c10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.6 MB (271602068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4148c1e5b7fea252f7458c7ecf09659195b74c760ea787cc0dc0368ea23dc2d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:00:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3975a415c70a582703af5a6d25f7b6ab2976130066120608bb8fef4936ab082`  
		Last Modified: Wed, 16 Aug 2023 02:15:26 GMT  
		Size: 43.9 MB (43888713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e3a228c1be7d7fb67b215e897afc46ce5832e6b00e93abb38c6d2d8f4a02bb`  
		Last Modified: Wed, 16 Aug 2023 02:16:21 GMT  
		Size: 183.7 MB (183741262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ead5c3b74a1b308a84ea43da09bc2c04761f4a51ff69fb75ea39b13d99286cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223828482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e4f9598e552d8b03ad050606aeef9a8cc92e510c28491e18d48e8ec738e940`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:28:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:30:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4d2ca10795ab9674ca09c980d55a84f444920c9f376729aa86df29e23983ca`  
		Last Modified: Wed, 16 Aug 2023 04:39:14 GMT  
		Size: 39.4 MB (39415890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9ae7a022bc926e602497a803fc2ba318c956f9c66d679e809d0fd3d33a37f`  
		Last Modified: Wed, 16 Aug 2023 04:39:38 GMT  
		Size: 148.7 MB (148734530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-curl`

```console
$ docker pull buildpack-deps@sha256:9a4f3770ddcbb5abef530b0f63462986ef979ea26544c0b6d4a95723ff04223e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:483b82bc040102243b07bcbb2bb61e88294953b57782d2ee84dc0b81db449cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37551100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a6f6f87887de69ba89a8eba29dd185ff073609b204037b4931d8322101cad3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:56577af195afd5422d9ecfe7417e22ba5fd0b6a9e410101b0975e30b24370335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34048886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aaf8b344d04e5a7cf7cee8a90956443b1a27253272b508d2192af5af19a9098`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d5180a814a3d67003fd3fa28cd6c26a857d47db8ef15e95d52855b2986bf8e82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994829797c5fefa7b4ef655e8643c5a0d83916c5984d16465f65489315a7cd51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:752573e2a0c2b750c4f0955e0ef1c44e4001e2534b12ff9554d6967750f3ca2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43972093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1722b70ab45b97523406b34ccf447edd8188aacaa4744a27be94d231d73b04a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:55b68aab71baf930050c4e24bd323974bff4e14835cf93f741e94d233fd5d787
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35678062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2291cf79328dbbcc70c7534a4e837c075a137ecaefaaa763466fab1521bd10d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:22.04-scm`

```console
$ docker pull buildpack-deps@sha256:2a2e28268de88785f14de8b3e871669c77a888b0b033b016d8fc07b67addbbe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:22.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c79e22f6262ffcc9eb5eee479f1728247ee7c37e1419034d7ef047a9cd8b649f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76979897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da96a2a7c92bf335b49390e599ef90eeedbad15d69f1c2f3bac70574468ac75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ceffe5bb7f37971ba502f342d42b22fde4d37c2bfaddeb0f03b26437b5bbed31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76293786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2801ef2b20fdc536062325b8f61fc4681d965f31312a81e88d8128c8f713d333`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcf856a6334dae4b42fc54fea2a58544fa35961851c6d1e3007586c1e0917f`  
		Last Modified: Wed, 16 Aug 2023 05:52:13 GMT  
		Size: 42.2 MB (42244900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4f5048207f874df8fbfc050b4517760eb23860f7f1fd21951d0f522b823f6ca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7076967d855557f64f160cf4366c5ecc6bfcb8cfaf2af9b9bcff432666952cc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6bfccc5cc58c82f10e31821cddd5b985299b78e91935c891542b24f2c62f3b`  
		Last Modified: Wed, 16 Aug 2023 01:42:14 GMT  
		Size: 39.4 MB (39368139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4c3eb26a7d946b19c481386715e1761a62073bf47fe5830640ca660923a53162
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87860806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:380b59efd0d618a11314b3eb0cb43fb9ddb4ee8437cb5067f1a03a1d75af9c2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3975a415c70a582703af5a6d25f7b6ab2976130066120608bb8fef4936ab082`  
		Last Modified: Wed, 16 Aug 2023 02:15:26 GMT  
		Size: 43.9 MB (43888713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:22.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cc3f2368befd688a4db83b00f731ea5b910aaa0cdec162156ee6f6bb1ce54ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8c28857d76ff033c28d3b0164808eb366e80313fc99d5eb350b0993683d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:28:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4d2ca10795ab9674ca09c980d55a84f444920c9f376729aa86df29e23983ca`  
		Last Modified: Wed, 16 Aug 2023 04:39:14 GMT  
		Size: 39.4 MB (39415890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04`

```console
$ docker pull buildpack-deps@sha256:594df2f870c56c720a6d79560aaba368ccb7baddb107cf9f703919e1a2057640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bfffaa002e603f1746d4140734bcb11d31f11d46f49bd15c8c87658dbe2bbd92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268512898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c62f01d447d75d9d7421d061d4f0060124ea4a4a5d099f94065d2d5f256cc11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:33:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7845fca4b254b8c361b6d30d8a0e5b9d6c5a8df43f1482a7c0ed841be440e66`  
		Last Modified: Thu, 03 Aug 2023 03:39:41 GMT  
		Size: 44.4 MB (44385831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13732bb59235c716d5feeb147388be0507a46221614c1bb12d7b021779e34d7`  
		Last Modified: Thu, 03 Aug 2023 03:40:12 GMT  
		Size: 182.8 MB (182761599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a565c3cb1f8cd41f245613f8957013b3a264838499c1bc2d8c580b5941160847
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232389301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3117034abfe05412e6279df4faaeedb6f2efe734b749483f02f70b23836ab7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:17:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ac461f8a1743501ef6bb272d8425c3b410e894c911165311e282e36b180636`  
		Last Modified: Thu, 03 Aug 2023 01:25:30 GMT  
		Size: 48.7 MB (48671997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecfeb569a89541933b15e8f732b6d5ea530c3db7a69ec0ec203b7616765941f`  
		Last Modified: Thu, 03 Aug 2023 01:25:58 GMT  
		Size: 145.6 MB (145617554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:413452ef2b8b21174edae216d7d575c62f1a75680d16a91bd602faef3fb6cd18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258111819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15472ea9645030f627ea62abc62f9b1dc183a64c830d7ddb5f042130d5c7e063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:39:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:43:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf1c6caaac9b5afe5c21f87c81ea52cb2f170dc8014fc97564f9337986ac802`  
		Last Modified: Thu, 03 Aug 2023 00:51:07 GMT  
		Size: 44.2 MB (44235418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca7ab853d6afc315714a36136c799da5283745fc8dd554205eacc854b029685`  
		Last Modified: Thu, 03 Aug 2023 00:51:33 GMT  
		Size: 173.5 MB (173511122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3108463e296ffe459ea82aa555c65cc845d282c08c133cbc3c89b478efebeed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (293045547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f528798424c0d5cbae974a62b5d3633cb2e55806c2fc356882a9bb10757052d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:38:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e1c2370aa8951d8926c5924bcf24547ca74703904b0527c7f23e46740815f0`  
		Last Modified: Thu, 03 Aug 2023 03:52:13 GMT  
		Size: 49.1 MB (49086146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa281b8d2db730035bc9fca050c2d962532df63e59ee2bf70160dc162d8fc5e`  
		Last Modified: Thu, 03 Aug 2023 03:53:10 GMT  
		Size: 196.1 MB (196103535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:44b784789004e2fccc14b9636f8fa0730efb5f1930d11d54f7c14c56311fabc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240153847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adfad68a288281bc1389101040be477a39a459346be0ac42cacc62af7ed7d1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57b46166fdc730877dcee11a4a6741fc625ecc917bc6560eedc5c318870915`  
		Last Modified: Thu, 03 Aug 2023 00:22:11 GMT  
		Size: 44.3 MB (44275485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2b0c7ea3a3d1a46630eb9d54eec8f2d9242f0b9406342b50959c7ae76e87ce`  
		Last Modified: Thu, 03 Aug 2023 00:22:38 GMT  
		Size: 155.6 MB (155628668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-curl`

```console
$ docker pull buildpack-deps@sha256:4a237279585f720efc7ea4a10525146e9f74927e5058c3a6811d74269068fa6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7dfd90454f1b7d84eb5851a9dd5fbfdc81c9861254e4e47e539856d99a355b94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41365468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a157e768e5dfca25628eecd31c1b7da3442b59c388bae96cc37df6bf96bc761`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ebfe84d045d0585a681615656ce2d21c178ab5958d759d84fcdd6911d5dddb9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38099750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53eaa098522872822fc82aa0430c77e40967328656235898a1766bd50e6f068b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:15e1b21e95f850df357ce2723b32b5ccf5191bcc1ab7476ec7bda4eec7b2dc98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40365279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d91090cdeb11e3d5f2aa2be50867a5582c1cf78e454986031a529673b37e45`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:98d110730769e1fef236121e4a9ae53b0c37b149dba6c92336743e2112d36bc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47855866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f04b9e892d08bce8686689ac9c25c8376a2d70e6dc91c625f4bdf95734b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2d8abebd9d4b6cc7fe03f5e7a5a9ef302dbd29def81c6e0f8041ef083e161e87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40249694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81083bbb06be2b6c5b21c6531f4a63810a49fefb639db3d8523c3c75bba5b77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.04-scm`

```console
$ docker pull buildpack-deps@sha256:e518e67ca402ce1fa4e0b46a64eb4708ac383ba71ac5599242ec01c2098295f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.04-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8454d70a3954956a848da37b18b384fcfcea44bf593c83edd71f86f02562325f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85751299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ad6024b68e422663a1c646150045aa8c2978a4fbc5f589970e5a60e2d05dfd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7845fca4b254b8c361b6d30d8a0e5b9d6c5a8df43f1482a7c0ed841be440e66`  
		Last Modified: Thu, 03 Aug 2023 03:39:41 GMT  
		Size: 44.4 MB (44385831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8a3d85eea75df8415bc37e043642e238772b6d488c2c5b0b5b3efbc781516702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86771747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66f15ddb3b5354fa88a8dd5ce6923e6a77a4a814a8a861e95f73098b9cf7be3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ac461f8a1743501ef6bb272d8425c3b410e894c911165311e282e36b180636`  
		Last Modified: Thu, 03 Aug 2023 01:25:30 GMT  
		Size: 48.7 MB (48671997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5da19ddb7546538c21ea08a02600a19310d9b4e70bceb38b8d28b5ab6e5dc414
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84600697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be6d65056494c7aefc18c52c927cc20d4bae8d5849b343a2b3d8b5258fd8c6d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:39:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf1c6caaac9b5afe5c21f87c81ea52cb2f170dc8014fc97564f9337986ac802`  
		Last Modified: Thu, 03 Aug 2023 00:51:07 GMT  
		Size: 44.2 MB (44235418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:42ef1049dcb29ba27d1b0c9d13142f7abe39fd6029a57a59714b42f7cc0d633e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96942012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0f62a5802f98787f750e871e9f4c643aed0ae466c85991466676a5ca8a4fd6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e1c2370aa8951d8926c5924bcf24547ca74703904b0527c7f23e46740815f0`  
		Last Modified: Thu, 03 Aug 2023 03:52:13 GMT  
		Size: 49.1 MB (49086146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.04-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bd38c179a2089a2fd31e1411fb8039d0fde3144a93ba16a28ed3fbb8a64e1b36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f1cdc23fc8fc1b831ac6c632f34b97cab184a6272ff438b716ebe8e1e0e1f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57b46166fdc730877dcee11a4a6741fc625ecc917bc6560eedc5c318870915`  
		Last Modified: Thu, 03 Aug 2023 00:22:11 GMT  
		Size: 44.3 MB (44275485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10`

```console
$ docker pull buildpack-deps@sha256:889d740fe04ac8069b368651b191c3dff372e77d75f6ee4c3ba79b72eb1fe50a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:15a9c82e91f6055ea56f7093ab3352b638354992022653c97d07bddafde2b927
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.9 MB (467936388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d443c7c75624e3e4d1d108e4ce75ef982f23faf61c6cb56002986ceb62509cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:36:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f019394434fbbf1dc0322c09dce1c54606b0a0995f99872a492c3de4219eb6b9`  
		Last Modified: Thu, 03 Aug 2023 03:41:32 GMT  
		Size: 381.5 MB (381510178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d2d3d8a109f9aee3a8a84b5db4b7a4ee8968e36ddc3b5444d516ff9a29e82fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.6 MB (421628972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad28e1633eea717ac4e3c294c3565d98ce72353358c4847cf40b1f7a874824fa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:46:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780d3e51aaa28824d8d5f1bec7531f98d5db35b9a576d6c08419ade5b0935f37`  
		Last Modified: Wed, 16 Aug 2023 05:54:09 GMT  
		Size: 334.5 MB (334541621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2b275e20b8b5fe54ce2809db704d194f38a8c16840cb8233af7f972b5e721af4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **450.9 MB (450948418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055f72bc14865f7b7ad19033e21241a2fc102800f09200345be0c66e6359bace`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:37:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940201d34510d57ca35e81b1408d0a6893688d7001f16225853e3ad50c4ec0fa`  
		Last Modified: Wed, 16 Aug 2023 01:43:48 GMT  
		Size: 365.7 MB (365681304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f0f104171eb5c17a8352d60506ca6b3fc243aa9f21f00276f864bb351d26963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.8 MB (461771891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4706d0db06585683cffa47739535f887ddcf98fc2bb6a0361061044183ae11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76da498d1d6703121456f54c7ec9587100db812456959db12ee2efca2da463b`  
		Last Modified: Wed, 16 Aug 2023 02:18:44 GMT  
		Size: 364.1 MB (364101369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:24d5d1fca2335cafda10036afa67a1e2b2f8015352f51db269db56f4173c0918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.5 MB (415542447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2315269bf260a2bfd983eea1e176a1b3df29ef2b983f6369a8a789c53d3cc0b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:35:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f743134a60cbf024185cb1ef08197ade21d0e304f5d3f6915df0822b32e9f`  
		Last Modified: Wed, 16 Aug 2023 04:40:51 GMT  
		Size: 329.7 MB (329684648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-curl`

```console
$ docker pull buildpack-deps@sha256:1a3e487623346261603db0f203a84daf1259e84828605400f1a8d93bbd87281a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cd3ff14aac5bd8abbcebc29597cbe8f4da268fed31446be6c300643c6cc3a132
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41640733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e7fea7440d087befe1a7723ef76adf9307317fb275ffdd2ab732c581234314`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b6b70fc65a86ef181308b9d4483306a21297953e302338b8b98dd429a421775c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38148463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682824261387f5531a8beaef8be345112bc3551257c13812203c72ed136de890`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9e5dc452e6b36370b11f94dbac9bae37e89073a8e9713c787528a7d5cbeb3f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40636151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e8f743594afe234ab66c579a551aff038aca5f366902e789b487cf05867a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:49e1f7029605cde20671acc2e750197dfa84e8b1749902240630c8d61fd2b0df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48118121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449f6529b4a74a21fda38d95eddd728bdb55d7eb1d0711936f509b804ca3dbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:219327f643dbe2a1a1e0cbbd61e31d93a8f2cad220aa3635e0bb34e4622ff1b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41043202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b11ab01ff2a750bdff354d4b274b8bfb22158a267a03ebda2ed609b5e32241`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:23.10-scm`

```console
$ docker pull buildpack-deps@sha256:54b98186614665cf884a24378777278a3601ca97609bd24fd164b42d662a056f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:23.10-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:917c5ae7b60b328a63cecd4eb385e1f713f23098c90670f2293a967b9633093c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86426210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5269e6bd4eb9dae1d4063ff31665600eef31956a07caf3e1813f1d2c08a755`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b032b3221baceedc2a1e8e4454f2955d27c547a28abe95a3668336b99ada9a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87087351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b33abfeb555801fa1a398068626db7d9739c33c31dfd97ed7a8eb5e18c59702`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c41c51b6ab982df780eae8161be6d38a64dcfa31eb5e1da76d36ac1df2f6bb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85267114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5e0c1c9ff336e4af720d7c08a9d1426f9825eb87fe1790baa88644d9a773da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd0eae220e0953f1e8f6db015f3819e7a0a745b01bb1d8e0c6cc7cc06b878fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97670522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6f57f844a17257f7bc458e8bd3b32b7ee6f2093e6627869cf392d633985d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:23.10-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8945d029070bc2a1c8a5d326be4e11613a9ab1f1a90a15688e4ea12ce0fef12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85857799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3591f1b927603a4a8b5d31122d54e999416e2ff7d66fe57d05e051a2124c6c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:887b7c1c6349f877496aff09f003d1a8ca44d7920f54c83a3ae5f1663655d7ea
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
$ docker pull buildpack-deps@sha256:cedca83f214f57a77af8d507c7bbd58b9618d324a7f76a8982bf04e0528c8f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348731829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e13db2bf545a7b1de49aa4b5dcd4843cfd4b9bb113c6b8a4352af25328976e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94`  
		Last Modified: Fri, 28 Jul 2023 03:08:11 GMT  
		Size: 211.0 MB (211031643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2c09193e02c99f22817e99a79d739d6a28a9ba088215ea6c54dd2bfa2dec1865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887d75961eb626b52dbbf5253690d3d966737baddd8965129d4d16db7f2965a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:41:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee620d7d428f8ab8f98bd01334daa0d3d3451ab6ce3c2604db13f25fb844b517`  
		Last Modified: Wed, 16 Aug 2023 00:47:56 GMT  
		Size: 184.4 MB (184362791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:346aa10945b5d3dfb334983e9ac38343786fba2b906d44ce42a61f690b17d089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301441954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf80e307949f46b37c0e68056e99719948729e088daf4c43c456f06911f28e5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:29:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d20fcbc5dc95c69a9da8c989746956c1a43040f526f2940cae30659253a710`  
		Last Modified: Wed, 16 Aug 2023 05:48:30 GMT  
		Size: 175.0 MB (175010240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0ced2d9d01077003c3c5d55a93f8e41b392902c6e5265edf70caf9c18429b4e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339572095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d922574f706f083376eb631710c25d0a21a3046824f98272107e43e9160407`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:22:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ae3b61eb9574588be7e73e31c31798e2cbf75f53f1f824d855afdf2be6437`  
		Last Modified: Wed, 16 Aug 2023 01:39:15 GMT  
		Size: 202.4 MB (202422266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c15e9b7c03bf0b95f3f1851dcfc9c0d106eb9f4ad6f70b264a297b2d0eb2328a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.4 MB (351357188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1198ab2df7d04bcf039232d26fd5e7f3df61a5052fc44bccdbf90da8b72d3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb23d9f6cfe824c8d50c7242bc34abd22d983eaf2b3d86f43dc174605402d4`  
		Last Modified: Wed, 16 Aug 2023 00:35:48 GMT  
		Size: 209.9 MB (209946980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:40ca01021b43c5582696c732c712900b7b4a8909c7fc5280c1de8fab1b1121b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325734198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfda94015496c32c381731065d8190dc80cd6a287df3a9363de97b109f153914`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:18:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19a5348eb78e6ca17f708ec635d0965eb52e17623be08930925d53c4e7910a`  
		Last Modified: Fri, 28 Jul 2023 01:34:25 GMT  
		Size: 189.6 MB (189628655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de4665916ba11daa50f4c9cfeb03b217dbd50f83c2200780e5e322bccfbcbb95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.9 MB (362863053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd81888fa25d94a8c677ec5865fdc3a4a6d8e90b13af90684f39c936db3ba470`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:43:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8b794b3ece578acf2202199e34306bae8447e86949ab7b4aa0a7ffa9560aad`  
		Last Modified: Wed, 16 Aug 2023 02:11:03 GMT  
		Size: 214.1 MB (214068144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9531f7edeedf64601eea231ca0a9df5886574ab064a48b54017d35728ad9229e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318160715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417b6bee7ce6cebab35f9a7b46928127192aba8cae28f38b88e80d126be28a70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:21:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fe9d5e378cd41e1b6d5bb16c3c1956dcdef66615bf00a9d29689cc471f4377`  
		Last Modified: Wed, 16 Aug 2023 04:36:59 GMT  
		Size: 183.1 MB (183096288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-curl`

```console
$ docker pull buildpack-deps@sha256:2e3eac33829d6b53d214289b54fe38fc84cf33c99b37237d5398c353d063950d
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

### `buildpack-deps:bookworm-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a313e1ca160fa76c5d9dc53ebd96e5bf59f30162a48a3489fce2e67c2532fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73587893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6cafaf6952dbc34eed9b6f6e2adb817a4b14779c23edc0da1b871b776864e8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a7592f1639d909f25dccc729a2b5aaa513a70ee28a85c4189038b9717092f588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70124664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a21d1f5171263c0576c940aba7c50a5812f345cc44bb53c3530243b7749caa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:70e09d598b5c38a406d30c717457f324114b7db7ef5693e0ae9cc939200c9f82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67169862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2b3159316a467ca9e01e173c57a3aaf9062379e269053863138bf9e55e1d1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cff052d3d1eaf4b534c62e5725852806e16aab4f90a4144c555a766ca1e1b901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73161356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb3957cb621c85ee2f7494fa16ccb1c65eeeff85c9b649dc3c245c2f03e78ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a837769bd3f8a9e4f69a513a0945a56bc51b71fe083f1ded5f3b22600433eed6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75437808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d4066bf6815648a7034016ade53e884437be1fde6892f2b3083044d74b7a86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a3e2a302292d240c5ef6a911d4bfedda10227f69539ea8c2ab29f62a31e82320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73154697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199c7f9557e825f1e7c85367c036809337980df0f60ab3bd943ec9c3ef5a701d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2850f04eb55d1c646bead20a4b56782278f56cac1945ead77243a32e21dbd376
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79224885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ce09dd7847a86d1a80c72f8b63f2fbcc394fc118b4fdb8db043e5ae72e30b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d921b58c4f6cfc3529e474bc5c5657b69f266389dbf9ca1e01a3f993d995631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0935d347529fc2d002323338e9b1d1227981a43082eb49f42287668f6cee7c76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bookworm-scm`

```console
$ docker pull buildpack-deps@sha256:b514f7a71ef85fb2535d7df3fa54310136f7cc6c52aa55040f822eb5803285b9
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

### `buildpack-deps:bookworm-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:529e163a2641648602b7c30f6628836a07309db7eec36b54bc1f3079fe1a0075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137700186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612d62ca1b84af9b3c9ea7d4f8f7451dea5d5280997f2995f5a5476d50e65656`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca109ee1bf05c7a25cab135c9f5f90087363f22e7e296b1345aebcafc2d4c87e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0f43441c554eb412fc1a6cae438793a4ced333e8a6a89228b9ff87bab33e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a1fa0530e19b09fbd7c6185d73d84a4bc942d0411671313e2938ef77ad01ab4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126431714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694ce6041bf7543b9d45b61b59f896cf7826c571374effb2a7e96d4db51004dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3420b56cdf17798958f80fd610bf3004621a3f02bfd92180f1cb4996eb07ea4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137149829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177d9930ddbbf17d991d76e9b71338fede111763111e1bbfe07c60588804ea5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a4d7df737a84cc83cbd61c2dc4edc98541d9bc7ace5cd833a1a14b8a5d027df5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141410208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147bc03aafb5bcbab9affe5fdb15a1a58291461d8982f37588936198fcee1337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9e6b325e9f83cee376fbde36a72981f811fae25c545e31c8915da5654dff04b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136105543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b95c96798319d28a7d61e576aca883a6bd72c3ba77b41f8b73169a8976c95c09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:09c65b2c916c3d1627cb0f348b84676386b69d2923931105735d0d62c5ee5f16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148794909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d2cb79031f827ec74172b6e7d6f32308c68e0b31222d978e62aaf41a7e4ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:48f4ce295c01fb2e62b6b64c1bd63eab67ca9e80601edef71244eb6a7f6a77b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135064427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fbcebb591453ddcf6b4344fadc51626a83a65bb4d445d480182536306e76ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:99d4fb447aa56853cca28eb6bec6af95a288e88df59f3794b318b436146180c4
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

### `buildpack-deps:bullseye` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:438b66cc977016632275ae9457ac3561e691ff7b8035f49159fd485752ae15b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322252653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4a6a6182dd5c7c765fa6e5894539d38a174d2c864885c42e3b8d404b289cbe`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:03:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d4a6da525a13b128e2e4f41081a5af59d2dda8045d40b207510cc3fdc84e1a`  
		Last Modified: Fri, 28 Jul 2023 03:09:11 GMT  
		Size: 196.9 MB (196851463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:17b532724b100b5f9a6c3652c32ce7b09ca9b35c6dba7117ccfe49ee8a3a2d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295307479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d66b8bb5760967b26a5f94dc6855fdce82dd85c5dbca25ec9a9c77c0c415760`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:44:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def812da7393c114766d8e90ea33083736120f2e8410c43c6e3293f0c5c898`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 52.3 MB (52340723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997fb3aae8d3febae5665017c86770b153edfad7973f9c0f8799ae76c9cc4e9a`  
		Last Modified: Wed, 16 Aug 2023 00:48:57 GMT  
		Size: 175.0 MB (175039510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b32b7a67c168925bf754a4aeca1479ed2b016a46dbfa4ef0d2b3d8a9841db7bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282777012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989e9e60b333c3548ba4b4dbef2a01770f2ccbb2232407f7aaec08cfaf9e137c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49800a0424211a8cc1edf5a26d1ebd1afb7c017be3b08cadf2d25abb85d291b`  
		Last Modified: Wed, 16 Aug 2023 05:49:04 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea65231b804ff3a87553e9e8aacba0dd7e706dcceac6cf36be583fbfde69d20`  
		Last Modified: Wed, 16 Aug 2023 05:49:40 GMT  
		Size: 167.3 MB (167333015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:844d16c47e1e2d17df96182fdcd4e61c0684972a54e6baa187b060c4743c2d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313905267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7924790b30f678ced1b1d25feea21aef26d5040f572f27e2c7ce82cce085203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8864a846a08e10fbf877e73678d1f0803227b00a1b16d9ba948070c6e58f6`  
		Last Modified: Wed, 16 Aug 2023 01:39:40 GMT  
		Size: 54.7 MB (54676094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5ec7e6673db06ba035c7c57c4c31b84c89e803ceeb3268a02b5175537b120`  
		Last Modified: Wed, 16 Aug 2023 01:40:04 GMT  
		Size: 189.8 MB (189777874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:34bae5aad734c62848b43b3a22c7e70bb3a643d4507d0d3902f91fd137fea33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327995494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b9ebde7f5d1003596c0622deccc60fd46bfbf4bfa4898c75b6e80e38d0ab95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:29:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fc8bca4c44908804dd201eac5ad8d9316cffd0de391511a9da2fcb3fb48c0`  
		Last Modified: Wed, 16 Aug 2023 00:36:22 GMT  
		Size: 55.9 MB (55922930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da0010c52f973a4d9c39043ad90ee5727579d72d1a34209b0ccc3f1f80515cc`  
		Last Modified: Wed, 16 Aug 2023 00:37:05 GMT  
		Size: 199.8 MB (199768301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:04fffa70f42079b89867ef930ba47542323fedfcc781dcdbb77fac36513759ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301071152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23b0a6fb6d6dc293c2bd5c92deeede8c91b218b1bbfcf8a7da8f3d0e9caff00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:26:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedbdbe02029d723bc1414bf8094fe7b1ac71ed4460a31db174ac0e221fc1b3`  
		Last Modified: Fri, 28 Jul 2023 01:35:29 GMT  
		Size: 53.3 MB (53306734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcffa2b1acd2a62702740ee307e4ae143652253f14c589200b83dad48f46522f`  
		Last Modified: Fri, 28 Jul 2023 01:37:23 GMT  
		Size: 179.0 MB (178972969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b7f2ef729b20579385bf44c5a8f7b2beba8359bf644d5e3b535cd4d9d62362a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330746353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1d9f13617425b5540cae22c07daa37cafee81180bb3a201469d40dc1dd209f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:48:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264ca3322295f7e8f8f191650911a824de696e167ce08aee16d14b5704ea4d14`  
		Last Modified: Wed, 16 Aug 2023 02:11:48 GMT  
		Size: 58.9 MB (58865273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8e5a575991fb77e9e7207e17459595a4a3bd1add713086e44f7190d05ac9b`  
		Last Modified: Wed, 16 Aug 2023 02:12:43 GMT  
		Size: 196.2 MB (196199625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4f9f17ee70cbe00fb5bc22aa1469cb6e15c02775c082b68cce78f7dd8900edc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295840012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:869ab6c8fadc208d4b1436e4cad1f785de717eaf91a2060cf067d3bfc1a7d0f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:24:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c13aebe3a1d06fd7930da9581f9ac789e148f33dd9a84008de9e5da614208`  
		Last Modified: Wed, 16 Aug 2023 04:37:22 GMT  
		Size: 54.1 MB (54061692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83fba4183bca79f260d587a76c94532cc7c3a0419169722dbbee232fee2d9dc`  
		Last Modified: Wed, 16 Aug 2023 04:37:47 GMT  
		Size: 172.9 MB (172855751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-curl`

```console
$ docker pull buildpack-deps@sha256:a895b5fc7d66746a583d5b3a8de5a62aa17f837ba00e4bce340eea6a91c59c5f
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

### `buildpack-deps:bullseye-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:765f83b96d5a3171dd95060b09769740f829e02da450d4de25c1e0799d84a14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70816156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c8a817556d148562359d5c71ce5a3b56490421d4acab107995d9c2302a9755`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:93b3abe77348f08b71522c036a5ca22a336ba6722e0b9d5a416bd6393423641d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67927246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1f7299b6c9682ee4de2673118efdd4d37b05bd5070ab6caecf06095465b9c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3e8e5c8b704a1e7108b413f5c3ac9d287848becc6da7f020e9eac097a482fb3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65088329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3401d58e46bbb699218d5ce23026e614fa7fd0f8d6a80b7410750a19990b22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:87db69382d408253d6331ba2f3acc990db07b546cb54209153e5b311582cc128
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69451299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48a220cd587f717272d10bb47fc8eec3fb65e0e425865dd2bd0d8a3a790e546`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c0ac3a855c0acba7d79a0a3e5f08e5df6bb608e5640c893cbdd94c06fea6e366
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72304263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab191c09fc96b7ed761406c1f6bb7fce32db191c3c30eb65900539dbcc1cc43d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9039063fe1bc35f199e092c3cc23d24ce8e031fb1f825b2b259d0c05d05203fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68791449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1ae7b77ee8867744f83a9dd4c8e0546a5248a7ba1c805c6e0a155413d02003`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12cff15e25bd30781a2e1c2d09d3e682d87156aada09021b1532f373926bbe22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75681455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526a075d6b3c700a1d8d75f6f869ae0719e7bc6c56bf35097da945ae6048fa35`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:acb9713373d6f573d0115ffdb72db6a5055a3f6f2eb042caa7f3565af683efa8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68922569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f39ba35c8d28886bd170e7d2d7d9b2bd37108153ae50e5027226419680ba5af8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:bullseye-scm`

```console
$ docker pull buildpack-deps@sha256:fe0040db0382ac581a1ab193009277a7d4fe87c2efef19e481c22b1eeadbba1b
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

### `buildpack-deps:bullseye-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4bae423df8eeba414176292d04ba3cd36c7cdbf9fb57aee7eba666c16d5647d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125401190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed57311c87c592557b79298b2f29ddeb0d29042e26414aaa59856ada65d01be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fa65fe73934264c4d9ee23ce0366e222f470a002b1cc7a87e8ad9fbc7563d089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120267969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:836038d13fceb192024c5d9a931b66f73f27172d154be24045d79f291ba5f867`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def812da7393c114766d8e90ea33083736120f2e8410c43c6e3293f0c5c898`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 52.3 MB (52340723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e7a1e27e1c8e9cdc898d21947c3eb25521d92ff8d456ea6c7b5c52d4d89197fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f92c6fc9e6de615b43e074d770c35f37177e9a23f8ed52a3ce72b881c0c68d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49800a0424211a8cc1edf5a26d1ebd1afb7c017be3b08cadf2d25abb85d291b`  
		Last Modified: Wed, 16 Aug 2023 05:49:04 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9222281f3a18fc1f68ea3ac87cae13cecd6102b3e6d3d2a963e198b9b149f4f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124127393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900914194df7ad3b6dd6d9b5ce4b277ac3924cb43f60a296c43e23ec0f78cfcb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8864a846a08e10fbf877e73678d1f0803227b00a1b16d9ba948070c6e58f6`  
		Last Modified: Wed, 16 Aug 2023 01:39:40 GMT  
		Size: 54.7 MB (54676094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a417452b134c7560ef87b1b81bfaf3bc47f4fa7f86fd4806520a456918a66f78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128227193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f2d6166d0c7afd732a0578cfaaa2cc6809a65a41a045e333d8e52930b7bc04`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fc8bca4c44908804dd201eac5ad8d9316cffd0de391511a9da2fcb3fb48c0`  
		Last Modified: Wed, 16 Aug 2023 00:36:22 GMT  
		Size: 55.9 MB (55922930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:de2ebe9c144a695a12a0f0c57c3cd8b792a84f597dba4c6c18005d4f0bd5da55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122098183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0552ed08f1ab1ca70de1a1f7134a552c58c6f55460faa2343f594e349ca09573`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedbdbe02029d723bc1414bf8094fe7b1ac71ed4460a31db174ac0e221fc1b3`  
		Last Modified: Fri, 28 Jul 2023 01:35:29 GMT  
		Size: 53.3 MB (53306734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:842a4c3acbebc913c51002c40c17c0b323fcb71c84a289556516203f2acb0512
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134546728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c8963e9ac71f3a1646ae9e35de4bd37f9dd002e1abf815edc5224f4b43081a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264ca3322295f7e8f8f191650911a824de696e167ce08aee16d14b5704ea4d14`  
		Last Modified: Wed, 16 Aug 2023 02:11:48 GMT  
		Size: 58.9 MB (58865273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c8e4fc3b1a6bfc55b26bab453040a0274970583846bf439f6b13dd696c301aa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122984261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:407d4b94d5f7066269549cad4832b06621feaf2d81e4b606cd7c9befe2d74b0e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c13aebe3a1d06fd7930da9581f9ac789e148f33dd9a84008de9e5da614208`  
		Last Modified: Wed, 16 Aug 2023 04:37:22 GMT  
		Size: 54.1 MB (54061692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:04c20d12fd1677dbed7598d833244bb475777d06fa6759ec2fd34aba4bc5a44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4edf3ca07fd5f768c4550f27782374c299069917c99ca367692ec7b0752124b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311846087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ceeb7ee443c80095761b84c6e6d14fe95695139a577f5896d82df863c05d739`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947969e624beff93eed664f9f52a08712f3d1e12cadbdf929ff928f93d2c383c`  
		Last Modified: Fri, 28 Jul 2023 03:09:36 GMT  
		Size: 51.9 MB (51872820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87da2254b9de06a71bc1828dec0a28f6a16af7cade75310533cf5cff9ac7e669`  
		Last Modified: Fri, 28 Jul 2023 03:10:06 GMT  
		Size: 191.9 MB (191895767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83de578f6c86e2358914904d27edcdf37ac4808f7f285f0c4c1fac77083afa24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277648206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d30fd2556a67937a5b7268b965735eacd708f8dc3d4e4ff1c08b76e81af2c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:33:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed6203f3da20d3e0f8ea7d7ec6e4fdd2cafd582b494e1e9fda0ddf4f9a1a2f5`  
		Last Modified: Wed, 16 Aug 2023 05:50:05 GMT  
		Size: 47.4 MB (47370312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d2cb1f3e23c88fb017f1bb7af1d240169a419bc5190369b10152b8b8255ef`  
		Last Modified: Wed, 16 Aug 2023 05:50:34 GMT  
		Size: 168.1 MB (168099748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e3957f362fd2e9f06d91adade8d2e044072cff03f6169e24f768f861a69e1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302423969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a874813819499ae0978b7c10310b76414d80e88fbb4de176610431986df9aeb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a2c1884c14fa4ef92ad6f8b2cc931880f6d1a02f21e866d6c636416741e74901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321279222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8df92c12e389a10a361e57c1ab32475ffb3eaf24c8aee4fea97676f158255cb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:30:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:31:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377913e8bda7ade79ce7bc10aab7401851a4cb9565903c8bca5b0360b4fab3bd`  
		Last Modified: Wed, 16 Aug 2023 00:37:36 GMT  
		Size: 53.5 MB (53486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772141f0f201b519ab5689ccf41e7601936a21705c554b9ee73448eb217def09`  
		Last Modified: Wed, 16 Aug 2023 00:38:19 GMT  
		Size: 198.4 MB (198441615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-curl`

```console
$ docker pull buildpack-deps@sha256:789ff8d52fc9bfa8c2d627b94509ab1dea950d9b9045d1bffd0366231cbd19dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:052ecd162488e2bd9bca20f30afddbb0364e89bdd3263929ce8565850abadcd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68077500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:253b3ab6acbb874be58d7fb897ab0e2421ec59ddae5eb5f5fd766b59c4317abc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f82d9d6d25056fe6fc40e32cccd2fb79b2b19a55a3b30d694740a37e1204751
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62178146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc04b2bd46b3344ee4a82315b3fb423ee077d0af9ac5592445f96d517929eb2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:693fba8369c38b01ea7646361a202296d268f8452d59f1622d04534bf8363085
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66741963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da913c23eb14e30f7e30aaada367ad899839db75c2d632e31b6c1d7ce8752659`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a2f6bc9bc0541882d918d0b6b577d0fc0176c4f25f15e3c1991d4650171fb292
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69351416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e1f222da00d74c27c7fc35eef2dacdd3f2a6c346602e90d5b74493308eb88e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:buster-scm`

```console
$ docker pull buildpack-deps@sha256:f8075fededa2e3d394adcf18195e24ebe2ec2e07b90cae9934d16f79c6bf783f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:buster-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ca3829a7e5276647ed7914a9f714c961f10aec2e35fd937df553b2c3bc4f1ae4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119950320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b38333a879cff0f96573c5ccb535b08b9462278d629bc91ad0539b1dc34d924`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947969e624beff93eed664f9f52a08712f3d1e12cadbdf929ff928f93d2c383c`  
		Last Modified: Fri, 28 Jul 2023 03:09:36 GMT  
		Size: 51.9 MB (51872820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:91958af6ba88267b2c1a8939a18048fdc1d3925fc906b6084585fae2d6595a0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109548458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ebbf20cc2fb0cc3bd845c46749f5519bd8993fca7af3933636ce84c0e57f3d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed6203f3da20d3e0f8ea7d7ec6e4fdd2cafd582b494e1e9fda0ddf4f9a1a2f5`  
		Last Modified: Wed, 16 Aug 2023 05:50:05 GMT  
		Size: 47.4 MB (47370312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:89051961c8ea98935f890b00aaba8c4e399234099c594595e60e083656063cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118960340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927f459518de5d7f199fb58be93dc1c5466f6d45cc64f9338916dc1d4101282b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d45c3ac03e143eb6954fa296ffdda449cfb86c2e40cb29fbfbc0e6dfc092ea74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122837607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2744c8f7c22a22faf342c3a48670f2e072667ac3fe46dc100663e370effa0632`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:30:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377913e8bda7ade79ce7bc10aab7401851a4cb9565903c8bca5b0360b4fab3bd`  
		Last Modified: Wed, 16 Aug 2023 00:37:36 GMT  
		Size: 53.5 MB (53486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:curl`

```console
$ docker pull buildpack-deps@sha256:2e3eac33829d6b53d214289b54fe38fc84cf33c99b37237d5398c353d063950d
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

### `buildpack-deps:curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a313e1ca160fa76c5d9dc53ebd96e5bf59f30162a48a3489fce2e67c2532fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73587893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6cafaf6952dbc34eed9b6f6e2adb817a4b14779c23edc0da1b871b776864e8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a7592f1639d909f25dccc729a2b5aaa513a70ee28a85c4189038b9717092f588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70124664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a21d1f5171263c0576c940aba7c50a5812f345cc44bb53c3530243b7749caa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:70e09d598b5c38a406d30c717457f324114b7db7ef5693e0ae9cc939200c9f82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67169862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2b3159316a467ca9e01e173c57a3aaf9062379e269053863138bf9e55e1d1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cff052d3d1eaf4b534c62e5725852806e16aab4f90a4144c555a766ca1e1b901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73161356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb3957cb621c85ee2f7494fa16ccb1c65eeeff85c9b649dc3c245c2f03e78ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a837769bd3f8a9e4f69a513a0945a56bc51b71fe083f1ded5f3b22600433eed6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75437808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d4066bf6815648a7034016ade53e884437be1fde6892f2b3083044d74b7a86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a3e2a302292d240c5ef6a911d4bfedda10227f69539ea8c2ab29f62a31e82320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73154697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199c7f9557e825f1e7c85367c036809337980df0f60ab3bd943ec9c3ef5a701d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2850f04eb55d1c646bead20a4b56782278f56cac1945ead77243a32e21dbd376
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79224885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ce09dd7847a86d1a80c72f8b63f2fbcc394fc118b4fdb8db043e5ae72e30b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d921b58c4f6cfc3529e474bc5c5657b69f266389dbf9ca1e01a3f993d995631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0935d347529fc2d002323338e9b1d1227981a43082eb49f42287668f6cee7c76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal`

```console
$ docker pull buildpack-deps@sha256:4012d4c808c46a9a637840bbdd390b6c376567bd757dd7f9e3f220cb6acb0172
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:acd56f331b33212692b155f660b552b4c88f58d5ff8872826cf7776d8254e736
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.8 MB (245803354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fda0fc31b0a48175e7336ca929f7ae5db6d6b985ec61f1eb2e34e09e47c0fd6`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:27:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e934f6d128d65c709d47ca01bccaae13c479a8306ec18c7fcd2b492f16089c4`  
		Last Modified: Thu, 03 Aug 2023 03:38:43 GMT  
		Size: 60.9 MB (60923971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d83c40e01065bb197fcf80fb04dacbe13913dfdd9d8f9536fc4585b63af296`  
		Last Modified: Thu, 03 Aug 2023 03:39:10 GMT  
		Size: 145.2 MB (145169180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:583ccef8d57e8083fb49465862f1d91a72c4c354463b55d48b40981af478232d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **212.0 MB (212026855 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aae217cb1499d44d0503a7acb9635a9ef089e3a054c66d3496428a9f59f7eadf`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:09:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:11:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab787541d8bd910e22e242d890b591088a8056ebe44d8f49093e22e780fefa7`  
		Last Modified: Thu, 03 Aug 2023 01:24:28 GMT  
		Size: 55.8 MB (55824728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1b16044bcb697f6b7460deb249f147af14046beb812b7673eb8c7b42ddb89cb`  
		Last Modified: Thu, 03 Aug 2023 01:24:54 GMT  
		Size: 122.0 MB (122010037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f4561f7a165e00049e2fd0d22f71bd39b9c943b958ffddf108fc8cb0c2d3352c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **236.1 MB (236070832 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:472e168e1909b18bfb49feb06a8f81249f49a2b79eeb8afffdef29e96cb40d03`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:33:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:36:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7d1a175de684642bf290a3882b913844851fa5b7582e492e466ed74035f035`  
		Last Modified: Thu, 03 Aug 2023 00:50:08 GMT  
		Size: 61.0 MB (61014742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257b81580f56d0fdcedfd9d17039d8c6225cadba4d0173a78cc30a3a8ba87562`  
		Last Modified: Thu, 03 Aug 2023 00:50:31 GMT  
		Size: 136.9 MB (136872285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:455def3ef4d52747cdbaab828e783a0881efde84a4f41064e8223ff241bc624d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **269.6 MB (269569036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b53b87cd5bed2144465a3b4f663a78abeed0b756f44e4adaf79bae8e7cfd6d0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726e55a0f98534a51453930e4c0788ba5f9425af2106a0f632242d22add5e029`  
		Last Modified: Thu, 03 Aug 2023 03:50:26 GMT  
		Size: 69.6 MB (69644291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aec136ee45fd038a87eceb7f9940509dbe2343c5dd06ad15175b2c74454a0520`  
		Last Modified: Thu, 03 Aug 2023 03:51:18 GMT  
		Size: 153.7 MB (153680155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:146a4f8c725380eec620a5f6d2f018386dc774ce13692cc79159c2f120c7137a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **226.6 MB (226607654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed94ac912c0ed9895b3abef8896dee8e605f2bc4e578bb2b29f23932a7ba0bea`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:11:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d1c95e4e206b384145bd8128e74027e092da89c7654f4aebfd616735756a6f9`  
		Last Modified: Thu, 03 Aug 2023 00:21:42 GMT  
		Size: 128.6 MB (128593276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-curl`

```console
$ docker pull buildpack-deps@sha256:18e96a2da642503b6b1dd2a822a6f08a04573f3641cb18ab50b7cae0a00648ff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:25f7002f1f22788abd523a869097b453d18139ad76634090717fcaadd420c8c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.7 MB (39710203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e0bf7833fb8ea45c517e7a264f113dd4ad0750a8ca080acdbe8175645371016`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:277a8c3f670eebf90abb7d136c5a7f7bbea2ba47c638604a7c3fde09b5a73623
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34192090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:86a4d7cc90e6e8e793f1b97cccf70c09f05538a4936ab7f69f3cf7297b7da660`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cf755867f779cd7d3788c2c3c8c6825ab43fb5487616afda3928d832cf0e7af2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.2 MB (38183805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a79375418b299d399ca410b47922d62003dde194891a752b910e8982ce198a0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ff870a684265eb22a3502debb0824422af014d8a4dc397696f8a589d12246045
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46244590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d6b65f4dbad88c0c655d3477312f05d99ba5d188ca0fb47c6caffc0a44050b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:028f59f497fa2c8e7f3a358182ef00c601e83780a8c7f9b0fd4e4f0f735ef4cc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37702848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:674186b606991aba08faede7dbb56393ab45900ba8c3e92969a9030076dba1be`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:focal-scm`

```console
$ docker pull buildpack-deps@sha256:6777277d166b7084754912e6fa30b35bc6e37a817429346aacaf3c99b544b60f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:focal-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:adfac55a5e84f9a71a4011f19ff1f92d9dd15e59dc30bd400dde2b3bc506a95a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **100.6 MB (100634174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cdb4a6f59d3ac3f984df2be0978789f608389a147873c4fd36ac32be18a0fd5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:43 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:44 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:44 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:45 GMT
ADD file:233702cd816c07bc9fed02881b11fb3bdcaee41f3ce3ec1c9f0c4a060b155d5b in / 
# Tue, 01 Aug 2023 06:16:46 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:25:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:26:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7007490126efaae58924972668256aaeb4858e6c4537eb4257e1978719b958c7`  
		Last Modified: Tue, 01 Aug 2023 08:35:40 GMT  
		Size: 28.6 MB (28580671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b760f979d621293059198043c3182e5ec2b4b45e69092400dde90539cb49b70`  
		Last Modified: Thu, 03 Aug 2023 03:38:26 GMT  
		Size: 11.1 MB (11129532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e934f6d128d65c709d47ca01bccaae13c479a8306ec18c7fcd2b492f16089c4`  
		Last Modified: Thu, 03 Aug 2023 03:38:43 GMT  
		Size: 60.9 MB (60923971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9d44afa60dd5fb0db64fb915f1251f44e3ebf76b47981d309412e717fdfe3419
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.0 MB (90016818 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8254924c1588feb35db2643cade83e5af7f78c7e94ef3a02c420fd8d5bce794`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:16:45 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:16:45 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:16:46 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:16:49 GMT
ADD file:60aa8465a6ba5538decc41365cc9b78ae86131e8c2cfc9177b4a336354ead988 in / 
# Tue, 01 Aug 2023 06:16:50 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:07:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:09:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c429b4536d4b2ab209b0a779f71ba68570f10acf9dd806c7e2011fce49bd5c97`  
		Last Modified: Wed, 02 Aug 2023 04:28:29 GMT  
		Size: 24.6 MB (24591882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46721bfba0a61dc74069a495cfc69b6d82652a48543529e8eff034aed6d1896b`  
		Last Modified: Thu, 03 Aug 2023 01:24:07 GMT  
		Size: 9.6 MB (9600208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab787541d8bd910e22e242d890b591088a8056ebe44d8f49093e22e780fefa7`  
		Last Modified: Thu, 03 Aug 2023 01:24:28 GMT  
		Size: 55.8 MB (55824728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a42388d0c67c42187cf6e82f611a70a45a4db4ab48b0282b7f8e420f4b8d0087
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.2 MB (99198547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f01d02871cdea6466854b6ebf99bb53d48314df82755480b0a7df3158700688`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:56 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:56 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:56 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:57 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:21:03 GMT
ADD file:ef6e767091d76c1461d099d5bc7a18c526ec80834cf87280803ab6480192f766 in / 
# Tue, 01 Aug 2023 06:21:03 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:32:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:33:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:edab87ea811e56041127f5e9eb4115fb62cb96d0e6a14056e0d2dbf51a945a22`  
		Last Modified: Wed, 02 Aug 2023 04:28:23 GMT  
		Size: 27.2 MB (27200587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff9cde664301b9f7595a7be10f0562bb40f4efb6461fab8f928eaaf190a3632`  
		Last Modified: Thu, 03 Aug 2023 00:49:49 GMT  
		Size: 11.0 MB (10983218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7d1a175de684642bf290a3882b913844851fa5b7582e492e466ed74035f035`  
		Last Modified: Thu, 03 Aug 2023 00:50:08 GMT  
		Size: 61.0 MB (61014742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ed245924e86e7281a3885a36bfffa044077c144dd55db087aafa03f503c8248e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.9 MB (115888881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12179e95e3e7c1da6373ed192b5977cea19225ea0c9e1e468ee59b5bd566c345`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:20:36 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:20:36 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:20:37 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:20:40 GMT
ADD file:822df76493d1d533c1a283ab7bb20ce81309f57279422a0eebb2ffb9fab55963 in / 
# Tue, 01 Aug 2023 06:20:40 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:24:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:25:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be0253994e7bea97e6b44cdeec04bf996c8dd3380e70409de3783a1d1971e747`  
		Last Modified: Thu, 03 Aug 2023 02:50:24 GMT  
		Size: 33.3 MB (33306772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6255c4b5159764b2cdd4af0a7217ac0e6340085f9d26760931982cc32ede902`  
		Last Modified: Thu, 03 Aug 2023 03:49:56 GMT  
		Size: 12.9 MB (12937818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:726e55a0f98534a51453930e4c0788ba5f9425af2106a0f632242d22add5e029`  
		Last Modified: Thu, 03 Aug 2023 03:50:26 GMT  
		Size: 69.6 MB (69644291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:focal-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:079f48635b01d56e2478857b7e0c5fb6212336f9e594e783bbf19cb9dda8b0f2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.0 MB (98014378 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2522830f5bbe1d8ea3e120ce6ff28c07dbc6f1a8b7f24c17fbb61b252bbab549`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 06:17:39 GMT
ARG RELEASE
# Tue, 01 Aug 2023 06:17:39 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 06:17:39 GMT
LABEL org.opencontainers.image.version=20.04
# Tue, 01 Aug 2023 06:17:41 GMT
ADD file:36efc3ec29bb54e0987fe91be1aa7cc849909b3cd2534af3de2d3d07a03804cf in / 
# Tue, 01 Aug 2023 06:17:41 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:08:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:09:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:365fa2124eb5f6f369204f3fe0210d9965952628707dfacd4194a8e15caf0420`  
		Last Modified: Thu, 03 Aug 2023 00:03:37 GMT  
		Size: 27.0 MB (27014233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b6082f2457965a87b9693265b680b0a0aa5d30ef936b6df14487a947354b10`  
		Last Modified: Thu, 03 Aug 2023 00:21:05 GMT  
		Size: 10.7 MB (10688615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5764a6c44dcfc11bcbd3dda534db4967a8ffd1443cbe922c189701e996c2c222`  
		Last Modified: Thu, 03 Aug 2023 00:21:19 GMT  
		Size: 60.3 MB (60311530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:70272962f14206151d3f524e9a2cb91913d4d36ff7109ccd76356c1600f5fd15
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8f28bd087741849791b564aea220968c88f2cace4063336681cd238858e05a79
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.8 MB (249847907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:442a35809fbea57170756e05e1a3bbb375ae8094fe1dbba784e092fd2935b0d5`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:42:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e13d40b1da6010e8c9c1adb56fc6fb577c2db289f338cac71cc1c97fd28e6bdb`  
		Last Modified: Tue, 04 Jul 2023 03:56:35 GMT  
		Size: 172.9 MB (172868010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:82dc71eec7f734241614d16b3a4eb66ebfef9c7a6ad60a3fcb9fe8819fad561c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **216.8 MB (216815905 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c67a668d45893320321a9b7d361c43ba1aae9afad349f124144018c6aff67fd9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:41:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcf856a6334dae4b42fc54fea2a58544fa35961851c6d1e3007586c1e0917f`  
		Last Modified: Wed, 16 Aug 2023 05:52:13 GMT  
		Size: 42.2 MB (42244900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b51d420affa83085eaf6a3e84b9fc5325fde73b64976b53d13bc996be9f681`  
		Last Modified: Wed, 16 Aug 2023 05:52:42 GMT  
		Size: 140.5 MB (140522119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:25554a1e81affd0a7148f3363ded7ad133e915712366dda969f4db3cba8dd0c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.3 MB (241336078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff063c8c03b0f010bed01ee0a96a37316ca6c1433490497ba5b53bc2f78a7494`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:32:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6bfccc5cc58c82f10e31821cddd5b985299b78e91935c891542b24f2c62f3b`  
		Last Modified: Wed, 16 Aug 2023 01:42:14 GMT  
		Size: 39.4 MB (39368139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb4614e2cec4ab0ddfa81eb3ced0780c45cdeece6b214d12aabf70908c95cfb9`  
		Last Modified: Wed, 16 Aug 2023 01:42:38 GMT  
		Size: 166.5 MB (166509502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d66a2fc9c52dd6d4f07d37dafb2ef3749f915a796dc77f6a928ae2246e368c10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.6 MB (271602068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4148c1e5b7fea252f7458c7ecf09659195b74c760ea787cc0dc0368ea23dc2d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:00:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3975a415c70a582703af5a6d25f7b6ab2976130066120608bb8fef4936ab082`  
		Last Modified: Wed, 16 Aug 2023 02:15:26 GMT  
		Size: 43.9 MB (43888713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e3a228c1be7d7fb67b215e897afc46ce5832e6b00e93abb38c6d2d8f4a02bb`  
		Last Modified: Wed, 16 Aug 2023 02:16:21 GMT  
		Size: 183.7 MB (183741262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ead5c3b74a1b308a84ea43da09bc2c04761f4a51ff69fb75ea39b13d99286cbb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.8 MB (223828482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9e4f9598e552d8b03ad050606aeef9a8cc92e510c28491e18d48e8ec738e940`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:28:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:30:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4d2ca10795ab9674ca09c980d55a84f444920c9f376729aa86df29e23983ca`  
		Last Modified: Wed, 16 Aug 2023 04:39:14 GMT  
		Size: 39.4 MB (39415890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9ae7a022bc926e602497a803fc2ba318c956f9c66d679e809d0fd3d33a37f`  
		Last Modified: Wed, 16 Aug 2023 04:39:38 GMT  
		Size: 148.7 MB (148734530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-curl`

```console
$ docker pull buildpack-deps@sha256:9a4f3770ddcbb5abef530b0f63462986ef979ea26544c0b6d4a95723ff04223e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:483b82bc040102243b07bcbb2bb61e88294953b57782d2ee84dc0b81db449cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37551100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57a6f6f87887de69ba89a8eba29dd185ff073609b204037b4931d8322101cad3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:56577af195afd5422d9ecfe7417e22ba5fd0b6a9e410101b0975e30b24370335
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34048886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aaf8b344d04e5a7cf7cee8a90956443b1a27253272b508d2192af5af19a9098`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d5180a814a3d67003fd3fa28cd6c26a857d47db8ef15e95d52855b2986bf8e82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35458437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:994829797c5fefa7b4ef655e8643c5a0d83916c5984d16465f65489315a7cd51`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:752573e2a0c2b750c4f0955e0ef1c44e4001e2534b12ff9554d6967750f3ca2a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43972093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1722b70ab45b97523406b34ccf447edd8188aacaa4744a27be94d231d73b04a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:55b68aab71baf930050c4e24bd323974bff4e14835cf93f741e94d233fd5d787
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35678062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2291cf79328dbbcc70c7534a4e837c075a137ecaefaaa763466fab1521bd10d7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:jammy-scm`

```console
$ docker pull buildpack-deps@sha256:2a2e28268de88785f14de8b3e871669c77a888b0b033b016d8fc07b67addbbe8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:jammy-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c79e22f6262ffcc9eb5eee479f1728247ee7c37e1419034d7ef047a9cd8b649f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.0 MB (76979897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da96a2a7c92bf335b49390e599ef90eeedbad15d69f1c2f3bac70574468ac75`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Wed, 28 Jun 2023 08:37:40 GMT
ARG RELEASE
# Wed, 28 Jun 2023 08:37:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Wed, 28 Jun 2023 08:37:40 GMT
LABEL org.opencontainers.image.version=22.04
# Wed, 28 Jun 2023 08:37:42 GMT
ADD file:140fb5108b4a2861b5718ad03b4a5174bba03589ea8d4c053e6a0b282f439ff3 in / 
# Wed, 28 Jun 2023 08:37:42 GMT
CMD ["/bin/bash"]
# Tue, 04 Jul 2023 03:39:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 04 Jul 2023 03:40:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d19ee268e0d7bcf6716e6658ee1b0384a71d6f2f9aa1ae2085610cf7c7b316f`  
		Last Modified: Wed, 28 Jun 2023 11:50:41 GMT  
		Size: 30.4 MB (30431229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97966f3f03442a3d645f8354f49cc622b4416879f6c59142fab244ca2663677b`  
		Last Modified: Tue, 04 Jul 2023 03:55:49 GMT  
		Size: 7.1 MB (7119871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e29c969f29843010dfda55528bfc810b4e577e4ba39fb2c788a8ea55bb92763`  
		Last Modified: Tue, 04 Jul 2023 03:56:05 GMT  
		Size: 39.4 MB (39428797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ceffe5bb7f37971ba502f342d42b22fde4d37c2bfaddeb0f03b26437b5bbed31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76293786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2801ef2b20fdc536062325b8f61fc4681d965f31312a81e88d8128c8f713d333`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:19 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:19 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:19 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:24 GMT
ADD file:ca783750060711e8590ab362921bae8d7b02201c48fa3d2cb3fdf6aac045a793 in / 
# Fri, 04 Aug 2023 05:03:25 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:37:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:37:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24758824a30b6e1f6132a6b6740dec1fc5723821f0f2b5b6513379480e0f74f9`  
		Last Modified: Sat, 05 Aug 2023 02:03:56 GMT  
		Size: 27.0 MB (27029194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2bbdb113a0790e21df8c0b5f40836a9900213d1d697e6ea968456f1516e8ec`  
		Last Modified: Wed, 16 Aug 2023 05:51:53 GMT  
		Size: 7.0 MB (7019692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47bcf856a6334dae4b42fc54fea2a58544fa35961851c6d1e3007586c1e0917f`  
		Last Modified: Wed, 16 Aug 2023 05:52:13 GMT  
		Size: 42.2 MB (42244900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:4f5048207f874df8fbfc050b4517760eb23860f7f1fd21951d0f522b823f6ca2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.8 MB (74826576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7076967d855557f64f160cf4366c5ecc6bfcb8cfaf2af9b9bcff432666952cc9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:51:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:51:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:51:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:51:18 GMT
ADD file:5cf7797cf86362218d2bd85debeff136ee897af7eef95a0b8baab9f9457c3e89 in / 
# Fri, 04 Aug 2023 04:51:18 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:28:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:29:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ea365e1e52efb9567c56f02f2200f0e95ddffd579225cc5b20a6333119d2811`  
		Last Modified: Fri, 04 Aug 2023 13:35:19 GMT  
		Size: 28.4 MB (28391903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a1fcb60c8beda77ecd71dcfb3b3564d3a6ac8f00400bfb5b94c463aa514292`  
		Last Modified: Wed, 16 Aug 2023 01:42:00 GMT  
		Size: 7.1 MB (7066534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6bfccc5cc58c82f10e31821cddd5b985299b78e91935c891542b24f2c62f3b`  
		Last Modified: Wed, 16 Aug 2023 01:42:14 GMT  
		Size: 39.4 MB (39368139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4c3eb26a7d946b19c481386715e1761a62073bf47fe5830640ca660923a53162
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.9 MB (87860806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:380b59efd0d618a11314b3eb0cb43fb9ddb4ee8437cb5067f1a03a1d75af9c2a`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 04:56:16 GMT
ARG RELEASE
# Fri, 04 Aug 2023 04:56:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 04:56:17 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 04:56:20 GMT
ADD file:0e9b840e6824ee009acbddc2d337fd5083ebe606393cf7532cdca4f108813ca3 in / 
# Fri, 04 Aug 2023 04:56:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:54:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:55:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09f4821f68917c7929419fff8bc583c406640180ea7d58eea03a95e463b8fb21`  
		Last Modified: Wed, 16 Aug 2023 02:15:01 GMT  
		Size: 35.7 MB (35712693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60af6561de43c48f5de8ff8e45c191bbcf92b6d63f8a10bd079217beb4fca6db`  
		Last Modified: Wed, 16 Aug 2023 02:14:55 GMT  
		Size: 8.3 MB (8259400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3975a415c70a582703af5a6d25f7b6ab2976130066120608bb8fef4936ab082`  
		Last Modified: Wed, 16 Aug 2023 02:15:26 GMT  
		Size: 43.9 MB (43888713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3cc3f2368befd688a4db83b00f731ea5b910aaa0cdec162156ee6f6bb1ce54ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.1 MB (75093952 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd8c28857d76ff033c28d3b0164808eb366e80313fc99d5eb350b0993683d06`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Fri, 04 Aug 2023 05:03:14 GMT
ARG RELEASE
# Fri, 04 Aug 2023 05:03:14 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Fri, 04 Aug 2023 05:03:14 GMT
LABEL org.opencontainers.image.version=22.04
# Fri, 04 Aug 2023 05:03:16 GMT
ADD file:d5b5687c046ca0689ccc4f42ddcc27543404ae2273aa12241e6636a2b3d675df in / 
# Fri, 04 Aug 2023 05:03:16 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:27:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:28:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:de1d106061fc0332ca262e39ed7d2aa6384ae341a084b39449e21c742802df9c`  
		Last Modified: Wed, 16 Aug 2023 04:39:02 GMT  
		Size: 28.6 MB (28644373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ac62e13283d0be6884e968c8608389358a6fd7c99cce2070d79fa4c2add41e`  
		Last Modified: Wed, 16 Aug 2023 04:38:59 GMT  
		Size: 7.0 MB (7033689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb4d2ca10795ab9674ca09c980d55a84f444920c9f376729aa86df29e23983ca`  
		Last Modified: Wed, 16 Aug 2023 04:39:14 GMT  
		Size: 39.4 MB (39415890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:latest`

```console
$ docker pull buildpack-deps@sha256:887b7c1c6349f877496aff09f003d1a8ca44d7920f54c83a3ae5f1663655d7ea
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

### `buildpack-deps:latest` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cedca83f214f57a77af8d507c7bbd58b9618d324a7f76a8982bf04e0528c8f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348731829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e13db2bf545a7b1de49aa4b5dcd4843cfd4b9bb113c6b8a4352af25328976e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94`  
		Last Modified: Fri, 28 Jul 2023 03:08:11 GMT  
		Size: 211.0 MB (211031643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2c09193e02c99f22817e99a79d739d6a28a9ba088215ea6c54dd2bfa2dec1865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887d75961eb626b52dbbf5253690d3d966737baddd8965129d4d16db7f2965a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:41:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee620d7d428f8ab8f98bd01334daa0d3d3451ab6ce3c2604db13f25fb844b517`  
		Last Modified: Wed, 16 Aug 2023 00:47:56 GMT  
		Size: 184.4 MB (184362791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:346aa10945b5d3dfb334983e9ac38343786fba2b906d44ce42a61f690b17d089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301441954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf80e307949f46b37c0e68056e99719948729e088daf4c43c456f06911f28e5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:29:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d20fcbc5dc95c69a9da8c989746956c1a43040f526f2940cae30659253a710`  
		Last Modified: Wed, 16 Aug 2023 05:48:30 GMT  
		Size: 175.0 MB (175010240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0ced2d9d01077003c3c5d55a93f8e41b392902c6e5265edf70caf9c18429b4e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339572095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d922574f706f083376eb631710c25d0a21a3046824f98272107e43e9160407`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:22:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ae3b61eb9574588be7e73e31c31798e2cbf75f53f1f824d855afdf2be6437`  
		Last Modified: Wed, 16 Aug 2023 01:39:15 GMT  
		Size: 202.4 MB (202422266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c15e9b7c03bf0b95f3f1851dcfc9c0d106eb9f4ad6f70b264a297b2d0eb2328a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.4 MB (351357188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1198ab2df7d04bcf039232d26fd5e7f3df61a5052fc44bccdbf90da8b72d3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb23d9f6cfe824c8d50c7242bc34abd22d983eaf2b3d86f43dc174605402d4`  
		Last Modified: Wed, 16 Aug 2023 00:35:48 GMT  
		Size: 209.9 MB (209946980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:40ca01021b43c5582696c732c712900b7b4a8909c7fc5280c1de8fab1b1121b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325734198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfda94015496c32c381731065d8190dc80cd6a287df3a9363de97b109f153914`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:18:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19a5348eb78e6ca17f708ec635d0965eb52e17623be08930925d53c4e7910a`  
		Last Modified: Fri, 28 Jul 2023 01:34:25 GMT  
		Size: 189.6 MB (189628655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de4665916ba11daa50f4c9cfeb03b217dbd50f83c2200780e5e322bccfbcbb95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.9 MB (362863053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd81888fa25d94a8c677ec5865fdc3a4a6d8e90b13af90684f39c936db3ba470`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:43:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8b794b3ece578acf2202199e34306bae8447e86949ab7b4aa0a7ffa9560aad`  
		Last Modified: Wed, 16 Aug 2023 02:11:03 GMT  
		Size: 214.1 MB (214068144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:latest` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9531f7edeedf64601eea231ca0a9df5886574ab064a48b54017d35728ad9229e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318160715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417b6bee7ce6cebab35f9a7b46928127192aba8cae28f38b88e80d126be28a70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:21:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fe9d5e378cd41e1b6d5bb16c3c1956dcdef66615bf00a9d29689cc471f4377`  
		Last Modified: Wed, 16 Aug 2023 04:36:59 GMT  
		Size: 183.1 MB (183096288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar`

```console
$ docker pull buildpack-deps@sha256:594df2f870c56c720a6d79560aaba368ccb7baddb107cf9f703919e1a2057640
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bfffaa002e603f1746d4140734bcb11d31f11d46f49bd15c8c87658dbe2bbd92
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **268.5 MB (268512898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c62f01d447d75d9d7421d061d4f0060124ea4a4a5d099f94065d2d5f256cc11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:33:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7845fca4b254b8c361b6d30d8a0e5b9d6c5a8df43f1482a7c0ed841be440e66`  
		Last Modified: Thu, 03 Aug 2023 03:39:41 GMT  
		Size: 44.4 MB (44385831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c13732bb59235c716d5feeb147388be0507a46221614c1bb12d7b021779e34d7`  
		Last Modified: Thu, 03 Aug 2023 03:40:12 GMT  
		Size: 182.8 MB (182761599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a565c3cb1f8cd41f245613f8957013b3a264838499c1bc2d8c580b5941160847
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **232.4 MB (232389301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db3117034abfe05412e6279df4faaeedb6f2efe734b749483f02f70b23836ab7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:17:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ac461f8a1743501ef6bb272d8425c3b410e894c911165311e282e36b180636`  
		Last Modified: Thu, 03 Aug 2023 01:25:30 GMT  
		Size: 48.7 MB (48671997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ecfeb569a89541933b15e8f732b6d5ea530c3db7a69ec0ec203b7616765941f`  
		Last Modified: Thu, 03 Aug 2023 01:25:58 GMT  
		Size: 145.6 MB (145617554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:413452ef2b8b21174edae216d7d575c62f1a75680d16a91bd602faef3fb6cd18
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **258.1 MB (258111819 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15472ea9645030f627ea62abc62f9b1dc183a64c830d7ddb5f042130d5c7e063`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:39:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:43:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf1c6caaac9b5afe5c21f87c81ea52cb2f170dc8014fc97564f9337986ac802`  
		Last Modified: Thu, 03 Aug 2023 00:51:07 GMT  
		Size: 44.2 MB (44235418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ca7ab853d6afc315714a36136c799da5283745fc8dd554205eacc854b029685`  
		Last Modified: Thu, 03 Aug 2023 00:51:33 GMT  
		Size: 173.5 MB (173511122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e3108463e296ffe459ea82aa555c65cc845d282c08c133cbc3c89b478efebeed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (293045547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f528798424c0d5cbae974a62b5d3633cb2e55806c2fc356882a9bb10757052d3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:38:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e1c2370aa8951d8926c5924bcf24547ca74703904b0527c7f23e46740815f0`  
		Last Modified: Thu, 03 Aug 2023 03:52:13 GMT  
		Size: 49.1 MB (49086146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fa281b8d2db730035bc9fca050c2d962532df63e59ee2bf70160dc162d8fc5e`  
		Last Modified: Thu, 03 Aug 2023 03:53:10 GMT  
		Size: 196.1 MB (196103535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:44b784789004e2fccc14b9636f8fa0730efb5f1930d11d54f7c14c56311fabc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **240.2 MB (240153847 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0adfad68a288281bc1389101040be477a39a459346be0ac42cacc62af7ed7d1f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:15:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57b46166fdc730877dcee11a4a6741fc625ecc917bc6560eedc5c318870915`  
		Last Modified: Thu, 03 Aug 2023 00:22:11 GMT  
		Size: 44.3 MB (44275485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2b0c7ea3a3d1a46630eb9d54eec8f2d9242f0b9406342b50959c7ae76e87ce`  
		Last Modified: Thu, 03 Aug 2023 00:22:38 GMT  
		Size: 155.6 MB (155628668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-curl`

```console
$ docker pull buildpack-deps@sha256:4a237279585f720efc7ea4a10525146e9f74927e5058c3a6811d74269068fa6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7dfd90454f1b7d84eb5851a9dd5fbfdc81c9861254e4e47e539856d99a355b94
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41365468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a157e768e5dfca25628eecd31c1b7da3442b59c388bae96cc37df6bf96bc761`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:ebfe84d045d0585a681615656ce2d21c178ab5958d759d84fcdd6911d5dddb9d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38099750 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53eaa098522872822fc82aa0430c77e40967328656235898a1766bd50e6f068b`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:15e1b21e95f850df357ce2723b32b5ccf5191bcc1ab7476ec7bda4eec7b2dc98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.4 MB (40365279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35d91090cdeb11e3d5f2aa2be50867a5582c1cf78e454986031a529673b37e45`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:98d110730769e1fef236121e4a9ae53b0c37b149dba6c92336743e2112d36bc9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47855866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c74f04b9e892d08bce8686689ac9c25c8376a2d70e6dc91c625f4bdf95734b0`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2d8abebd9d4b6cc7fe03f5e7a5a9ef302dbd29def81c6e0f8041ef083e161e87
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40249694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a81083bbb06be2b6c5b21c6531f4a63810a49fefb639db3d8523c3c75bba5b77`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:lunar-scm`

```console
$ docker pull buildpack-deps@sha256:e518e67ca402ce1fa4e0b46a64eb4708ac383ba71ac5599242ec01c2098295f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:lunar-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8454d70a3954956a848da37b18b384fcfcea44bf593c83edd71f86f02562325f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.8 MB (85751299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71ad6024b68e422663a1c646150045aa8c2978a4fbc5f589970e5a60e2d05dfd`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:16:11 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:16:11 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:16:11 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:16:12 GMT
ADD file:3ff011e7c817c9b010391c2b2f74a111d8c37165e6fdff18e18ccfa67ff7667b in / 
# Mon, 31 Jul 2023 17:16:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:28:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:29:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b631a20f124dbf4ef89945623fa5c94460561f9c7b119e17fd3c1a4bb50ced01`  
		Last Modified: Thu, 03 Aug 2023 03:39:26 GMT  
		Size: 27.6 MB (27620888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3da929c5e27c82b25b247dc649219b7fe3bf48f28e76bed18114af4abd4791a`  
		Last Modified: Thu, 03 Aug 2023 03:39:23 GMT  
		Size: 13.7 MB (13744580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7845fca4b254b8c361b6d30d8a0e5b9d6c5a8df43f1482a7c0ed841be440e66`  
		Last Modified: Thu, 03 Aug 2023 03:39:41 GMT  
		Size: 44.4 MB (44385831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:8a3d85eea75df8415bc37e043642e238772b6d488c2c5b0b5b3efbc781516702
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.8 MB (86771747 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c66f15ddb3b5354fa88a8dd5ce6923e6a77a4a814a8a861e95f73098b9cf7be3`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:20:03 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:20:03 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:20:03 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:20:04 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:20:13 GMT
ADD file:3ec1cc20b36a86b78ff00125a182fab6d7ee8916dbdc6f52d40e182e2892dd06 in / 
# Mon, 31 Jul 2023 17:20:14 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 01:13:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:13:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:76c3febaf312f99233e7db5cc744fa3ec8c5db0830dcbc8c5125cfdd72aecf67`  
		Last Modified: Thu, 03 Aug 2023 01:25:14 GMT  
		Size: 25.4 MB (25435340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0a700903f5f3ce05aabebc3211881ef254b83adf35f632c84c489992fa28ba`  
		Last Modified: Thu, 03 Aug 2023 01:25:11 GMT  
		Size: 12.7 MB (12664410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6ac461f8a1743501ef6bb272d8425c3b410e894c911165311e282e36b180636`  
		Last Modified: Thu, 03 Aug 2023 01:25:30 GMT  
		Size: 48.7 MB (48671997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5da19ddb7546538c21ea08a02600a19310d9b4e70bceb38b8d28b5ab6e5dc414
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84600697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be6d65056494c7aefc18c52c927cc20d4bae8d5849b343a2b3d8b5258fd8c6d1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:24:02 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:24:02 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:24:02 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:24:11 GMT
ADD file:8af4f6767fc5b6665bedd4600c0601ee7d7f803de51e979a40bd3d6ebcd25f95 in / 
# Mon, 31 Jul 2023 17:24:12 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:38:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:39:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dc3ebe95800c7b88cce17a04cb6a4e51211ef73656bd15c0885a6f96b173aeef`  
		Last Modified: Thu, 03 Aug 2023 00:50:53 GMT  
		Size: 27.0 MB (27031709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c53b82c57224a6aeb0716a4227436ebcf006fbd33ca9346c8875243d0ba942`  
		Last Modified: Thu, 03 Aug 2023 00:50:50 GMT  
		Size: 13.3 MB (13333570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdf1c6caaac9b5afe5c21f87c81ea52cb2f170dc8014fc97564f9337986ac802`  
		Last Modified: Thu, 03 Aug 2023 00:51:07 GMT  
		Size: 44.2 MB (44235418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:42ef1049dcb29ba27d1b0c9d13142f7abe39fd6029a57a59714b42f7cc0d633e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.9 MB (96942012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0f62a5802f98787f750e871e9f4c643aed0ae466c85991466676a5ca8a4fd6e`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:18:51 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:18:51 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:18:51 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:18:54 GMT
ADD file:98fe279e3c3239702ac2eef51540228e24a3e15e923342cb3e7cd7dd3684a090 in / 
# Mon, 31 Jul 2023 17:18:54 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:31:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:32:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c8f1d2c62b1aacc6f999b01ed9c6ef10bc5fd3a989af86649162cf5292934393`  
		Last Modified: Thu, 03 Aug 2023 03:51:49 GMT  
		Size: 32.0 MB (32013471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71dd1b07037748833f21cbeb83084ac8ff4a0ca93e61d3e0ac3914daf1beac24`  
		Last Modified: Thu, 03 Aug 2023 03:51:45 GMT  
		Size: 15.8 MB (15842395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e1c2370aa8951d8926c5924bcf24547ca74703904b0527c7f23e46740815f0`  
		Last Modified: Thu, 03 Aug 2023 03:52:13 GMT  
		Size: 49.1 MB (49086146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:lunar-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:bd38c179a2089a2fd31e1411fb8039d0fde3144a93ba16a28ed3fbb8a64e1b36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84525179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51f1cdc23fc8fc1b831ac6c632f34b97cab184a6272ff438b716ebe8e1e0e1f1`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 31 Jul 2023 17:25:09 GMT
ARG RELEASE
# Mon, 31 Jul 2023 17:25:09 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 31 Jul 2023 17:25:09 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 31 Jul 2023 17:25:10 GMT
LABEL org.opencontainers.image.version=23.04
# Mon, 31 Jul 2023 17:25:11 GMT
ADD file:02e6a6123ef99d36f86e3e53231b3ba93c90b4ac9fc0bdebe8f01f2a6c2efb4e in / 
# Mon, 31 Jul 2023 17:25:11 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 00:12:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:13:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ec64faa69090fa13dbf3419726044381d0c7137866daa46daa6a85f785a5389a`  
		Last Modified: Thu, 03 Aug 2023 00:21:59 GMT  
		Size: 26.2 MB (26244138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6910656a90f2717882b9ec910b9f54fd6d237915853a5ffd4b160913158408a2`  
		Last Modified: Thu, 03 Aug 2023 00:21:57 GMT  
		Size: 14.0 MB (14005556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c57b46166fdc730877dcee11a4a6741fc625ecc917bc6560eedc5c318870915`  
		Last Modified: Thu, 03 Aug 2023 00:22:11 GMT  
		Size: 44.3 MB (44275485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:889d740fe04ac8069b368651b191c3dff372e77d75f6ee4c3ba79b72eb1fe50a
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
$ docker pull buildpack-deps@sha256:15a9c82e91f6055ea56f7093ab3352b638354992022653c97d07bddafde2b927
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **467.9 MB (467936388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d443c7c75624e3e4d1d108e4ce75ef982f23faf61c6cb56002986ceb62509cb`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:36:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f019394434fbbf1dc0322c09dce1c54606b0a0995f99872a492c3de4219eb6b9`  
		Last Modified: Thu, 03 Aug 2023 03:41:32 GMT  
		Size: 381.5 MB (381510178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:d2d3d8a109f9aee3a8a84b5db4b7a4ee8968e36ddc3b5444d516ff9a29e82fd7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **421.6 MB (421628972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad28e1633eea717ac4e3c294c3565d98ce72353358c4847cf40b1f7a874824fa`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:46:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780d3e51aaa28824d8d5f1bec7531f98d5db35b9a576d6c08419ade5b0935f37`  
		Last Modified: Wed, 16 Aug 2023 05:54:09 GMT  
		Size: 334.5 MB (334541621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2b275e20b8b5fe54ce2809db704d194f38a8c16840cb8233af7f972b5e721af4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **450.9 MB (450948418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:055f72bc14865f7b7ad19033e21241a2fc102800f09200345be0c66e6359bace`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:37:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940201d34510d57ca35e81b1408d0a6893688d7001f16225853e3ad50c4ec0fa`  
		Last Modified: Wed, 16 Aug 2023 01:43:48 GMT  
		Size: 365.7 MB (365681304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:3f0f104171eb5c17a8352d60506ca6b3fc243aa9f21f00276f864bb351d26963
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **461.8 MB (461771891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b4706d0db06585683cffa47739535f887ddcf98fc2bb6a0361061044183ae11`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76da498d1d6703121456f54c7ec9587100db812456959db12ee2efca2da463b`  
		Last Modified: Wed, 16 Aug 2023 02:18:44 GMT  
		Size: 364.1 MB (364101369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:24d5d1fca2335cafda10036afa67a1e2b2f8015352f51db269db56f4173c0918
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **415.5 MB (415542447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2315269bf260a2bfd983eea1e176a1b3df29ef2b983f6369a8a789c53d3cc0b7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:35:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1f743134a60cbf024185cb1ef08197ade21d0e304f5d3f6915df0822b32e9f`  
		Last Modified: Wed, 16 Aug 2023 04:40:51 GMT  
		Size: 329.7 MB (329684648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-curl`

```console
$ docker pull buildpack-deps@sha256:1a3e487623346261603db0f203a84daf1259e84828605400f1a8d93bbd87281a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cd3ff14aac5bd8abbcebc29597cbe8f4da268fed31446be6c300643c6cc3a132
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41640733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08e7fea7440d087befe1a7723ef76adf9307317fb275ffdd2ab732c581234314`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b6b70fc65a86ef181308b9d4483306a21297953e302338b8b98dd429a421775c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.1 MB (38148463 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:682824261387f5531a8beaef8be345112bc3551257c13812203c72ed136de890`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9e5dc452e6b36370b11f94dbac9bae37e89073a8e9713c787528a7d5cbeb3f5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.6 MB (40636151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:022e8f743594afe234ab66c579a551aff038aca5f366902e789b487cf05867a9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:49e1f7029605cde20671acc2e750197dfa84e8b1749902240630c8d61fd2b0df
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.1 MB (48118121 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449f6529b4a74a21fda38d95eddd728bdb55d7eb1d0711936f509b804ca3dbe9`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:219327f643dbe2a1a1e0cbbd61e31d93a8f2cad220aa3635e0bb34e4622ff1b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41043202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99b11ab01ff2a750bdff354d4b274b8bfb22158a267a03ebda2ed609b5e32241`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:mantic-scm`

```console
$ docker pull buildpack-deps@sha256:54b98186614665cf884a24378777278a3601ca97609bd24fd164b42d662a056f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:mantic-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:917c5ae7b60b328a63cecd4eb385e1f713f23098c90670f2293a967b9633093c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.4 MB (86426210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be5269e6bd4eb9dae1d4063ff31665600eef31956a07caf3e1813f1d2c08a755`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Tue, 01 Aug 2023 05:32:47 GMT
ARG RELEASE
# Tue, 01 Aug 2023 05:32:47 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Tue, 01 Aug 2023 05:32:47 GMT
LABEL org.opencontainers.image.version=23.10
# Tue, 01 Aug 2023 05:32:49 GMT
ADD file:7d5373d4ccc5f70f68afa885a495329e33f2bf9f97a437251cfc79e7b85a1a88 in / 
# Tue, 01 Aug 2023 05:32:49 GMT
CMD ["/bin/bash"]
# Thu, 03 Aug 2023 03:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:316675922a661ce4c35389bdeea6e9ec8d4708e41f08671b586c7aaea469b2c1`  
		Last Modified: Thu, 03 Aug 2023 03:40:24 GMT  
		Size: 27.9 MB (27857084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a7def12313ae9d69537ed1d4ea003f137f16c5789329735bfd447f8c86cfca`  
		Last Modified: Thu, 03 Aug 2023 03:40:22 GMT  
		Size: 13.8 MB (13783649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476103e20eaed817175054747eac1aeb5b843e57c0d9a11994cdf770c7fba77d`  
		Last Modified: Thu, 03 Aug 2023 03:40:39 GMT  
		Size: 44.8 MB (44785477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b032b3221baceedc2a1e8e4454f2955d27c547a28abe95a3668336b99ada9a3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **87.1 MB (87087351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b33abfeb555801fa1a398068626db7d9739c33c31dfd97ed7a8eb5e18c59702`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:43:12 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:43:12 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:43:12 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:43:20 GMT
ADD file:443a623a513d24fb17f92fecba92ab4b48c5cd58f4c71a4d1017f68cb28ed803 in / 
# Mon, 07 Aug 2023 16:43:20 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 05:42:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:43:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a882830b71793138cc20048eb0866464a2a925cea19f5d96e75bef586f07b01`  
		Last Modified: Wed, 16 Aug 2023 05:52:57 GMT  
		Size: 25.5 MB (25451971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69c48a8564dd51e9033d498988912470fd0761ce0f5546103b27b81cf550ee6`  
		Last Modified: Wed, 16 Aug 2023 05:52:54 GMT  
		Size: 12.7 MB (12696492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59849160634729b9bd9592e9a03ab989ba30317f88c213629a7f24a45111cf44`  
		Last Modified: Wed, 16 Aug 2023 05:53:13 GMT  
		Size: 48.9 MB (48938888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2c41c51b6ab982df780eae8161be6d38a64dcfa31eb5e1da76d36ac1df2f6bb2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85267114 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac5e0c1c9ff336e4af720d7c08a9d1426f9825eb87fe1790baa88644d9a773da`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:59:38 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:59:38 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:59:39 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:59:47 GMT
ADD file:a621d5a90b1c5e05eb41dfa44616425f9e9c474acc76e148c36a525e99ff2bac in / 
# Mon, 07 Aug 2023 16:59:48 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 01:33:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:34:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4b4647be7125cb643de6d0a75158905d697da4afc1e9edcd35dbb27a43edf604`  
		Last Modified: Wed, 16 Aug 2023 01:42:51 GMT  
		Size: 27.3 MB (27266349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f74bc0fb029a079dcd558844cc26c5973e7ec9efc2db4555c60ab536a1a11f`  
		Last Modified: Wed, 16 Aug 2023 01:42:49 GMT  
		Size: 13.4 MB (13369802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7156641b60d58d063ba957dec8ada8f9f2a4052eae760ec0c791b84480868de1`  
		Last Modified: Wed, 16 Aug 2023 01:43:05 GMT  
		Size: 44.6 MB (44630963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd0eae220e0953f1e8f6db015f3819e7a0a745b01bb1d8e0c6cc7cc06b878fa7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.7 MB (97670522 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f6f57f844a17257f7bc458e8bd3b32b7ee6f2093e6627869cf392d633985d30`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:57:20 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:57:20 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:57:20 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:57:23 GMT
ADD file:4cb180718bb451f8c264f3c3ca17e21c2f353537e1350e7285186274e7c13aa1 in / 
# Mon, 07 Aug 2023 16:57:23 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 02:01:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 02:02:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fdf3d625c5c62f16c8647b6f71fb3627aa49027d553c24dfb5bb5fe384576e06`  
		Last Modified: Wed, 16 Aug 2023 02:16:46 GMT  
		Size: 32.2 MB (32220285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4266d044f5749871179995f4d16bfab0f930c8a7fc456be89d9dde4ff53c9a04`  
		Last Modified: Wed, 16 Aug 2023 02:16:42 GMT  
		Size: 15.9 MB (15897836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a546e021bdd3317f25b6399220a698c011a5ef8050a924b3d8d5e67bdc99f46a`  
		Last Modified: Wed, 16 Aug 2023 02:17:11 GMT  
		Size: 49.6 MB (49552401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b8945d029070bc2a1c8a5d326be4e11613a9ab1f1a90a15688e4ea12ce0fef12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.9 MB (85857799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3591f1b927603a4a8b5d31122d54e999416e2ff7d66fe57d05e051a2124c6c8`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Mon, 07 Aug 2023 16:41:40 GMT
ARG RELEASE
# Mon, 07 Aug 2023 16:41:40 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Mon, 07 Aug 2023 16:41:40 GMT
LABEL org.opencontainers.image.version=23.10
# Mon, 07 Aug 2023 16:41:42 GMT
ADD file:7038e8b287279d65872808b33572bb449a981ceacdc4533e8e1047544044f524 in / 
# Mon, 07 Aug 2023 16:41:42 GMT
CMD ["/bin/bash"]
# Wed, 16 Aug 2023 04:32:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:32:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e4b480e7bad6fd35ac328034bc72b280c0019028bc95dd0dbf78d168750430e`  
		Last Modified: Wed, 16 Aug 2023 04:39:53 GMT  
		Size: 26.9 MB (26884397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44867c9f8a414f35f7e550468ffda8aadf82a61ad02779247fe2d748d28e5390`  
		Last Modified: Wed, 16 Aug 2023 04:39:51 GMT  
		Size: 14.2 MB (14158805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e837d29076d6daa1f70750605bd3c0d36bced4e25e6e7f34c8bc4360af79e30`  
		Last Modified: Wed, 16 Aug 2023 04:40:06 GMT  
		Size: 44.8 MB (44814597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:04c20d12fd1677dbed7598d833244bb475777d06fa6759ec2fd34aba4bc5a44d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4edf3ca07fd5f768c4550f27782374c299069917c99ca367692ec7b0752124b4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.8 MB (311846087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ceeb7ee443c80095761b84c6e6d14fe95695139a577f5896d82df863c05d739`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947969e624beff93eed664f9f52a08712f3d1e12cadbdf929ff928f93d2c383c`  
		Last Modified: Fri, 28 Jul 2023 03:09:36 GMT  
		Size: 51.9 MB (51872820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87da2254b9de06a71bc1828dec0a28f6a16af7cade75310533cf5cff9ac7e669`  
		Last Modified: Fri, 28 Jul 2023 03:10:06 GMT  
		Size: 191.9 MB (191895767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:83de578f6c86e2358914904d27edcdf37ac4808f7f285f0c4c1fac77083afa24
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **277.6 MB (277648206 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d30fd2556a67937a5b7268b965735eacd708f8dc3d4e4ff1c08b76e81af2c4`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:33:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed6203f3da20d3e0f8ea7d7ec6e4fdd2cafd582b494e1e9fda0ddf4f9a1a2f5`  
		Last Modified: Wed, 16 Aug 2023 05:50:05 GMT  
		Size: 47.4 MB (47370312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36d2cb1f3e23c88fb017f1bb7af1d240169a419bc5190369b10152b8b8255ef`  
		Last Modified: Wed, 16 Aug 2023 05:50:34 GMT  
		Size: 168.1 MB (168099748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3e3957f362fd2e9f06d91adade8d2e044072cff03f6169e24f768f861a69e1e1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.4 MB (302423969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a874813819499ae0978b7c10310b76414d80e88fbb4de176610431986df9aeb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:25:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e89467a67e13dedd46298880cc34cb6a78d65e3f4c66175ee80f87892403a46`  
		Last Modified: Wed, 16 Aug 2023 01:40:52 GMT  
		Size: 183.5 MB (183463629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a2c1884c14fa4ef92ad6f8b2cc931880f6d1a02f21e866d6c636416741e74901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.3 MB (321279222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8df92c12e389a10a361e57c1ab32475ffb3eaf24c8aee4fea97676f158255cb0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:30:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:31:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377913e8bda7ade79ce7bc10aab7401851a4cb9565903c8bca5b0360b4fab3bd`  
		Last Modified: Wed, 16 Aug 2023 00:37:36 GMT  
		Size: 53.5 MB (53486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:772141f0f201b519ab5689ccf41e7601936a21705c554b9ee73448eb217def09`  
		Last Modified: Wed, 16 Aug 2023 00:38:19 GMT  
		Size: 198.4 MB (198441615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-curl`

```console
$ docker pull buildpack-deps@sha256:789ff8d52fc9bfa8c2d627b94509ab1dea950d9b9045d1bffd0366231cbd19dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:052ecd162488e2bd9bca20f30afddbb0364e89bdd3263929ce8565850abadcd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68077500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:253b3ab6acbb874be58d7fb897ab0e2421ec59ddae5eb5f5fd766b59c4317abc`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:1f82d9d6d25056fe6fc40e32cccd2fb79b2b19a55a3b30d694740a37e1204751
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62178146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbc04b2bd46b3344ee4a82315b3fb423ee077d0af9ac5592445f96d517929eb2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:693fba8369c38b01ea7646361a202296d268f8452d59f1622d04534bf8363085
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66741963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da913c23eb14e30f7e30aaada367ad899839db75c2d632e31b6c1d7ce8752659`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a2f6bc9bc0541882d918d0b6b577d0fc0176c4f25f15e3c1991d4650171fb292
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.4 MB (69351416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52e1f222da00d74c27c7fc35eef2dacdd3f2a6c346602e90d5b74493308eb88e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldoldstable-scm`

```console
$ docker pull buildpack-deps@sha256:f8075fededa2e3d394adcf18195e24ebe2ec2e07b90cae9934d16f79c6bf783f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:ca3829a7e5276647ed7914a9f714c961f10aec2e35fd937df553b2c3bc4f1ae4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.0 MB (119950320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b38333a879cff0f96573c5ccb535b08b9462278d629bc91ad0539b1dc34d924`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:25:17 GMT
ADD file:46b31c893ada083f38702e21d80e5ea4b674cbc78bddd3d80020d7b8e8beb467 in / 
# Thu, 27 Jul 2023 23:25:18 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:03:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:04:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9918064ebccea7fc961fe71dad46105b217763b4b1b3a9dfa7bee2ab29d2039b`  
		Last Modified: Thu, 27 Jul 2023 23:30:27 GMT  
		Size: 50.5 MB (50497996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2345e1e5f82d8963240db3c8e8ccfd431d0962d14219e24bbcc756ef217bba48`  
		Last Modified: Fri, 28 Jul 2023 03:09:21 GMT  
		Size: 17.6 MB (17579504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:947969e624beff93eed664f9f52a08712f3d1e12cadbdf929ff928f93d2c383c`  
		Last Modified: Fri, 28 Jul 2023 03:09:36 GMT  
		Size: 51.9 MB (51872820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:91958af6ba88267b2c1a8939a18048fdc1d3925fc906b6084585fae2d6595a0f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.5 MB (109548458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01ebbf20cc2fb0cc3bd845c46749f5519bd8993fca7af3933636ce84c0e57f3d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:42 GMT
ADD file:9ad3ed36bade2e2cd71bd8f66dc47946e90d205f1846692ae9c240560758b4f4 in / 
# Wed, 16 Aug 2023 00:17:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:31:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:32:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ed63aeb0ff951576d398ae0e8de7a2dc582157c60523055321f47ef26ce88e00`  
		Last Modified: Wed, 16 Aug 2023 00:22:28 GMT  
		Size: 46.0 MB (45966229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee91fed073f248f84b680e14ae33a93203a05d62cf51fef886cd7ce0b3ac7d45`  
		Last Modified: Wed, 16 Aug 2023 05:49:50 GMT  
		Size: 16.2 MB (16211917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed6203f3da20d3e0f8ea7d7ec6e4fdd2cafd582b494e1e9fda0ddf4f9a1a2f5`  
		Last Modified: Wed, 16 Aug 2023 05:50:05 GMT  
		Size: 47.4 MB (47370312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:89051961c8ea98935f890b00aaba8c4e399234099c594595e60e083656063cad
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.0 MB (118960340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:927f459518de5d7f199fb58be93dc1c5466f6d45cc64f9338916dc1d4101282b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:18 GMT
ADD file:366546a703fa234d38591d2a54f10fbced83cc0e407775ad31751f0111c348c8 in / 
# Tue, 15 Aug 2023 23:40:18 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:24:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:745797452665e0b4d6f5d0f9b05ae67a86bccfea4ec3a2cf7c6dd89cbfafdd37`  
		Last Modified: Tue, 15 Aug 2023 23:44:16 GMT  
		Size: 49.3 MB (49290964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0d4e21e88dbd3e72136906f1d37cb7c9b29c4a4c107fbe1c8b0385f5e663d2e`  
		Last Modified: Wed, 16 Aug 2023 01:40:15 GMT  
		Size: 17.5 MB (17450999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed6dff3c26e414861add902b18ad78500d9300d96e33af1ad4d3795dc9cf10cd`  
		Last Modified: Wed, 16 Aug 2023 01:40:28 GMT  
		Size: 52.2 MB (52218377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d45c3ac03e143eb6954fa296ffdda449cfb86c2e40cb29fbfbc0e6dfc092ea74
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122837607 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2744c8f7c22a22faf342c3a48670f2e072667ac3fe46dc100663e370effa0632`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:33 GMT
ADD file:f985eed393788dbeb3e4d9ab7f77d632d72f60bc5da30c59bb7de8fa3de0681c in / 
# Tue, 15 Aug 2023 23:39:33 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:30:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ce293edb9c35c6521b0a7d87a0d8e0252e4b0cab665a3103cb6d06e3e37cf414`  
		Last Modified: Tue, 15 Aug 2023 23:44:33 GMT  
		Size: 51.3 MB (51255460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d7c3776eae51e29722c4381d59391e00b49339c7298dcbef6adffe94829182`  
		Last Modified: Wed, 16 Aug 2023 00:37:17 GMT  
		Size: 18.1 MB (18095956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:377913e8bda7ade79ce7bc10aab7401851a4cb9565903c8bca5b0360b4fab3bd`  
		Last Modified: Wed, 16 Aug 2023 00:37:36 GMT  
		Size: 53.5 MB (53486191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:99d4fb447aa56853cca28eb6bec6af95a288e88df59f3794b318b436146180c4
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

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:438b66cc977016632275ae9457ac3561e691ff7b8035f49159fd485752ae15b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.3 MB (322252653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af4a6a6182dd5c7c765fa6e5894539d38a174d2c864885c42e3b8d404b289cbe`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:03:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d4a6da525a13b128e2e4f41081a5af59d2dda8045d40b207510cc3fdc84e1a`  
		Last Modified: Fri, 28 Jul 2023 03:09:11 GMT  
		Size: 196.9 MB (196851463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:17b532724b100b5f9a6c3652c32ce7b09ca9b35c6dba7117ccfe49ee8a3a2d36
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.3 MB (295307479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d66b8bb5760967b26a5f94dc6855fdce82dd85c5dbca25ec9a9c77c0c415760`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:44:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def812da7393c114766d8e90ea33083736120f2e8410c43c6e3293f0c5c898`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 52.3 MB (52340723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997fb3aae8d3febae5665017c86770b153edfad7973f9c0f8799ae76c9cc4e9a`  
		Last Modified: Wed, 16 Aug 2023 00:48:57 GMT  
		Size: 175.0 MB (175039510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b32b7a67c168925bf754a4aeca1479ed2b016a46dbfa4ef0d2b3d8a9841db7bd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.8 MB (282777012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:989e9e60b333c3548ba4b4dbef2a01770f2ccbb2232407f7aaec08cfaf9e137c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:31:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49800a0424211a8cc1edf5a26d1ebd1afb7c017be3b08cadf2d25abb85d291b`  
		Last Modified: Wed, 16 Aug 2023 05:49:04 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea65231b804ff3a87553e9e8aacba0dd7e706dcceac6cf36be583fbfde69d20`  
		Last Modified: Wed, 16 Aug 2023 05:49:40 GMT  
		Size: 167.3 MB (167333015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:844d16c47e1e2d17df96182fdcd4e61c0684972a54e6baa187b060c4743c2d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313905267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7924790b30f678ced1b1d25feea21aef26d5040f572f27e2c7ce82cce085203`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:24:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8864a846a08e10fbf877e73678d1f0803227b00a1b16d9ba948070c6e58f6`  
		Last Modified: Wed, 16 Aug 2023 01:39:40 GMT  
		Size: 54.7 MB (54676094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db5ec7e6673db06ba035c7c57c4c31b84c89e803ceeb3268a02b5175537b120`  
		Last Modified: Wed, 16 Aug 2023 01:40:04 GMT  
		Size: 189.8 MB (189777874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:34bae5aad734c62848b43b3a22c7e70bb3a643d4507d0d3902f91fd137fea33b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **328.0 MB (327995494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33b9ebde7f5d1003596c0622deccc60fd46bfbf4bfa4898c75b6e80e38d0ab95`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:29:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fc8bca4c44908804dd201eac5ad8d9316cffd0de391511a9da2fcb3fb48c0`  
		Last Modified: Wed, 16 Aug 2023 00:36:22 GMT  
		Size: 55.9 MB (55922930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da0010c52f973a4d9c39043ad90ee5727579d72d1a34209b0ccc3f1f80515cc`  
		Last Modified: Wed, 16 Aug 2023 00:37:05 GMT  
		Size: 199.8 MB (199768301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:04fffa70f42079b89867ef930ba47542323fedfcc781dcdbb77fac36513759ff
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.1 MB (301071152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f23b0a6fb6d6dc293c2bd5c92deeede8c91b218b1bbfcf8a7da8f3d0e9caff00`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:26:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedbdbe02029d723bc1414bf8094fe7b1ac71ed4460a31db174ac0e221fc1b3`  
		Last Modified: Fri, 28 Jul 2023 01:35:29 GMT  
		Size: 53.3 MB (53306734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcffa2b1acd2a62702740ee307e4ae143652253f14c589200b83dad48f46522f`  
		Last Modified: Fri, 28 Jul 2023 01:37:23 GMT  
		Size: 179.0 MB (178972969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:b7f2ef729b20579385bf44c5a8f7b2beba8359bf644d5e3b535cd4d9d62362a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.7 MB (330746353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1d9f13617425b5540cae22c07daa37cafee81180bb3a201469d40dc1dd209f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:48:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264ca3322295f7e8f8f191650911a824de696e167ce08aee16d14b5704ea4d14`  
		Last Modified: Wed, 16 Aug 2023 02:11:48 GMT  
		Size: 58.9 MB (58865273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c8e5a575991fb77e9e7207e17459595a4a3bd1add713086e44f7190d05ac9b`  
		Last Modified: Wed, 16 Aug 2023 02:12:43 GMT  
		Size: 196.2 MB (196199625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:4f9f17ee70cbe00fb5bc22aa1469cb6e15c02775c082b68cce78f7dd8900edc7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.8 MB (295840012 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:869ab6c8fadc208d4b1436e4cad1f785de717eaf91a2060cf067d3bfc1a7d0f3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:24:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c13aebe3a1d06fd7930da9581f9ac789e148f33dd9a84008de9e5da614208`  
		Last Modified: Wed, 16 Aug 2023 04:37:22 GMT  
		Size: 54.1 MB (54061692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83fba4183bca79f260d587a76c94532cc7c3a0419169722dbbee232fee2d9dc`  
		Last Modified: Wed, 16 Aug 2023 04:37:47 GMT  
		Size: 172.9 MB (172855751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-curl`

```console
$ docker pull buildpack-deps@sha256:a895b5fc7d66746a583d5b3a8de5a62aa17f837ba00e4bce340eea6a91c59c5f
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

### `buildpack-deps:oldstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:765f83b96d5a3171dd95060b09769740f829e02da450d4de25c1e0799d84a14b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.8 MB (70816156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:24c8a817556d148562359d5c71ce5a3b56490421d4acab107995d9c2302a9755`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:93b3abe77348f08b71522c036a5ca22a336ba6722e0b9d5a416bd6393423641d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67927246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed1f7299b6c9682ee4de2673118efdd4d37b05bd5070ab6caecf06095465b9c8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3e8e5c8b704a1e7108b413f5c3ac9d287848becc6da7f020e9eac097a482fb3c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.1 MB (65088329 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd3401d58e46bbb699218d5ce23026e614fa7fd0f8d6a80b7410750a19990b22`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:87db69382d408253d6331ba2f3acc990db07b546cb54209153e5b311582cc128
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.5 MB (69451299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e48a220cd587f717272d10bb47fc8eec3fb65e0e425865dd2bd0d8a3a790e546`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c0ac3a855c0acba7d79a0a3e5f08e5df6bb608e5640c893cbdd94c06fea6e366
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72304263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab191c09fc96b7ed761406c1f6bb7fce32db191c3c30eb65900539dbcc1cc43d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9039063fe1bc35f199e092c3cc23d24ce8e031fb1f825b2b259d0c05d05203fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.8 MB (68791449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c1ae7b77ee8867744f83a9dd4c8e0546a5248a7ba1c805c6e0a155413d02003`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:12cff15e25bd30781a2e1c2d09d3e682d87156aada09021b1532f373926bbe22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75681455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:526a075d6b3c700a1d8d75f6f869ae0719e7bc6c56bf35097da945ae6048fa35`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:acb9713373d6f573d0115ffdb72db6a5055a3f6f2eb042caa7f3565af683efa8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68922569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f39ba35c8d28886bd170e7d2d7d9b2bd37108153ae50e5027226419680ba5af8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:oldstable-scm`

```console
$ docker pull buildpack-deps@sha256:fe0040db0382ac581a1ab193009277a7d4fe87c2efef19e481c22b1eeadbba1b
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

### `buildpack-deps:oldstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:4bae423df8eeba414176292d04ba3cd36c7cdbf9fb57aee7eba666c16d5647d5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **125.4 MB (125401190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ed57311c87c592557b79298b2f29ddeb0d29042e26414aaa59856ada65d01be`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:55 GMT
ADD file:b493776b6d91132ce50735e2d82076620774a1e0a690cf96777ddd6b85f513ef in / 
# Thu, 27 Jul 2023 23:24:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:02:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a9e034800a1747ea288f38f6087c036acac99dd3ec5255bf7798abd8c23a304`  
		Last Modified: Thu, 27 Jul 2023 23:29:45 GMT  
		Size: 55.1 MB (55055571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91c1fad56dc2c387d016dbcaaecfbfb5e2b479f8dd644803dead02566f3479`  
		Last Modified: Fri, 28 Jul 2023 03:08:24 GMT  
		Size: 15.8 MB (15760585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dd6a2c0cfa3eb4e8012b3f2df526acc8711a4a9515e0e968419a8ab1e9899e4`  
		Last Modified: Fri, 28 Jul 2023 03:08:40 GMT  
		Size: 54.6 MB (54585034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:fa65fe73934264c4d9ee23ce0366e222f470a002b1cc7a87e8ad9fbc7563d089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.3 MB (120267969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:836038d13fceb192024c5d9a931b66f73f27172d154be24045d79f291ba5f867`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:40 GMT
ADD file:d044e64aab907424be649252b5ff1d9f5e8c9494db5b60c0e54f5962bfb73478 in / 
# Tue, 15 Aug 2023 23:48:40 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:42:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:42:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0b63bbf2e6f6026dfaed9cbedf777472a04812b7d291501b1d416e49e3ce885e`  
		Last Modified: Tue, 15 Aug 2023 23:51:54 GMT  
		Size: 52.6 MB (52558130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf207734195f34506f2f636cb92d7f51b200a26c1264dcbb6ba6e8de4ad0a3f1`  
		Last Modified: Wed, 16 Aug 2023 00:48:08 GMT  
		Size: 15.4 MB (15369116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24def812da7393c114766d8e90ea33083736120f2e8410c43c6e3293f0c5c898`  
		Last Modified: Wed, 16 Aug 2023 00:48:25 GMT  
		Size: 52.3 MB (52340723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e7a1e27e1c8e9cdc898d21947c3eb25521d92ff8d456ea6c7b5c52d4d89197fd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.4 MB (115443997 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75f92c6fc9e6de615b43e074d770c35f37177e9a23f8ed52a3ce72b881c0c68d`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:17:21 GMT
ADD file:b529de8b48c1e507ad6f29320c3c5cd83d8d06fa66e8d89bb62faff62700e9f2 in / 
# Wed, 16 Aug 2023 00:17:22 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:30:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:30:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c53151c23650f086e15d3652b8a931fb4623765c0112e8adc74eb8853c8c9232`  
		Last Modified: Wed, 16 Aug 2023 00:21:46 GMT  
		Size: 50.2 MB (50219496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abbe9a81a850f9760477ffa3083b63d636090316a05f81146ffd62a60638926a`  
		Last Modified: Wed, 16 Aug 2023 05:48:44 GMT  
		Size: 14.9 MB (14868833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49800a0424211a8cc1edf5a26d1ebd1afb7c017be3b08cadf2d25abb85d291b`  
		Last Modified: Wed, 16 Aug 2023 05:49:04 GMT  
		Size: 50.4 MB (50355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9222281f3a18fc1f68ea3ac87cae13cecd6102b3e6d3d2a963e198b9b149f4f1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **124.1 MB (124127393 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:900914194df7ad3b6dd6d9b5ce4b277ac3924cb43f60a296c43e23ec0f78cfcb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:03 GMT
ADD file:8973cddb2d84a543b71001635599951bea6485a3526ae4ff916443b584864c83 in / 
# Tue, 15 Aug 2023 23:40:04 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:23:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e837d9f05c625de5b814b851adbc03559ba02ea7078f57c81a01e18fc65bf42b`  
		Last Modified: Tue, 15 Aug 2023 23:43:37 GMT  
		Size: 53.7 MB (53704779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abd0588cbb35597a784666f0dc97746829b8b4b730b73e8781fb90678ffef22`  
		Last Modified: Wed, 16 Aug 2023 01:39:26 GMT  
		Size: 15.7 MB (15746520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85a8864a846a08e10fbf877e73678d1f0803227b00a1b16d9ba948070c6e58f6`  
		Last Modified: Wed, 16 Aug 2023 01:39:40 GMT  
		Size: 54.7 MB (54676094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a417452b134c7560ef87b1b81bfaf3bc47f4fa7f86fd4806520a456918a66f78
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **128.2 MB (128227193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78f2d6166d0c7afd732a0578cfaaa2cc6809a65a41a045e333d8e52930b7bc04`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:11 GMT
ADD file:efc88a19b31e68ca41f555bcc51338b0f135cbbd72b90637d8c73969d53addd2 in / 
# Tue, 15 Aug 2023 23:39:12 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:27:49 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:28:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:822e033fa7b169545d5890de01438a9dd87774ff938ff440e823a3ec3f73996d`  
		Last Modified: Tue, 15 Aug 2023 23:43:47 GMT  
		Size: 56.0 MB (56040520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52269d7973f191a6cedbd1545cfe71ec1c659072be43d51f8741b18f05423e2b`  
		Last Modified: Wed, 16 Aug 2023 00:36:01 GMT  
		Size: 16.3 MB (16263743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16fc8bca4c44908804dd201eac5ad8d9316cffd0de391511a9da2fcb3fb48c0`  
		Last Modified: Wed, 16 Aug 2023 00:36:22 GMT  
		Size: 55.9 MB (55922930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:de2ebe9c144a695a12a0f0c57c3cd8b792a84f597dba4c6c18005d4f0bd5da55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122098183 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0552ed08f1ab1ca70de1a1f7134a552c58c6f55460faa2343f594e349ca09573`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:11:57 GMT
ADD file:ccccca3acf3759fd714159d3c3beff86d84a9751b947e148348d523272fc1bb9 in / 
# Thu, 27 Jul 2023 23:12:02 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:19:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:21:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9d9a0c35af83dc10b6307f02a48749b4d8024123530a89d5173f70981e00b9e3`  
		Last Modified: Thu, 27 Jul 2023 23:23:10 GMT  
		Size: 53.3 MB (53270927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12aa6a7cf9a2dd39c4a36e47b26cc0ca1c9e8ad55d149bdf74bcbc866c92718`  
		Last Modified: Fri, 28 Jul 2023 01:34:45 GMT  
		Size: 15.5 MB (15520522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cedbdbe02029d723bc1414bf8094fe7b1ac71ed4460a31db174ac0e221fc1b3`  
		Last Modified: Fri, 28 Jul 2023 01:35:29 GMT  
		Size: 53.3 MB (53306734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:842a4c3acbebc913c51002c40c17c0b323fcb71c84a289556516203f2acb0512
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.5 MB (134546728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25c8963e9ac71f3a1646ae9e35de4bd37f9dd002e1abf815edc5224f4b43081a`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:50 GMT
ADD file:23fe4ecb2d3d302e0df50109aee416120a138fad47d1614500f98b65fa288281 in / 
# Wed, 16 Aug 2023 01:09:54 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:43:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:44:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:148c97e5e41c60dd4fc440664aeee1e57ab7158b53ea7d1f9132198b3d35bc5e`  
		Last Modified: Wed, 16 Aug 2023 01:16:30 GMT  
		Size: 58.9 MB (58928436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901a6153e1feb9026260a32acce3bc3acf29f7186a1458d2b343ee865d054c45`  
		Last Modified: Wed, 16 Aug 2023 02:11:21 GMT  
		Size: 16.8 MB (16753019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264ca3322295f7e8f8f191650911a824de696e167ce08aee16d14b5704ea4d14`  
		Last Modified: Wed, 16 Aug 2023 02:11:48 GMT  
		Size: 58.9 MB (58865273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c8e4fc3b1a6bfc55b26bab453040a0274970583846bf439f6b13dd696c301aa9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.0 MB (122984261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:407d4b94d5f7066269549cad4832b06621feaf2d81e4b606cd7c9befe2d74b0e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:43 GMT
ADD file:021ebd89eb6b326058b4fc3aeca5d0d93925ed29a443618fedef034618e8f2db in / 
# Tue, 15 Aug 2023 23:42:48 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:22:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:22:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cf9beb6f1941863d1df3b7a9c4f925894662762a3ceeba920f164d9e8c8bab57`  
		Last Modified: Tue, 15 Aug 2023 23:48:07 GMT  
		Size: 53.3 MB (53290642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:431e34cc72373b43e9a06943d5dbedf8eb4769be085ac405ff5a810430093689`  
		Last Modified: Wed, 16 Aug 2023 04:37:08 GMT  
		Size: 15.6 MB (15631927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c13aebe3a1d06fd7930da9581f9ac789e148f33dd9a84008de9e5da614208`  
		Last Modified: Wed, 16 Aug 2023 04:37:22 GMT  
		Size: 54.1 MB (54061692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:scm`

```console
$ docker pull buildpack-deps@sha256:b514f7a71ef85fb2535d7df3fa54310136f7cc6c52aa55040f822eb5803285b9
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

### `buildpack-deps:scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:529e163a2641648602b7c30f6628836a07309db7eec36b54bc1f3079fe1a0075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137700186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612d62ca1b84af9b3c9ea7d4f8f7451dea5d5280997f2995f5a5476d50e65656`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca109ee1bf05c7a25cab135c9f5f90087363f22e7e296b1345aebcafc2d4c87e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0f43441c554eb412fc1a6cae438793a4ced333e8a6a89228b9ff87bab33e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a1fa0530e19b09fbd7c6185d73d84a4bc942d0411671313e2938ef77ad01ab4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126431714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694ce6041bf7543b9d45b61b59f896cf7826c571374effb2a7e96d4db51004dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3420b56cdf17798958f80fd610bf3004621a3f02bfd92180f1cb4996eb07ea4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137149829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177d9930ddbbf17d991d76e9b71338fede111763111e1bbfe07c60588804ea5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a4d7df737a84cc83cbd61c2dc4edc98541d9bc7ace5cd833a1a14b8a5d027df5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141410208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147bc03aafb5bcbab9affe5fdb15a1a58291461d8982f37588936198fcee1337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9e6b325e9f83cee376fbde36a72981f811fae25c545e31c8915da5654dff04b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136105543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b95c96798319d28a7d61e576aca883a6bd72c3ba77b41f8b73169a8976c95c09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:09c65b2c916c3d1627cb0f348b84676386b69d2923931105735d0d62c5ee5f16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148794909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d2cb79031f827ec74172b6e7d6f32308c68e0b31222d978e62aaf41a7e4ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:48f4ce295c01fb2e62b6b64c1bd63eab67ca9e80601edef71244eb6a7f6a77b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135064427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fbcebb591453ddcf6b4344fadc51626a83a65bb4d445d480182536306e76ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:0571dc0ae118e64a0334c074e5e490775c01995a5fa1d7f430644f83a7e099db
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

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:bc0bb95e08ed205a17de1379a423d4d44e52a9488c7fe9cab2bbfcb7ad141298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.3 MB (557269293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc38cd003d8e650a25ad517e8d5712030439ce1980704ff4cf2e0d69b818b39`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:24:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c5a779e1a53b62babe3fb9204c1be41796097067190b79b67822f58d7293d`  
		Last Modified: Thu, 03 Aug 2023 03:38:15 GMT  
		Size: 418.8 MB (418845194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3cba1948c3b97628ad52a9c62d2e817ca47973f768eedf96322185146a3a2b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337513714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c295b52d7de4d81008aff9a1611f40ecfdb08a270deb5f23a02cfae746f6041e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:46:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ea5e28c6c87005a46ad476c9b4f15160056117290320261d90a2241b5237f2`  
		Last Modified: Wed, 16 Aug 2023 00:49:27 GMT  
		Size: 62.3 MB (62299617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647be011a70a1d8cb1dfb1d0afb023010a89f62a9a6e0d82f2b93815bf4d610`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 204.9 MB (204867568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a6a6e2933f4fe4cdb7aacd5fb8b1b5abde5f97bd9e5257fbee772c03c9e7d281
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320151464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a9929ca4554ad801cc1e8e609d3a64463241c751f234e8627b4c74066d6cdc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:34:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:36:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916b1beb64303951348c4609b860a99cd5d81954299ea9ae649cc3d0d51fda`  
		Last Modified: Wed, 16 Aug 2023 05:51:01 GMT  
		Size: 59.9 MB (59937940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5492b3f9added58b496e3ea6da2043a8fbefb6532b2420c18476c76a9db53ce`  
		Last Modified: Wed, 16 Aug 2023 05:51:40 GMT  
		Size: 192.9 MB (192853583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a12c54dc2ff3d11715e904b8db919e2517afdfae35a7e7b59008efb5c52c84ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.2 MB (358217052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e78407adc2610c61a745e8426d80dc5bb139a2472320b762038bf188d2c45f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:27:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5bcfe9fb2496b09fb02f12a4c5eab9ce200446746f7c777fc1a0025d3a400`  
		Last Modified: Wed, 16 Aug 2023 01:41:19 GMT  
		Size: 64.6 MB (64637449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e8a69e947e5f68e66c6a9a127741df87951c498a5ad8d446ff015d7f56373`  
		Last Modified: Wed, 16 Aug 2023 01:41:48 GMT  
		Size: 220.2 MB (220237253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a051074a4cc184320a02289fd343291bbb98f143e22f02c9132594a3a867ba7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.7 MB (370741062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9f8698e8fdd7e8ed02cfd14ba7c974886d7633a36030dd548d9388d1de892`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:34:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84633700d0e0c5a1fd8bad79e5e4601602218914f21595af58697a382ad3c928`  
		Last Modified: Wed, 16 Aug 2023 00:38:54 GMT  
		Size: 66.5 MB (66513490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b41b59cf71c0596e7c00b5aaeebc3212e55085655c713c093e7efd3411e724d`  
		Last Modified: Wed, 16 Aug 2023 00:39:42 GMT  
		Size: 228.5 MB (228480503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2b0f9147d252c8ba32e8cdd3b352887252f4906f8158d3539bdda46a5c120067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.6 MB (641552716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05efffdd05a2a9414dbddc4b50581de33a6bd45816b1262cf64b4f983a5e54a9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:18:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9085ce02bdf495dae6f1b38c84f07f4cd662a4ca17153a9b1478678a4196dd`  
		Last Modified: Tue, 08 Aug 2023 21:24:03 GMT  
		Size: 504.8 MB (504772567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45b3c7ed26f2a264761ba4df36f122e891d0db394334bd080629cd91ee1023a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377654498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a4096243039871d1ba7854c5d70b1a6bbe52f1a581ec8ba200d55cfdda31c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:53:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b549a05446434e911aa7f23d6d7d3bbd3e215ad66876361d6e02362eab38a`  
		Last Modified: Wed, 16 Aug 2023 02:13:30 GMT  
		Size: 70.1 MB (70136139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8210cc7ae63d1a84c252e719574868919ae783dc9fd2dc72f4084f58d6d8b`  
		Last Modified: Wed, 16 Aug 2023 02:14:34 GMT  
		Size: 228.0 MB (228022931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0150bb87b97db7106a8883b1971dae5b87fbd5391ec9118cf15f6932d83b0f8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.9 MB (584935368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77126be424a00a29f764cd8e7f8da503eebb4c14608d89dd3edd5a2278ccba0d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d3e46d641c1277be46ab521cccf04aeac468f053836ff4e0626b3a862cb7d`  
		Last Modified: Thu, 27 Jul 2023 23:57:35 GMT  
		Size: 455.5 MB (455541137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a93b138fd3b934f4dc0a7982cd9b735f56f95dd1af09935e0654afd57b453cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339461658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2c2ff61aa1f806db15fe7f1e44d2044c4c9bcfc6dbef062b36ea2f7eb4fdaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:26:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45414c0dac5eed7c0002a6ec3f910c9ab1430c15501a8f4ac7399a32a19be528`  
		Last Modified: Wed, 16 Aug 2023 04:38:12 GMT  
		Size: 63.9 MB (63911557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16663081eb6f5dd01559432e43375fcc1d345dd3c74367ce1554e5dcce76c379`  
		Last Modified: Wed, 16 Aug 2023 04:38:45 GMT  
		Size: 202.5 MB (202499932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-curl`

```console
$ docker pull buildpack-deps@sha256:021706d0d55d40a96982ded0e76f1b459dc2b5c4ae0fb28e6076d9232929e2e7
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

### `buildpack-deps:sid-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d2668493b4f046b71c6260d3279c31c6ba4f2a286b05c50c2f5b4e868e1cf3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73749616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6413f0d2d0378de2d6a8d9d1402a6084483971c14f3fd113e9eb890502af0b02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:774563c7ab34b698df26f2291a44ab24b899f0da48b5794c4a9e51b889427e90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70346529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be2e6d9a14df3fc131f09bce7ad48cdbaba68d086d00efc976e7c7d409a7f17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7aa62e1d9c56fdf41c87e3887595f8c62f23d55bc0264ed2eed3cb92781c30a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67359941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbae1d38f1729ba21724854f9beb2bc47acb5dda4f340347d633af0d94e57f0b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f357b484f94d65bee85830215f8a99bd873b9b6c588d9b18d73a660d1b7d230b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73342350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad8010747ba13453458120a56606c915f892703fb198850dde407010ab2ae49`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d97b42d29a664dcae93cfd874db1be9d3c194cb92623f2447128c5bb0a572761
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75747069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ac27c3bf31307e25bfee6c4ee200ddeab2b6f606757de278d52f1d0566c9aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6d22f564936ef6047f439f288c6487d49ea9ea94a3d3d823ba789aae0b57477f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a82efa8a0cbd2145763c100f743ab0c6073cedbe7ab03288024f57dd678d67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd603885105b996b2f2ac71bdbc6418f425ef338b8ccd9a0f89d91b542e774a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79495428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a1a539a3d7557346dd1bc8a2d6ee409a1be725c2e2443794e3c9a9de8a62ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5df31820934ef52dc9dc24dd1fcdb4b91a3fe8bf2ad43a7f4804416b0d88d208
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73050169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e8ca8ec8e68c1439425282cb5c2b9588e08b3dfb887b123af12009d46531388`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:sid-scm`

```console
$ docker pull buildpack-deps@sha256:3580956c9b85d435795cdcf2244a4e7d190309302f99161995532414d892be08
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

### `buildpack-deps:sid-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8a363c27455cd9f6fcde5596efa71102fa5c2cebfbf12fb0c5157e2fd3ab60b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138424099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cd89db58a3ce0a728b12a56803552a04aa7aacfc0b27734d53addf8a3d8ac2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:995b60c9e41b030f0344790a1dff3b20c9cae8ee4c703b977c9b0d9430ab4061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132646146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a6c98e02bcec94970ee808e61c9a8590a882a8226f1b368af55d851188919a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ea5e28c6c87005a46ad476c9b4f15160056117290320261d90a2241b5237f2`  
		Last Modified: Wed, 16 Aug 2023 00:49:27 GMT  
		Size: 62.3 MB (62299617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:71e545c4c300ac58377187dbd4799d9b01e698fcb27446348a1c64491d93b188
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127297881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cddd27e18a2b66911c51d5c160ed1e3ce962332301bbd360d705d4c34c88a93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:34:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916b1beb64303951348c4609b860a99cd5d81954299ea9ae649cc3d0d51fda`  
		Last Modified: Wed, 16 Aug 2023 05:51:01 GMT  
		Size: 59.9 MB (59937940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2be3ea85b4c5c86e9424499855e28f42a6e36f936bc56f533cb789ae866bc12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137979799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e5d9a52e4fa2879e47cae94ed7921d770e284c2b20f66a2e9e08faa8857704`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5bcfe9fb2496b09fb02f12a4c5eab9ce200446746f7c777fc1a0025d3a400`  
		Last Modified: Wed, 16 Aug 2023 01:41:19 GMT  
		Size: 64.6 MB (64637449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4e2ce5378c4db0184f2a5113732e97908ed485193eb9df0b315b2257f4f2d8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142260559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518bb0c85280b757bff997cb92e6a086ab364b971d4d25fa86e8f1e53e0ec81e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84633700d0e0c5a1fd8bad79e5e4601602218914f21595af58697a382ad3c928`  
		Last Modified: Wed, 16 Aug 2023 00:38:54 GMT  
		Size: 66.5 MB (66513490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:13c2f443dbe0048ee66a2dc9ba3c4726b576afd4987d853bbe4be5fd6c3035e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136780149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b5b566617eecf28afb7200ea107a9a85c4a5a8df702a8b6ef7b47930e217b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1522fa112776c1cbab6ae7bfc1609c9608e3575fa24e818e55ddc5ffe0e5c2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149631567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf814f247c4e74e1ae8028615dc5de955a05011d9f2f8a5799e6b4b77fc66d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b549a05446434e911aa7f23d6d7d3bbd3e215ad66876361d6e02362eab38a`  
		Last Modified: Wed, 16 Aug 2023 02:13:30 GMT  
		Size: 70.1 MB (70136139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cfb04e68ce0c0aa89915d342517d5997324c820a3d6fc788f8df7964c3208fe6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136961726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfcc1107c502eef2ef6942ab279be71a861768c71f2e77d5c0259e1a2da8e0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45414c0dac5eed7c0002a6ec3f910c9ab1430c15501a8f4ac7399a32a19be528`  
		Last Modified: Wed, 16 Aug 2023 04:38:12 GMT  
		Size: 63.9 MB (63911557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable`

```console
$ docker pull buildpack-deps@sha256:887b7c1c6349f877496aff09f003d1a8ca44d7920f54c83a3ae5f1663655d7ea
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

### `buildpack-deps:stable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cedca83f214f57a77af8d507c7bbd58b9618d324a7f76a8982bf04e0528c8f8a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **348.7 MB (348731829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5e13db2bf545a7b1de49aa4b5dcd4843cfd4b9bb113c6b8a4352af25328976e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:02:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d207285f6d296b9806bd00340437406c25207412c52fcfcbf229a5ecff7bf94`  
		Last Modified: Fri, 28 Jul 2023 03:08:11 GMT  
		Size: 211.0 MB (211031643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2c09193e02c99f22817e99a79d739d6a28a9ba088215ea6c54dd2bfa2dec1865
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.0 MB (316041553 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9887d75961eb626b52dbbf5253690d3d966737baddd8965129d4d16db7f2965a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:41:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee620d7d428f8ab8f98bd01334daa0d3d3451ab6ce3c2604db13f25fb844b517`  
		Last Modified: Wed, 16 Aug 2023 00:47:56 GMT  
		Size: 184.4 MB (184362791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:346aa10945b5d3dfb334983e9ac38343786fba2b906d44ce42a61f690b17d089
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.4 MB (301441954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf80e307949f46b37c0e68056e99719948729e088daf4c43c456f06911f28e5e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:29:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1d20fcbc5dc95c69a9da8c989746956c1a43040f526f2940cae30659253a710`  
		Last Modified: Wed, 16 Aug 2023 05:48:30 GMT  
		Size: 175.0 MB (175010240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:0ced2d9d01077003c3c5d55a93f8e41b392902c6e5265edf70caf9c18429b4e3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.6 MB (339572095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48d922574f706f083376eb631710c25d0a21a3046824f98272107e43e9160407`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:22:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56ae3b61eb9574588be7e73e31c31798e2cbf75f53f1f824d855afdf2be6437`  
		Last Modified: Wed, 16 Aug 2023 01:39:15 GMT  
		Size: 202.4 MB (202422266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c15e9b7c03bf0b95f3f1851dcfc9c0d106eb9f4ad6f70b264a297b2d0eb2328a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.4 MB (351357188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b1198ab2df7d04bcf039232d26fd5e7f3df61a5052fc44bccdbf90da8b72d3b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:27:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fb23d9f6cfe824c8d50c7242bc34abd22d983eaf2b3d86f43dc174605402d4`  
		Last Modified: Wed, 16 Aug 2023 00:35:48 GMT  
		Size: 209.9 MB (209946980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:40ca01021b43c5582696c732c712900b7b4a8909c7fc5280c1de8fab1b1121b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.7 MB (325734198 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfda94015496c32c381731065d8190dc80cd6a287df3a9363de97b109f153914`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:18:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f19a5348eb78e6ca17f708ec635d0965eb52e17623be08930925d53c4e7910a`  
		Last Modified: Fri, 28 Jul 2023 01:34:25 GMT  
		Size: 189.6 MB (189628655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:de4665916ba11daa50f4c9cfeb03b217dbd50f83c2200780e5e322bccfbcbb95
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **362.9 MB (362863053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd81888fa25d94a8c677ec5865fdc3a4a6d8e90b13af90684f39c936db3ba470`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:43:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8b794b3ece578acf2202199e34306bae8447e86949ab7b4aa0a7ffa9560aad`  
		Last Modified: Wed, 16 Aug 2023 02:11:03 GMT  
		Size: 214.1 MB (214068144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:9531f7edeedf64601eea231ca0a9df5886574ab064a48b54017d35728ad9229e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318160715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:417b6bee7ce6cebab35f9a7b46928127192aba8cae28f38b88e80d126be28a70`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:21:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6fe9d5e378cd41e1b6d5bb16c3c1956dcdef66615bf00a9d29689cc471f4377`  
		Last Modified: Wed, 16 Aug 2023 04:36:59 GMT  
		Size: 183.1 MB (183096288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-curl`

```console
$ docker pull buildpack-deps@sha256:2e3eac33829d6b53d214289b54fe38fc84cf33c99b37237d5398c353d063950d
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

### `buildpack-deps:stable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:a313e1ca160fa76c5d9dc53ebd96e5bf59f30162a48a3489fce2e67c2532fa98
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.6 MB (73587893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb6cafaf6952dbc34eed9b6f6e2adb817a4b14779c23edc0da1b871b776864e8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a7592f1639d909f25dccc729a2b5aaa513a70ee28a85c4189038b9717092f588
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.1 MB (70124664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a21d1f5171263c0576c940aba7c50a5812f345cc44bb53c3530243b7749caa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:70e09d598b5c38a406d30c717457f324114b7db7ef5693e0ae9cc939200c9f82
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.2 MB (67169862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee2b3159316a467ca9e01e173c57a3aaf9062379e269053863138bf9e55e1d1b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:cff052d3d1eaf4b534c62e5725852806e16aab4f90a4144c555a766ca1e1b901
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73161356 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eb3957cb621c85ee2f7494fa16ccb1c65eeeff85c9b649dc3c245c2f03e78ec`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a837769bd3f8a9e4f69a513a0945a56bc51b71fe083f1ded5f3b22600433eed6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.4 MB (75437808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32d4066bf6815648a7034016ade53e884437be1fde6892f2b3083044d74b7a86`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:a3e2a302292d240c5ef6a911d4bfedda10227f69539ea8c2ab29f62a31e82320
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73154697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:199c7f9557e825f1e7c85367c036809337980df0f60ab3bd943ec9c3ef5a701d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:2850f04eb55d1c646bead20a4b56782278f56cac1945ead77243a32e21dbd376
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.2 MB (79224885 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25ce09dd7847a86d1a80c72f8b63f2fbcc394fc118b4fdb8db043e5ae72e30b7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3d921b58c4f6cfc3529e474bc5c5657b69f266389dbf9ca1e01a3f993d995631
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.0 MB (71950786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0935d347529fc2d002323338e9b1d1227981a43082eb49f42287668f6cee7c76`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:stable-scm`

```console
$ docker pull buildpack-deps@sha256:b514f7a71ef85fb2535d7df3fa54310136f7cc6c52aa55040f822eb5803285b9
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

### `buildpack-deps:stable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:529e163a2641648602b7c30f6628836a07309db7eec36b54bc1f3079fe1a0075
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.7 MB (137700186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:612d62ca1b84af9b3c9ea7d4f8f7451dea5d5280997f2995f5a5476d50e65656`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:29 GMT
ADD file:cc1376ecb3d9e93e4160573c110da753ffeb2efe2223351f1fbf483d89f1a756 in / 
# Thu, 27 Jul 2023 23:24:30 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:00:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:785ef8b9b236a5f027f33cae77513051704c0538bff455ff5548105c954c3b1c`  
		Last Modified: Thu, 27 Jul 2023 23:29:02 GMT  
		Size: 49.6 MB (49557354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6dad8f55ae6c733e986316bd08205c8b2c41640bf8d08ff6e9bbcb6884304f`  
		Last Modified: Fri, 28 Jul 2023 03:07:18 GMT  
		Size: 24.0 MB (24030539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd36c7bfe5f4bdffcc0bbb74b0fb38feb35c286ea58b5992617fb38b0c933603`  
		Last Modified: Fri, 28 Jul 2023 03:07:36 GMT  
		Size: 64.1 MB (64112293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ca109ee1bf05c7a25cab135c9f5f90087363f22e7e296b1345aebcafc2d4c87e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.7 MB (131678762 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c4c0f43441c554eb412fc1a6cae438793a4ced333e8a6a89228b9ff87bab33e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:48:23 GMT
ADD file:f079a473284b30bb99c4a21c61719c499c0a305c49fedaa717bbfefef021b7fe in / 
# Tue, 15 Aug 2023 23:48:24 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:40:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:40:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1efc9639d902ebaa56d5e963066d5ab28cdf0e5fac5aa967c72326db76357b0e`  
		Last Modified: Tue, 15 Aug 2023 23:51:10 GMT  
		Size: 47.4 MB (47415020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e34e7b4c1a2c0700b8db12eb4cb9569ce104cda1989e5b4a480e35dd71690d33`  
		Last Modified: Wed, 16 Aug 2023 00:47:01 GMT  
		Size: 22.7 MB (22709644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b77d20c8ff916e804bfb695aec7b06de85d30fe17cb0e067d2cfc9f75356d56b`  
		Last Modified: Wed, 16 Aug 2023 00:47:21 GMT  
		Size: 61.6 MB (61554098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a1fa0530e19b09fbd7c6185d73d84a4bc942d0411671313e2938ef77ad01ab4b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **126.4 MB (126431714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:694ce6041bf7543b9d45b61b59f896cf7826c571374effb2a7e96d4db51004dd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:16:59 GMT
ADD file:03964ab92340a6f07fac7e332ca5f5401b3a35aa1e4a5c0b2484a71ff345bc29 in / 
# Wed, 16 Aug 2023 00:16:59 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:28:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:28:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:22c91d9cbb3cbc0e4a05c1bfc86da0b5a439ded4f68eb2fbc055ba6b85ca1d90`  
		Last Modified: Wed, 16 Aug 2023 00:21:04 GMT  
		Size: 45.2 MB (45232937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24238a7fc18d7c6089f4f19e3e3d866f42674716043768c48cf6cabb7c8855b0`  
		Last Modified: Wed, 16 Aug 2023 05:47:31 GMT  
		Size: 21.9 MB (21936925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696afa3824e29b9ed0a2d2d4938069d1122051fc3db7a03f0ba2a9271d6ba10`  
		Last Modified: Wed, 16 Aug 2023 05:47:52 GMT  
		Size: 59.3 MB (59261852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:3420b56cdf17798958f80fd610bf3004621a3f02bfd92180f1cb4996eb07ea4d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.1 MB (137149829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:177d9930ddbbf17d991d76e9b71338fede111763111e1bbfe07c60588804ea5b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:49 GMT
ADD file:ca43018e3d97d44b49e60fe002bb20834a74cc1163d7e95ad50d549f072de158 in / 
# Tue, 15 Aug 2023 23:39:49 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:21:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:21:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a014e5e7d08c37cf1703b97e701ccdc850e4a18d0ee679f03aa875dcd520aa85`  
		Last Modified: Tue, 15 Aug 2023 23:42:59 GMT  
		Size: 49.6 MB (49591310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715cea74ecbb15cb82efef1e77dd60c31d90b01d1286d6f39b4562afaebe75f3`  
		Last Modified: Wed, 16 Aug 2023 01:38:30 GMT  
		Size: 23.6 MB (23570046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003f1109a21287fa17dc866e87e8c6685113960cbb0379fee8f42b83de63c647`  
		Last Modified: Wed, 16 Aug 2023 01:38:47 GMT  
		Size: 64.0 MB (63988473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a4d7df737a84cc83cbd61c2dc4edc98541d9bc7ace5cd833a1a14b8a5d027df5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **141.4 MB (141410208 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:147bc03aafb5bcbab9affe5fdb15a1a58291461d8982f37588936198fcee1337`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:38:49 GMT
ADD file:3f0a4d6b18b22088d0785bc2e351d829ad1ed6f154058017035842bdbe2a8d1e in / 
# Tue, 15 Aug 2023 23:38:51 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:25:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:26:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1dc6cc826af02d533745c4612f635e028f3471e46f50422fd20a6dc913b60574`  
		Last Modified: Tue, 15 Aug 2023 23:43:02 GMT  
		Size: 50.6 MB (50568054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ca8436c5a9dc8b9ea408612ff7210bcceebd896671ed3e31c61f398f9a00f25`  
		Last Modified: Wed, 16 Aug 2023 00:34:36 GMT  
		Size: 24.9 MB (24869754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4ec215b1e0b3f7f5034048ddb02b52122b17ef3885d242da7fca37250884e3`  
		Last Modified: Wed, 16 Aug 2023 00:35:00 GMT  
		Size: 66.0 MB (65972400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:9e6b325e9f83cee376fbde36a72981f811fae25c545e31c8915da5654dff04b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.1 MB (136105543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b95c96798319d28a7d61e576aca883a6bd72c3ba77b41f8b73169a8976c95c09`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:10:44 GMT
ADD file:3568f288ff9791a341f5cb0e99c0a63e09a68f3816d7f7a9971127b9b98a04b8 in / 
# Thu, 27 Jul 2023 23:10:50 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:11:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:13:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e4dbd8372ba202a8b430bce8d5c5b8a4bfdbc6ef2703180665e5964d51bb0437`  
		Last Modified: Thu, 27 Jul 2023 23:21:43 GMT  
		Size: 49.5 MB (49542050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69206dfad992d03f1e8e833ae728ffacf2c6919f78c4822d849e341473efebb`  
		Last Modified: Fri, 28 Jul 2023 01:31:27 GMT  
		Size: 23.6 MB (23612647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fab0a49ca1e0cd2eb4b9660e3a70dc1ab671984cc4843ea845a6cf76532eaa`  
		Last Modified: Fri, 28 Jul 2023 01:32:19 GMT  
		Size: 63.0 MB (62950846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:09c65b2c916c3d1627cb0f348b84676386b69d2923931105735d0d62c5ee5f16
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **148.8 MB (148794909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:917d2cb79031f827ec74172b6e7d6f32308c68e0b31222d978e62aaf41a7e4ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:09:14 GMT
ADD file:8397677919f9bbf5273ddf61e008bcaace9195b46bcb2c31aff4f0a88617f12e in / 
# Wed, 16 Aug 2023 01:09:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:38:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:39:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c59f7b2759f74830e13fa72caeaf898f560f72787aa9d5aec28bcf8585f2f066`  
		Last Modified: Wed, 16 Aug 2023 01:15:22 GMT  
		Size: 53.5 MB (53543761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cce374dd487e4d067dd2727a6401d31bd379da6e10a83e5a902a80be18aabaf`  
		Last Modified: Wed, 16 Aug 2023 02:09:27 GMT  
		Size: 25.7 MB (25681124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acab4f12553730c8f77e5e6b7ef103cdaf3f7db095c145c4b58ec1da135086b1`  
		Last Modified: Wed, 16 Aug 2023 02:09:59 GMT  
		Size: 69.6 MB (69570024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:48f4ce295c01fb2e62b6b64c1bd63eab67ca9e80601edef71244eb6a7f6a77b9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.1 MB (135064427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40fbcebb591453ddcf6b4344fadc51626a83a65bb4d445d480182536306e76ce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:42:11 GMT
ADD file:eeb165e8fcc9b8f3a9e8f10fdbd507a91bc934046a4f23f2d636ca4b1796d1e3 in / 
# Tue, 15 Aug 2023 23:42:17 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:20:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2bf08d586558a71fd0c5172579e7c378968a16f427fb3af772e4aa11c6b0a7af`  
		Last Modified: Tue, 15 Aug 2023 23:47:38 GMT  
		Size: 47.9 MB (47922016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7afba98ba5dea198ec27ff40c833c54ce73ca11dccc94b59611cb506b44fa422`  
		Last Modified: Wed, 16 Aug 2023 04:36:16 GMT  
		Size: 24.0 MB (24028770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc50673f1af082588bca57ac1eaff982b89ce5badbe6d6b389ad96961fe54a81`  
		Last Modified: Wed, 16 Aug 2023 04:36:31 GMT  
		Size: 63.1 MB (63113641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:0571dc0ae118e64a0334c074e5e490775c01995a5fa1d7f430644f83a7e099db
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
$ docker pull buildpack-deps@sha256:bc0bb95e08ed205a17de1379a423d4d44e52a9488c7fe9cab2bbfcb7ad141298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.3 MB (557269293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc38cd003d8e650a25ad517e8d5712030439ce1980704ff4cf2e0d69b818b39`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:24:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c5a779e1a53b62babe3fb9204c1be41796097067190b79b67822f58d7293d`  
		Last Modified: Thu, 03 Aug 2023 03:38:15 GMT  
		Size: 418.8 MB (418845194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3cba1948c3b97628ad52a9c62d2e817ca47973f768eedf96322185146a3a2b44
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.5 MB (337513714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c295b52d7de4d81008aff9a1611f40ecfdb08a270deb5f23a02cfae746f6041e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:46:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ea5e28c6c87005a46ad476c9b4f15160056117290320261d90a2241b5237f2`  
		Last Modified: Wed, 16 Aug 2023 00:49:27 GMT  
		Size: 62.3 MB (62299617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9647be011a70a1d8cb1dfb1d0afb023010a89f62a9a6e0d82f2b93815bf4d610`  
		Last Modified: Wed, 16 Aug 2023 00:50:04 GMT  
		Size: 204.9 MB (204867568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a6a6e2933f4fe4cdb7aacd5fb8b1b5abde5f97bd9e5257fbee772c03c9e7d281
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.2 MB (320151464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51a9929ca4554ad801cc1e8e609d3a64463241c751f234e8627b4c74066d6cdc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:34:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:36:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916b1beb64303951348c4609b860a99cd5d81954299ea9ae649cc3d0d51fda`  
		Last Modified: Wed, 16 Aug 2023 05:51:01 GMT  
		Size: 59.9 MB (59937940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5492b3f9added58b496e3ea6da2043a8fbefb6532b2420c18476c76a9db53ce`  
		Last Modified: Wed, 16 Aug 2023 05:51:40 GMT  
		Size: 192.9 MB (192853583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a12c54dc2ff3d11715e904b8db919e2517afdfae35a7e7b59008efb5c52c84ef
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **358.2 MB (358217052 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e78407adc2610c61a745e8426d80dc5bb139a2472320b762038bf188d2c45f9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:27:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5bcfe9fb2496b09fb02f12a4c5eab9ce200446746f7c777fc1a0025d3a400`  
		Last Modified: Wed, 16 Aug 2023 01:41:19 GMT  
		Size: 64.6 MB (64637449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e8a69e947e5f68e66c6a9a127741df87951c498a5ad8d446ff015d7f56373`  
		Last Modified: Wed, 16 Aug 2023 01:41:48 GMT  
		Size: 220.2 MB (220237253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a051074a4cc184320a02289fd343291bbb98f143e22f02c9132594a3a867ba7f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.7 MB (370741062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2a9f8698e8fdd7e8ed02cfd14ba7c974886d7633a36030dd548d9388d1de892`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:34:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84633700d0e0c5a1fd8bad79e5e4601602218914f21595af58697a382ad3c928`  
		Last Modified: Wed, 16 Aug 2023 00:38:54 GMT  
		Size: 66.5 MB (66513490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b41b59cf71c0596e7c00b5aaeebc3212e55085655c713c093e7efd3411e724d`  
		Last Modified: Wed, 16 Aug 2023 00:39:42 GMT  
		Size: 228.5 MB (228480503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:2b0f9147d252c8ba32e8cdd3b352887252f4906f8158d3539bdda46a5c120067
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **641.6 MB (641552716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05efffdd05a2a9414dbddc4b50581de33a6bd45816b1262cf64b4f983a5e54a9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 21:18:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9085ce02bdf495dae6f1b38c84f07f4cd662a4ca17153a9b1478678a4196dd`  
		Last Modified: Tue, 08 Aug 2023 21:24:03 GMT  
		Size: 504.8 MB (504772567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:45b3c7ed26f2a264761ba4df36f122e891d0db394334bd080629cd91ee1023a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **377.7 MB (377654498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5a4096243039871d1ba7854c5d70b1a6bbe52f1a581ec8ba200d55cfdda31c7`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:53:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b549a05446434e911aa7f23d6d7d3bbd3e215ad66876361d6e02362eab38a`  
		Last Modified: Wed, 16 Aug 2023 02:13:30 GMT  
		Size: 70.1 MB (70136139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36a8210cc7ae63d1a84c252e719574868919ae783dc9fd2dc72f4084f58d6d8b`  
		Last Modified: Wed, 16 Aug 2023 02:14:34 GMT  
		Size: 228.0 MB (228022931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0150bb87b97db7106a8883b1971dae5b87fbd5391ec9118cf15f6932d83b0f8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.9 MB (584935368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77126be424a00a29f764cd8e7f8da503eebb4c14608d89dd3edd5a2278ccba0d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d3e46d641c1277be46ab521cccf04aeac468f053836ff4e0626b3a862cb7d`  
		Last Modified: Thu, 27 Jul 2023 23:57:35 GMT  
		Size: 455.5 MB (455541137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2a93b138fd3b934f4dc0a7982cd9b735f56f95dd1af09935e0654afd57b453cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **339.5 MB (339461658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d2c2ff61aa1f806db15fe7f1e44d2044c4c9bcfc6dbef062b36ea2f7eb4fdaf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:26:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45414c0dac5eed7c0002a6ec3f910c9ab1430c15501a8f4ac7399a32a19be528`  
		Last Modified: Wed, 16 Aug 2023 04:38:12 GMT  
		Size: 63.9 MB (63911557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16663081eb6f5dd01559432e43375fcc1d345dd3c74367ce1554e5dcce76c379`  
		Last Modified: Wed, 16 Aug 2023 04:38:45 GMT  
		Size: 202.5 MB (202499932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-curl`

```console
$ docker pull buildpack-deps@sha256:021706d0d55d40a96982ded0e76f1b459dc2b5c4ae0fb28e6076d9232929e2e7
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

### `buildpack-deps:unstable-curl` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:7d2668493b4f046b71c6260d3279c31c6ba4f2a286b05c50c2f5b4e868e1cf3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.7 MB (73749616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6413f0d2d0378de2d6a8d9d1402a6084483971c14f3fd113e9eb890502af0b02`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:774563c7ab34b698df26f2291a44ab24b899f0da48b5794c4a9e51b889427e90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.3 MB (70346529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6be2e6d9a14df3fc131f09bce7ad48cdbaba68d086d00efc976e7c7d409a7f17`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7aa62e1d9c56fdf41c87e3887595f8c62f23d55bc0264ed2eed3cb92781c30a3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67359941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbae1d38f1729ba21724854f9beb2bc47acb5dda4f340347d633af0d94e57f0b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:f357b484f94d65bee85830215f8a99bd873b9b6c588d9b18d73a660d1b7d230b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.3 MB (73342350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ad8010747ba13453458120a56606c915f892703fb198850dde407010ab2ae49`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d97b42d29a664dcae93cfd874db1be9d3c194cb92623f2447128c5bb0a572761
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **75.7 MB (75747069 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ac27c3bf31307e25bfee6c4ee200ddeab2b6f606757de278d52f1d0566c9aa`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6d22f564936ef6047f439f288c6487d49ea9ea94a3d3d823ba789aae0b57477f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73200135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73a82efa8a0cbd2145763c100f743ab0c6073cedbe7ab03288024f57dd678d67`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:dd603885105b996b2f2ac71bdbc6418f425ef338b8ccd9a0f89d91b542e774a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79495428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18a1a539a3d7557346dd1bc8a2d6ee409a1be725c2e2443794e3c9a9de8a62ab`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:463277650cb87ff963c4f3e246c78101c2bf595bfdcfda04fb4db350e9dc1592
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (69007846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a46d4dea6048745e0f58711f73e97cfebd76971edb90fbbf0cf7dc14a24ec144`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-curl` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5df31820934ef52dc9dc24dd1fcdb4b91a3fe8bf2ad43a7f4804416b0d88d208
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.1 MB (73050169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e8ca8ec8e68c1439425282cb5c2b9588e08b3dfb887b123af12009d46531388`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `buildpack-deps:unstable-scm`

```console
$ docker pull buildpack-deps@sha256:3580956c9b85d435795cdcf2244a4e7d190309302f99161995532414d892be08
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

### `buildpack-deps:unstable-scm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8a363c27455cd9f6fcde5596efa71102fa5c2cebfbf12fb0c5157e2fd3ab60b6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.4 MB (138424099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4cd89db58a3ce0a728b12a56803552a04aa7aacfc0b27734d53addf8a3d8ac2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:995b60c9e41b030f0344790a1dff3b20c9cae8ee4c703b977c9b0d9430ab4061
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.6 MB (132646146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67a6c98e02bcec94970ee808e61c9a8590a882a8226f1b368af55d851188919a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:49:11 GMT
ADD file:2d486f4790de50d5a173ed5147c22ebcaaade283f5bdf6b62bc072050fc164c1 in / 
# Tue, 15 Aug 2023 23:49:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:44:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:45:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0fb27bc4b8f884dd1bc1129dd87397bcc993ec915005657bd21811eb84745100`  
		Last Modified: Tue, 15 Aug 2023 23:53:08 GMT  
		Size: 47.4 MB (47403781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f883267a6e0fd23a7321e7809daf18ea9fde5af7d382347913aa6b73346ef73`  
		Last Modified: Wed, 16 Aug 2023 00:49:09 GMT  
		Size: 22.9 MB (22942748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72ea5e28c6c87005a46ad476c9b4f15160056117290320261d90a2241b5237f2`  
		Last Modified: Wed, 16 Aug 2023 00:49:27 GMT  
		Size: 62.3 MB (62299617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:71e545c4c300ac58377187dbd4799d9b01e698fcb27446348a1c64491d93b188
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.3 MB (127297881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cddd27e18a2b66911c51d5c160ed1e3ce962332301bbd360d705d4c34c88a93`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 00:18:42 GMT
ADD file:2a1f1ecc1cfa876ccc22e6ef2a3a4ea39a83aec70ecde3f7cdaddee69dac2002 in / 
# Wed, 16 Aug 2023 00:18:43 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 05:34:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 05:34:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ccc7cdd48defe44f9a45f06f57d69b192155657bc5d244f915958c2027d645c3`  
		Last Modified: Wed, 16 Aug 2023 00:24:10 GMT  
		Size: 45.2 MB (45189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6609fcf5feea7fb712abd4f4cc12586f4960ac4271da561ebf2ff0717e096c5`  
		Last Modified: Wed, 16 Aug 2023 05:50:44 GMT  
		Size: 22.2 MB (22170662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a916b1beb64303951348c4609b860a99cd5d81954299ea9ae649cc3d0d51fda`  
		Last Modified: Wed, 16 Aug 2023 05:51:01 GMT  
		Size: 59.9 MB (59937940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d2be3ea85b4c5c86e9424499855e28f42a6e36f936bc56f533cb789ae866bc12
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.0 MB (137979799 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e5d9a52e4fa2879e47cae94ed7921d770e284c2b20f66a2e9e08faa8857704`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:41:01 GMT
ADD file:8064072457ccf7b4072e08095fa84f96b0fe3387ec8f302afde022186aa3eab5 in / 
# Tue, 15 Aug 2023 23:41:01 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:26:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4513653e4d749342b34f60c592adaf0ef4af993e76a913a1c086a4229a0e3afe`  
		Last Modified: Tue, 15 Aug 2023 23:45:54 GMT  
		Size: 49.5 MB (49531730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11f5de6e756ae0263d5d8056bc2a6f2a8e87f5e28dde8b746fa6cb29bcd33513`  
		Last Modified: Wed, 16 Aug 2023 01:41:04 GMT  
		Size: 23.8 MB (23810620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3c5bcfe9fb2496b09fb02f12a4c5eab9ce200446746f7c777fc1a0025d3a400`  
		Last Modified: Wed, 16 Aug 2023 01:41:19 GMT  
		Size: 64.6 MB (64637449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:4e2ce5378c4db0184f2a5113732e97908ed485193eb9df0b315b2257f4f2d8f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.3 MB (142260559 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518bb0c85280b757bff997cb92e6a086ab364b971d4d25fa86e8f1e53e0ec81e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:34 GMT
ADD file:d86f66385d3993c597ac040a976cd8a826b097d014cc4f3b69d8ebfaa5aa6eff in / 
# Tue, 15 Aug 2023 23:40:35 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 00:32:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 00:32:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e41394c7daa90fb4aae0f67d43af5ee9838fb125e249fc0002bfdc3b90bb6c05`  
		Last Modified: Tue, 15 Aug 2023 23:46:33 GMT  
		Size: 50.6 MB (50631355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fb36009acd0e1d753239daf3a185a717a7e268ceb556a566bab97416024ee1`  
		Last Modified: Wed, 16 Aug 2023 00:38:32 GMT  
		Size: 25.1 MB (25115714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84633700d0e0c5a1fd8bad79e5e4601602218914f21595af58697a382ad3c928`  
		Last Modified: Wed, 16 Aug 2023 00:38:54 GMT  
		Size: 66.5 MB (66513490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:13c2f443dbe0048ee66a2dc9ba3c4726b576afd4987d853bbe4be5fd6c3035e5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.8 MB (136780149 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b5b566617eecf28afb7200ea107a9a85c4a5a8df702a8b6ef7b47930e217b4`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:14:28 GMT
ADD file:5d5d4b53ad51debb95681500ba4a990279ff7fdd2ff80d4d4333b7dc647c0543 in / 
# Thu, 27 Jul 2023 23:14:34 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:28:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:29:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9b48d6f46b6cff8bfdf81f7ffbfa05dff828e1d7545e640bf61d5486c1b79892`  
		Last Modified: Thu, 27 Jul 2023 23:25:52 GMT  
		Size: 49.3 MB (49334598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dde2d4334b6bd5986094b014a83b3832c21ffb948989d6fb842246593177f671`  
		Last Modified: Fri, 28 Jul 2023 01:37:45 GMT  
		Size: 23.9 MB (23865537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86218b2ed81ed0041845b0b5b1e95efe348740465925fef57859a751cd7a6596`  
		Last Modified: Fri, 28 Jul 2023 01:38:35 GMT  
		Size: 63.6 MB (63580014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1522fa112776c1cbab6ae7bfc1609c9608e3575fa24e818e55ddc5ffe0e5c2a7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.6 MB (149631567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bf814f247c4e74e1ae8028615dc5de955a05011d9f2f8a5799e6b4b77fc66d9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 16 Aug 2023 01:11:08 GMT
ADD file:34567402b37eab48970f90189fd56c47e39acba6d260f0587409ca36a8d36458 in / 
# Wed, 16 Aug 2023 01:11:10 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 01:49:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 01:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c0db36c7b4f2702f9e0075ee892fe4761e0f37f5cc9d73192725313c01591737`  
		Last Modified: Wed, 16 Aug 2023 01:18:29 GMT  
		Size: 53.6 MB (53551877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08327233d2cd5240264b2d14e300da4220731205ebdb79a082288235d814fe5f`  
		Last Modified: Wed, 16 Aug 2023 02:13:00 GMT  
		Size: 25.9 MB (25943551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b549a05446434e911aa7f23d6d7d3bbd3e215ad66876361d6e02362eab38a`  
		Last Modified: Wed, 16 Aug 2023 02:13:30 GMT  
		Size: 70.1 MB (70136139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:82b54224e16141b3d128a2c7213a413e390b1216abe389f923a2eaf497c751af
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129394231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4d1a4d2d9108164c640ce2247e18e16b8a958c777fd7a7181f424ddb829d083`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable-scm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:cfb04e68ce0c0aa89915d342517d5997324c820a3d6fc788f8df7964c3208fe6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136961726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfcc1107c502eef2ef6942ab279be71a861768c71f2e77d5c0259e1a2da8e0a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Aug 2023 23:43:50 GMT
ADD file:a27e7d7c954291d644437a8054f06f492700f1ce13d3a9e2c3bbd71afd0869cf in / 
# Tue, 15 Aug 2023 23:43:56 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 04:24:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 04:25:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:db9f34e47daed3854a411cee94f611a7139b82002ae54802c9a44d3faccaaea7`  
		Last Modified: Tue, 15 Aug 2023 23:49:01 GMT  
		Size: 48.6 MB (48594395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2492f56fd0a0d7311e408655d1a40ad1f5ce8d34da47a127ae2f85baf9cdfd9b`  
		Last Modified: Wed, 16 Aug 2023 04:37:57 GMT  
		Size: 24.5 MB (24455774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45414c0dac5eed7c0002a6ec3f910c9ab1430c15501a8f4ac7399a32a19be528`  
		Last Modified: Wed, 16 Aug 2023 04:38:12 GMT  
		Size: 63.9 MB (63911557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
