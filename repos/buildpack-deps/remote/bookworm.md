## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:5b9354bdffe627351a2a1639a788ee2f4ce0f7a834885cdf658f9b1358eeed74
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
$ docker pull buildpack-deps@sha256:2a74e7708643f1dca876eda741ce5f006cc2c3a308e1570a8ade2a56f174ab1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.0 MB (341019416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c56bbb0964aa922e28ae82d15bad182bfa406e5a658ebbbb28256bd16edc908`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:23 GMT
ADD file:7d616c027c138495879d0578d333124a7a41f161d38339949eae9fc46a97bafc in / 
# Tue, 15 Nov 2022 04:04:23 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 10:21:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:21:13 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 10:21:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 10:23:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e44dba964a0f1646d06ab7f617603ef51c645dd641b4ce74411770449b003f3`  
		Last Modified: Tue, 15 Nov 2022 04:07:53 GMT  
		Size: 50.3 MB (50297005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65df78b7eb3f0a3cb19c3e7e1eee5c5f93e45ff73ff9fa0a57ea8d5bbf289837`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 9.0 MB (9017903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df801fdaea384702a5d171a41a11d9e52f28f2ef21d2c34c289602d6933bfc14`  
		Last Modified: Tue, 15 Nov 2022 10:30:32 GMT  
		Size: 11.4 MB (11372948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8830a043c9df19400a0998e5ffbc747e2ec2c6839411650f62fa97df03bab938`  
		Last Modified: Tue, 15 Nov 2022 10:30:50 GMT  
		Size: 57.2 MB (57210022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a184a2a99486a7b9b4cf41053d97ff4c818ffef550bbd8714a270386ee50db4`  
		Last Modified: Tue, 15 Nov 2022 10:31:27 GMT  
		Size: 213.1 MB (213121538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:9adf0e6aff65f60e16c27aa267102c1b1183bc9666507374eaaea3d9b5e1f6e0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.7 MB (308740254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b5c08a9a039b7cd94577f7eb3b8e64b0e3c188d35315d1399c73fc701b6f648`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 01:48:32 GMT
ADD file:f5954c36a3601d3dcf67f8701fe7691c7a94bc36e88827c06ff7338a52d56c5f in / 
# Tue, 15 Nov 2022 01:48:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:38:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:39:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 05:39:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:41:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:34757784ba8ccecfd4a2f549aff99cd98b7b291a61176def51827463bc77aa00`  
		Last Modified: Tue, 15 Nov 2022 01:53:14 GMT  
		Size: 49.3 MB (49265841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf55f2cf20315f11c0568b2c8e64fa08c08d44cd3c2ed5e281caebe13320c93c`  
		Last Modified: Tue, 15 Nov 2022 05:47:05 GMT  
		Size: 8.5 MB (8471441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889ed4552e2f48445b3ae801a3f6bf662eac23614471014335840669c23ecf4`  
		Last Modified: Tue, 15 Nov 2022 05:47:06 GMT  
		Size: 11.0 MB (11025735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdcd3cad57bb08b27e14dae1282646677672ad58c572057c39db8a0145596cb`  
		Last Modified: Tue, 15 Nov 2022 05:47:27 GMT  
		Size: 55.0 MB (54962468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b59758eecff625fdee6093614dde58eb0c0764a1ffda0ef0f1a7a362000759d`  
		Last Modified: Tue, 15 Nov 2022 05:48:10 GMT  
		Size: 185.0 MB (185014769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:329cc819de3afbd35d53f0827c3c3cb8ddbeb6038d97c06e662908324c74b3b9
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.8 MB (294776371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecd5acd13b424d3266c051681bee457a411565d8822c3b78287f4ce33ed67155`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 03:42:37 GMT
ADD file:7196c14a33cd1774b746a830598de6b6368174bf15faa83c36c244a6e27938fc in / 
# Tue, 15 Nov 2022 03:42:38 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 12:15:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:15:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 12:16:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 12:17:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:192a2a7ee5b2cd81557e51320bddd5cf2b318283cd7f7c0c0998525448fcf94a`  
		Last Modified: Tue, 15 Nov 2022 03:49:02 GMT  
		Size: 47.1 MB (47088370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbf2f82dd6bc5c9f45ea459022b7744bc671cdbbf0e4a75b81f8f7806c95bec9`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 8.1 MB (8119764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a83154b6af543fb7c117afa8a800dcc4616a91acfe5de9000b91948e1dbd258`  
		Last Modified: Tue, 15 Nov 2022 12:27:19 GMT  
		Size: 10.7 MB (10650100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef9b01aff410cffd1e3702451f2b73f686cb7a9e4b7bd73491ff9630bb896eed`  
		Last Modified: Tue, 15 Nov 2022 12:27:39 GMT  
		Size: 53.0 MB (52967688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c88a6a9062b055499e16dd1113bed78669bcf30edd7049c08c4ded4cf7f6d2`  
		Last Modified: Tue, 15 Nov 2022 12:28:18 GMT  
		Size: 176.0 MB (175950449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:acc5fd6070cf55370a05834fac8fb49668e28c1561302bf0b9e09fdf37ce32aa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.4 MB (330386723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca00d3db2430f0ad6ff841c366e768d7820a80b42a50966b726bd449fe2d80f6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:50 GMT
ADD file:de3ed89259c63b45a553c11db2206a6ca4201bfd264f04890af2c672736c15b4 in / 
# Tue, 06 Dec 2022 01:39:50 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:02:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:02:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:03:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:04:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6d78ccc24e38e1c539440b7f90d65e136bba8366864c2b4a45e3956272709049`  
		Last Modified: Tue, 06 Dec 2022 01:43:02 GMT  
		Size: 50.3 MB (50307715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bb26845d7157ae0fdc105d1666dd413b3f1236876c9e38fe497d4b566c5b8a0`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 8.9 MB (8851114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aee48d89e1a98c15d782346793fdaba61be0e798358172b68670681463bdd69f`  
		Last Modified: Tue, 06 Dec 2022 02:10:56 GMT  
		Size: 11.3 MB (11325483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2882696f0c89ced811afa19b67056d882fbab71ccb7f7e31631ccdc1d1349d0`  
		Last Modified: Tue, 06 Dec 2022 02:11:13 GMT  
		Size: 57.1 MB (57130706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d70607a1852f44ad7df922b590cf97aba81583fa390f7780b337589ffbb47b`  
		Last Modified: Tue, 06 Dec 2022 02:11:43 GMT  
		Size: 202.8 MB (202771705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a91f66a41af7ef62f269ca9b380c17a99c3c7fbb0256ff935104d3fe766205b1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.3 MB (343289313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d2d7e290c6e842cc340bcc16cd0973798bde9a686c94b0806f6f98421c201818`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:38:43 GMT
ADD file:6064ead20e3d5415784fcb74157c3ba1b90982f542deb132e9dabb2a1712e396 in / 
# Tue, 06 Dec 2022 01:38:44 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:05:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:05:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:05:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:07:09 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45070d389a5ecd4dae6cdcb3e06567c8481416cfb2efb085e318fb5e2d11393b`  
		Last Modified: Tue, 06 Dec 2022 01:44:36 GMT  
		Size: 51.3 MB (51301574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efe8313be6a60f2abeebcfad5a2e4539e7d4b28618e0b019908926dd39c9c1bd`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 9.2 MB (9196657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4a90125b538cbb0d87c8c0d37737cdc01ed561a27c8ecfae4cc4f708aecc3`  
		Last Modified: Tue, 06 Dec 2022 02:14:11 GMT  
		Size: 11.6 MB (11560721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c4c1fe8d1b528c380407ded013fe72d397a8e0cc5e05d87cde0f468224efdfd`  
		Last Modified: Tue, 06 Dec 2022 02:14:30 GMT  
		Size: 58.7 MB (58685451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afbe805e9e59720eeaaab1b679e34b1b62ae1dec847175d1ef30259e6576c94`  
		Last Modified: Tue, 06 Dec 2022 02:15:05 GMT  
		Size: 212.5 MB (212544910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6b270982043a2c589f81bbf4227bfd17a455ddd51879657d257611edcfd72882
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **316.1 MB (316107998 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7e3682bdb8d357a63a19b106cc7a8676d89cc800bbf1793552d3d75b2c6ecce`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 04:11:59 GMT
ADD file:0d439a2fdede63b0646f17fe0578b4ebab24012a35c93e6e63e5c511ccce8fe7 in / 
# Tue, 15 Nov 2022 04:12:04 GMT
CMD ["bash"]
# Wed, 16 Nov 2022 02:02:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:03:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 16 Nov 2022 02:05:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 16 Nov 2022 02:11:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:52449a481885eb7aca2b2fbb088c8d233a6249a8aaaf65e32f8c268ad8340850`  
		Last Modified: Tue, 15 Nov 2022 04:19:19 GMT  
		Size: 50.3 MB (50314192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d29bbc0f4e1684560d462982ab292feb495140fdd75d13e6826460b19d90c0`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 8.4 MB (8383819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:232356f6f3990a119f67b1a72642482a16966341b02a7f077b08d38e1d12852a`  
		Last Modified: Wed, 16 Nov 2022 02:27:31 GMT  
		Size: 11.1 MB (11132477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:705e4f6a2f0ed68bc3f782b429fc0c3d447a4f512e41434fa2668233d6417a9f`  
		Last Modified: Wed, 16 Nov 2022 02:28:20 GMT  
		Size: 56.1 MB (56081961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6706090d5e90f71280e5e17fdf9da1714f19e450135909c7a9697f438d359122`  
		Last Modified: Wed, 16 Nov 2022 02:30:30 GMT  
		Size: 190.2 MB (190195549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:774604d8c9e10a23e2b3eff69867f1ba8639d1b6ef97dcdf5aafe8ddc1800113
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **352.5 MB (352463337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56ad94118cd798fc347a59cb27650dfc45f14d2a90e9553dac41dd8a243ada64`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 15 Nov 2022 05:17:43 GMT
ADD file:b13da8e7ee4f9b71f42de64cf2dfe92a09d9d6be3537a8b151db32013e632fb4 in / 
# Tue, 15 Nov 2022 05:17:45 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 11:51:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 15 Nov 2022 11:53:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 11:56:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:24f3e6cef4f753f77f6e0b5b4e73cf7a7fdbfa85b11f29916d1d4fe28bee544c`  
		Last Modified: Tue, 15 Nov 2022 05:22:58 GMT  
		Size: 54.4 MB (54360800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e462c1bdfc268a97c6033242cd34635559a926155991efd84c30d93ce39ce6ee`  
		Last Modified: Tue, 15 Nov 2022 12:06:33 GMT  
		Size: 9.6 MB (9596802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:970a93fcc7e991ae16e04be69f70dc91326e712c64e700b5ee5a6a3f14bb797f`  
		Last Modified: Tue, 15 Nov 2022 12:06:34 GMT  
		Size: 12.1 MB (12129037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32858cde7d5ae6256db15870fd4843b2b1d1b45a97333630926091c571385bc5`  
		Last Modified: Tue, 15 Nov 2022 12:07:02 GMT  
		Size: 62.1 MB (62063332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72264eb8197b779840f3fba9053d7550ab959125c6e517f8d73ea46863ec354c`  
		Last Modified: Tue, 15 Nov 2022 12:08:02 GMT  
		Size: 214.3 MB (214313366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d56a29df625fd854b919433ceb4d22250c1a831ba92bb7f4a72cbdaefcae3ed0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **308.5 MB (308465893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d3964b210cdd3d22cf34d2d55718003ebdc367a5f304f371f389ffdf1a9a32f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 06 Dec 2022 01:41:45 GMT
ADD file:45186e2067a128e8dbf3558a97cd5853548faaf7c2bb93ef1544ed66907fcf19 in / 
# Tue, 06 Dec 2022 01:41:55 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:06:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:06:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 06 Dec 2022 02:07:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:09:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:effa21bde36181862f20d53853fc03e36421f6a13d6aad41051d593fe9c7c097`  
		Last Modified: Tue, 06 Dec 2022 01:47:58 GMT  
		Size: 48.7 MB (48664905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f5dcd56007991a3866c8b0bf2ee7220f18a57fb48ff74112e6c810f63c8b96`  
		Last Modified: Tue, 06 Dec 2022 02:18:52 GMT  
		Size: 8.7 MB (8652754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1216521a137ae490612192a50d936077fcb94da6292a8ef16485599b92a5ace`  
		Last Modified: Tue, 06 Dec 2022 02:18:51 GMT  
		Size: 11.2 MB (11226716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49291721bb021828aa82c6d2c7e2c9cc22d7fe71b2f0406cef91b807704ecbea`  
		Last Modified: Tue, 06 Dec 2022 02:19:06 GMT  
		Size: 56.4 MB (56389158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53292faa787570e0592bb487a5b9841704d7b7bfe37340c85dabccac0bf5fba0`  
		Last Modified: Tue, 06 Dec 2022 02:19:34 GMT  
		Size: 183.5 MB (183532360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
