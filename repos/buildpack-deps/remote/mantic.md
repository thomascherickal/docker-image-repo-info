## `buildpack-deps:mantic`

```console
$ docker pull buildpack-deps@sha256:bda82b5ce4abbfcca5aa613c7b4eefa7244fdaa78274a1257ce3fed7c7b468aa
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
$ docker pull buildpack-deps@sha256:e1640709591c9d9e0038347965dec617f717cceec03895d42666cfbaea33545c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.8 MB (279758764 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bfef5d2082eaa961e2d3cefef8e67a7d13c9269c329297040dd1ca2d2360b92f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:54:17 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:54:17 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:54:17 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:54:19 GMT
ADD file:5430e0b4ea856c760b6e2b88e8c2cd2d49704ed2f3c53ae34c10750a608d40ec in / 
# Thu, 30 Nov 2023 17:54:19 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:21:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:22:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:26:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cb8122a41e708f03d563c8ba7400f85d27af325fae5fbf4e00380a11f4ca1fa9`  
		Last Modified: Sat, 02 Dec 2023 02:22:28 GMT  
		Size: 28.1 MB (28070890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3950b4737b0d86b7d5a2758a2148e06120a5a73d9f1593fe22ad1a7c8e83a83`  
		Last Modified: Sat, 02 Dec 2023 04:30:04 GMT  
		Size: 9.9 MB (9907996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760243c1a983844f069a293b501cd9301cbd819c4fb9551cc389ff6e1e7cb238`  
		Last Modified: Sat, 02 Dec 2023 04:30:20 GMT  
		Size: 44.8 MB (44753276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8938a8634af1b782bcdc4d1714f961d7e4beb6bf923b888e9ff9db9a53165adf`  
		Last Modified: Sat, 02 Dec 2023 04:30:54 GMT  
		Size: 197.0 MB (197026602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9b6a8197e03c16a5e5c64bfe05fb54494947096f94b9d8aac266320b571278e8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.7 MB (246704690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eb114e88bdc70517c782d36daab42fa65b90488add07631546f47e8c48d2b46`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:34 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:34 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:34 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:36 GMT
ADD file:f2094c969cf67a5474ae23a10eed122a6aa80b1fe7f01fda1a770b8fa11f8a98 in / 
# Thu, 30 Nov 2023 17:41:37 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:44:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:46:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2a01529681dd04180ded851c403d6b511fd3cdbb968992acde066a32e0e7c6c8`  
		Last Modified: Sat, 02 Dec 2023 06:51:25 GMT  
		Size: 26.0 MB (26021484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90ae82e93d9fd7e2e58d6f4fbe50295346193ea460ba3e6b8be58dae105da215`  
		Last Modified: Sat, 02 Dec 2023 06:51:23 GMT  
		Size: 9.1 MB (9145862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e3624564a762546bdc52895b1c66bc1408260d1efaa2e2b2b765adadd9c8f8`  
		Last Modified: Sat, 02 Dec 2023 06:51:41 GMT  
		Size: 48.9 MB (48942472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19aeb74102316977bd7618d2394b9a9b8f7871ce0db4fa7f72ff72287befbde4`  
		Last Modified: Sat, 02 Dec 2023 06:52:11 GMT  
		Size: 162.6 MB (162594872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d62de9add5227d3e50479035c3a5c90546bf4eb61de363dc77bbf7c5630518a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **271.8 MB (271776124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6002b7cadfd93e9864d95610be91fd2b4e31e9530491ec54797bf44df2f7a49f`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:41:07 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:41:07 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:41:07 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:41:09 GMT
ADD file:973e000ef2f95dfa48695815ebd7027db718c9fe80260271e43ee06fddfd073b in / 
# Thu, 30 Nov 2023 17:41:09 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 05:22:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:23:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 05:25:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a1727374770547196a050f3f410bce47450929c3bd7b9e1e44530bd290614b70`  
		Last Modified: Sat, 02 Dec 2023 05:29:22 GMT  
		Size: 27.4 MB (27354913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95613e6e791d7d51806e9f81060d333d4ec85becf758d4921c664403daff14f2`  
		Last Modified: Sat, 02 Dec 2023 05:29:19 GMT  
		Size: 9.6 MB (9646950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3c268c4f8b402b3f9907fba74a035e04caa79bd82292e937192630e4a7e64e`  
		Last Modified: Sat, 02 Dec 2023 05:29:35 GMT  
		Size: 44.7 MB (44665066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282eba19e4b5f40a7947b90ee497e8544dd23f1b54758d9068e3352ce8847e32`  
		Last Modified: Sat, 02 Dec 2023 05:30:03 GMT  
		Size: 190.1 MB (190109195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:4d837a54ed79c3697e81fe74410d427abcc9ebfde406fe98a1aed32710212ac1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.6 MB (293583524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dbf6c27960d11c3cacd25fa84f3c4a28ccd7e42d8b3b888bdbff7212085aed7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:57:33 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:57:33 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:57:33 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:57:34 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:57:37 GMT
ADD file:d08e45288fbc31570a3a92ae480bf6ac3ed8e4900b3260d56a51ce024818b6fe in / 
# Thu, 30 Nov 2023 17:57:37 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 04:40:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:41:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 04:46:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e6a2519a5ea0f832b2e35477f84cb47f263c19385218548bfd1ef20a7b0ef71`  
		Last Modified: Sat, 02 Dec 2023 04:51:30 GMT  
		Size: 32.3 MB (32337524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78920d0cdc2c45a2f364052f0f3ae1ca5ad03f12e0ca0ede2059df652d0396b`  
		Last Modified: Sat, 02 Dec 2023 04:51:26 GMT  
		Size: 11.6 MB (11574817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c14fb2f649d6e1f2a6ecdb5517e059449e766f72791aa8c47aa868b20d52f1`  
		Last Modified: Sat, 02 Dec 2023 04:51:47 GMT  
		Size: 49.5 MB (49544508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7b8396201f82cfdb61aa43db57c73838c2ee3354bbba5efa522ec63f8a82ed`  
		Last Modified: Sat, 02 Dec 2023 04:52:25 GMT  
		Size: 200.1 MB (200126675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:mantic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:eabf406ea7248077acda817b048130604c4d31ca60b0de1626699a3e2eb097cf
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.6 MB (257648877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b6ba5eec539c6ac927968b4411466cd495be79e29749d9cdb335895cc3fcab7`
-	Default Command: `["\/bin\/bash"]`

```dockerfile
# Thu, 30 Nov 2023 17:42:50 GMT
ARG RELEASE
# Thu, 30 Nov 2023 17:42:50 GMT
ARG LAUNCHPAD_BUILD_ARCH
# Thu, 30 Nov 2023 17:42:50 GMT
LABEL org.opencontainers.image.ref.name=ubuntu
# Thu, 30 Nov 2023 17:42:51 GMT
LABEL org.opencontainers.image.version=23.10
# Thu, 30 Nov 2023 17:42:53 GMT
ADD file:63283c7c5d335fa063fe3da82fa78d45ed5af9327a2d154bad18a8711485db77 in / 
# Thu, 30 Nov 2023 17:42:53 GMT
CMD ["/bin/bash"]
# Sat, 02 Dec 2023 06:09:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:09:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Dec 2023 06:12:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:93c83e99bb380c6b7ce7bb2c3847727b3387d6638d0e59e8c1b2eeddbd82ecac`  
		Last Modified: Sat, 02 Dec 2023 06:15:43 GMT  
		Size: 27.6 MB (27643359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3461f23023b426766431d5f005571cba59c114d2e78379817dd2d4cfbf813a`  
		Last Modified: Sat, 02 Dec 2023 06:15:40 GMT  
		Size: 9.7 MB (9697312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5727db7a5897b08af6f62472ddfb225235a5740723521606d98d708b40b5b5c`  
		Last Modified: Sat, 02 Dec 2023 06:15:55 GMT  
		Size: 45.2 MB (45237357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:924da814eb1bd8f1adf34e963bb6011fa2589858be016a1a9960442bf68fcc2f`  
		Last Modified: Sat, 02 Dec 2023 06:16:22 GMT  
		Size: 175.1 MB (175070849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
