## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:6a6a70352134e2642d7a6a2d9739a8bff97493c7beb2c6e52ee5d2347a2837b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:kinetic` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:cc0a19e97e67f15036d5378a96c362841360a1e59c2791ffa9cb516d5d84b19d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **251.1 MB (251115277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db54a842dfeadd0fafb843607483607f5a218d73c908a50a0428dc86fd5216c3`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:33 GMT
ADD file:440048faae869c09f5819655d93c479ac0282dace791dc6077f035c8481f45b8 in / 
# Mon, 06 Jun 2022 22:21:33 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:20:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:20:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:20:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:22:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:415d72858c745ad20ae2769e6ba46966432d24b0cb79e2ebcb65280ce8248a31`  
		Last Modified: Mon, 06 Jun 2022 22:23:23 GMT  
		Size: 27.3 MB (27347519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd927167c75021e878fd8d0927d91affc71fc2a4e099b9c4fbab2d9230f68492`  
		Last Modified: Tue, 07 Jun 2022 02:28:12 GMT  
		Size: 6.8 MB (6796121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a5f9c7747d58c8108a20268f5d5b0603de8d390dfcb3d66f0bb462ed4757290`  
		Last Modified: Tue, 07 Jun 2022 02:28:12 GMT  
		Size: 3.6 MB (3565227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04747b6263a57bc12429b7c92af3b57c8ae582309a19f04352c61a18dfe62bfa`  
		Last Modified: Tue, 07 Jun 2022 02:28:28 GMT  
		Size: 39.7 MB (39676725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:154418f4afdf7449eb9cd8a21b0dd5b150a5cf28fdc5c2d509c05968e00daf4f`  
		Last Modified: Tue, 07 Jun 2022 02:29:01 GMT  
		Size: 173.7 MB (173729685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:0473d9fa4d933e5f8efde24bc335634ed50f33aaa88b2cc82c5f0ac750f41269
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.8 MB (217785460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:416e81585b4cb0cd15a4549287fdcfc7b286c489b748080d4a07eec7f7dbce97`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:52:00 GMT
ADD file:243d0f716fbef71d7d9cc76cf15c0b298f5b3460b6533ab2a8e88b0d618dc144 in / 
# Tue, 07 Jun 2022 05:52:01 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 09:09:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:10:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 09:10:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 09:12:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:88f853be8de2fbdcfad5b9be55e0f368887c6cad36efaf35cc75b81a8ecd9841`  
		Last Modified: Tue, 07 Jun 2022 05:56:37 GMT  
		Size: 24.7 MB (24676229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8309bc9e188c93b03413a75296e80a55a55d4c4cba09aa7a59044c6b2cdb680`  
		Last Modified: Tue, 07 Jun 2022 09:30:23 GMT  
		Size: 6.0 MB (5975769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc52d4a1356b55b3c78029b3cc039697533033c4bc0d17a13f479f27eb467f5c`  
		Last Modified: Tue, 07 Jun 2022 09:30:21 GMT  
		Size: 3.7 MB (3714177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e63839d7ac5bea9a287ece8da8807fc2777c0ab6f22e91064e2b2e23f9bc9a2`  
		Last Modified: Tue, 07 Jun 2022 09:31:04 GMT  
		Size: 42.2 MB (42237858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d33c06fec115a97cc09b74dba2ffb431b6ae57d7be0f277285658a37a90429`  
		Last Modified: Tue, 07 Jun 2022 09:32:38 GMT  
		Size: 141.2 MB (141181427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:12519e9a699fc78189777ff28ac940f0cd63d9826da4fccb748e24f47ba434e0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.8 MB (241842738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8644cb2b3906df0590494dda4822b463100a7aa2cf35f0fa9712579b84e6778`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:41 GMT
ADD file:436ba9358911a376f8184a243173151b7b2ef9c66c14edfcd003f07c65a22f1c in / 
# Tue, 07 Jun 2022 01:25:41 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:49:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:50:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 04:50:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:51:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:46465228a6c0c2b6f599636b0a2e73f8b6954a9be77e8b309c72783a93fcb092`  
		Last Modified: Tue, 07 Jun 2022 01:28:07 GMT  
		Size: 25.5 MB (25459707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1173afc37d77836d87cb4f01d6e5b5960d43aab0605773475fef37da1902d856`  
		Last Modified: Tue, 07 Jun 2022 04:58:28 GMT  
		Size: 6.6 MB (6625122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8db28861a6be1cb9b6df04a34d51a5f92117bf390da3935a0260bd09e93e1c`  
		Last Modified: Tue, 07 Jun 2022 04:58:27 GMT  
		Size: 3.3 MB (3324720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c30bcdd1e505f330a7f17fd74ff65634b9629d0717b77343612f914970a3d8e`  
		Last Modified: Tue, 07 Jun 2022 04:58:45 GMT  
		Size: 39.5 MB (39546321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c81bf5bf954cdad03cf314de2713b9a39606a99333ba78b8ccfc0f452d2a7cd3`  
		Last Modified: Tue, 07 Jun 2022 04:59:20 GMT  
		Size: 166.9 MB (166886868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f597545f67ab5d02c47625480f385c1770c3cfee2268aed57556a64f5b9f095a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **279.5 MB (279507381 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34dc37d9ac2fe532ec7a2a7e12a2df7622729ce555d47d97ed497b984a6594f2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 05:47:11 GMT
ADD file:94cf6534c6b66a46a13144239fd0bba4180772804f5826d12fd030c1199457bb in / 
# Tue, 07 Jun 2022 05:47:14 GMT
CMD ["bash"]
# Tue, 26 Jul 2022 23:25:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 23:26:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 26 Jul 2022 23:28:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 26 Jul 2022 23:34:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9ce8aa65c6465c42b081a5642262f289b2db6cfd58b6e49f7f2c24742205c2c`  
		Last Modified: Tue, 07 Jun 2022 05:50:20 GMT  
		Size: 32.1 MB (32131305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a03c5d4a4a30095b5986889adae05bbb0933ce7e48e115e1b7fd75ae323e8e`  
		Last Modified: Tue, 26 Jul 2022 23:58:38 GMT  
		Size: 7.8 MB (7802631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afe96d280d0e21317e7cdab167420493ea718b004c6e2a490a3e7e242cb0db32`  
		Last Modified: Tue, 26 Jul 2022 23:58:38 GMT  
		Size: 5.5 MB (5529202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f751ab6988cdaf74b065930f90fcb1067e074a2299e6a7164d90731e2f7af76`  
		Last Modified: Tue, 26 Jul 2022 23:59:03 GMT  
		Size: 46.7 MB (46652953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea83a8b43805b04fd4f427d78a1909683fbabeac649872c28f5f4b46b8bf87b`  
		Last Modified: Wed, 27 Jul 2022 00:00:00 GMT  
		Size: 187.4 MB (187391290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:e238323ff7b3b040b5312082aa60efd835a9ea19922a11da4a6f895fab8632ba
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.6 MB (275641971 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:172c759238278fcf032b2099e473befcf587fca99ec4631ff82a4e1d999974a5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:21:26 GMT
ADD file:7360bdaa4ea5ec8b4eb9b93f92717ed4fb377c6910368b3f1af3f2524989f28c in / 
# Mon, 06 Jun 2022 18:21:27 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:45:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:46:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jun 2022 19:49:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:56:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1df12f21536751a4a4297772577c4c96de0f5030dfb5243599bd956eca3d066a`  
		Last Modified: Mon, 06 Jun 2022 18:45:02 GMT  
		Size: 25.4 MB (25435182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:665f6f3ab1186a3216e891819468ac8dc7d533ab721c7be256ba7c56bcfc03dd`  
		Last Modified: Mon, 06 Jun 2022 20:38:03 GMT  
		Size: 6.0 MB (5960974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33fcae399ce23346d8006049bedfc5c045fcd5e2575d2549db9d528ed359ac49`  
		Last Modified: Mon, 06 Jun 2022 20:37:59 GMT  
		Size: 3.8 MB (3780819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7c0ccb055a215687cbefa5c726c1fae98476e4db6af3a2b75ea8eb42916d93`  
		Last Modified: Mon, 06 Jun 2022 20:40:15 GMT  
		Size: 42.5 MB (42451273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d33b8174dce129e8204b6d0ce74692a7621f86b62b699883968678687b2f82`  
		Last Modified: Mon, 06 Jun 2022 20:46:25 GMT  
		Size: 198.0 MB (198013723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:f095635ffa37ea8f89ef99026eb819b3fdafacd9035fc732078b14cb41aeecb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **224.6 MB (224612579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a51999a268a11f79fc86eb6dfee5aab5c139df71880e65fd104e1545b575155f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:06:01 GMT
ADD file:73b8105e3f6b064f2f8039d2102cfa51946b6b268f19a0e6a348fa49cd0ed2de in / 
# Tue, 07 Jun 2022 04:06:06 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 06:00:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:00:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 06:01:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 06:02:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94e4f8254e7672b5bdebe620b1922baa63fd40872238ee59c3f48a8d9485d43a`  
		Last Modified: Tue, 07 Jun 2022 04:08:31 GMT  
		Size: 25.9 MB (25857245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c529509938b721f50f025e2e2969140aa4cbdae823eb10b1c6b51389f52f11f5`  
		Last Modified: Tue, 07 Jun 2022 06:09:53 GMT  
		Size: 6.5 MB (6482918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56dacc17ee1afc9652d0228a5819da87c6f3b86fe26afe6a68c817070d114946`  
		Last Modified: Tue, 07 Jun 2022 06:09:53 GMT  
		Size: 3.5 MB (3477476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a1162af6534ac596f101dd5d13176ce140a9cffd4170f2b1c14375451708cb`  
		Last Modified: Tue, 07 Jun 2022 06:10:06 GMT  
		Size: 39.6 MB (39599799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:781f48ae56a9fe53aadc7d739902e0e99c785a4c0ef51b8beef50805ec620163`  
		Last Modified: Tue, 07 Jun 2022 06:10:32 GMT  
		Size: 149.2 MB (149195141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
