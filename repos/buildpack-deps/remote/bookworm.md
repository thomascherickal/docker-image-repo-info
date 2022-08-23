## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:919161841fe334d750eff9b6decf745e8761a6bb1ea0640f21b13fae4880f1b0
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
$ docker pull buildpack-deps@sha256:c499dd57309b82d2d43be6cd76563d9713b78e09edac66558e8adb44d73140f2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **562.1 MB (562080993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ce38a856ecb08376f79b2d4fd6cca8d215ab17103b6274edcd9aa076032ade5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:20:15 GMT
ADD file:7507edfdf016128615e9ba278d471fd6d27c96436e543786b691c93b6f94b56b in / 
# Tue, 23 Aug 2022 00:20:16 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:46:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:46:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:46:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:47:49 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5e784af754e1c7855decd29b818520a98b5b539515cd7c199c5dbceb6cc4a45f`  
		Last Modified: Tue, 23 Aug 2022 00:23:57 GMT  
		Size: 52.7 MB (52725730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c06352499c53ea1415d7d7121128de838e832cbc465b145c71d05fb7b74a91c0`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 9.3 MB (9298815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88fbc1ce3af2aec72e131f3b876f2554849f8d6291840fbaf61b24970e54c3`  
		Last Modified: Tue, 23 Aug 2022 00:54:04 GMT  
		Size: 11.3 MB (11272439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2afebddf0d45a19b246f4ff1ead1dd600b48cc494afd00873819774f29c6f388`  
		Last Modified: Tue, 23 Aug 2022 00:54:22 GMT  
		Size: 57.6 MB (57602962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7909283d0b83eb6d0800ae7c471c60ae0891ef4c36524f7ff60b725616e553ed`  
		Last Modified: Tue, 23 Aug 2022 00:55:27 GMT  
		Size: 431.2 MB (431181047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:97f078f2318ddd0d5e369b26b804cae7895b80a64cfdb38598ed08f09b59de96
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **512.6 MB (512603026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9338cdc62f6d8b5386b6ceae633ea50d5f36bd4d30c72201040efca568d03302`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:16:08 GMT
ADD file:dbc0c48f409cbe73d340bec8639492807b8c28fa6907379a17a958448dca1829 in / 
# Tue, 23 Aug 2022 01:16:08 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:16:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:16:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:18:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3204f8dd2e8fdf47391628664d2c96551393e3e0abd1e471abeb57296519c816`  
		Last Modified: Tue, 23 Aug 2022 01:21:24 GMT  
		Size: 51.8 MB (51814042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2edbed2d89089bed15e37327dce17d68521ccd0390a9172314785a01bb2918c5`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 8.7 MB (8740375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ead884b6cf02ae26001f7fa32ee0d5127f5b1f36fe6d675bf0ab7b8b81baa00`  
		Last Modified: Tue, 23 Aug 2022 06:24:42 GMT  
		Size: 10.9 MB (10946896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e395af4802fa3dfe5d8dc10a19e4fb9ea0adaa8951ba0595e9c756a12d412bb8`  
		Last Modified: Tue, 23 Aug 2022 06:25:07 GMT  
		Size: 55.3 MB (55284425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509d388565301a498f7b95d89df044727bf2633fd54aacd973fc712a97327789`  
		Last Modified: Tue, 23 Aug 2022 06:26:41 GMT  
		Size: 385.8 MB (385817288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9a600d1bd9f374ba63199357fb2b43f0e3d84ff00611579519f7dc7eb4015653
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.7 MB (297698577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49dc73618886f3fd7c4d92c655d62e9893b318f326792a44d4fb294b963702ab`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:57:55 GMT
ADD file:359193f5179bfdc5181bda2e05bd0b22ae4a86c638b0bbf09f289d1727fad222 in / 
# Tue, 02 Aug 2022 00:57:55 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:45:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:45:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:537407bee93780ba0135c6d74e62d8cee8d32e85ab926669d3cc9bedeef28852`  
		Last Modified: Tue, 02 Aug 2022 01:05:20 GMT  
		Size: 49.5 MB (49527674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f21e0c1ecdb66b081e679eaee092b97020507b0a7735843a508a74b1ecb86429`  
		Last Modified: Tue, 02 Aug 2022 02:07:51 GMT  
		Size: 8.4 MB (8417992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b2371236f490dda856391359574a3e2e3ecf9d8d39f77649c8c6839a1846326`  
		Last Modified: Tue, 02 Aug 2022 02:07:51 GMT  
		Size: 10.6 MB (10589533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503864111e2b00823bf24541ba248d5caaa84e32bc41634a765833fba8201148`  
		Last Modified: Tue, 02 Aug 2022 02:08:17 GMT  
		Size: 53.4 MB (53402629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:893b751166610da667d89fe195a173fc7be85f007e70bfb691ca710de49c23cc`  
		Last Modified: Tue, 02 Aug 2022 02:08:56 GMT  
		Size: 175.8 MB (175760749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:b8074d04677387c84532dbc39903d4a7ba2dbac38fa624956417e4b251024d25
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.9 MB (551918652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1473f33d94d3c58cb12b6d618f9cafa967b830841c427a4fa8717f924dd351b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:51:53 GMT
ADD file:f94a576f262c4fcf5112164145c04850c826787b299878e7e126754d1211a51c in / 
# Tue, 23 Aug 2022 01:51:53 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:25:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:26:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:27:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7dd208a8a7339c037c691e6ace1cd3f94803ee4c17a3211b9ccadf01d1ff2ca9`  
		Last Modified: Tue, 23 Aug 2022 01:56:50 GMT  
		Size: 53.1 MB (53117563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6d7761ab15abc5f27917ed7e543565cb302e30ac8bd10819c205f079ec603`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 9.1 MB (9133938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d472709c6f5c8abe91373fba2db77fd3b0946f573269803173452485abc6ff8b`  
		Last Modified: Tue, 23 Aug 2022 02:35:05 GMT  
		Size: 11.1 MB (11062413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247b0fb5989ae9d485d4b97b959d16adfaeb2e92bf9a74bd8b1f677bb7f3e1c5`  
		Last Modified: Tue, 23 Aug 2022 02:35:25 GMT  
		Size: 57.5 MB (57496084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e62402acaffd55bc794eef07b132e4223f8f48067c5d1df8909da8f8de8e39`  
		Last Modified: Tue, 23 Aug 2022 02:36:32 GMT  
		Size: 421.1 MB (421108654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8539ef8ee56afeb586b85e49787586a5111a6de92bc10b9f37ca69bd9309ad13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.1 MB (355072478 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b32f2b395672361202ddd299bd9ee7fb01a3d461778187967fb1f32cdf4a2d82`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:01:59 GMT
ADD file:1c8ebe8b69a2d3c236c8a947162fab2e579f4bf01bff01695a3c46557f6c73f4 in / 
# Tue, 23 Aug 2022 01:02:00 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:28:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:29:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:31:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:29bf8f676853094720e43096224f2ec8a31ffa3752cf7a1e52fb9e72ae069480`  
		Last Modified: Tue, 23 Aug 2022 01:07:13 GMT  
		Size: 54.1 MB (54096938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0426ba96c16ee4ea8eb5b5322685d94b842c455938234d92ca07814c6ae081`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 9.5 MB (9475146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86201f3e5308e2da4dad080700c08b4d6a0a02c265e56c7a0cdae2889f16b442`  
		Last Modified: Tue, 23 Aug 2022 01:38:51 GMT  
		Size: 11.5 MB (11473600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4eae1a3c8a2b637c155af3a0e81b010eea8632db588e887a59f57d020ad81a8`  
		Last Modified: Tue, 23 Aug 2022 01:39:11 GMT  
		Size: 59.1 MB (59102590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ecd69ec89ab5cbb90df7026e375153b4bae6f2e062807e484c266484a434f19`  
		Last Modified: Tue, 23 Aug 2022 01:39:48 GMT  
		Size: 220.9 MB (220924204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:e8528c6f8b9cbb5874dd13fc82568ef6113dd851dad05c8f38248f352ad465bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.4 MB (320403475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2f881dd4c7e9a1d28c30f6d42c5261e89899a0f4dc6f6f747f404089ceeff53`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:08:47 GMT
ADD file:071fbdfd189eb16d9f6ef75de927dc676c1f54b47bc4e17163522108782b28ec in / 
# Tue, 02 Aug 2022 01:08:52 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:45:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:45:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:53:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d875d0bc6e0221f25e9536bae93056c28a4346ebdefd9847e38ca0c0b536a4b7`  
		Last Modified: Tue, 02 Aug 2022 01:19:01 GMT  
		Size: 53.1 MB (53099858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcedaf5d854c546aa8dfba8a69de72201352b43af6678144af78e6ba1b4eb4f6`  
		Last Modified: Tue, 02 Aug 2022 02:20:57 GMT  
		Size: 8.7 MB (8674895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb36366f74dff43a81dc4efc0c8dcf582b8f4dae63bff044706dcb2816f1d22`  
		Last Modified: Tue, 02 Aug 2022 02:20:58 GMT  
		Size: 11.0 MB (11041565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea48d16111b1cb59aaff2b057672e96116d9de657a96d6821918a319f7d6e2ec`  
		Last Modified: Tue, 02 Aug 2022 02:21:47 GMT  
		Size: 56.4 MB (56418644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62d9a6ebd0844034a170c863fea950d99b4e619bb51f21d8e56658c7c3afb77`  
		Last Modified: Tue, 02 Aug 2022 02:23:57 GMT  
		Size: 191.2 MB (191168513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:ee2a6c73ac3292db2fa2fbf661eb2e89b0efb41e7d31d177c394eef94afc20fe
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **561.4 MB (561424552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f377208d9b0ee3a46f734c8e72364e0683ef2f7b1516eaa2a8fc4b2eb0878050`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:23:48 GMT
ADD file:92444ce23c3227ef88446469c37fc41decda1ba975ddfb1be3e1ebb1e694471b in / 
# Tue, 23 Aug 2022 01:23:51 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:52:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:52:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:57:32 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a2d2f2c5b4e64eabb8a7632609e67883239433d932129bf478f7614059a9aabe`  
		Last Modified: Tue, 23 Aug 2022 01:29:05 GMT  
		Size: 57.3 MB (57289866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b43c7a1c5614eda4b722aada1632b2b42c7499b945bcd902a405d6811943e66`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 9.9 MB (9888870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e4983e94a7031bdb88baa08be05b8f42254ef49f65245663476650772c95d77`  
		Last Modified: Tue, 23 Aug 2022 02:08:15 GMT  
		Size: 12.1 MB (12083610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aea4205d8530bba3b66567e144b76048ea3deb5e2f1d3604690cc87c10af416f`  
		Last Modified: Tue, 23 Aug 2022 02:08:43 GMT  
		Size: 62.4 MB (62419202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e108af90182e1e05955b926792132c93a713e0f0ae2b578251685acee0a56d`  
		Last Modified: Tue, 23 Aug 2022 02:10:29 GMT  
		Size: 419.7 MB (419743004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:57fb9cda7864376befccdba60b0413224dc32ed2b9bff5f027364c801ba026f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **310.5 MB (310501027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdfb704283aef4b05b84723b02d390716be945c6a0e085d3c009420045e590ed`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:41:38 GMT
ADD file:9364324d9e3e24a6e417365a226c42bac5c3c9589b444096a65d5bf539eec127 in / 
# Tue, 02 Aug 2022 00:41:45 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:07:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:07:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:07:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:08:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1a5bd7c6618b65a5948f8c07805e4109ef4f5aac36711b43d0fabe6f11fe0ec8`  
		Last Modified: Tue, 02 Aug 2022 00:47:13 GMT  
		Size: 51.5 MB (51514530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c61b0b54c9dc1946fb336e5a04c532d39a45e681f19f307f477085013dd8bc`  
		Last Modified: Tue, 02 Aug 2022 01:34:07 GMT  
		Size: 9.0 MB (8952435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edc88e19b9b0261e01462a1883dcbc8fd4849c5a80450a4659c246ae5188132`  
		Last Modified: Tue, 02 Aug 2022 01:34:07 GMT  
		Size: 11.2 MB (11166761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:322fa986d6da7624363b347b0ecc23718b41b493d8ee8b8ff0ff9e1c158ce17e`  
		Last Modified: Tue, 02 Aug 2022 01:34:21 GMT  
		Size: 57.0 MB (57027041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218863b80cd9b0b84378aa603587fa1a63bed8644c193bb83a697b01ddfcac7f`  
		Last Modified: Tue, 02 Aug 2022 01:35:03 GMT  
		Size: 181.8 MB (181840260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
