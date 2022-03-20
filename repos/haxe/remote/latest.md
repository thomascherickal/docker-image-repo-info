## `haxe:latest`

```console
$ docker pull haxe@sha256:db3c8162e8e008d35c9053847f8701771077aa6ab5594c74a9bed6eafc41b861
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.587; amd64
	-	windows version 10.0.17763.2686; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:d4813fab541705bcb5e09dabac3726ebb942e194e04737fb15eacae38030db26
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139878734 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7b6204e4ba79cdac2da5b37f2199a4c0e63f698ae5257cbefa74c3805e8fcee`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 17 Mar 2022 04:03:47 GMT
ADD file:19873be7a1c793d8edefb5d64edb99fe05ac5b1d304d167661ac3d8f21b4bd65 in / 
# Thu, 17 Mar 2022 04:03:47 GMT
CMD ["bash"]
# Fri, 18 Mar 2022 06:29:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 06:30:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 18 Mar 2022 06:30:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 06:52:46 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 19 Mar 2022 06:52:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 06:52:50 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 19 Mar 2022 06:54:04 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sat, 19 Mar 2022 06:54:05 GMT
ENV HAXE_VERSION=4.2.4
# Sat, 19 Mar 2022 06:54:05 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sat, 19 Mar 2022 06:57:26 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sat, 19 Mar 2022 06:57:26 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:5492f66d270062ddb73f28649d80eef162f2c9376d53973a3557158390af4f30`  
		Last Modified: Thu, 17 Mar 2022 04:09:37 GMT  
		Size: 54.9 MB (54922831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540ff8c0841d610e4cc2ad3b9ed4c6edcad4f5be2add8765f416515fbc2be2a8`  
		Last Modified: Fri, 18 Mar 2022 07:03:14 GMT  
		Size: 5.2 MB (5153360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0bf850a0df065fb202ebf8a3527699dc18322469c34733a6cb7f412a7aaefa6`  
		Last Modified: Fri, 18 Mar 2022 07:03:15 GMT  
		Size: 10.9 MB (10871980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d751dc38ae511bbc21c148bffa7e863057cbc7b4a8ff5155f2eca7e8d03740c6`  
		Last Modified: Fri, 18 Mar 2022 07:03:40 GMT  
		Size: 54.6 MB (54577140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d56c99d44f00d94c5d49d071cd126fdee5b87e081ff6d75f2ccd2bd566db6d2`  
		Last Modified: Sat, 19 Mar 2022 08:33:45 GMT  
		Size: 1.4 MB (1366731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9f193477c8cd2734a6fe143c1407636078d2d9f6933bf3a912e72d5a394a00f`  
		Last Modified: Sat, 19 Mar 2022 08:33:45 GMT  
		Size: 1.4 MB (1446887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e3c678a6cb2b61f4b3dce66d46c61a308ba0ef9260672fbffea9119745a1d0`  
		Last Modified: Sat, 19 Mar 2022 08:33:48 GMT  
		Size: 11.5 MB (11539805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:bd687afde4e038af22658f51c889fcc5beb2b064ed5565a54d5de8eb7f2800d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129362429 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f6ed654ec478a49de0def8554684507c7f101588a65a93a8b0e306cb321a42c`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 17 Mar 2022 09:30:27 GMT
ADD file:a76bfdf79974fef637725f4c4d8afd998baacd9f3852ac94ce4db52fd65edd8c in / 
# Thu, 17 Mar 2022 09:30:28 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:52:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:52:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 02:53:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 16:08:18 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 20 Mar 2022 16:08:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 20 Mar 2022 16:08:28 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 20 Mar 2022 16:11:28 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 20 Mar 2022 16:11:29 GMT
ENV HAXE_VERSION=4.2.4
# Sun, 20 Mar 2022 16:11:29 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 20 Mar 2022 16:16:54 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 20 Mar 2022 16:16:54 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4a0c373b7fd878320ee1d0810692c38f8079bd0783a53740b236b67ccd6eab4f`  
		Last Modified: Thu, 17 Mar 2022 09:45:54 GMT  
		Size: 50.1 MB (50122251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a9d199c77419ab8067bd77407cb0151e23cf09849e1fc7f550156c8d5ff053`  
		Last Modified: Sat, 19 Mar 2022 03:29:05 GMT  
		Size: 4.9 MB (4922780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a175e3c76032f69174aba6e645720559d1bef82bbf1946d37266a8543cec9b75`  
		Last Modified: Sat, 19 Mar 2022 03:29:07 GMT  
		Size: 10.2 MB (10216952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ef8cc586469458a5d1e2e47026303e46cf29e47935386efe16d91d34fe708c`  
		Last Modified: Sat, 19 Mar 2022 03:29:56 GMT  
		Size: 50.3 MB (50328447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c193dc76a0bbefc01063fd5e2b7e97755fe81176e04225016292e5e6b8aa95d`  
		Last Modified: Sun, 20 Mar 2022 17:31:40 GMT  
		Size: 1.3 MB (1280002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d569fa8b8da595c24c924018d6e26941e1d5b89ec2dc92bba13a2278baa052cc`  
		Last Modified: Sun, 20 Mar 2022 17:31:40 GMT  
		Size: 1.4 MB (1387664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5d9dec331b9b49fa569f6e20061c0cca19a9888291c77bb8ac84070e550886`  
		Last Modified: Sun, 20 Mar 2022 17:31:48 GMT  
		Size: 11.1 MB (11104333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:b5e26301efa48c1d5a1206da7b2a3475cdf29abf1ff1e7c7cd93e4b790cab3c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.4 MB (139403666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a3717774de53998b040df1a3d3c81feb47704c122ff4edab031ba574b0fb2fb`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 17 Mar 2022 03:21:41 GMT
ADD file:5effc7e0ab7312f14a7ee81c06c71400aae31219d477ebe1a4f7a9156797c42a in / 
# Thu, 17 Mar 2022 03:21:42 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:10:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:11:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:11:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 16:42:01 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 18 Mar 2022 16:42:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Fri, 18 Mar 2022 16:42:06 GMT
ENV NEKO_VERSION=2.3.0
# Fri, 18 Mar 2022 16:43:15 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Fri, 18 Mar 2022 16:43:16 GMT
ENV HAXE_VERSION=4.2.4
# Fri, 18 Mar 2022 16:43:17 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Fri, 18 Mar 2022 16:45:57 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Fri, 18 Mar 2022 16:45:58 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:260ad8146ed2447d5587608b10fed4f80de80cdc559e619f3a235d3ba09eaf7b`  
		Last Modified: Thu, 17 Mar 2022 03:28:04 GMT  
		Size: 53.6 MB (53616308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1399f445da611be3789923cf26d158e3f4f80449b7295fa069a8eaecaaf137e6`  
		Last Modified: Thu, 17 Mar 2022 22:20:58 GMT  
		Size: 4.9 MB (4937558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd9e43777fa6c09c341f3aa922f47b5b3ace26de1d779124afd2f1d435731d9`  
		Last Modified: Thu, 17 Mar 2022 22:20:58 GMT  
		Size: 10.7 MB (10655858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f81267e40a2df9e572fe797e45dbc086008422eb2216df18b7a91f1cf13e22b`  
		Last Modified: Thu, 17 Mar 2022 22:21:21 GMT  
		Size: 54.7 MB (54671322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327a4ffcf61a5085fc45599cb7477ed64cab07f12ae62057793f3432465f19de`  
		Last Modified: Fri, 18 Mar 2022 18:00:49 GMT  
		Size: 1.1 MB (1133699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c934b255f42d406d3fe73af8cc2337fcd564a84b3b00a48e8b6148263d29998`  
		Last Modified: Fri, 18 Mar 2022 18:00:49 GMT  
		Size: 1.4 MB (1432548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb320e7b7501f00b229daa38365bc0af34da120ec0974089d0235068432c97e`  
		Last Modified: Fri, 18 Mar 2022 18:00:51 GMT  
		Size: 13.0 MB (12956373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.587; amd64

```console
$ docker pull haxe@sha256:17a8ae5f9af5d9241d8c7a0439d05e267ca3d88e799148b68f8029c77b7f3ff2
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2249688691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07ea73ec6de0ed379e2079ce3d749af1c5fa265b6975f02d893ce4d1ece9f0ee`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 03 Mar 2022 05:02:11 GMT
RUN Install update ltsc2022-amd64
# Tue, 08 Mar 2022 20:08:18 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 14:24:01 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 09 Mar 2022 14:24:02 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 09 Mar 2022 14:24:03 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 09 Mar 2022 14:24:04 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 09 Mar 2022 14:24:05 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 09 Mar 2022 14:24:30 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 14:25:37 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:26:29 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 09 Mar 2022 14:26:30 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 09 Mar 2022 14:27:02 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:27:03 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 09 Mar 2022 14:31:03 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:31:27 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 09 Mar 2022 14:31:28 GMT
ENV HOMEDRIVE=C:
# Wed, 09 Mar 2022 14:31:47 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 14:32:06 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 09 Mar 2022 14:32:26 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 09 Mar 2022 14:32:27 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:037d5740b40414bc505c21324142a1cd3eab10c176189a9a74d1a90354ac7cd4`  
		Size: 969.5 MB (969547968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:100676d020cbb3f3df522078bdbd67f9bbdab3dee71a4ec647a43b6b2b1e0b8f`  
		Last Modified: Tue, 08 Mar 2022 20:37:10 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a2069c9cc255f33d18e9a71e269b0cc7e1cde84e7ce380bda3f2d92ec666cb`  
		Last Modified: Wed, 09 Mar 2022 16:04:21 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f97f378b52fd5b4706eb9ca878cc7897314a7bc7bbfad9e94f462e01334ea995`  
		Last Modified: Wed, 09 Mar 2022 16:04:21 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e5ccf4bb1126542da547a775e759e2ee0aa508d4990d177015667bf85772163`  
		Last Modified: Wed, 09 Mar 2022 16:04:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9785eea6109f76c966f1869923959b2bb10bcb495c65d359352c8c873899d6c`  
		Last Modified: Wed, 09 Mar 2022 16:04:19 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe001215f057b6869efaf97a83665181b696e82f41faf1029d58113b6909de9`  
		Last Modified: Wed, 09 Mar 2022 16:04:19 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec9a848317142d5c2365a13de2b7adfb682821a44542082c432e41dd973b2d61`  
		Last Modified: Wed, 09 Mar 2022 16:04:17 GMT  
		Size: 598.5 KB (598528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b5d3d0372481616d0d324b05e7f1283df13479063f2ff09717e4ac86525f28`  
		Last Modified: Wed, 09 Mar 2022 16:04:30 GMT  
		Size: 13.1 MB (13096550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb531f026137da08aae151c1432ddc7c5cbff517a78e6de506e27bb7e1e500c5`  
		Last Modified: Wed, 09 Mar 2022 16:04:16 GMT  
		Size: 519.4 KB (519360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb097b41441c535b7e43b56ff7f887b878aafc86976028bceb763ece97aad060`  
		Last Modified: Wed, 09 Mar 2022 16:04:14 GMT  
		Size: 1.4 KB (1359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c744ee1515e5ba4b2e484d210e3ab6b056a25c2e554f0e2f2c546f67e2da1b9a`  
		Last Modified: Wed, 09 Mar 2022 16:04:16 GMT  
		Size: 2.4 MB (2356107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f274bb1d795f1bf2099dfb9c07721a4a7ffd835ced80997f1d58378728b475`  
		Last Modified: Wed, 09 Mar 2022 16:04:14 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390a487182ffbdf9d4524e1c6701e89b292e700e0b8225a10224dca4d8950f76`  
		Last Modified: Wed, 09 Mar 2022 16:04:19 GMT  
		Size: 9.5 MB (9524185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5108165024b7504cb1aa95876b34adfd312b08f84bb75fe5595c185d91a7c7`  
		Last Modified: Wed, 09 Mar 2022 16:04:13 GMT  
		Size: 570.6 KB (570559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8f47b97a8c011fbe23ff93f1bce5e3ad483729ebf0ea8fa678057ce815d4ef`  
		Last Modified: Wed, 09 Mar 2022 16:04:11 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed51450328df10bcc71b7bdc33d49465843980f50d89abd6abdbca3dc29dd69`  
		Last Modified: Wed, 09 Mar 2022 16:04:11 GMT  
		Size: 575.9 KB (575859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f9ed19999af7dd05a3433766d375fe59c13fc807e4f3b67fd56070f154677`  
		Last Modified: Wed, 09 Mar 2022 16:04:11 GMT  
		Size: 580.9 KB (580942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3dc4760abeeddd8c098fd36527d0ae0ddedaf2a6b1f85b64c3b92d6611b772`  
		Last Modified: Wed, 09 Mar 2022 16:04:11 GMT  
		Size: 605.7 KB (605694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a32cc214418d668c9252ceade63ada42180b4514c14f481f37deb891019d185`  
		Last Modified: Wed, 09 Mar 2022 16:04:11 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2686; amd64

```console
$ docker pull haxe@sha256:13dcc7a5696f5a700acdbff492d19ec9a244d245a7ef82024b852376501732cd
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2741914049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1590f8c746e05aff130e18439ae2843a22a6bc3b265df2a6c760357c07aaf46`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Mar 2022 15:05:04 GMT
RUN Install update 1809-amd64
# Tue, 08 Mar 2022 20:10:01 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Mar 2022 14:32:40 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 09 Mar 2022 14:32:41 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 09 Mar 2022 14:32:42 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 09 Mar 2022 14:32:43 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 09 Mar 2022 14:32:43 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 09 Mar 2022 14:33:55 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 14:35:35 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:36:28 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 09 Mar 2022 14:36:29 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 09 Mar 2022 14:37:40 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:37:41 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 09 Mar 2022 14:42:20 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 09 Mar 2022 14:43:19 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 09 Mar 2022 14:43:20 GMT
ENV HOMEDRIVE=C:
# Wed, 09 Mar 2022 14:44:18 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Mar 2022 14:45:10 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 09 Mar 2022 14:46:04 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 09 Mar 2022 14:46:05 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0a6173b79e25f2ebc0ed51b0ac32a6f65ca5a3bbfcbeab8b74a6c24324121dea`  
		Size: 997.1 MB (997119751 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4688be73f177648e78a5e4d7da9b850d16dafa3dbf1700a2ed3e35e1ffff22ed`  
		Last Modified: Tue, 08 Mar 2022 20:38:24 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e2525ef441f87ed93ca0b157c1f8132fd78d7752c3f74862009920c0d822d7`  
		Last Modified: Wed, 09 Mar 2022 16:04:53 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb6da520c8b4a7aeebce80fbf6de166986727c9bcaeae31ee21ad6358fcfea8`  
		Last Modified: Wed, 09 Mar 2022 16:04:51 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b7625dd9f468d831f36de6ba8121b979b4df81bab8de04637be5bdcbab0aa4`  
		Last Modified: Wed, 09 Mar 2022 16:04:51 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9b02dc5f010c3afe11ce87a196cbf91009a25ec39d6650dae11662083e17cf`  
		Last Modified: Wed, 09 Mar 2022 16:04:51 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c7d70aae6f1d863c6fbc1d2befa32119e5e5367776d5a6040901ad440f0055`  
		Last Modified: Wed, 09 Mar 2022 16:04:49 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e86c564fc648e8e0bb05965c6c0cc5aa4b5d8a89d94969c3aa3a2d24bc3b70`  
		Last Modified: Wed, 09 Mar 2022 16:04:48 GMT  
		Size: 353.9 KB (353929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1343a6e3f9c04370ec18ac6ac5c932ef1a006b4164582349dcea1ea1e907644e`  
		Last Modified: Wed, 09 Mar 2022 16:05:00 GMT  
		Size: 12.9 MB (12922810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a414635fa2aedc58696dc2b97ca42f4a68cda67318ef7d68a683726e38be1bb`  
		Last Modified: Wed, 09 Mar 2022 16:04:47 GMT  
		Size: 317.0 KB (317026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7f7fb99672b0c59db114e5cd5d166a3168067b69377dc230a27e2c0400fec4`  
		Last Modified: Wed, 09 Mar 2022 16:04:45 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52361975707a20d168c7f7c6f8fc666e4259c3869bb1386436c60a5a1bbd4311`  
		Last Modified: Wed, 09 Mar 2022 16:04:44 GMT  
		Size: 2.1 MB (2149199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b15db5c152107e8dbd6b698a132574f00f9eb174880760becac10883c66cd51f`  
		Last Modified: Wed, 09 Mar 2022 16:04:43 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c6931e26ed5e6a35dc6bfc39d904f1ec67ceeb5eacd7300af45311b1f1c6d00`  
		Last Modified: Wed, 09 Mar 2022 16:04:48 GMT  
		Size: 9.2 MB (9240519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02404b2871715e3d088c2b28e13c4afc0dc605f7e97f91b7ed33353c80f50c8`  
		Last Modified: Wed, 09 Mar 2022 16:04:44 GMT  
		Size: 344.0 KB (343972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bcb5a4b484529436d7d0b08e1a8dd764d41dae9c0a986a76420c811f978a11d`  
		Last Modified: Wed, 09 Mar 2022 16:04:41 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f1e2e375bbb59d43f197602028a5e9ba52651edd83c911e4be9649069c5ae8`  
		Last Modified: Wed, 09 Mar 2022 16:04:41 GMT  
		Size: 354.4 KB (354359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a2fa3f97ca1880bbdc0918c5c0e85de8ccef8a0c2b1249db65f7eb2621f49`  
		Last Modified: Wed, 09 Mar 2022 16:04:41 GMT  
		Size: 375.4 KB (375418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:908c1824b4ed3aaed8658b4362ee3a52967d1e2ad2a08e21263b12ce8a17a802`  
		Last Modified: Wed, 09 Mar 2022 16:04:41 GMT  
		Size: 390.0 KB (390049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342b6780a10139dd06337cd775037a2853aec812215da32c3c8f66362cfc477`  
		Last Modified: Wed, 09 Mar 2022 16:04:41 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
