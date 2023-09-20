## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:5977b8c26f29486c6b087568bdab3e31c704f94e05baf44e8569ef12e18ec847
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

### `buildpack-deps:trixie` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:aa176341f4c3d6c4fb5456a5c4a823c82c22816f1f377315c22d1057df75ea38
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **370.9 MB (370893021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9757632b447fc4059155fe799515b85035b2f13c175db9136cf9a33cc09848be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:58:17 GMT
ADD file:cd33732baf7a8215a9cb532ae6f2fe0be64d030adb1f3e0085e461cf4f22ec4d in / 
# Wed, 20 Sep 2023 04:58:18 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:27:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:27:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:28:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3954180d94025620e480192adbba35d582d59582f662e17f992f954d83539feb`  
		Last Modified: Wed, 20 Sep 2023 05:04:48 GMT  
		Size: 49.5 MB (49467670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e565cc2b6bbf1308bd8312f40ad760a99d8567113763dec2537af6652bb673`  
		Last Modified: Wed, 20 Sep 2023 09:34:11 GMT  
		Size: 20.3 MB (20269130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd10974eceaa5affd1244428fad92105303c6661b8d09326a7a85b3f11de3125`  
		Last Modified: Wed, 20 Sep 2023 09:34:28 GMT  
		Size: 64.7 MB (64669125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4505d43bc4385e169467514465a55c52a3f1e653b207da717c4fc7baef34cc87`  
		Last Modified: Wed, 20 Sep 2023 09:35:05 GMT  
		Size: 236.5 MB (236487096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:31a0df46c9266c44c6c6e57737885688c782605f2e849c6e42b829a12edb8007
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.7 MB (340655115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4650cbf27e8a18e5e7599968c26bcbfccffad53f63603af1cfbfbce555d2cebd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:52:20 GMT
ADD file:c6e1ebf545b4fe8a3d6b8e0eccf515df1d8291411d23a0e5002f40428db8b992 in / 
# Wed, 20 Sep 2023 00:52:21 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:02:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:03:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:04:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e7cf8ed3fa4a717011b456890e76475bcc7f559140833924436b7fe1266ee31f`  
		Last Modified: Wed, 20 Sep 2023 00:58:49 GMT  
		Size: 47.2 MB (47170081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2095ec2ed427a717bbeb48fd093ccb5d091ef08c9a25fade3d48178836b9f874`  
		Last Modified: Wed, 20 Sep 2023 10:08:49 GMT  
		Size: 19.3 MB (19346047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb293bf1cbd7cb52e62601f49f2c2be990e63ec593b249e5cbe527fee70844d0`  
		Last Modified: Wed, 20 Sep 2023 10:09:08 GMT  
		Size: 62.3 MB (62272465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b15c6c849aa07d4f318426b17e8cba4ebcce3bfadc1727b9f2215fe7b0eff09`  
		Last Modified: Wed, 20 Sep 2023 10:09:46 GMT  
		Size: 211.9 MB (211866522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:590926cfd516a542bad45c454c797918b72e3a9505ee53842bd12baf662875f3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317268017 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:276000b05ff0dd3a64319315498bf7ed996b2a2de22b465f9b72d101b16d08db`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:00:27 GMT
ADD file:56aa0cd11d12862eaf421a2ff6a2a518ae07f7d6180a2f0f58a9d10930215950 in / 
# Thu, 07 Sep 2023 01:00:28 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 01:42:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:42:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 01:43:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cbe28254d81156b7683ab6feb96334538a6b59d12717973205a1077d3bcabba5`  
		Last Modified: Thu, 07 Sep 2023 01:06:54 GMT  
		Size: 45.0 MB (45010494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfbe3001385a2b717c083b0eb81363b8210958afe6ccf0dfe6a62a78df022ec5`  
		Last Modified: Thu, 07 Sep 2023 01:49:25 GMT  
		Size: 18.6 MB (18600941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b39960ddda116bc7eddff9010f7bdc11c97332a0ea990a5a7e825d0cdcc2868a`  
		Last Modified: Thu, 07 Sep 2023 01:49:43 GMT  
		Size: 60.0 MB (59954833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df2a9fd326611756b102fbf1f32201a871a9cc44f1b01f52d1718b7febec80e4`  
		Last Modified: Thu, 07 Sep 2023 01:50:27 GMT  
		Size: 193.7 MB (193701749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:62b07d08b86893d60594a7bb1ac48209a0c539beba2fcba84ac299fac94af5b1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.9 MB (361904388 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4c0a4472053631efbf86462b54243bffc27d3c501fafffe269653e47ec181a0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:45:58 GMT
ADD file:dc9be3a1e3e1904a1eb81053b568b583a58307e861fc56fb1b7ce9349d2faa18 in / 
# Wed, 20 Sep 2023 02:45:59 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:30:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:30:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:31:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4d433462e04ded836d58eebb0fee68803768bcf3c9f92338a2cdda77bf7bef8d`  
		Last Modified: Wed, 20 Sep 2023 02:51:30 GMT  
		Size: 49.4 MB (49404499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f21fb48a05deec994e76626b5ba27bca3dceb8c7026037ba821d1ea929fbf5`  
		Last Modified: Wed, 20 Sep 2023 09:35:50 GMT  
		Size: 20.1 MB (20054013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb2f4db47f9fa43103b397742352887aade94ad72694c0f3eb40923c90c10f5`  
		Last Modified: Wed, 20 Sep 2023 09:36:05 GMT  
		Size: 64.7 MB (64653605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45e3f2a32df6d4636e89c69f8ef14af47f6e5f33bc49169303bd7bed9715f95b`  
		Last Modified: Wed, 20 Sep 2023 09:36:36 GMT  
		Size: 227.8 MB (227792271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:804add1c5eb5066e1f42e28617f5079a01a1373a83636786a3c3a388fcbb0d53
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.3 MB (367251235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17808699970975ed4678c2c8abd7f73dec53f69c7caf53b9ed9901b97adcd3cd`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 00:41:44 GMT
ADD file:5d53bf28b6cbc8eac8124a07c0bb8e04ee2d0c8989a8b7219612f6ced4f064bc in / 
# Thu, 07 Sep 2023 00:41:45 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 05:35:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:35:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 05:36:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e0d37cd24f690f803c53e61b67871ef6d1dd8980331679da74a8059a191a9fa`  
		Last Modified: Thu, 07 Sep 2023 00:49:00 GMT  
		Size: 50.5 MB (50534548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b76d6a16699dd100cc2549b60405a4d0d78dc30f81cc263bee0da056e922a5`  
		Last Modified: Thu, 07 Sep 2023 05:42:45 GMT  
		Size: 20.8 MB (20840661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc12640afdfa7cf01b8781ab7883502fe26134031f798e3a1391eb3c53ff9125`  
		Last Modified: Thu, 07 Sep 2023 05:43:08 GMT  
		Size: 66.5 MB (66496032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5bdc306c93ecc02bc8f68764ecfdd187f44bc6070663218e06d088087161eab`  
		Last Modified: Thu, 07 Sep 2023 05:43:58 GMT  
		Size: 229.4 MB (229379994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:37482b1d331a254d7171d495ed9c44bef186c96a2b866d4ebaed827281f00fde
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343128595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc581fa28d162e14edb423bdfb9a50d2d6d9848c593e5cccca8d3ddbe54fbc9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 07 Sep 2023 01:15:52 GMT
ADD file:83fc4a798915040b0cd8aee9a3ff972cb051d033b36a5b578933e29e1b55dc9a in / 
# Thu, 07 Sep 2023 01:15:58 GMT
CMD ["bash"]
# Thu, 07 Sep 2023 04:11:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:13:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 07 Sep 2023 04:19:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2b910e4082f491e2e9e9e85a065d99a76c730b5911893631d48aebe5740c1e71`  
		Last Modified: Thu, 07 Sep 2023 01:27:12 GMT  
		Size: 49.4 MB (49357507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f9d654b3c49c164cc43a4683b85bf2e1374ecf02ddb2c3f7187cfd204ec3309`  
		Last Modified: Thu, 07 Sep 2023 04:30:10 GMT  
		Size: 19.6 MB (19559687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8decd0a052b38d92ca1b1753f6ddbe6c1df433473ed31f5705fe4bb91479355`  
		Last Modified: Thu, 07 Sep 2023 04:31:01 GMT  
		Size: 63.6 MB (63632011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7253faa6a584f3038d8c0ba13b36cce92c4856df173cea2e353941235ec3ef`  
		Last Modified: Thu, 07 Sep 2023 04:33:17 GMT  
		Size: 210.6 MB (210579390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:e6999439896c3ab211b8f939a13744bd8fedd747cd191b15228fdf1488cac91d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **383.2 MB (383151466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8894e52ab10e1f0aaa007b9583c5a21c7140f3d0910e5c44a5e459d9930d73a9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 08:47:34 GMT
ADD file:67c6bc6190a4808adcfff4395e6c56581b3752c48d672a8e0f2219a636f2a300 in / 
# Wed, 20 Sep 2023 08:47:36 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 10:10:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:11:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 10:18:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a9a74cf8b7ffbe83932cf1e965d34b5885f2faaf418add2de59cab2819786fdd`  
		Last Modified: Wed, 20 Sep 2023 08:54:05 GMT  
		Size: 53.4 MB (53395271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c71db45c4ad54904bb2bce74d8d742f2d8dbdd2d22c4dfa8a8f5fc93560b7`  
		Last Modified: Wed, 20 Sep 2023 10:25:35 GMT  
		Size: 21.6 MB (21603073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7335db3fce1eb0b4617264ad0d31360a888034f9609729b7030179a1f1377309`  
		Last Modified: Wed, 20 Sep 2023 10:26:02 GMT  
		Size: 70.1 MB (70147190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3b68ebebf94bc53bce695102b219358a1e223b8fde7ad642d7183c00bcdedf`  
		Last Modified: Wed, 20 Sep 2023 10:27:06 GMT  
		Size: 238.0 MB (238005932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:53378fe23f1ede320d9ad15981dea6500e2dd4eabdb227ad0c9416881c8a0940
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.4 MB (342405728 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ede672e2c43305b3e0274dd97b8401f9473ae542c2449c50b036a9255beab1c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 02:57:24 GMT
ADD file:77b51e0abb2ed786e762b44ab5463930ac60fc37a4a4404ee62cf4653a99e1fa in / 
# Wed, 20 Sep 2023 02:57:28 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 09:54:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:55:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 09:56:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dcfbcf60cde4d1764ae5735832195c5a57365459959cebb93c0e57bd40fd54a4`  
		Last Modified: Wed, 20 Sep 2023 03:02:19 GMT  
		Size: 48.8 MB (48760791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b239420005ab6c651870ef013ed3c379e88028e2ae4355642040198cb4a863c6`  
		Last Modified: Wed, 20 Sep 2023 10:01:14 GMT  
		Size: 20.0 MB (20005597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:724dc0240d930e9ebf4eb3a0070c3eb553d06a44798e05283cc1cd48b73a5b82`  
		Last Modified: Wed, 20 Sep 2023 10:01:29 GMT  
		Size: 64.3 MB (64286239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93256ebbfd1df8e4641400040bcfb8607350dbe3e66591092348a73248ad4c32`  
		Last Modified: Wed, 20 Sep 2023 10:02:00 GMT  
		Size: 209.4 MB (209353101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
