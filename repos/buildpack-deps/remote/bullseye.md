## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:1e1fe4817c0bea712c7d114c89447fa6dbacb6045364784abb7e4c75e72e63c2
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
$ docker pull buildpack-deps@sha256:d582b60b8fadf217583329602c7581ce65866517e8ad7fffe50376bcd74802c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.1 MB (571116303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f315aa40a0484571eb393bbb9de01c09c69e4b8c9799ec1c4e3455213781b754`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:24 GMT
ADD file:fa865518757ef9e0af03796e7abd6cbfd59e20f5ae325422e41524615051a2d1 in / 
# Tue, 17 Nov 2020 20:20:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d004aa4da82e9e47169ac4cccf33df9b52bef6dda8aa5f7b0bcb03af34078173`  
		Last Modified: Tue, 17 Nov 2020 20:26:32 GMT  
		Size: 55.6 MB (55578105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5514b41a34cf855f2908da965f01f2b0f68fc62b29b9fb67811a07e7c61d16`  
		Last Modified: Wed, 18 Nov 2020 00:47:23 GMT  
		Size: 5.1 MB (5063216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3985bf4e3bf68c52363fd7853ecc6142b55501eb8457558d27ae10a0358e8907`  
		Last Modified: Wed, 18 Nov 2020 00:47:24 GMT  
		Size: 10.6 MB (10645972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f00fbcbbd3c3783e061ff8d861834c157f06601ed495383250dabb36682027`  
		Last Modified: Wed, 18 Nov 2020 00:47:43 GMT  
		Size: 53.5 MB (53498354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea11244fb3f5d36092406898f5b457e9f31dff55684878b37961efee3354135`  
		Last Modified: Wed, 18 Nov 2020 00:49:33 GMT  
		Size: 446.3 MB (446330656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:a1644a92d3129128db0927452fdb772ed6a6a89d5ad88bebdbaf8c25608a9014
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **528.3 MB (528349723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8966ed99348393fe8dc45f35f07eb5d692f57e483cabe6748bcbbc63ec459a40`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:15 GMT
ADD file:1825c9ae9f20eb2576f772d68892699ef4ca90dff36b8f247bf78ce04ad41a91 in / 
# Tue, 17 Nov 2020 20:19:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:35:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:35:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:36:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:41:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8172f634b664f563947e1ba480d8a7e04acd125ff144bde0dabb4ef26db6d3b1`  
		Last Modified: Tue, 17 Nov 2020 20:29:25 GMT  
		Size: 53.2 MB (53174409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a9bcac9e1b17a227267b364ec33a309b567898a11a1049896dfb513508befa`  
		Last Modified: Tue, 17 Nov 2020 22:05:34 GMT  
		Size: 5.0 MB (4974569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af90ca1b550dfe775778350f5133681fd06314fe43ae77642bada174068cdcf`  
		Last Modified: Tue, 17 Nov 2020 22:05:35 GMT  
		Size: 10.3 MB (10331991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:169b1d8db5b8210961e24b26bc3d718e185f5af3264a1eed9a03e56f5f21aaea`  
		Last Modified: Tue, 17 Nov 2020 22:06:02 GMT  
		Size: 51.3 MB (51292009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e86d35ce06233ee7f1bb29651cf7dbb3c1e5487fd2885d528c8576de7fd9888`  
		Last Modified: Tue, 17 Nov 2020 22:08:09 GMT  
		Size: 408.6 MB (408576745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:7a5fc3b14c0a2d911e08a208d4ce3d2afe616d428ce90a3a0a40f53fcdd67e50
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **514.4 MB (514393990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a9b706b7de5e471ea6abaa1b66d0be37a207b639fdced9dae389fde1d67cca0`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:26 GMT
ADD file:f2393813e8311e27cf255e78079f523184619c1ee8ff9ccdf51a5cbc61751e1b in / 
# Tue, 17 Nov 2020 20:19:29 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:35:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:36:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:40:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:907906fd9e2e517e45080a90701520c1c3c654647630763a4cd9f181ae039252`  
		Last Modified: Tue, 17 Nov 2020 20:30:29 GMT  
		Size: 50.8 MB (50756959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:644a164f19b5f5e429261a5effb8cbcbbe66d7f6da9e93d9ff34b86f08ed6a42`  
		Last Modified: Tue, 17 Nov 2020 22:04:14 GMT  
		Size: 4.8 MB (4838545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54d419d3ef4e0a73ebe3cf3ced0bfa50e1e9961d81ecb60e542323b9bc441e6d`  
		Last Modified: Tue, 17 Nov 2020 22:04:15 GMT  
		Size: 10.0 MB (9971053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb56c58816ba83f360d684e04fd465ae4514e3f503575978543166b4671d81a`  
		Last Modified: Tue, 17 Nov 2020 22:04:40 GMT  
		Size: 49.3 MB (49299704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a1d95e5345597457c827018c139be28edef24b95bb2200e8eb52c729a0d87b`  
		Last Modified: Tue, 17 Nov 2020 22:06:48 GMT  
		Size: 399.5 MB (399527729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:895a78fc9ac9ba086e07be640403bbd60569de798579bd194b7eeab72ec213c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.4 MB (547430153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e820d1e3d83cf7165e1fc16ea00ea4e7066f78e8eac2ca47e25578964bffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:22:08 GMT
ADD file:58908becb64a88c580fc5d9fea54a7e73507d1e537e70b5567f5d58c26ad000d in / 
# Tue, 17 Nov 2020 20:22:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:20:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df1866c47e1fa1c26619e32544732be4853c6b58bfe5ea76c192ae970daf5da7`  
		Last Modified: Tue, 17 Nov 2020 20:30:56 GMT  
		Size: 54.3 MB (54323419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71907b4dd26e793f4e9841e590a1a930f7265a02f7c07e57767ef9cbe91f8b`  
		Last Modified: Tue, 17 Nov 2020 22:33:52 GMT  
		Size: 5.1 MB (5055744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2cf86d1130240ba8633c0151d4a4a4b9e6a251bf8ec2bf14d72ce40a67727c`  
		Last Modified: Tue, 17 Nov 2020 22:33:53 GMT  
		Size: 10.6 MB (10648270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c6056c2ca2fb8c36f5f80c875444bbf38dab5bc7ebf358fd257bac133169fb`  
		Last Modified: Tue, 17 Nov 2020 22:34:20 GMT  
		Size: 53.6 MB (53614998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f24020986f5e30e52733c264f645d35dacf69520bc2abf1c13b0608aed506fe`  
		Last Modified: Tue, 17 Nov 2020 22:36:18 GMT  
		Size: 423.8 MB (423787722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c92030662a686441a5e93e32096e01bedc2b544bf5910ab2eb7f2b7bebe1d900
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332725177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43fa2dee6195f96591017ac3f63ef37c728e91f82616bcda99c5cc0273b94a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:01 GMT
ADD file:df88ece8f6b35ea6811921d958952eb8431b76449597cb6d5151e88c62167964 in / 
# Tue, 17 Nov 2020 20:19:01 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:01:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:01:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:02:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:03:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9137c9a05e5bbf8d80413499157abbe788cac975a7926ded72bd9ff285f7520`  
		Last Modified: Tue, 17 Nov 2020 20:25:46 GMT  
		Size: 56.7 MB (56728874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd9994454c4b84708c2d9754f396aac9f662a7169c2322418210f8d161ac4d`  
		Last Modified: Tue, 17 Nov 2020 21:22:12 GMT  
		Size: 5.2 MB (5182817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87786a5db1b57a9ac7c14addd518c4d55f9ac878f951e8110866257d83d6d82c`  
		Last Modified: Tue, 17 Nov 2020 21:22:13 GMT  
		Size: 11.0 MB (11022570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88de8fd349f0d1c859351edc10905c5adca2e975f84e43d737a1933c7ee86944`  
		Last Modified: Tue, 17 Nov 2020 21:22:35 GMT  
		Size: 54.8 MB (54828092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b5e03aa9f809ea152b55fbb2eb45ba9f45b0e5e35e08a60e6843fab15388e7`  
		Last Modified: Tue, 17 Nov 2020 21:23:39 GMT  
		Size: 205.0 MB (204962824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:5a3c2b40d1ab5a95364106e0cf72f8599ee6dafee46d38ee6f477add5cdbffca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **311.4 MB (311417458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:702f5655dee906af6bc3148dea47f24de11754ec47bd707fa3c13e8dce32afe6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:18:02 GMT
ADD file:b3efb0da03cf858a9bc305dec420c5a2fd85b3ba7212cd26f4012b931492bcc2 in / 
# Tue, 17 Nov 2020 20:18:03 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:34:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:34:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:35:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:39:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b53392aabcbd30c0ebb343f6223dffd1e0d3a034f1683d60ac80a65254522359`  
		Last Modified: Tue, 17 Nov 2020 20:24:23 GMT  
		Size: 53.9 MB (53861718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58b5272c361da3f94922fc2e154b2c7092b6abb657a2857ef7684f41294c60e`  
		Last Modified: Tue, 17 Nov 2020 22:48:33 GMT  
		Size: 5.0 MB (5025865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03528b3943b7f8558ee96ae85f7871910f47c9b5f5e89e078ae6da0783a2ff3`  
		Last Modified: Tue, 17 Nov 2020 22:48:36 GMT  
		Size: 10.7 MB (10652787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:948afd46ba6a632c8ebf47f170254ed3eeb087a1f06b0ae45b1d02b59145894f`  
		Last Modified: Tue, 17 Nov 2020 22:49:27 GMT  
		Size: 52.3 MB (52340693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f3b34e6a75ddd1840f2fe27e6cd3fa5ebabf26764c7ac4d300bb9cc1ebd5c`  
		Last Modified: Tue, 17 Nov 2020 22:51:43 GMT  
		Size: 189.5 MB (189536395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:1f24cd44d68a838789aef49f98dd8cf02062060c73a9f3652bb6302a15303c59
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.4 MB (344377550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5405673ae4e53462f89b9aa5e300afde40daef3c18e508ffac50fe203e0f6b0f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Oct 2020 01:36:17 GMT
ADD file:29c9502df00306ab143f7a4895ecbd5188710e18fa501d1931dfffe0d2281c6f in / 
# Tue, 13 Oct 2020 01:36:23 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 08:44:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:45:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 08:47:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 08:57:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e449e1f1ecdd90acbe5e4ea9a9f941aa8dcee06a83eb2eff72fe4dd55cc20576`  
		Last Modified: Tue, 13 Oct 2020 01:47:12 GMT  
		Size: 56.5 MB (56486527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b868bd306c5ff6ba6bbe52fb1cc3deaa47fed5a1362d135d89cfca87a684e4a4`  
		Last Modified: Tue, 13 Oct 2020 09:29:49 GMT  
		Size: 8.3 MB (8307201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca5bd324b7e56f3121bd85c3a06132da98d95654678c2a01b4439cab8adc5b5`  
		Last Modified: Tue, 13 Oct 2020 09:29:49 GMT  
		Size: 11.4 MB (11392086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e26769c811da7971c25f9fab265e60dd509f2c8522ff89eea05deda913a34b33`  
		Last Modified: Tue, 13 Oct 2020 09:31:06 GMT  
		Size: 64.7 MB (64729192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77d111d1f21d3276ec3457e2a87edf499ebfa7d68721fabc9d29cc21105ffadb`  
		Last Modified: Tue, 13 Oct 2020 09:33:50 GMT  
		Size: 203.5 MB (203462544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0d92757fb776cbb76801d6c464f96da5df977b1bcf1104e75c575ec1c4f4230
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **515.7 MB (515677520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c28e4522f30508f99f2de88279f2b5ddb72e6d71860938682b75b169fd237ceb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:17:06 GMT
ADD file:b2aa936914932ddd337990ffdd06ceff2628d7198e962be967a9781efaba51d9 in / 
# Tue, 17 Nov 2020 20:17:17 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:25:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:25:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:26:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:30:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:069a0f569bbab3514d40a8e2575a33e70926c0aeacc9099b083427a84cafc126`  
		Last Modified: Tue, 17 Nov 2020 20:22:44 GMT  
		Size: 53.8 MB (53806147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e0c6c52e6336a9fffb0f96f9bb643f4f181052948188c1e0453ed3ab253217`  
		Last Modified: Tue, 17 Nov 2020 21:43:23 GMT  
		Size: 5.0 MB (5048357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce85daf872edba752735571ddb26859c12b6e958818465881a345aa93faeef1`  
		Last Modified: Tue, 17 Nov 2020 21:43:23 GMT  
		Size: 10.5 MB (10514397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecce1269b139cf68c0820b2ca3d17dcb95e08de624942ba2d3b6512f98f009e`  
		Last Modified: Tue, 17 Nov 2020 21:44:43 GMT  
		Size: 53.0 MB (52970704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fef7fc974d286bf3d370b740ecba7a9fbcb940a4538c564717920c4bcb499d1`  
		Last Modified: Tue, 17 Nov 2020 21:47:13 GMT  
		Size: 393.3 MB (393337915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
