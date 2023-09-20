## `buildpack-deps:trixie`

```console
$ docker pull buildpack-deps@sha256:ff2047d9bc7bcc830c42a761f7840425e2d7af5cc33deeb425cadf327871d9b1
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
$ docker pull buildpack-deps@sha256:4c045dc4f0a40ef7ea8aa643d85295c297dae4a7e62109ad9f9646ca46b7e814
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321887047 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:334991229eb00270da6c788fd956080cef3f7293ac3606209e71a1bd04874714`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 04:59:32 GMT
ADD file:48b3882ac99c385930d3ac71ac20fda8a1b071b08088814bf1a41054078ecd14 in / 
# Wed, 20 Sep 2023 04:59:32 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 15:32:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:33:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 15:34:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:219658aab374640dcbab3bd1cbe574955f68e4305522bfc19564d1ce15fed88d`  
		Last Modified: Wed, 20 Sep 2023 05:05:38 GMT  
		Size: 45.0 MB (44955127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e0f2039e0f302927a38df2eb35fc70587db403fbc14273b4fe098c21cb0969`  
		Last Modified: Wed, 20 Sep 2023 15:39:33 GMT  
		Size: 18.6 MB (18617697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba45c0e5519ac44055eac6898a4c8abe790e1be149095e9a8db5eaf719de3e2`  
		Last Modified: Wed, 20 Sep 2023 15:39:51 GMT  
		Size: 59.9 MB (59891965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b18f2abd66df756bc6a06d8b163ff75670f87a21b572f5fde1dca495dc25c9`  
		Last Modified: Wed, 20 Sep 2023 15:40:30 GMT  
		Size: 198.4 MB (198422258 bytes)  
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
$ docker pull buildpack-deps@sha256:710e32d02fc24ce4b0361576e781bc8e93e2f8869d9750a5fc626fb1b7534087
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **376.3 MB (376298473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c80d2e0f89be4e199ccec82d70165f50968010af18572d91ac1111e35bfed0e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 00:44:37 GMT
ADD file:9e992ca17751b113240a189433e8f77647c4ebe62d129da1b528a8d6a3702972 in / 
# Wed, 20 Sep 2023 00:44:38 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 11:34:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:34:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 11:36:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd505a05e9a1d549793b6c0278e192920932cc3051d24604cbaee75803a68342`  
		Last Modified: Wed, 20 Sep 2023 00:51:58 GMT  
		Size: 50.5 MB (50484788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37cc9ae28e9bda901dc51164cf94a986ae909c659e90d0c25cd8875aa954d2de`  
		Last Modified: Wed, 20 Sep 2023 11:42:34 GMT  
		Size: 20.9 MB (20853303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:918107427c2cb228f04a420f2253a41cf0b3eb4b65b3ba84caf3838923d4cd15`  
		Last Modified: Wed, 20 Sep 2023 11:42:57 GMT  
		Size: 66.5 MB (66486028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bc9f1e250fb0c7ce8f75dce7d9ffa31e885eb42d90bc230ec4885735804ed44`  
		Last Modified: Wed, 20 Sep 2023 11:43:50 GMT  
		Size: 238.5 MB (238474354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:trixie` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dca0a86138fbc50e65519ae1cb8864e2c188c758bcf38f11e36636b7656d341d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **347.9 MB (347936742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54fde2b02e81071bbe4ec5cae65d324e798d69935ed9fad301e0b1ace2d656be`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Sep 2023 03:16:43 GMT
ADD file:feafc03e82af46c6c55a0a73cf1d1107968b6694a898de04dbd04b90bd98508d in / 
# Wed, 20 Sep 2023 03:16:48 GMT
CMD ["bash"]
# Wed, 20 Sep 2023 22:12:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:13:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Sep 2023 22:19:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0c3624a744ac0024156b087e27ec700730d5abd850c903edaefd0cd35bb20d02`  
		Last Modified: Wed, 20 Sep 2023 03:28:01 GMT  
		Size: 49.3 MB (49302317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee833587bbee7c28ebb44ce27cbd72e6bb33739d9203cf1e4464b7ae564d8c1`  
		Last Modified: Wed, 20 Sep 2023 22:30:41 GMT  
		Size: 19.6 MB (19560312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8fb39bb7824bc4241044104821fb808dc3b6465ce10625a02aee85775a106d`  
		Last Modified: Wed, 20 Sep 2023 22:31:30 GMT  
		Size: 63.6 MB (63606238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5964edc07d833070936e9b5e5c05b3f5b96bb59c525d17412a61cdb6a1f393`  
		Last Modified: Wed, 20 Sep 2023 22:33:49 GMT  
		Size: 215.5 MB (215467875 bytes)  
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
