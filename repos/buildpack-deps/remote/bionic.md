## `buildpack-deps:bionic`

```console
$ docker pull buildpack-deps@sha256:ba35ef55ff884cbc728dab8711d0fc4eec24c450dcf838bc2d2893208364726a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bionic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:182300ddfbd837dca054e673d02871f5b41c0e6cc4a3192c79d3106258664705
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.3 MB (221277614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38c3a7e0952ad516a0716695b4d358959f1b246f884c7fc6fa01d0c5bffb0d86`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:04 GMT
ADD file:40290d9a94ae76c35ab1f57178130ce1c5b976e34a91e77472ecf7e945ab64f9 in / 
# Mon, 06 Jun 2022 22:21:05 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:03:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:04:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:07:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:09db6f815738b9c8f25420c47e093f89abaabaa653f9678587b57e8f4400b5ff`  
		Last Modified: Wed, 01 Jun 2022 21:51:21 GMT  
		Size: 26.7 MB (26711626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d3b7a8084f0f50ac1b09fe5b075dd39627cf2d5bf67659da7c41138cda7b67`  
		Last Modified: Tue, 07 Jun 2022 02:23:53 GMT  
		Size: 6.6 MB (6644325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd97ebd2067d1a4bead88f69c0cdcc55b5a30fce0416079338359fc29d2bb4a8`  
		Last Modified: Tue, 07 Jun 2022 02:23:52 GMT  
		Size: 3.0 MB (3026631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41735452950ad5e0d9fa366c8a9bffb525845e2594e2a650de86b24b125d7dae`  
		Last Modified: Tue, 07 Jun 2022 02:24:10 GMT  
		Size: 45.5 MB (45489985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e8acd3998c8b9238900cdcf4a4d1ca85be8d2060a00747f2ff12bd909569918`  
		Last Modified: Tue, 07 Jun 2022 02:24:39 GMT  
		Size: 139.4 MB (139405047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dc239add12cc13f43e05709d8c65d05ae78aeffd30279f2aa91be0173f35b386
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **189.5 MB (189490310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c839f29d4b7ee613f2ae6e56a3ee7c097aa7d5c2643aac3ffc2218efeca2a826`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:50:28 GMT
ADD file:d6d276f8f40c095bc2411f4d370eb87f8042a092ebb5bb0076863b2b6182b34f in / 
# Tue, 07 Jun 2022 05:50:29 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 08:54:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:54:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 08:55:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 08:57:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9242055bc3f039f3566a5154c8b1a602652bfe444e9b4291817caae906444e75`  
		Last Modified: Tue, 07 Jun 2022 05:54:37 GMT  
		Size: 22.3 MB (22306284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b9e0fc77e018e0629159e8465b477b65e58a477dd79b5c9657adde06acd2624`  
		Last Modified: Tue, 07 Jun 2022 09:19:05 GMT  
		Size: 5.7 MB (5715279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cfde4df52faba0aeefc79d4a9a00fcd3d09382a20655a600fa7626de41c4f7`  
		Last Modified: Tue, 07 Jun 2022 09:19:02 GMT  
		Size: 2.6 MB (2589202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97798877efcd9155df278ef0f5408f8312d407daa2a0531de6412d63d2e9d638`  
		Last Modified: Tue, 07 Jun 2022 09:19:44 GMT  
		Size: 40.7 MB (40687652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed0b3205febfa1e61d36176ecb772943d1326e060afde45f7e82d409ad433c87`  
		Last Modified: Tue, 07 Jun 2022 09:21:08 GMT  
		Size: 118.2 MB (118191893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:c08775bf7c9fc784b445ae45ecd86203e66933876314a06ea12a5c21e818d9d9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.4 MB (205396680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e26b57947dde922544885b45b01139b6c8a4497e6eff9590e64824703f8f7b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:07 GMT
ADD file:c562239bf6872889a22d15dda4c7dab53664b0697b60b9d09ba352b7c66719ce in / 
# Tue, 07 Jun 2022 01:25:08 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:43:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:43:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 04:43:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:44:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8376114ff9b387126c379fb7f6f90b3752e3082ce48b0c727c0e1b683e1244da`  
		Last Modified: Thu, 02 Jun 2022 08:34:27 GMT  
		Size: 23.7 MB (23734664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89616c81f795aeebdc336526b5d6120f4952baddbda6e27e6d138749bb23cc6`  
		Last Modified: Tue, 07 Jun 2022 04:53:59 GMT  
		Size: 6.1 MB (6083855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459cfb9478ba071444e39cdf4d9428c854e2438ae482b10dbea4dadee121c4b6`  
		Last Modified: Tue, 07 Jun 2022 04:53:59 GMT  
		Size: 2.6 MB (2573803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb10e7f64cb1a6c3e4dacfb15c2a96365f4faeb36c6fccc292d28f6c4df741f`  
		Last Modified: Tue, 07 Jun 2022 04:54:17 GMT  
		Size: 43.3 MB (43287767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08131cc239c6c07320ed8fbbfe4b5d5c30b8e3b8860126840efd80bce33f3107`  
		Last Modified: Tue, 07 Jun 2022 04:54:46 GMT  
		Size: 129.7 MB (129716591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; 386

```console
$ docker pull buildpack-deps@sha256:046e9db61bb416285f19648017502afb5d8aa6163704ac907f84eb71079bbee5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **218.1 MB (218143262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957464bc4955cb42948c4c39ace96be403d841eae80c7f11d91bf402038a72d6`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 21:18:54 GMT
ADD file:c1118975f50d6835777043d4b807b4fcf30db0151d1e7659e077e9e33c4ea7c7 in / 
# Mon, 06 Jun 2022 21:18:54 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 21:45:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 21:45:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jun 2022 21:46:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 21:48:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1408ae6e2634d0ef0a2f110363deef0fdf35ee2958852f9d20b92b57495a9fb7`  
		Last Modified: Mon, 06 Jun 2022 21:19:41 GMT  
		Size: 27.2 MB (27165461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9997a51874c52f806343d9609c83d010ef99ca07d34fe33a866c72416728b1`  
		Last Modified: Mon, 06 Jun 2022 21:51:19 GMT  
		Size: 6.9 MB (6931382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5698bd6c395573f235a617e94df59b4d8e7c54b59065059267f6aa81e685a7ea`  
		Last Modified: Mon, 06 Jun 2022 21:51:17 GMT  
		Size: 3.0 MB (3041855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6196e18ef02eb07ef39a9b49d2c47f9c40556ac3696ef8742efa88473ed99eca`  
		Last Modified: Mon, 06 Jun 2022 21:51:36 GMT  
		Size: 47.1 MB (47085407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523b1385bba6652b6f656fa5e2b91108b130068bad2d8d30e606a7d13af8e4f5`  
		Last Modified: Mon, 06 Jun 2022 21:52:10 GMT  
		Size: 133.9 MB (133919157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:df750ef730fcd2783242d3cffb5531228c569292ceb51a7767b26f02fe815979
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.6 MB (246568223 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408cd2f3e0d732a536cd4acd99f7649579b9c263e1231d0df316c460a3b763ea`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:45:31 GMT
ADD file:00feca269255d07b1ddb816beb48357c556d80ab79aa81bc448abc4271d845a5 in / 
# Tue, 07 Jun 2022 05:45:36 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 22:54:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 22:54:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 22:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 23:03:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:868ede65862ecf99802bf8944efd378ff1e0751772424cea9084f390deb9f9b2`  
		Last Modified: Tue, 07 Jun 2022 05:48:49 GMT  
		Size: 30.4 MB (30442859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17b26565b0d35480b1dfc4921d472a42568f0d9b39e64be90de6533774e53fd9`  
		Last Modified: Tue, 26 Jul 2022 23:53:55 GMT  
		Size: 7.1 MB (7056280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00d8045f40230dba407517829fb31be26b3dd8bc8353c97dbc491385bfce305`  
		Last Modified: Tue, 26 Jul 2022 23:53:54 GMT  
		Size: 4.0 MB (4021721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61828bfb9f7bcc74a5614301750ec2a4626ccf1418227bfcc7e0259ad8f5eaa1`  
		Last Modified: Tue, 26 Jul 2022 23:54:22 GMT  
		Size: 53.7 MB (53744463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f054456c9b4f152dda5ed337536df7d0561ff91e26b9bfd2c3741fa6bcfa95d0`  
		Last Modified: Tue, 26 Jul 2022 23:55:11 GMT  
		Size: 151.3 MB (151302900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bionic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:46cdbf3b5ae25792f036aa62dfcfa512da95c5b4ff9a02859e83ce033f0341c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **205.6 MB (205636943 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ea285ff2425c5b8742902ccfa096c86566e2ec11fce57b031b049f2a85c876d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:04:44 GMT
ADD file:e2caa30d22701eeadebe1abd66923745f75d170d7baa51a62119576c31b7f89c in / 
# Tue, 07 Jun 2022 04:04:47 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:45:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:45:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 05:46:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:47:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:048a87c6fcb9ea8de843bbbe647d14716098af0741f7f59e30c60f39b96b4397`  
		Last Modified: Tue, 07 Jun 2022 04:07:30 GMT  
		Size: 25.4 MB (25370236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daeabcd99a1d7b951343f0d1932013865edf701d725a76082d0e91a7cf9bea4f`  
		Last Modified: Tue, 07 Jun 2022 06:06:25 GMT  
		Size: 6.3 MB (6334562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9df68dac810e4f12a4ed62d3aa3fb927a412ad018af6c10348e2f7a7a2e0568`  
		Last Modified: Tue, 07 Jun 2022 06:06:24 GMT  
		Size: 3.0 MB (2980130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb907eb58cc3a0d86c0f8edca3398c7d39aaa966ebbe16fa1fb47c856e934519`  
		Last Modified: Tue, 07 Jun 2022 06:06:38 GMT  
		Size: 45.0 MB (45033854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c74a9f4b163d0b2017217afe222709e1913e0c137c59b1633e02dad11567ad6f`  
		Last Modified: Tue, 07 Jun 2022 06:07:03 GMT  
		Size: 125.9 MB (125918161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
