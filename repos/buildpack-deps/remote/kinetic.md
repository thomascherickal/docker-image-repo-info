## `buildpack-deps:kinetic`

```console
$ docker pull buildpack-deps@sha256:a0608bedcb444072ecafaae7504d9ab57bf7c65bef3384571e2c83ec57359d10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
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
$ docker pull buildpack-deps@sha256:c7670357ec87bcb2a9750dcf2fc0fbe3acc5c7d784c4cf54eb69f1c6cd748c8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.0 MB (221017288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa5432207211c535947ef3b0f50084b0195874c8f7212c4c241ed463e406131d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:55 GMT
ADD file:063f432f8adfa6ad56a7bb07ff90f71f00c47c30a03bd892e04ddd744042a0d3 in / 
# Fri, 29 Apr 2022 22:59:56 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:03:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:03:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:05:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1fc430d8f49d4d10815388bc3cb533e89d8123bcc10ffd2a333c16216f2e4303`  
		Last Modified: Fri, 29 Apr 2022 23:04:36 GMT  
		Size: 27.0 MB (27015929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c89783a5b9c1d5f0a22dbcdf255a84e8909a4e61a4eac70b41381b61121e2a38`  
		Last Modified: Wed, 18 May 2022 18:12:46 GMT  
		Size: 5.6 MB (5625692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253307b1acbd5f7f7e968c3da0fb29b31baa5f85c808566b01a3db407d77e1bf`  
		Last Modified: Wed, 18 May 2022 18:12:44 GMT  
		Size: 3.7 MB (3715955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d88d2a61ec5acd97d4faf8d5a7b2d44ae9bd535a9de00e899f87884d2c063d7`  
		Last Modified: Wed, 18 May 2022 18:13:27 GMT  
		Size: 41.9 MB (41896307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9857334dde1134110030c385fee86258aefe2d67020902f1de8a9f6ef0f820`  
		Last Modified: Wed, 18 May 2022 18:15:02 GMT  
		Size: 142.8 MB (142763405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:kinetic` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:042f3eb89cb0660bbb3871a7c60b889c0fcef8e37bab7700ce4233fe1bac4c6f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **245.7 MB (245725882 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:559f553e596b1bf0f7b7959de800eb9282495e44b33bdbe70b7b137fa8d7c842`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:02 GMT
ADD file:1dcfa00d31cec211ba91522ed6fcf6f72e3f1f4ad30c4f7ca398add7eba377c0 in / 
# Fri, 29 Apr 2022 22:50:03 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:41:44 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:41:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:42:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:43:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:957fa4daed10cc16359daab2a50b5ffbbc1d762035c4eba567b3d4205e7afbde`  
		Last Modified: Fri, 29 Apr 2022 22:52:30 GMT  
		Size: 28.4 MB (28376165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecf88994911b3123256118b9bd96f3264984301fdeab08165451ae9e6a702ef`  
		Last Modified: Wed, 18 May 2022 18:46:03 GMT  
		Size: 6.2 MB (6200595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d271b6a5485276e4f0ae87970e4f3c9559a1dd51586b0c37d3a98260fae490b3`  
		Last Modified: Wed, 18 May 2022 18:46:03 GMT  
		Size: 3.3 MB (3326759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9d6cf5bae98dba51fa83bfb0f6271fa75c7bd5b07e76434b1612cd7004ba2a`  
		Last Modified: Wed, 18 May 2022 18:46:21 GMT  
		Size: 39.2 MB (39242714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b24717fdc92b09bfb3f6a6447619030376dff0f1b563d993e1ecefd5fab6280`  
		Last Modified: Wed, 18 May 2022 18:46:54 GMT  
		Size: 168.6 MB (168579649 bytes)  
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
$ docker pull buildpack-deps@sha256:3c1123a994b3153d147f891c1e080edf1e05711a04404f72c0381cf151f33a6b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **228.4 MB (228425023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c6f8e616a486f9d8aebd06f68309128b75dbc6e59e43ca3203fa87a3890f521`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:44 GMT
ADD file:55affb702d0be7976581cacdb7c77f2c1b0d6921d2cd689a427471c2fd9d4daf in / 
# Fri, 29 Apr 2022 22:50:46 GMT
CMD ["bash"]
# Wed, 18 May 2022 18:44:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:44:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 May 2022 18:45:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 May 2022 18:46:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c551bbcabccfb0977b8a9e2ba72099b05f9ba8b7c7106d8a29073b45bc73a9a4`  
		Last Modified: Fri, 29 Apr 2022 22:52:38 GMT  
		Size: 28.6 MB (28637139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc99034c1c5069115fde088e65757003cf7565698429334337590bf0a86bda5`  
		Last Modified: Wed, 18 May 2022 18:50:09 GMT  
		Size: 6.1 MB (6084504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:690461f48e9ac677dc791f777d46ec994250897ad6d015fc260a2de96eaa82ae`  
		Last Modified: Wed, 18 May 2022 18:50:09 GMT  
		Size: 3.5 MB (3479076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37fda6c39e0ad2735d675f8a329621f3311eb325813ab3252ef68ce119bae80`  
		Last Modified: Wed, 18 May 2022 18:50:22 GMT  
		Size: 39.3 MB (39296016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f297f6ae7688f2d733bb3dfd838fb5354c56211f3f723631f9cf094131f80f0b`  
		Last Modified: Wed, 18 May 2022 18:50:49 GMT  
		Size: 150.9 MB (150928288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
