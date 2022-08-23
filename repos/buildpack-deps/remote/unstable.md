## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:69b3b7958eb5c095143cebb78552da3ca1cd0257f13b193e7a99f2144058a0dc
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
$ docker pull buildpack-deps@sha256:82d0d6d789a9d69e6ccfb63feae242155bb785aabec9d1e662cd8fc14bb54548
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **555.9 MB (555872054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9a609cc81c34f54d9832c5a0065808f39e2800dc81394bbdc99d0e1c4105fc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:21:39 GMT
ADD file:0ded1ec762355d6c32b4a9f1eff5fbd5e60d15824d6bde678ef85cbdd03fe0ce in / 
# Tue, 23 Aug 2022 00:21:40 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:50:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:51:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 00:51:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:52:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6649fedb76d916c1041e321eca86994acdb4cd14cc61ef93b5d2a397c15af4ad`  
		Last Modified: Tue, 23 Aug 2022 00:26:41 GMT  
		Size: 52.8 MB (52768784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52383a4258951f21b40d1c18a5c708ecfd3cc7f76838fc8fbe3c1fa248f7b133`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 9.3 MB (9302218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8bf82596b529ddf3a818d599c3bed1bef1e54925ac4df0a1a6bf6467ce1bd2`  
		Last Modified: Tue, 23 Aug 2022 00:57:51 GMT  
		Size: 11.3 MB (11274041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f934be4bad0fbf951546a8aaa20f158e16a48d2a373a3b5cab06448c354bae14`  
		Last Modified: Tue, 23 Aug 2022 00:58:09 GMT  
		Size: 58.1 MB (58057519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a459942b0771eb68ff654a202259ff2306d2ca50d850f5595b425216a794380`  
		Last Modified: Tue, 23 Aug 2022 00:59:13 GMT  
		Size: 424.5 MB (424469492 bytes)  
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
$ docker pull buildpack-deps@sha256:f65c062dad155784f1db4ae20b840c286a7a1358e895f7104323cc43018e42ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.9 MB (493899488 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e85fe1b0724a32203a7777cc4b0bc595334bbdc7bbb336aa30862fa968a59231`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:00:45 GMT
ADD file:a1d27fd37cd41b3026c10df50adfd5a93a40194548a87a372c97149f63b096b3 in / 
# Tue, 02 Aug 2022 01:00:46 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:50:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:50:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:51:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:52:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:23e34b183a37464e321571d2a75fa33fded0e5a8506066db5c4f20153a665c2c`  
		Last Modified: Tue, 02 Aug 2022 01:09:03 GMT  
		Size: 49.7 MB (49735351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af50b5c584586bbf2589138734167dd8e14560e75cd854cd9bca75019a3f530b`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 8.4 MB (8423017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4818fead9ad7b4ed572aa86d08f341272cc2cbb418cbe22f7f7d71f2be3778d`  
		Last Modified: Tue, 02 Aug 2022 02:12:03 GMT  
		Size: 10.6 MB (10589650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd163d2eebe4936202350772d43aa0c00eba5ca32eca150d0f23e01feae220c5`  
		Last Modified: Tue, 02 Aug 2022 02:12:28 GMT  
		Size: 53.4 MB (53362005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed71a925d384b4f3b392cd9ba839a4b122f4d360d9712ecacca6706b586cc1d`  
		Last Modified: Tue, 02 Aug 2022 02:13:43 GMT  
		Size: 371.8 MB (371789465 bytes)  
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
$ docker pull buildpack-deps@sha256:0421ab38dfce253136a79f68b758068d850da17fb98cab8852459b5ee1656115
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **581.7 MB (581725849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:368ea79eb10d4c2651a045b86a7b46034491e02579dd7f596cdbbd107aae4683`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 01:13:16 GMT
ADD file:6165703835b4dbffafda027e272e21bf37cfc276085814fa1d03c1db0162e605 in / 
# Tue, 02 Aug 2022 01:13:21 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:11:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:11:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 02:13:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:20:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:71112f7b4dfd928d54aaa23ee1023fef50d2dc747bf6e2168afe69932ce8aa1a`  
		Last Modified: Tue, 02 Aug 2022 01:24:23 GMT  
		Size: 53.3 MB (53305987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523353756f561bdc5914e25ea1cfeda5bc330e894285664b88d8ce11aa594a29`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 8.7 MB (8659688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2258650534e83b3efae8fb3f1ce269322b09b63e553775a7c0b8c8104b2451b0`  
		Last Modified: Tue, 02 Aug 2022 02:30:34 GMT  
		Size: 11.0 MB (11041802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e365e2051b826228522cde5e4dc082e794b8ccbcf39513ac4bb385212b6277`  
		Last Modified: Tue, 02 Aug 2022 02:31:24 GMT  
		Size: 56.3 MB (56282656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c83aed82ba7c9d114a345b104ffde9472e9a1ffe42aca05f8d441ae514b3eeb`  
		Last Modified: Tue, 02 Aug 2022 02:35:57 GMT  
		Size: 452.4 MB (452435716 bytes)  
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
$ docker pull buildpack-deps@sha256:89615e24846bec4e9c2210ffa40781e7fe3b0bb100785fb53d9f3d9771959639
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **355.2 MB (355224975 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64060694992efd7dc9bad5501308cc2bafe39fcf7438d5a09721771171d1ed27`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 23 Aug 2022 00:12:03 GMT
ADD file:beb3c4d0f1887ccbbe2b266a156b7658d2e1d7d48cbcd416a0410554dfafdf12 in / 
# Tue, 23 Aug 2022 00:12:06 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 00:58:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 00:59:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 01:03:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 01:12:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:11998c1ffc96119253ef35ecbcfd66c2cb0d69f51a294f603a54496ec02d329c`  
		Last Modified: Tue, 23 Aug 2022 00:30:27 GMT  
		Size: 49.3 MB (49268189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237ee2e31cf68d3cd2675680cbf1e3c574c76f74440375dc1b8c1ad1d3d9768e`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 8.4 MB (8399080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e69eb487c5f4d1ba65732a0b11d3a69780177b7ed0357581fce4eb347813a643`  
		Last Modified: Tue, 23 Aug 2022 01:41:12 GMT  
		Size: 10.7 MB (10659901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3572ed314e6c0604916ece49e3a546ec2fcc60391daae870152b56b8fdc14d98`  
		Last Modified: Tue, 23 Aug 2022 01:43:43 GMT  
		Size: 54.0 MB (54034717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a20268cb682347428f2402e200fcf1a6f64026d72fa43eb8b171c47218c4e398`  
		Last Modified: Tue, 23 Aug 2022 01:51:06 GMT  
		Size: 232.9 MB (232863088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b5e5eb2e89ee6e720e75ca36a2281597de240ce21f5fb250d6f6a256010ea03e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **500.5 MB (500475359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa54a4ef283eb54a28dd4bc552330112a16ce9eabe3b5915b94536263ff3032`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 02 Aug 2022 00:43:36 GMT
ADD file:19dee33de85aac92620de3bd92768833a889db0b60b7445419bccb4285c46f94 in / 
# Tue, 02 Aug 2022 00:43:39 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:12:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:12:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:13:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:31888e988211ae2cd4058438d0fd3d3420a26d35f21e97741527c1e85ad2d476`  
		Last Modified: Tue, 02 Aug 2022 00:49:29 GMT  
		Size: 51.7 MB (51734666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dd60a4351ebe5fad9f32c09d0a6f7ec29b6c6dcb5ff8c29e6650149557447e2`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 9.0 MB (8960873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440b0db795ce4385e2a159326c7d9ab52e109942607b82b1c377894e874e601d`  
		Last Modified: Tue, 02 Aug 2022 01:36:55 GMT  
		Size: 11.2 MB (11166864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6891cb8548d01d5cd140a6d90fa3462f4433c9891f74f6d5405b9556edaca1a0`  
		Last Modified: Tue, 02 Aug 2022 01:37:13 GMT  
		Size: 56.9 MB (56935914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9889f124f3e95bd877e0a305131f335147bbe379811baf82c7a74227c39adac0`  
		Last Modified: Tue, 02 Aug 2022 01:38:00 GMT  
		Size: 371.7 MB (371677042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
