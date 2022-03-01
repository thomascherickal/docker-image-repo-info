## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:5522a7dedf8354d5c3ac2c560de20ab24050272e398b5dee2d02c7f71ca1fb0b
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
$ docker pull buildpack-deps@sha256:e1bdfb7b1ef283972d3445e885a1e09a59e7161837dd49b26057b8f109595ae2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.2 MB (332187006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c234031eecdd72a069f263966d0ff59c6aca4d2e810a780b94cbe15cdf70cb72`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:12:48 GMT
ADD file:ba00d13bcd1098159b17d28658733d14360751081a0ff0ae5e599ea2b24d8bfb in / 
# Tue, 01 Mar 2022 02:12:49 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 06:24:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:24:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 06:24:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 06:25:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4e0d8da139e3fe03100d4937bc5abe5a82000a26ba213987f21c101384e663b3`  
		Last Modified: Tue, 01 Mar 2022 02:18:16 GMT  
		Size: 55.8 MB (55764122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d860ac80d90a3973e603f905ad5187aa30b4c4bc1166661080e7b5d70eb9b7`  
		Last Modified: Tue, 01 Mar 2022 06:34:57 GMT  
		Size: 5.3 MB (5275155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439be32a1f7086d86d5df8e4bc94c4e6afe93efcf848747f2a0414cf45ba26e2`  
		Last Modified: Tue, 01 Mar 2022 06:34:58 GMT  
		Size: 10.9 MB (10915420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d55bfedab5c66617cbef5e27ef99e597f5fa0d602ff494db70a20d8d483d24ec`  
		Last Modified: Tue, 01 Mar 2022 06:35:17 GMT  
		Size: 57.0 MB (56975332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9894d63f2dcbb3d2642ed6d129d3ab8cf3b31f2ef0bfb75c2bfcfab98707c26c`  
		Last Modified: Tue, 01 Mar 2022 06:36:01 GMT  
		Size: 203.3 MB (203256977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:f60147abdd7df4b130c24264396a0c44cab96b0dd593bd5e89958e2be00796d3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.2 MB (303166590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab52e75a6a450afab9a24c0a84da2af5322d01454c966ffd4012d1ab53dee1a8`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:15 GMT
ADD file:1c7800709331eb899ffb3adab213dd035f158fbb5682366917ca9b29bca0df53 in / 
# Tue, 01 Mar 2022 02:01:15 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 02:56:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 02:57:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 02:58:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:00:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:73894112358cdc16a19d6f8dc64e5d28dbe24c82ac6079e97e3750913f71a9bd`  
		Last Modified: Tue, 01 Mar 2022 02:16:26 GMT  
		Size: 53.2 MB (53159389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85671ba5fc3ddadb093aa6d64a5f20d876e7de8441908798eb76d8ae77670100`  
		Last Modified: Tue, 01 Mar 2022 03:21:22 GMT  
		Size: 5.2 MB (5174924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f1d9a4597c4c1fcff57e018f1450613480d9459062fbda983eb61aacf9903cc`  
		Last Modified: Tue, 01 Mar 2022 03:21:24 GMT  
		Size: 10.6 MB (10582879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5236207ccfaed595b8a0b1f8a30a1a773ffa5152b875797d1784012fe3214b79`  
		Last Modified: Tue, 01 Mar 2022 03:22:15 GMT  
		Size: 54.6 MB (54604486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edea6003139fe9d9f51047a5a0e6fffac65952fcc583d307eccc7ec00ec33e3`  
		Last Modified: Tue, 01 Mar 2022 03:24:15 GMT  
		Size: 179.6 MB (179644912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44f3ca55306b3d178f89e0ae8641bc58ef590df3f3392663e3669d39764460b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289522761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb89fd5d09eb00693e09506e6ff4535cf3a21f9a87730b7aab058358150d601`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:29 GMT
ADD file:0d5c36134a34929922dcd5c83256b9539a94c46d5b7dcd23ae6cc29721bdc320 in / 
# Wed, 26 Jan 2022 01:40:30 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:34:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:37:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9276ec53f1a5aac51c0a8a27bcc855b50a696f144903a4c1dfab1a458f7f7af0`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 50.7 MB (50662778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faba8178fd562af6ed1b6193d73a2eefb5dbc9bc34e5e155d0b644f8d23281a`  
		Last Modified: Wed, 26 Jan 2022 17:00:54 GMT  
		Size: 5.0 MB (5040739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de84da60e6b5c715dc34fc6124ae223b3288b8777242a15fdfb7dd0d91a9261`  
		Last Modified: Wed, 26 Jan 2022 17:00:56 GMT  
		Size: 10.2 MB (10241353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3548f7f03a19175e426fc70dd9fcd2f355f5cc861cbc242716094aa8d3f704d9`  
		Last Modified: Wed, 26 Jan 2022 17:01:39 GMT  
		Size: 52.3 MB (52310560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1221c786b8cfe9790ffbade36b9404f126bd6b960189d8575269b65fa75acda1`  
		Last Modified: Wed, 26 Jan 2022 17:03:27 GMT  
		Size: 171.3 MB (171267331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dfa15397131918f58fb56169119ba855bd22dfbc6c9c748232dc17e0555daf8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324052315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bce7649115aa58126549651592c9456887e3b5fe653bf61005d9968e25d7361`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:585d9a04ed59d36d1ee8be3ad5a7a488962b12f0b7d737826e25a7ab617521fe in / 
# Wed, 26 Jan 2022 01:41:53 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f9f8cc8e22fa2c53a109b770bcaab20fb907dd9957eb312d9f49000ff4185f8c`  
		Last Modified: Wed, 26 Jan 2022 01:47:52 GMT  
		Size: 54.5 MB (54535243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8a0926c8b86f048958ba5be5355985e20305f2a6df3fd52b867ac3cfcb7ee`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 5.3 MB (5269783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7042a90d872d1ef29a580051968c7437ef7f8f185841fa2ddf3e7bf37bb0593`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 10.7 MB (10676573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7233b23063ef3fe482c0973a9442a36485028dadbd3cb2d8bf3bb8269274f7`  
		Last Modified: Wed, 26 Jan 2022 02:22:58 GMT  
		Size: 56.8 MB (56825175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eeab825e0d90da9cc97a2f862aaa656e6795a97aace95a5c083be0e8e3fec5`  
		Last Modified: Wed, 26 Jan 2022 02:23:35 GMT  
		Size: 196.7 MB (196745541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2a148537ee74a0833c7a74556b6aa468858213de93497f17740debc1b8c86dab
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **335.6 MB (335605243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d83222059d3e7d2dc975d0b07c14bc99d3b0e1acad226e01ff2cd04b8756071d`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:06:44 GMT
ADD file:2e2ec9677737b8bd29e3af438e4f72a00e4024d7771df47c835bc532f3955901 in / 
# Tue, 01 Mar 2022 02:06:44 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 05:39:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:39:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 05:39:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 05:40:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:86f9569b4496bcb71f9a06eca983db008f228f89df9115b51deb7ba67bce86ba`  
		Last Modified: Tue, 01 Mar 2022 02:14:26 GMT  
		Size: 56.8 MB (56800248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc642b9c58ccfd6d24ba39de754790979cb5f4259049a1024063ce9ecd8048b3`  
		Last Modified: Tue, 01 Mar 2022 05:50:18 GMT  
		Size: 5.4 MB (5407350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a03eabfe59d42c8a3ee934b6d80db7f1185e56951d5ec5a9561133731b6ff2d`  
		Last Modified: Tue, 01 Mar 2022 05:50:19 GMT  
		Size: 11.3 MB (11307416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf25e617660ac5db1f4151bbb260abc3f5330b37a67e7d43f48b6f5966bbb024`  
		Last Modified: Tue, 01 Mar 2022 05:50:45 GMT  
		Size: 58.4 MB (58393620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76570adf4796e6a45c9f30952a2243bd7ff6a21a66e4b0950f9434ad5b02150f`  
		Last Modified: Tue, 01 Mar 2022 05:51:41 GMT  
		Size: 203.7 MB (203696609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:055adb463397355ab524867765537a61d3338809ee2528a5bbe76f5e2d287253
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.9 MB (312929677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63f354c4cfa4c4510d2efac12e774d3bf4f200ba2861f5ffb9486e200c2094ef`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:16 GMT
ADD file:205e6fa10b349b94cd09f9ab81d41ac5b9cc551f15798915ab0db37a758e13ed in / 
# Tue, 01 Mar 2022 02:01:16 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 02:57:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 02:58:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 02:59:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f016bfd811ef5b25e78858421fa083872f3db557018c6de8e9e19a3db5d69e73`  
		Last Modified: Tue, 01 Mar 2022 02:10:17 GMT  
		Size: 54.4 MB (54412288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1db773d06493b0e4fe3289f2a2bab8a332145545a6d356ae31f7c1daeda745`  
		Last Modified: Tue, 01 Mar 2022 03:18:13 GMT  
		Size: 5.2 MB (5232019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f55060d22611a46bff620b26ad27b1ccccea40ec3d18f5f2fb5712efa15c5b9d`  
		Last Modified: Tue, 01 Mar 2022 03:18:15 GMT  
		Size: 10.9 MB (10874821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95190bbea2f5622f90e93b782a17ea09bf555524c1063b8108ca896c2dbd1b8a`  
		Last Modified: Tue, 01 Mar 2022 03:19:01 GMT  
		Size: 55.8 MB (55783298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d57a0a2810b75bdd63fac199f873c7c02629ee17b47387d0c94dcb85e250896`  
		Last Modified: Tue, 01 Mar 2022 03:21:03 GMT  
		Size: 186.6 MB (186627251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d26c277e578ae70fc07da169bd2c9f7bc0fb3ba463b80694c4b12c54d0d6997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.5 MB (341483154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7951d8e301c4c859d6e551c802f3a6566c70ea7b8b877f4d6d3ea4a0908b4443`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:815d918aa7e03d3a0e2d0dd87d7d9696feb37b5054d103e1ac83847b08e877a2 in / 
# Wed, 26 Jan 2022 01:45:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:35:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fe2b17ea8278b5a905731f1d003664a61c7774f4a23cda61a596487a1b51210`  
		Last Modified: Wed, 26 Jan 2022 01:54:29 GMT  
		Size: 59.9 MB (59942176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4cbdc2b57b1d5abc56a5ce2448279d438e672ad3740a30808c6aca777b1ba7`  
		Last Modified: Wed, 26 Jan 2022 03:13:11 GMT  
		Size: 5.5 MB (5544663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46175642455b8055d9ddc0cbcac8518413ed6ae29f42a87871058a9c7df76e08`  
		Last Modified: Wed, 26 Jan 2022 03:13:14 GMT  
		Size: 11.7 MB (11693166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2209b60fdeff528905267562368c5bb713edc81a5b929e3c31387a9f3cb62a6`  
		Last Modified: Wed, 26 Jan 2022 03:14:10 GMT  
		Size: 61.5 MB (61468948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeffa132ae31c5417aeefeaef389fe0141f2bac5bfb078135b40dc4ee438b7`  
		Last Modified: Wed, 26 Jan 2022 03:16:09 GMT  
		Size: 202.8 MB (202834201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5ed5db6953401c7e699848b7694ee5f369308c3e2b4b6e72f6f5ec3bab7badc5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.5 MB (304469056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f7b1cea4d98d05e3a0be9e16f118b90fd9d51e75bb6086f7108175fc48d3d46`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 01 Mar 2022 02:01:03 GMT
ADD file:97ccc226b81c90fe178edd1d68832f3a504aa1ef983753f12fed36e4fa09c796 in / 
# Tue, 01 Mar 2022 02:01:10 GMT
CMD ["bash"]
# Tue, 01 Mar 2022 03:49:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:49:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 01 Mar 2022 03:50:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Mar 2022 03:51:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d7c29f1e9903c84021327567eb513269c7f0b92b6f050037783556a33deac133`  
		Last Modified: Tue, 01 Mar 2022 02:06:47 GMT  
		Size: 54.0 MB (54007195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed9e936b2203a39badf459e13626bb8073e325e33067ce97b014c0f2564b7be`  
		Last Modified: Tue, 01 Mar 2022 03:59:12 GMT  
		Size: 5.3 MB (5256848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b370eba2faadba4103ab569fe90fa51ac4c8f6634d504e481540d47ad92f7`  
		Last Modified: Tue, 01 Mar 2022 03:59:12 GMT  
		Size: 10.8 MB (10807240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d45193a064820414c9ad891c79c41aeec7b351b45dfe7bb4c3631e05a9b1ca1`  
		Last Modified: Tue, 01 Mar 2022 03:59:26 GMT  
		Size: 56.4 MB (56362036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71a8a91b0ea5860e608ef124f417b70e0f75853ad98e50b7d871c8b387be12`  
		Last Modified: Tue, 01 Mar 2022 03:59:51 GMT  
		Size: 178.0 MB (178035737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
