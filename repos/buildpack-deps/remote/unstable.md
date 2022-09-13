## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:ed26ca3adab1914ccfc59061e9f588b3242ffaa91bb347ee576dc39e487f0857
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:db6bbe1b47461494b07e4ccf08863f7920f995babcf8b79a06d2d33940614b66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **344.5 MB (344536691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ced5c01daf393dc64fd1bc7067bc47f053da4f30f88cfb32b6f2de8fd17bf75`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 00:57:16 GMT
ADD file:7b7161ef988532de9a1ae3caee50f4337a445cd5d88bfe1da455ad45111e2a4f in / 
# Tue, 13 Sep 2022 00:57:17 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 03:46:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 03:46:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 03:47:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fbb5199f866b772d7999f8d0fead2c513b95972d6d32ec2c8e29311458f0855f`  
		Last Modified: Tue, 13 Sep 2022 01:02:12 GMT  
		Size: 52.6 MB (52643556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5abee259a1d9101a0890f49e244222094315b4c017c58d8cb8a6cc0cd43e833`  
		Last Modified: Tue, 13 Sep 2022 03:52:28 GMT  
		Size: 9.3 MB (9298049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a8698192cb686ddacc8322753abf5c95c28d7cca2e06243ec755c2044f89760`  
		Last Modified: Tue, 13 Sep 2022 03:52:27 GMT  
		Size: 11.4 MB (11380792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a113e2744da1b277bfdaa7b2eb0ce67a02441dae47ae08b93fc8cade18fed1`  
		Last Modified: Tue, 13 Sep 2022 03:52:47 GMT  
		Size: 58.1 MB (58067914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacfc029773ae889d3d70c7c7a697f979aca0586699838016d7647e998071dab`  
		Last Modified: Tue, 13 Sep 2022 03:53:26 GMT  
		Size: 213.1 MB (213146380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ae6debf772cd416d3418020d444b526e6dbb85caf44ec3d847d6ece14fdddbd5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.9 MB (313920314 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:346d312be574d74cdc36cf1bba138bd96a787ab9df0c21436f66850af54f9485`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:17:35 GMT
ADD file:dd3257a03b58fae4238ad4fccb1c79ff49c76b1294f5fb6f57ecee4bb748c9ca in / 
# Tue, 23 Aug 2022 01:17:35 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 06:21:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:21:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 06:22:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 06:23:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4cd09bc891cabc28c38273b3b8e22a810888bfc449c6fd4ec5610c27492b2603`  
		Last Modified: Tue, 23 Aug 2022 01:23:14 GMT  
		Size: 51.9 MB (51911406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f224d9458f88dbd5a7ba922c9cb4a7116b314d234615e7981e233157663a02`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 9.7 MB (9741837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3836f63f5d9bf55c4350c9f89c9a7b420aa71f6408278b53d58e61634cb3fa`  
		Last Modified: Tue, 23 Aug 2022 06:28:49 GMT  
		Size: 10.9 MB (10949073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c127ba25c98f2eef6419ecfbb5bb63c8da103c1ea0298e7e61e2103424e530a`  
		Last Modified: Tue, 23 Aug 2022 06:29:16 GMT  
		Size: 55.7 MB (55747826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e249ad29978f097d481f4bfe9ce42ca0c44552bf26944aea2b847496fd0838`  
		Last Modified: Tue, 23 Aug 2022 06:30:09 GMT  
		Size: 185.6 MB (185570172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:fd0b31ddb28465a985e9b4e90815a6fa47d188e9408ecf7c3d5c831fcfc241dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **299.8 MB (299844414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72da89b2937b052cd65b23069be33ca9069f1824886bb639b596cf2a764aecb3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:44:30 GMT
ADD file:63335401d9730857a474088e836b58820d062d53a4d008379a3f0bab91891ee7 in / 
# Tue, 23 Aug 2022 01:44:30 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 13:04:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:04:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 13:04:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 13:05:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:abce9a6a026c05f336d24d7c79af29d2f108767252a4737864125c7cd16cb946`  
		Last Modified: Tue, 23 Aug 2022 01:52:08 GMT  
		Size: 49.6 MB (49637416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:789e63ee7b15faa5255a98e78ca57f7b79165de31d27f0d20a810e2e8f2f6fbe`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 8.4 MB (8404984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:866f5f3461f124a4ec2d43c116d5e4f8a2783872d85516deec64b8873fb850ab`  
		Last Modified: Tue, 23 Aug 2022 13:15:09 GMT  
		Size: 10.6 MB (10590651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519438e1fee2b230fe7b1ef7d878f221dfd76d39406a621b5ac5c6a6d9977d8d`  
		Last Modified: Tue, 23 Aug 2022 13:15:36 GMT  
		Size: 53.7 MB (53721931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116396eb184bdf4a369bbff811214de4b5044eb77672394f3d62ce8fd8b07b69`  
		Last Modified: Tue, 23 Aug 2022 13:16:25 GMT  
		Size: 177.5 MB (177489432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:bcb381e04a2732ab250a0bc43cf4a8661b7020a0b532d7bfd5bcfdd5b4366c62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **545.4 MB (545439369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18475cf95c9af1adee7cf3b17f92a8afed4f8d29ce264fe5b1d9f71f49b05775`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:53:33 GMT
ADD file:03a6abbfc4f7f5b036b595b68d32dab2760788223365adbadd691cc6b97d3f9f in / 
# Tue, 23 Aug 2022 01:53:34 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:30:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:31:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:32:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11a10710f625b85736b19b89ebf063edde4e3f2dedab0a6cc94db39e134d8cfe`  
		Last Modified: Tue, 23 Aug 2022 01:59:52 GMT  
		Size: 53.2 MB (53220635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52438f7d6f6695685610119446105c5c9522703362332bff254bc8eda29485`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 9.1 MB (9135715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c781af42aca050a89e2c2b2ae998b642dd1e62096b74d1479568d49d2b43581`  
		Last Modified: Tue, 23 Aug 2022 02:39:08 GMT  
		Size: 11.1 MB (11058895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b655e4c924d786599e6214f6298b4a90d6bb1e4e1bc66096185648662d73d55`  
		Last Modified: Tue, 23 Aug 2022 02:39:29 GMT  
		Size: 57.9 MB (57942074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4468d1c3ff674531ee48a976061d1c38abad49092b9887b6d908ec3376e65abc`  
		Last Modified: Tue, 23 Aug 2022 02:40:35 GMT  
		Size: 414.1 MB (414082050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8cd9f265050b2a89f2b0e789b66ee74878574934646dae66d370dbb1631b95b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **349.1 MB (349084797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6f5e1d87a25966aa07a6b1a0ddb507d3f52fec56499334037cc0df2fff4cf09`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:03:44 GMT
ADD file:56a765ed5b9c59576a105c4e82da61f928406a2ef950e7cada80b5c269a1acda in / 
# Tue, 23 Aug 2022 01:03:44 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 01:35:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:35:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:36:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:37:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:05690d5133887cdda89e6ae4808c08e8a92acf2163ce992d8bacbed497b1ddd7`  
		Last Modified: Tue, 23 Aug 2022 01:10:25 GMT  
		Size: 54.1 MB (54133693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6de5521fae7f54e276230f1136f3c889618c53b37f387bcb06db2c09c9ea96`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 9.5 MB (9480147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1ad46fde87250408a791d37517179cd6427cd46421e84e138f00437a005cc8`  
		Last Modified: Tue, 23 Aug 2022 01:42:35 GMT  
		Size: 11.5 MB (11473735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc96324d4abcfddd315fc320b0f834fa9ab7e220e914962ae1d8af8c95bc0b94`  
		Last Modified: Tue, 23 Aug 2022 01:42:56 GMT  
		Size: 59.7 MB (59690126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3314db2a67edcee49b0f6254dd94eccdab07b0b303150ecab178769c20454ef8`  
		Last Modified: Tue, 23 Aug 2022 01:43:32 GMT  
		Size: 214.3 MB (214307096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:44932d5ac5c7c5b4769849503ca026630ef64ad261f181908e37e315f4a6a562
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321764495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aaf48cd27b846d1c74c094bed63d9fc6bdcad9711050ce213db2592c1f435d3f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:11:52 GMT
ADD file:372730632835dde60a084d1dc5d1d8d7840a118d3aa6413f1568d2a939e39e05 in / 
# Tue, 23 Aug 2022 00:11:58 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 22:34:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:34:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 22:36:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 22:42:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6fdf476c348ab651944f6f008015e5c5184fa9f5620904fc65599b044dd5761`  
		Last Modified: Tue, 23 Aug 2022 00:20:20 GMT  
		Size: 53.2 MB (53216630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f889c0bad3c21c23d5613d840cb6194f047e7bd8b0ab913aa4c3aeb3f22ff6aa`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 8.7 MB (8666700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e682c1b586301933075fc1a74ded2cb91e71a70eb9e075ab5291aec1d56e833`  
		Last Modified: Tue, 23 Aug 2022 22:52:22 GMT  
		Size: 11.0 MB (11041861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec7b75657e271145b112803a3b136f6eba775667758887ede8d7bf5eea806dd`  
		Last Modified: Tue, 23 Aug 2022 22:53:13 GMT  
		Size: 56.9 MB (56881826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ccde40f554bb70ef53d85d915e58944b5bde8dea04124f47de1cc710a908bde`  
		Last Modified: Tue, 23 Aug 2022 22:55:22 GMT  
		Size: 192.0 MB (191957478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d31682460f32ab995f6123d1861469234e2e9cec6e306c62c4947a3ae5e3d32c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **553.9 MB (553947352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e93f9fd28ad6ce94afa2ae176b65b01afb61979bba69a588a1f8caa26f8dc039`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 01:25:10 GMT
ADD file:7b8a9c1fc05e75d845ea719c57047ae432cceb7645d270a99b117d0e4e0ffb33 in / 
# Tue, 23 Aug 2022 01:25:13 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:02:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:02:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:02:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:05:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:515f00ecba82250b75d6d9987193afd77293c07bfaf7a95ae024c05c73a8cb3a`  
		Last Modified: Tue, 23 Aug 2022 01:31:07 GMT  
		Size: 57.3 MB (57313882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:759d55c9749119adb9c0cff41513f89896055da109781a9c493c462426691120`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 9.9 MB (9892227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419401365d91198049a8c6620087ce51a751ce8891e8a184d06c31216b0773b8`  
		Last Modified: Tue, 23 Aug 2022 02:12:40 GMT  
		Size: 12.1 MB (12081297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50e6911c1af381860ef781b5463a576d34cf58ff5ca18e69333ab7d054a1d2a4`  
		Last Modified: Tue, 23 Aug 2022 02:13:10 GMT  
		Size: 62.9 MB (62860983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4d3b983d1afeef2ed30145913f73fdca87605ede854ebf973821980ed7bb889`  
		Last Modified: Tue, 23 Aug 2022 02:14:53 GMT  
		Size: 411.8 MB (411798963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0b603f88c28fb8429fd05206b79945930b5fa5ce8d8d9427b2652d28e5f11ad6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **361.4 MB (361359664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49edae0a85c7897d7dd6a29945939bd7d3f18568d25701d3e7853f7d0cf9d594`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Sep 2022 01:11:44 GMT
ADD file:cf4408ac501f6e39f1a9c7abb24ec07a6bc62afa97f48fd63879c903abfaaf4c in / 
# Tue, 13 Sep 2022 01:11:46 GMT
CMD ["bash"]
# Tue, 13 Sep 2022 01:57:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 01:58:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Sep 2022 02:03:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Sep 2022 02:13:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8cced8b0f3f30b0928735c74d8208eae12a348b798bd4253f1b4acb6d9d6728`  
		Last Modified: Tue, 13 Sep 2022 01:29:57 GMT  
		Size: 49.3 MB (49268300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cdf2efe1eb61fd0bbcf2b293d4e031b05f13a19f3ee4f9691262666970b15c1`  
		Last Modified: Tue, 13 Sep 2022 02:42:01 GMT  
		Size: 8.4 MB (8401065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f281e9cb277bf50237e9e04b09169648d24499c56aa01f94bedcadcb173d0a3`  
		Last Modified: Tue, 13 Sep 2022 02:42:02 GMT  
		Size: 11.4 MB (11435697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9f5ac0089cbc5e6a2fd5b2e4f0a87d121dfc9b18f21dfa4cbfa5fc80eea4dfb`  
		Last Modified: Tue, 13 Sep 2022 02:44:33 GMT  
		Size: 54.0 MB (54030810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ef7a6f28e22ddd1f3cc453a92dfebf08b8c3f176ed1b1d213b66b076a2c7b1`  
		Last Modified: Tue, 13 Sep 2022 02:52:05 GMT  
		Size: 238.2 MB (238223792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:3380f5eb469b98e12046ee103b120a9bc84afb65a17f38812751e1b32fd6da22
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.2 MB (499173410 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76a19518653a77d77c1c607b119f24c614cdd67c4fdc9f27f4385f192cc0ed7a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:54:14 GMT
ADD file:fb4926c73b650f18bc1eb6b58287dc0872251073fd0bc72bcd007f74315f89a5 in / 
# Tue, 23 Aug 2022 00:54:17 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 09:53:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:53:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 09:53:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 09:55:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0aaf3bb8cf1626ddbd85331fa1967c48ccf9d314270b99a2a506e53979592f79`  
		Last Modified: Tue, 23 Aug 2022 01:06:53 GMT  
		Size: 51.6 MB (51581993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b9f9f1f0cb3b7d4b45cdcacf5c7c93102c09bc71207f7dcc091136f732a622`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 8.9 MB (8943771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f6fca0053787f32630628512d8ae3f948e6ae085840b8a4083d3ac745fa220`  
		Last Modified: Tue, 23 Aug 2022 10:01:01 GMT  
		Size: 11.2 MB (11168320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e0960b87cafae9e1bf612df6c73bfb7680cbb0139fd149d5c6e367e797b282`  
		Last Modified: Tue, 23 Aug 2022 10:01:16 GMT  
		Size: 57.2 MB (57210664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886ef7d8187dc34f74cbea7c999fbf59f6940f6f469d36dc12cf47527ef36d7a`  
		Last Modified: Tue, 23 Aug 2022 10:02:03 GMT  
		Size: 370.3 MB (370268662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
