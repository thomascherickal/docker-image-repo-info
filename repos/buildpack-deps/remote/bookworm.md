## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:4944b743981be3fbd5120270d8e22ac5b3bc3668f809feb9a155b4ecd44850c2
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
$ docker pull buildpack-deps@sha256:05dee752f37660eea34b04a28f3ee8ed431d10b990d9f9e51b5b95db7e929d16
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.5 MB (343473611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:292c057a82a578bd4e3ccb794d6e857287b71058e1c8e8b7bd588bd2d1b6a7d6`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:34:06 GMT
ADD file:cbb7762965e1100a173296573d49c70a5e56d5318572ae1b037854e45a3c81df in / 
# Wed, 11 Jan 2023 02:34:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 03:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:02:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 03:02:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 03:03:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:248f02a8d7fb9e98e764c3ef93b9922d99e6b305be444aa17bace4ac12a55508`  
		Last Modified: Wed, 11 Jan 2023 02:38:08 GMT  
		Size: 50.1 MB (50106530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f922aacf80e8d4f20a47bafd73d9b7865d169f43635eaabc15b5e25eeb6057`  
		Last Modified: Wed, 11 Jan 2023 03:11:00 GMT  
		Size: 9.0 MB (9032940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76b287e34dfb83462bf58f6751173d64481c601980dc53909c7d198527f44e88`  
		Last Modified: Wed, 11 Jan 2023 03:11:00 GMT  
		Size: 11.4 MB (11352159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8760a729a20f23e47ce926dd7b082265854f8834280377051a238bfaf725e51e`  
		Last Modified: Wed, 11 Jan 2023 03:11:17 GMT  
		Size: 60.8 MB (60811248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c0a5422e204e57af5c2a3f081124cfef40a74906a16e082ee673f602e5f00fb`  
		Last Modified: Wed, 11 Jan 2023 03:11:54 GMT  
		Size: 212.2 MB (212170734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c16abfa0b5a07dcb1b57b169f19dfb3cb5a86af394a93969202aeea651f631ae
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.9 MB (312939324 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb03bc8575a08c9ac6c25acb77e8c6e762c6e15c84fdfc303c7e4dac85bbcc5b`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 01:54:53 GMT
ADD file:5d45a8dd4f8495c2419fecb2fbe1375bee8fdd9c4ecd8482c9d93073ceaf0eb1 in / 
# Wed, 11 Jan 2023 01:54:53 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:22:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:22:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 02:23:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:25:23 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c18e65c95b83dd67fa3b288d25c836639aed042685d4b545ff41efbf3046505d`  
		Last Modified: Wed, 11 Jan 2023 01:59:27 GMT  
		Size: 49.1 MB (49082333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2627725f148bd514b2afb35f5ee907f5f061ac39a52d6f89b1cf91b8a80f46e8`  
		Last Modified: Wed, 11 Jan 2023 02:31:26 GMT  
		Size: 8.5 MB (8484837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a81a8997d0bb710a3d95fc77245088619618e15dc87431056622547133566c3`  
		Last Modified: Wed, 11 Jan 2023 02:31:27 GMT  
		Size: 11.0 MB (11000015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949aacd5a13ab1919fbce97d65475583ac45fdc71c7ecee03b091614645ce8e`  
		Last Modified: Wed, 11 Jan 2023 02:31:49 GMT  
		Size: 58.4 MB (58390014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394a027b1ca48c3c7b1757e511250690f4cab59aac32033b5320789cada04a6d`  
		Last Modified: Wed, 11 Jan 2023 02:32:32 GMT  
		Size: 186.0 MB (185982125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dd790e4ab96cafb9c74c9191b9ec0b423a2c18900ec68a4bd52df99e7389187b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.0 MB (295039671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf29462b326dbfb45c27b4d6b360edfab18c3f9fb81ace95c294fe06a4cd2ab2`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:57:40 GMT
ADD file:3a39343b0809f063616f72499663466e4a509b48e03fab9262c152a211f015f7 in / 
# Wed, 21 Dec 2022 01:57:41 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:25:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:25:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:26:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:27:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5d2b0b92caaf35a430a2b891b3ae1c59a6cf60477263bd8e7a30cda427435d63`  
		Last Modified: Wed, 21 Dec 2022 02:03:55 GMT  
		Size: 47.1 MB (47101260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a36589bec34c9187227f581132ae596646abfc864ef9c4f049dcc7cb80d9e3`  
		Last Modified: Wed, 21 Dec 2022 02:36:46 GMT  
		Size: 8.1 MB (8119430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa4da363e919b9e1ffa0593e59ab1b23caa6d60c84b20ebfea4db0863532e5c`  
		Last Modified: Wed, 21 Dec 2022 02:36:47 GMT  
		Size: 10.6 MB (10646191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca23736de3322232278a50330b166e2dc3a96e13bc603c0a868f7c6ed03aed8`  
		Last Modified: Wed, 21 Dec 2022 02:37:07 GMT  
		Size: 52.9 MB (52925737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5490550e73309c3d20201befafe5f69a532b1149118c1519a15d78e1849532e`  
		Last Modified: Wed, 21 Dec 2022 02:37:48 GMT  
		Size: 176.2 MB (176247053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:443f22d1117086034aa16e171494417a2ccde57c70928ed9b683e9cad4bc6496
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.9 MB (330854528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9626341e921dc9919810a16eb80f8a2d5483729e6f5238414b3762268dcb545`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:39:25 GMT
ADD file:b83d427ad5bc07aecb363a59c19809d66f1425c1d8df7a4d66eb56624cf5fcf3 in / 
# Wed, 21 Dec 2022 01:39:26 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 02:03:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:03:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 02:04:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 02:05:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:be520eae96ff7c486efeba591ba872089e3b618ce226d23bf2b72f07277fb6fc`  
		Last Modified: Wed, 21 Dec 2022 01:42:15 GMT  
		Size: 50.4 MB (50372842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2fd22e8d17dba55cc72a876a3a9244c7b617edbf94a17fdaad2f9d803c02d5f`  
		Last Modified: Wed, 21 Dec 2022 02:11:45 GMT  
		Size: 8.8 MB (8849270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7950c3893d7d3fd9cc5fb052ba3abdcdc532147811125fdba6efec5d9b4efee5`  
		Last Modified: Wed, 21 Dec 2022 02:11:45 GMT  
		Size: 11.3 MB (11325894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53d0bb157e7432bcc4ced269bd85ce3c558f9fcefaac7844b601556fd5cffe72`  
		Last Modified: Wed, 21 Dec 2022 02:12:00 GMT  
		Size: 57.1 MB (57094158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b1db73f34c700043ec7eb90a1aae08d85c52d7526ec8e4bd4a3c0f7ce7a0a1`  
		Last Modified: Wed, 21 Dec 2022 02:12:30 GMT  
		Size: 203.2 MB (203212364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:91fb02366e9717f97dadcda313895f1b414a6c4fe91f68989f36ee9b120f7807
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.8 MB (343770539 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fa575e271aff10438b80f395a7e0eb478bbe62f22319325d669a4edae920457`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:38:43 GMT
ADD file:f11f9a6e73a1ba42c97eb037cc53f119df6d6b050eaeb10df2ae716f4eabd8bf in / 
# Wed, 21 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 09:50:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 09:51:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 09:52:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bce8ae6c08a69b30b85b1e939b782fc4dee31791e21ed3abbf56d1ec1dde0381`  
		Last Modified: Wed, 21 Dec 2022 01:43:40 GMT  
		Size: 51.4 MB (51363529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d633e3250ed10016905229f6d67f3386ceb15eb9d1bc3deb88c518444ced27`  
		Last Modified: Wed, 21 Dec 2022 09:59:17 GMT  
		Size: 9.2 MB (9194506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e65f66728bfc6f4d6de6d54692bc94e1c8972c2fb1d47052d38b89b8d33481a2`  
		Last Modified: Wed, 21 Dec 2022 09:59:17 GMT  
		Size: 11.6 MB (11561149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883b0fff1e223e986f26eda6c09aecaf9bf292dbb243e2d42df8aa52d520818a`  
		Last Modified: Wed, 21 Dec 2022 09:59:35 GMT  
		Size: 58.6 MB (58640479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfbc944a3662672fc817188a98c16bd2795868ff0c1200fd91c031af024b30d`  
		Last Modified: Wed, 21 Dec 2022 10:00:10 GMT  
		Size: 213.0 MB (213010876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c6cf84d06eab5653cc49f6b146e6a717c40632aacc67b5238f25f7f24d94440b
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.7 MB (316653859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebbc47732d4f0caa92b2060637b9aa52104a52ffb641f0d5782e773b55f1fb0c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:08:43 GMT
ADD file:b2458569ae73892acee2eab6d63bd5fac233b8f2939355fc7605c8906c1bbd30 in / 
# Wed, 21 Dec 2022 01:08:49 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 23:43:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:43:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 23:45:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 23:52:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63a99937a40bd4c10c6b0d4be0826a18d963fdd5ca9c794853e98ca819d68691`  
		Last Modified: Wed, 21 Dec 2022 01:16:43 GMT  
		Size: 50.3 MB (50336746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b476ebedac13b0ac645f8735e4d8a8321d9d6dab455dfb083f909d760d43de10`  
		Last Modified: Thu, 22 Dec 2022 00:12:05 GMT  
		Size: 8.4 MB (8382953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d4410a7d6810d0cf4de163bed3aa485a268050cff9cdd1b1d2690d3843d528`  
		Last Modified: Thu, 22 Dec 2022 00:12:05 GMT  
		Size: 11.1 MB (11118852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f052e411ea81eab6516c87a7e7d7d322c9ad6bac847ad1805b31941908d5f2`  
		Last Modified: Thu, 22 Dec 2022 00:12:53 GMT  
		Size: 56.0 MB (56021823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d352f9ed84314710517c22407ebfaae0ae093067ff8ee4a0431f08e7a78d6a94`  
		Last Modified: Thu, 22 Dec 2022 00:15:07 GMT  
		Size: 190.8 MB (190793485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:5d2efa53d257d4f0ad9a6316e720c892de2b71ebb7cfafefd537994a7cbcbe94
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.8 MB (352836079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e1fb3ca1a2847a3dcc1162b9da355a576afa8efb643648e708461a73bb75109`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 21 Dec 2022 01:16:40 GMT
ADD file:ddf53eeecd4e99f9ac6dd446b84eed33212dae1b2a9476907b99dc988c316e5e in / 
# Wed, 21 Dec 2022 01:16:44 GMT
CMD ["bash"]
# Wed, 21 Dec 2022 04:49:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:49:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 21 Dec 2022 04:50:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 21 Dec 2022 04:53:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9a50dadcc8beda7926088df1652aba274c8cf1817cd6956a9342f3b25db470e6`  
		Last Modified: Wed, 21 Dec 2022 01:21:57 GMT  
		Size: 54.4 MB (54373822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9716abced382581cab26adfab0007029a5bb1dda4112dbb4ba74c5cfc7f06ad`  
		Last Modified: Wed, 21 Dec 2022 05:04:22 GMT  
		Size: 9.6 MB (9596165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dbde01939e5586504281eded1dd73c49a0b03f58c2cd890cc840b8267967f3`  
		Last Modified: Wed, 21 Dec 2022 05:04:22 GMT  
		Size: 12.1 MB (12128890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eadf6b46d5863b425edea1179a79cfa53aa4e33b4f2e8df8cfb2127727d75f3`  
		Last Modified: Wed, 21 Dec 2022 05:04:50 GMT  
		Size: 62.0 MB (62002362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0adaac3511b77b3f22097236e252891819da52fcf18eac0b12d3bc48b2a18`  
		Last Modified: Wed, 21 Dec 2022 05:05:53 GMT  
		Size: 214.7 MB (214734840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c1a44d4375ebba51b8c88aa6250d8f50ad003e00cd8ca16c51b9ffa165ef86db
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312586011 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d019727c665a09ef86b66ba41115976fb0432607176249bf043aa181578077c`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 11 Jan 2023 02:21:33 GMT
ADD file:1ba7db44596ea26688f29eb4d23da5507a0d71de49facb85ffddbea04928e97b in / 
# Wed, 11 Jan 2023 02:21:37 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 02:46:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:46:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 11 Jan 2023 02:47:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 02:48:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc45c63d26bf6e7676d21861c5543952964197c106b2cd255789a8aa3734c0de`  
		Last Modified: Wed, 11 Jan 2023 02:26:06 GMT  
		Size: 48.5 MB (48490381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b941bcdefcde17ded465ffd68a2ebb6d2c7db9642b4c6e5df1e8f72eb96d886`  
		Last Modified: Wed, 11 Jan 2023 02:55:46 GMT  
		Size: 8.7 MB (8665948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccacc30d10abfa911c54fe2ac56c3afb46ad1b934aed0943fb3ef1ff2b4fe619`  
		Last Modified: Wed, 11 Jan 2023 02:55:46 GMT  
		Size: 11.2 MB (11215678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc6339bd7d1b55d1a706abd8cfd85402705ea34b3ae5b1d868a704008e244fc`  
		Last Modified: Wed, 11 Jan 2023 02:56:01 GMT  
		Size: 59.7 MB (59746863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a690acb6c343aa32b373f1a0dc804271b2e8c079fa5d7b8f531ed39833caaff`  
		Last Modified: Wed, 11 Jan 2023 02:56:30 GMT  
		Size: 184.5 MB (184467141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
