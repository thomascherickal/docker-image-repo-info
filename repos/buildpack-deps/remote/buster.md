## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:49298fa94057e243638bb9fe10825962b5cb311d87042c1100d460a1fca5343e
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

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:6cf6765f5a3d6ae185a0cca26f00844b3d2693a658986c95ce53adc3d25da703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.6 MB (312622451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbdff219ec50522763e1ed3e346dea2dc848222fd1ecab42cac248ca67c103fb`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:22:28 GMT
ADD file:8c5e9f12fd3b6e830ec0ee1800d8e9dcebf217896148f2dc72c010c8a88d9b8f in / 
# Tue, 29 Mar 2022 00:22:28 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:31:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:31:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:31:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:32:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b281ebec60d2630a225601bd58a4681375a31b7316263b64d3b149f49694c3fe`  
		Last Modified: Tue, 29 Mar 2022 00:27:37 GMT  
		Size: 50.4 MB (50437915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74dae484504b039004d1f23b1777be24e9e8d0f126ee1f38b97544d6343fb9fa`  
		Last Modified: Tue, 29 Mar 2022 17:39:22 GMT  
		Size: 7.9 MB (7856401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21739e3ef21a7c9983fdfc82d5a3837c633779965fb0b2cd7b746ec9c260664b`  
		Last Modified: Tue, 29 Mar 2022 17:39:22 GMT  
		Size: 10.0 MB (9997192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98d6bb51c7ccadb2f72a1498db713088ec7c3f449b3c810d95dbca6ba7511ba`  
		Last Modified: Tue, 29 Mar 2022 17:39:41 GMT  
		Size: 51.8 MB (51843446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:517ebafd9747d2829907c94c586a296ef74a55250cef7b8230a7f844e08a3659`  
		Last Modified: Tue, 29 Mar 2022 17:40:14 GMT  
		Size: 192.5 MB (192487497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b4856c2db035370fba2643efb7bd6b281988e8fe3a0bdf67213dea799e6019c5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.3 MB (286254793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98038a0a472589025c19f16afb9db8a7a9895e3a4b82ad7315536934aaf511d6`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:51:04 GMT
ADD file:e7d31ee8f990df96d5922feb35173a364a0832e8fce2d32fd4e703aa3b66e1b2 in / 
# Tue, 29 Mar 2022 00:51:05 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:46:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:47:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:48:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:51:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0bbc2517bf9c8d842997ba8f85b59bfd92c5bb6bba79c39047eecda859dcae27`  
		Last Modified: Tue, 29 Mar 2022 01:06:08 GMT  
		Size: 48.2 MB (48158294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c1b4a5e78fec7573050b1b9220718c42ec377971effed53f70015af0614fe3d`  
		Last Modified: Tue, 29 Mar 2022 08:08:45 GMT  
		Size: 7.4 MB (7400493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4f39bb570fd924ca89ef560a7dcf08a5b1bdb060fffc39839196ea306860e0`  
		Last Modified: Tue, 29 Mar 2022 08:08:45 GMT  
		Size: 9.7 MB (9687634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330afa3bdec5391c629c4f733ee4cb7c34676c6ad602c7fc098081610752eede`  
		Last Modified: Tue, 29 Mar 2022 08:09:32 GMT  
		Size: 49.6 MB (49583760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986f1f04990f163d564f74b84c29d50a046f25f445b478f3bd0678bcfd32b091`  
		Last Modified: Tue, 29 Mar 2022 08:11:26 GMT  
		Size: 171.4 MB (171424612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:3123c74430062702fbeb96d4dfd6ed5c0beea82fa25ccaf044b72e516d314532
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.4 MB (278411145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5cfaf2368da4a0e63e4d17e99afc8a9fbff8024bed22c4ebb041bd2b8b92f1`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:31:32 GMT
ADD file:7fe62421fc35de4e6311d22de22ded33c729d98a51fa41d57e04c76ec092827a in / 
# Thu, 17 Mar 2022 09:31:33 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:56:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:56:14 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 02:57:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:58:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f82e094db40ddc4d9b2e16ec4c7f28c689bdd532358e18ab566e90aa5975838c`  
		Last Modified: Thu, 17 Mar 2022 09:47:22 GMT  
		Size: 45.9 MB (45918162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6141a0e962d9abc8740d150bc5bf7f5a58f74cc0e97601134c7ceccc5dc31eb3`  
		Last Modified: Sat, 19 Mar 2022 03:32:03 GMT  
		Size: 7.1 MB (7125521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f529c02d4e740677c379f14554a5eea0184ff342fd3986da4914383e499ccb1e`  
		Last Modified: Sat, 19 Mar 2022 03:32:04 GMT  
		Size: 9.3 MB (9343898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204f4ebdbf43a4e4fc442a8c4357334aeeb1b1e7b231f7975bdc20a2013a3fd1`  
		Last Modified: Sat, 19 Mar 2022 03:32:47 GMT  
		Size: 47.4 MB (47357665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8404a7019be482002ee9bf8e123ac3cb3c5ed62d29b7e736b931af55746f400`  
		Last Modified: Sat, 19 Mar 2022 03:34:34 GMT  
		Size: 168.7 MB (168665899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2bf98ea6bfd870692e031c9130d159baec7d7d90271f579491cff893d75fb50e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.9 MB (302895803 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce5b13d6e762bd90de8c17d161532c3732def30b58cc5b87716e9fdc6e889655`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:22:08 GMT
ADD file:37cabd1fec04269c22fc158f62ce5bc655934f2e58fb1ff3a1e366a33ba9bc18 in / 
# Thu, 17 Mar 2022 03:22:09 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:12:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:12:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:12:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:13:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3996f04b7c6c17d8b25c04c7287353b896b4a0b10ab440f47d00573a7d5c3e17`  
		Last Modified: Thu, 17 Mar 2022 03:28:59 GMT  
		Size: 49.2 MB (49222993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80907b498681187ef4aa817ec6f39ba351e376afbb4fcf4415841ab9015cfc59`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 7.7 MB (7695349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8327dc7899c1a628cf11f95bb594fca3c86e45d1f4f0eb73d2ba9058eba5927`  
		Last Modified: Thu, 17 Mar 2022 22:22:15 GMT  
		Size: 9.8 MB (9767203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1431347b40fe69ed685917a6ef1b8c28d5de6147f3c62ea11a1951ead75ccdd`  
		Last Modified: Thu, 17 Mar 2022 22:22:34 GMT  
		Size: 52.2 MB (52174886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6df5b0cd9b56b640f0f401d463c7ef2450f177165445568d3a4644f629b1708`  
		Last Modified: Thu, 17 Mar 2022 22:23:08 GMT  
		Size: 184.0 MB (184035372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:61bfa329ec09be8dd23e6bd692db2729fca88ff4e8ea202024d27ba190a27ae3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321800428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb06691066fdd6dd224b703f8bc3ea95bd5a48a8c7cd1d42ef28cf75c9564002`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:42:12 GMT
ADD file:fb2c1bf394c39b5bf948ceaa00317518326bd846b3f6802dc39cfb7fcf404c69 in / 
# Tue, 29 Mar 2022 00:42:13 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:58:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:58:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:58:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:59:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b86fabf064e35595b9c8543deb0dba50a95e438387a9877ebfe189bbfce3c87b`  
		Last Modified: Tue, 29 Mar 2022 00:49:34 GMT  
		Size: 51.2 MB (51206670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fecf9ef7e2149c926eaf909af17e48d32080f3777447e28017d8277168ef61`  
		Last Modified: Tue, 29 Mar 2022 18:16:16 GMT  
		Size: 8.0 MB (8022197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12ba7e132575662e21e001c19449819145d8c04740ee029d58abb3883fa71010`  
		Last Modified: Tue, 29 Mar 2022 18:16:17 GMT  
		Size: 10.1 MB (10121846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c5696fbd4895db85e5fa3fb1725010f71720ee2d70f2474e0a1ded9a485fd5`  
		Last Modified: Tue, 29 Mar 2022 18:16:38 GMT  
		Size: 53.4 MB (53442716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6992e3aba00d0d943f42c7361ec02a73b7dcd63c6bf79bb9765230b4f93dd61`  
		Last Modified: Tue, 29 Mar 2022 18:17:20 GMT  
		Size: 199.0 MB (199006999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6e3e1abf04dca69d73fc66bb9c9fbef3cdb7edcb9040b0875f18d81b63b4fb81
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297026346 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0989ffd9a29f6a09e3ddd85b7be7f139d8944840add1c2c6d608de78348e5f1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:43:01 GMT
ADD file:c86010b52f782f910842586e6abc81e64c7a659d001b89799314a59f4fb96573 in / 
# Tue, 29 Mar 2022 07:43:06 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:35:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:36:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:38:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:44:57 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e0bee9c4b9257c0ad7469830be5e890536feef4e8ffe6c2613b7e8be7e060f6`  
		Last Modified: Tue, 29 Mar 2022 07:53:41 GMT  
		Size: 49.1 MB (49079891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc690a0cd1092524bdd12063c730cdf1df3dfa2f8c5920231d8477654c04b854`  
		Last Modified: Tue, 29 Mar 2022 09:38:05 GMT  
		Size: 7.3 MB (7272773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06fe0e6a034874e5b70e892d14e911e5aaa7f314b7588616996be6ff22190b1a`  
		Last Modified: Tue, 29 Mar 2022 09:38:06 GMT  
		Size: 9.8 MB (9800273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce84f8d8d66208e065df79ad5efc3776584f6dd13891c8f9eafa9c02a12aaf58`  
		Last Modified: Tue, 29 Mar 2022 09:38:52 GMT  
		Size: 50.9 MB (50859745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13876620bf13ddb0a90ac352ea4aa991b4215b6d3e91eb84e189559155991d28`  
		Last Modified: Tue, 29 Mar 2022 09:40:54 GMT  
		Size: 180.0 MB (180013664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:f1d3dcffc07a3862782097fdef34d9d2903c170ab9f575ecdcf43d7aad6eb88d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333995940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:546520f251f43295870e2789ef2093bb6d08918352806c6cddafece8346d4adf`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 11:18:17 GMT
ADD file:f75a960e2412d5d93ea52573154078e69481bda1da84f66aac3871c0c0776bfd in / 
# Thu, 17 Mar 2022 11:18:29 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 05:48:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:49:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 05:51:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:57:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c525619180c8f2ab5210413380ee35a9d0855c7e877e0ebe8841a1724e9605fd`  
		Last Modified: Thu, 17 Mar 2022 11:28:49 GMT  
		Size: 54.2 MB (54183837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aab80fef29bfe486fc89cd31900757a3db86e74b037ab36d6d675a9d3ce9e750`  
		Last Modified: Sat, 19 Mar 2022 06:42:35 GMT  
		Size: 8.3 MB (8273595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca60d3aaebf7006e51596f47c9c245b72f01999ee68dbd0071b1903bfd578386`  
		Last Modified: Sat, 19 Mar 2022 06:42:34 GMT  
		Size: 10.7 MB (10727760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a8aaeab00841b8deb7a50caaa5ed2641b6d5be2f766c1e2bd74f601abacdb0`  
		Last Modified: Sat, 19 Mar 2022 06:43:38 GMT  
		Size: 57.5 MB (57457879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2be5b02264140966901f8282ed25d6f57335d4631e3158609b392d60a4061669`  
		Last Modified: Sat, 19 Mar 2022 06:45:25 GMT  
		Size: 203.4 MB (203352869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:202b857bf2e0f8284a2672aa5a0f55fdaca6071f4564d16588602594e327e815
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.6 MB (294612100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e95ee812555c1fe624b4f1b52862b22585db452bcfd66241beebb4625d518d9d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:07:11 GMT
ADD file:6505b8e134084dbb9f879838b24cf47cd265cfdc5952f50ba2ddc63ff4553145 in / 
# Thu, 17 Mar 2022 03:07:14 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:22:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 18:22:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:23:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1e9fa32475c4074341da88d0325d6e125bf7587795cba4bef553a90bf7472c7b`  
		Last Modified: Thu, 17 Mar 2022 03:13:01 GMT  
		Size: 49.0 MB (49005525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dfc7a2d5d979460a379f74fd1adf756566aaaf27b9ad22b518b7b0b13b7b2a`  
		Last Modified: Thu, 17 Mar 2022 18:29:59 GMT  
		Size: 7.4 MB (7401708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1517a8cbcd9e9cd84fd94cb3e7e7a02def9f47cf27b751461484d31f85725361`  
		Last Modified: Thu, 17 Mar 2022 18:29:59 GMT  
		Size: 9.9 MB (9883064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e2eeea69f115ed70563efadcae6ee48a38e8ebc96a88421d8b99f8728276da`  
		Last Modified: Thu, 17 Mar 2022 18:30:12 GMT  
		Size: 51.4 MB (51382425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c30e1445da9205d243c7807748e16a4268c57e2ed1b42d02b978a7405e26a56`  
		Last Modified: Thu, 17 Mar 2022 18:30:38 GMT  
		Size: 176.9 MB (176939378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
