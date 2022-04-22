## `haxe:latest`

```console
$ docker pull haxe@sha256:5f3b86ad91f08140a484d9cc86f5c553dc61a789a71d73170512efdb355e6c9c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.643; amd64
	-	windows version 10.0.17763.2803; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:c33f203746d42c325bb9f927000c23c98e9735de611973374e957d1c2586b1b5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139907564 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f5e14f69376783dac3c89273611ebc6ff16a3c23bb4917c47b9b1c0cb501caa`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Apr 2022 04:43:15 GMT
ADD file:3a81c181c66f226bd6abd48d0c7ed8a9c599c9f521ec7229286c83161afec8c2 in / 
# Wed, 20 Apr 2022 04:43:16 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:57:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:57:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:58:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:51:19 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:51:23 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 20 Apr 2022 22:52:38 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 20 Apr 2022 22:52:38 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 20 Apr 2022 22:52:38 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 20 Apr 2022 22:55:09 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 20 Apr 2022 22:55:09 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:6aefca2dc61dcbcd268b8a9861e552f9cdb69e57242faec64ac120d2355a9c1a`  
		Last Modified: Wed, 20 Apr 2022 04:47:57 GMT  
		Size: 54.9 MB (54941777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:967757d5652770cfa81b6cc7577d65e06d336173da116d1fb5b2d349d5d44127`  
		Last Modified: Wed, 20 Apr 2022 07:05:43 GMT  
		Size: 5.2 MB (5155716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c357e2c68cb3bf1e98dcb3eb6ceb16837253db71535921d6993c594588bffe04`  
		Last Modified: Wed, 20 Apr 2022 07:05:45 GMT  
		Size: 10.9 MB (10874928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c766e27afb21eddf9ab3e4349700ebe697c32a4c6ada6af4f08282277a291a28`  
		Last Modified: Wed, 20 Apr 2022 07:06:05 GMT  
		Size: 54.6 MB (54578663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3879e1e3f754d2b11cdcfd7d36e851c7ba63cf3ce26699894779b69b4ba763`  
		Last Modified: Wed, 20 Apr 2022 23:29:01 GMT  
		Size: 1.4 MB (1367952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81104760b38dcc197fb7a9c7574be2520a80205135655e8528ed2a1ce1304380`  
		Last Modified: Wed, 20 Apr 2022 23:29:01 GMT  
		Size: 1.4 MB (1446971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10825dbe3c4eafacd1c0458e077af43bf80d26a4b55d74793bedbb6e7e1608ae`  
		Last Modified: Wed, 20 Apr 2022 23:29:04 GMT  
		Size: 11.5 MB (11541557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:a89387c040407f1e26ed7270beaf3d8dc0e11c85d5fa0acc01af16a04734b8bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129382515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d6d8d706372c76dd4690875773e3149e70240a8d5efbcf4b6219a947e5d3953`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Apr 2022 13:26:39 GMT
ADD file:1c05c50014bbd32a4cf1edd085996a8c62abc3c8969b64d2355475827a07475e in / 
# Wed, 20 Apr 2022 13:26:40 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 20:06:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 20:07:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 20:07:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 05:43:09 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 22 Apr 2022 05:43:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Fri, 22 Apr 2022 05:43:19 GMT
ENV NEKO_VERSION=2.3.0
# Fri, 22 Apr 2022 05:46:20 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Fri, 22 Apr 2022 05:46:21 GMT
ENV HAXE_VERSION=4.2.5
# Fri, 22 Apr 2022 05:46:21 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Fri, 22 Apr 2022 05:51:52 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Fri, 22 Apr 2022 05:51:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:0a2c02101ee4340d4a9ebb962e9331486e417a3835c9adefb9badd2f0c116ab6`  
		Last Modified: Wed, 20 Apr 2022 13:42:55 GMT  
		Size: 50.1 MB (50133696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:301394875428f05a3ac7068600f0d729f8c7df313e7c9574aec8362194fb4e56`  
		Last Modified: Wed, 20 Apr 2022 20:30:57 GMT  
		Size: 4.9 MB (4924850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f80b9e8049b2a4b26cc100bccded1ae7d0bc8ff2e1fa9fc7e255631328f0af`  
		Last Modified: Wed, 20 Apr 2022 20:30:59 GMT  
		Size: 10.2 MB (10218007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bb57ee492f81d7ea44b47b65fd9782dfb9241e2f5c66bd60aaba1aa5d4fcb2`  
		Last Modified: Wed, 20 Apr 2022 20:31:49 GMT  
		Size: 50.3 MB (50327803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e144c3acc21cebc51223862efae5ffdb4bf248b8f441a51bf1cc3afc6afde8bc`  
		Last Modified: Fri, 22 Apr 2022 07:07:15 GMT  
		Size: 1.3 MB (1281107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6f289c607329f1234b25b044cd934e1ec1194d13ed19f9b2cba090d9eed8cdb`  
		Last Modified: Fri, 22 Apr 2022 07:07:15 GMT  
		Size: 1.4 MB (1387811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90e4728a02a3aed95caecf2a358e466a7ab4dde3dab7af5c638a010450c60a4`  
		Last Modified: Fri, 22 Apr 2022 07:07:23 GMT  
		Size: 11.1 MB (11109241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:67596c29c0892c1a42fcf5d2e566ed64f3e699f124a46945791de37a880f59c2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139429304 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0bb7abbcb579508514359d0a65ee3c31e106c0b3530279ae4bfdb14d731c74e`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 20 Apr 2022 04:28:55 GMT
ADD file:ece192802cbdaf1a141d04f0c2e90cfd3479e5e3e82c6a00206970684494cf48 in / 
# Wed, 20 Apr 2022 04:28:56 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:44:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:44:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:44:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:08:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 20 Apr 2022 22:08:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 22:08:48 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 20 Apr 2022 22:09:58 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 20 Apr 2022 22:09:59 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 20 Apr 2022 22:10:00 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 20 Apr 2022 22:12:51 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 20 Apr 2022 22:12:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:83d5dcfea08e6927083bc886bf182fc39d87bb04b54b63002ac0c4c0b9aab682`  
		Last Modified: Wed, 20 Apr 2022 04:35:19 GMT  
		Size: 53.6 MB (53633096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cfa86b7b1aca6d694057e4d42ee1440527f41c00b9e577df729244380c9eba`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 4.9 MB (4938663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c79b19335f27cc78840bf9159e875322f3252ac06113c73756f9d4fba905f9b`  
		Last Modified: Wed, 20 Apr 2022 06:54:10 GMT  
		Size: 10.7 MB (10656971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350ecaf08eac09037b05465ab97a1b8f7bc9b7a9b1fcef900dedd7dba9bbcf4d`  
		Last Modified: Wed, 20 Apr 2022 06:54:32 GMT  
		Size: 54.7 MB (54672934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd27a88b890d17f88d1a3748e3e0f9d87879b1c1675cebe67bc3964242556aba`  
		Last Modified: Thu, 21 Apr 2022 00:32:02 GMT  
		Size: 1.1 MB (1135074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960b20a05cb475ba1a11a2834041da1a3c3c2f25a351e00a10ef969ddca85a9b`  
		Last Modified: Thu, 21 Apr 2022 00:32:02 GMT  
		Size: 1.4 MB (1432657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514595002cfd47ff2bc121031a1ed1ce8e1ac1dfdf095174f61440041d29bd99`  
		Last Modified: Thu, 21 Apr 2022 00:32:04 GMT  
		Size: 13.0 MB (12959909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.643; amd64

```console
$ docker pull haxe@sha256:0df7805447eb60ca0401661339ccc5bf8b70998b79ef5b60aab48781b88cbb08
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2255174961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7680200087a99657f87d0e7a5a69e138a4c6deb526939f7ef25b37c6e90908f1`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Sun, 03 Apr 2022 05:50:25 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Apr 2022 12:34:30 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 12:34:31 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 13 Apr 2022 12:34:32 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 13 Apr 2022 12:34:34 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 13 Apr 2022 12:34:35 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 13 Apr 2022 12:34:36 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 13 Apr 2022 12:35:12 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 12:36:18 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:36:40 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 13 Apr 2022 12:36:41 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 13 Apr 2022 12:37:18 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:37:19 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 13 Apr 2022 12:41:36 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:42:26 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 13 Apr 2022 12:42:27 GMT
ENV HOMEDRIVE=C:
# Wed, 13 Apr 2022 12:42:52 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 12:43:16 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Wed, 13 Apr 2022 12:43:17 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:dccd9e4d14d3d5a6e93f87350b903e117368ada32d711986f779b5a3ef8657cc`  
		Size: 975.3 MB (975255801 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2a5d28823cc7f2a78cb6b52a2cadb350e978705d7634adbcfbc4bd80d4637c2`  
		Last Modified: Wed, 13 Apr 2022 14:11:56 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b9796f00891fa445860de4dd056937d609ffb53116192d6960426d73e12d94`  
		Last Modified: Wed, 13 Apr 2022 14:11:53 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbf417305b769b8bc1c6a9e89de110fd8ccb215d000436440fc46b7b5b71bb6`  
		Last Modified: Wed, 13 Apr 2022 14:11:53 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec03e013902af7b47da63ccd80f18a4f56f2a2ccc1abfec4f5b68abb3dff5b0d`  
		Last Modified: Wed, 13 Apr 2022 14:11:53 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d5ece452e79d5da6de4ae0a8ccea3e78cfb6f891425190b1e0bd6ddc7a03ad7`  
		Last Modified: Wed, 13 Apr 2022 14:11:51 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09cb02cf499e53ff17901bb0b082d79bb2175b75dccd8db84743b83ab943761`  
		Last Modified: Wed, 13 Apr 2022 14:11:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29055a526ceed7f09d80bbf647ac6d147e47740acbdb219b7b3912bcbda632d5`  
		Last Modified: Wed, 13 Apr 2022 14:11:51 GMT  
		Size: 627.9 KB (627870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97160166a348858cfa09390bfcad35ec1d92cbd86cc498279aee4ea71e30c50e`  
		Last Modified: Wed, 13 Apr 2022 14:12:03 GMT  
		Size: 13.1 MB (13146368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8c62c2be0bcac1e7216496d0dc46e42f362f334c992a270394138fb2ae399a5`  
		Last Modified: Wed, 13 Apr 2022 14:11:48 GMT  
		Size: 570.2 KB (570215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa21c37c8237ebdb7d3edf04f1daf57f440127410ecd95add38d76b8bd2fbb42`  
		Last Modified: Wed, 13 Apr 2022 14:11:47 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fe85893018d2471914c02d786d01de7a57f06097caabc39b12e32f83c93765`  
		Last Modified: Wed, 13 Apr 2022 14:11:48 GMT  
		Size: 2.4 MB (2422977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9611215d1df57989bb45945a94a7aa2734f0071052888710bfd6304ceee3ca2e`  
		Last Modified: Wed, 13 Apr 2022 14:11:47 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98456a23904dc75d4916cd91e21a8c54f48cbb572d7017a0dcc6d7e583867166`  
		Last Modified: Wed, 13 Apr 2022 14:11:58 GMT  
		Size: 9.6 MB (9574302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90cb3f653dacc51d3983853c00892ed7c5e684fac280bf7ab42f2a596ba06ec`  
		Last Modified: Wed, 13 Apr 2022 14:11:45 GMT  
		Size: 615.8 KB (615793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d73d9421e85426958f393f27585c65c29d9c21cf695ef99bf95e29d8ff54f7e`  
		Last Modified: Wed, 13 Apr 2022 14:11:44 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d9e389fa29d7ad6796a8bbd280a50ffc16fe5bc12e057af4f22548b272a690`  
		Last Modified: Wed, 13 Apr 2022 14:11:45 GMT  
		Size: 621.8 KB (621791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77a7e101fe46f710f1a2790101a22583f2803b692b925e4e7333bde115b08d9c`  
		Last Modified: Wed, 13 Apr 2022 14:11:45 GMT  
		Size: 626.7 KB (626690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0b01bd407b8cb9386976b423cad442715c0459a56b6ccde6c9ed9d26932730`  
		Last Modified: Wed, 13 Apr 2022 14:11:44 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2803; amd64

```console
$ docker pull haxe@sha256:208a07ef1596177ad3faff7042ad2933a0e092fe9df639b89f0c2817adb1ceb7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2742115269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:275ff24d833bf9c34a94a89196385a4cefe06885e1418ee4a6f14f43823de205`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 04 Apr 2022 11:20:25 GMT
RUN Install update 1809-amd64
# Wed, 13 Apr 2022 12:43:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 13 Apr 2022 12:43:33 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 13 Apr 2022 12:43:34 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 13 Apr 2022 12:43:35 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 13 Apr 2022 12:43:36 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 13 Apr 2022 12:43:37 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 13 Apr 2022 12:44:38 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 12:46:32 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:47:29 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 13 Apr 2022 12:47:29 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 13 Apr 2022 12:48:44 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:48:45 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 13 Apr 2022 12:53:46 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 13 Apr 2022 12:55:00 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 13 Apr 2022 12:55:01 GMT
ENV HOMEDRIVE=C:
# Wed, 13 Apr 2022 12:55:57 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 13 Apr 2022 12:56:58 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Wed, 13 Apr 2022 12:56:59 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ba8181afd4264392fbbf8df14fb4cddc55fbe085ab000e986b789678bc2bb171`  
		Size: 997.6 MB (997587446 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:7ebb23aa64bff633cfa3c62b190d84f0e870b04fecb1910f65d0870b5c7f8981`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bda8f18f987ede083484f6055546d8bb17b08e8b96d2818d553da3da4e46e38c`  
		Last Modified: Wed, 13 Apr 2022 14:12:24 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95e56d7dba37ae2352c0d7fe59fa7201538c2fe4b87b62bfe3921e3946d8ac4`  
		Last Modified: Wed, 13 Apr 2022 14:12:22 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1186b514c1f5d38a16595e17bf06e24a59e74167d459e902ded03f40170e84ff`  
		Last Modified: Wed, 13 Apr 2022 14:12:22 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d165e34f8b68ff2a6c18409dacd4019ff67dfb40e8e0e6e8f2c316e42b0cc843`  
		Last Modified: Wed, 13 Apr 2022 14:12:21 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8bc44ec145faa9d56e3c976085f883c677e7e74b6247f276f940d8348fb6966`  
		Last Modified: Wed, 13 Apr 2022 14:12:19 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b5e7cb2f9e9734639336d670a35a94a8855e3e6a857f24473c0a9f48c50ddf`  
		Last Modified: Wed, 13 Apr 2022 14:12:20 GMT  
		Size: 363.7 KB (363747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9262018838a295d99c4938f4be0acb935d54dc4ca8bad136ec06a62fdf5598a`  
		Last Modified: Wed, 13 Apr 2022 14:12:33 GMT  
		Size: 12.9 MB (12937586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bba721f197dcc3535dd2b6fb2773eb9bd3a2d2b04542bfc78c275bbda19b5799`  
		Last Modified: Wed, 13 Apr 2022 14:12:17 GMT  
		Size: 330.6 KB (330555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70d9c9768adb9901e8db4e57004acce5b73002fd634fedb0bef1b15ac1ac359`  
		Last Modified: Wed, 13 Apr 2022 14:12:17 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6d389552db3da75529bad43643076013357360f2c75991f6d5fe796dfa2f622`  
		Last Modified: Wed, 13 Apr 2022 14:12:19 GMT  
		Size: 2.2 MB (2163990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6783e117f5a42da309365175a4a8b33eb3cff44292e3e1534a94055ef09830a2`  
		Last Modified: Wed, 13 Apr 2022 14:12:16 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12eab6bcd2c4a1ec2ec332ca1f6a73e70b9eaaa8e3f19859620e3e31ef1e08bc`  
		Last Modified: Wed, 13 Apr 2022 14:12:21 GMT  
		Size: 9.3 MB (9261019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d732b5c1adc8fb3076743a2aa901bff5f458048ff0fba8d39f2d517e2e5b7dc2`  
		Last Modified: Wed, 13 Apr 2022 14:12:14 GMT  
		Size: 358.7 KB (358691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c45a7ebc08eccdae65db58b36e613da8c5026eeca5804b1c209e3adce869d3bc`  
		Last Modified: Wed, 13 Apr 2022 14:12:14 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d9743fab55fcd1438fefc9d0f84405f920c3b0018f4e799eddafbb52895815`  
		Last Modified: Wed, 13 Apr 2022 14:12:14 GMT  
		Size: 370.0 KB (370016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca514ed5b7b7298dc7bedbdf4b02172537c7c9d20a9f3e826a7be422a8e39a3f`  
		Last Modified: Wed, 13 Apr 2022 14:12:15 GMT  
		Size: 395.2 KB (395222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0c6533f55d2ad8905503359a11c80509a2bbc4554cf396d86b2a205931e9a23`  
		Last Modified: Wed, 13 Apr 2022 14:12:14 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
