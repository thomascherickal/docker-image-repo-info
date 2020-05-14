## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:0a8a4bf435abf54bbf5bd0e36ceee6360a067fb88a83fa3740fcffa018ac60a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:5b3206d7dd29c7f8e9991a0b7ae570799da9638565860944bd277efc94afad2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247166903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c96f285a599fc0b6e4ff2ec21dc5dfc6b08a462239f5265714e489dc83032020`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:20:54 GMT
ADD file:63fdbdcc45a46a993700d252a6f9652db8ab25688daa8bbceaed90b73b2654cf in / 
# Wed, 13 May 2020 21:20:55 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:31:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:31:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:36:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bc53e9ecf017dd9c8c8ba0c497d08e2d7c04f4a57dfce491d755cb37613f58a`  
		Last Modified: Wed, 13 May 2020 21:26:59 GMT  
		Size: 54.4 MB (54390659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cedf82ca715cf8b41a88bfb26ad7225ae77537b5999a2f9a3ed1c430b19bc98d`  
		Last Modified: Wed, 13 May 2020 22:46:29 GMT  
		Size: 17.5 MB (17546015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb3decbe8c76a4818f476de7732333bc00cdb7c3a75887374dd6d6450202e76`  
		Last Modified: Wed, 13 May 2020 22:46:46 GMT  
		Size: 43.3 MB (43334784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2417d595dacc6492feeb4ed843e3148b8eba618781c085dd45c08428b541fe15`  
		Last Modified: Wed, 13 May 2020 22:47:22 GMT  
		Size: 131.9 MB (131895445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:23a94255414b37736b35846f45973596b3a4fe511ff7030ab2162bae827757e6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227140177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46a3a8012c88873b01c70cc84f0ab7755bb8235c83b516be2e8ca0e62a0ca78f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:50:39 GMT
ADD file:621441e8cf0bd677ecfb646d7c54417894fedb89b8b03295c25a4ea0ebefbaf3 in / 
# Wed, 13 May 2020 21:50:42 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:39:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:43:02 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:535d6dc5159c1d8f20f2d1a86a8433d89941a1933de7a6930246eef7811be611`  
		Last Modified: Wed, 13 May 2020 21:59:45 GMT  
		Size: 52.6 MB (52581076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73189ba1a9ac8eb7f3c4a34630c9eacf6ef34fde77675eed4b21857d50d7a3e`  
		Last Modified: Wed, 13 May 2020 22:56:53 GMT  
		Size: 17.0 MB (17037185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd7802ce38e2c324b7cc2c2773a4bdda1c88367f6d1823d6807df3c2d00a9ce`  
		Last Modified: Wed, 13 May 2020 22:57:15 GMT  
		Size: 41.2 MB (41156562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311a88ec1bec506cd1aaa951469b373c436fd1dc83b93cc211bf502370e27bec`  
		Last Modified: Wed, 13 May 2020 22:57:56 GMT  
		Size: 116.4 MB (116365354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:60c67e4b400cbf9a7bad4231644d890669303a1fe42e57518a8b2400d81f3992
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221426584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04ed927599f883008fd3d4a1c709c7342880d11c0509f984f17fe4cce7e89538`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:14:33 GMT
ADD file:c27f6b9fb44500f82ed124d104a7cab3fed859c9cca4bbd0be2c77f3db082fa2 in / 
# Wed, 13 May 2020 21:14:36 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:01:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:01:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:02:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:05:43 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fb6d2bc03cec7adf4767dfcb7ac7a2740b65bd196c1071b809768619b12a0d4`  
		Last Modified: Wed, 13 May 2020 21:25:14 GMT  
		Size: 50.3 MB (50304251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32375e9074306a5d2a3cec4864995cabaaefd56b21eace9822bfed9dc2169d1`  
		Last Modified: Thu, 14 May 2020 00:21:41 GMT  
		Size: 16.7 MB (16723434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5c0933ac15f5a3d4ea8317d3ccec86327de17987d9262818b5c832440327fe`  
		Last Modified: Thu, 14 May 2020 00:22:01 GMT  
		Size: 39.8 MB (39779306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4837353aca3eb4b51409cd9cca1523915e9fde757c4416e8ea18ad8cb7d8c14f`  
		Last Modified: Thu, 14 May 2020 00:22:36 GMT  
		Size: 114.6 MB (114619593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b92ffbafb76efb517082584c27a4552aead1c7740219b93414beb9b0ce384e8f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254328864 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5ec4cae980be05e01d8709c29bc5c9681ac679c69beed671ff1c0a99aaf4d1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:39:42 GMT
ADD file:c41a548ee5a118fc5c8efefd084aca1f4629d3f462ed9d1bc5ddc568db89b0d2 in / 
# Wed, 13 May 2020 21:39:43 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:46:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:46:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:49:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:53:28 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3ecac86f3144ef4bfa8747d585400212884f0a7fb2a71c1eb54483af30ca0449`  
		Last Modified: Wed, 13 May 2020 21:46:50 GMT  
		Size: 54.6 MB (54607906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f067623bec4e0179ef9af3ffa91e7197a238ad23d31f534e3ee78a83f4547351`  
		Last Modified: Thu, 14 May 2020 00:03:33 GMT  
		Size: 19.9 MB (19855823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716e17289a4b0c8f800234eeecfdaac67fe336e111d4cfefafa845d074a0c65`  
		Last Modified: Thu, 14 May 2020 00:04:00 GMT  
		Size: 44.0 MB (43989891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab703bd2a16bca2a81b8368df78424fb309c5f3333e5ed321eb282d1e51adff6`  
		Last Modified: Thu, 14 May 2020 00:04:41 GMT  
		Size: 135.9 MB (135875244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
