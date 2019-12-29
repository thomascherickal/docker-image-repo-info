## `haxe:latest`

```console
$ docker pull haxe@sha256:0706a44e0b39fbda5315cf65cb404b67fa5897481a282a8f44c5de9017f5ea3a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.914; amd64
	-	windows version 10.0.14393.3384; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:32be548b470107ac9d413117e3030bacbd3bfe2c20d47bbbe3577b4d30010dd0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131946551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a96d2bc60ca1a7cf3284c1bc8d1da76129b60623799ea6b73d4037bceafe570`
-	Default Command: `["haxe"]`

```dockerfile
# Fri, 22 Nov 2019 14:54:40 GMT
ADD file:9b7d9295bf7e8307ba4e81ce20770256b964da70dea966568b3515ad026d0b27 in / 
# Fri, 22 Nov 2019 14:54:40 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 00:00:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 00:00:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 23 Nov 2019 00:01:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:45:17 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 23 Nov 2019 16:45:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sat, 23 Nov 2019 16:45:23 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 23 Nov 2019 16:47:08 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 18 Dec 2019 00:26:04 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 18 Dec 2019 00:26:05 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 18 Dec 2019 00:28:55 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 18 Dec 2019 00:28:55 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:16ea0e8c887910fe167687a0169991b4c1fc165257aab6b116f6a5e61a64e7af`  
		Last Modified: Fri, 22 Nov 2019 15:02:34 GMT  
		Size: 50.4 MB (50379708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50024b0106d53dcbd29889c65bc040439b2bb8947dac16c8c670db894a2c5ba6`  
		Last Modified: Sat, 23 Nov 2019 00:17:22 GMT  
		Size: 7.8 MB (7811508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff95660c69375e19e287b2ea87ca9b4be008cd036e95d541515262b86cc521d9`  
		Last Modified: Sat, 23 Nov 2019 00:17:21 GMT  
		Size: 10.0 MB (9996013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c7d0e5c0bc204b3a36e3f8ff320741da0bd0225e0a67e224c6265c1e208f80a`  
		Last Modified: Sat, 23 Nov 2019 00:17:43 GMT  
		Size: 51.8 MB (51786970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4e2e157ce50f9182214c51a35ffc89b45a806fefecb4c123a8c851c06bac30`  
		Last Modified: Sat, 23 Nov 2019 17:33:05 GMT  
		Size: 1.3 MB (1310687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a05df382bee4957733089362d0cbf07c9df598fe0450d80659aa4f2d484ccf36`  
		Last Modified: Sat, 23 Nov 2019 17:33:06 GMT  
		Size: 2.3 MB (2307033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c9bef00f9671f0b8debaf3a40eb790fa7a6c31c3e3d3e6a003ed2d46ac9ca2`  
		Last Modified: Wed, 18 Dec 2019 01:00:27 GMT  
		Size: 8.4 MB (8354632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:6ec09f224b91ad3850990f8ad6ca91ff2fa55040c463386198363983f59b578d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.1 MB (121149416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a5e24b381e30eb154354561cf90146e7901921b412f78a3154d49ae2d1ea8ae`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:43:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:43:30 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:44:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:36:36 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 23:36:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 23:36:48 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 28 Dec 2019 23:40:11 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sat, 28 Dec 2019 23:40:13 GMT
ENV HAXE_VERSION=4.0.5
# Sat, 28 Dec 2019 23:40:14 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sat, 28 Dec 2019 23:47:28 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sat, 28 Dec 2019 23:47:29 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93dc761fecef183bb949ae59f45d1f618cc3e8879cb25946ab48737d1d8a59b0`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 7.1 MB (7096250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73181b0fe903be79034378988be75730f983b13ada732a04ea4f46f73b332896`  
		Last Modified: Sat, 28 Dec 2019 07:07:06 GMT  
		Size: 9.3 MB (9343271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870abc97e939a1f3c484e5c9aec16d33497f3603c57bd4581d15915528703890`  
		Last Modified: Sat, 28 Dec 2019 07:07:28 GMT  
		Size: 47.3 MB (47315646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e56fc17b53aadccefb46bb89432dfb4ad06d0fe6c77bb9d5c7f880fee85710f`  
		Last Modified: Sun, 29 Dec 2019 00:23:14 GMT  
		Size: 1.2 MB (1232774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af450a211c43cb407d6f318a157bc6e27503132d08fe037d9e77921384f8dbd5`  
		Last Modified: Sun, 29 Dec 2019 00:23:14 GMT  
		Size: 2.2 MB (2249302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8d73ca888a5cfbb27347c29b2f31d652c8b321d1b9701525ca3ddb0531f9d20`  
		Last Modified: Sun, 29 Dec 2019 00:23:17 GMT  
		Size: 8.1 MB (8052545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:234de6e80813a3edbdc15b89c647a31ee7615f89783e8b9eeb41e559556417cd
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132892294 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4695d8a7d7cdf63bd4c6d3376deec59c7e6b37776f884ce3ad6ae22052ad6442`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:04:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 28 Dec 2019 06:05:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 02:41:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 29 Dec 2019 02:42:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 29 Dec 2019 02:42:10 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 29 Dec 2019 02:47:25 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 29 Dec 2019 02:47:26 GMT
ENV HAXE_VERSION=4.0.5
# Sun, 29 Dec 2019 02:47:27 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 29 Dec 2019 02:53:55 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 29 Dec 2019 02:53:58 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6ac1923ab7a97ecdde2a4f034a8b716d51594ba6fc823c6aaac579c31f51906`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 7.7 MB (7681148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b000e01546d5b9b3a40a3797f15bc0a1f579786c5ec8da31cbe9502f1927d367`  
		Last Modified: Sat, 28 Dec 2019 06:21:16 GMT  
		Size: 10.0 MB (9983835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc8fe6ebd465d85dc79039fbd39712f1fadf5d7ac5fbefe405ef7a4f957a94ce`  
		Last Modified: Sat, 28 Dec 2019 06:21:39 GMT  
		Size: 52.1 MB (52102816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ff4d8b72f1f0c43345bb772c4e63e588f7c34bd6326ec6f55c459edc3b9503a`  
		Last Modified: Sun, 29 Dec 2019 03:31:12 GMT  
		Size: 1.3 MB (1301844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26205a484c349c37e7a2b6dc4e8ce699816e2b22ba6e21d4476e2c609a32f13f`  
		Last Modified: Sun, 29 Dec 2019 03:31:12 GMT  
		Size: 2.3 MB (2303755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db68ec685108b11eb9fbe14647ca2e28236f36e0cfdff93c9fde583f8d9e7f6`  
		Last Modified: Sun, 29 Dec 2019 03:31:13 GMT  
		Size: 10.3 MB (10347020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.914; amd64

```console
$ docker pull haxe@sha256:e4c029c468c31a0dd38527eb66cbfe7d366c5f63ad80fae62682d4c3cc7383e0
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2249244348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1e7a05b25dfbc911ac90cb0f41fe5abd8b11612599c69115b03aa27c3a92f82`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 29 Nov 2019 04:34:15 GMT
RUN Install update 1809-amd64
# Wed, 11 Dec 2019 14:56:24 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 14:56:25 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 11 Dec 2019 14:56:27 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 11 Dec 2019 14:56:28 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 11 Dec 2019 14:56:29 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 11 Dec 2019 14:56:30 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 11 Dec 2019 14:57:15 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Dec 2019 14:58:27 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 14:58:52 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 11 Dec 2019 14:58:53 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 11 Dec 2019 14:59:33 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 00:20:50 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 18 Dec 2019 00:25:26 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 00:25:47 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 18 Dec 2019 00:25:49 GMT
ENV HOMEDRIVE=C:
# Wed, 18 Dec 2019 00:56:20 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Dec 2019 00:56:43 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 18 Dec 2019 02:51:53 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 18 Dec 2019 02:51:54 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:faf31ee0aa3d3c60a38dd03c7554d632065cef50eab052ef1444590786249d07`  
		Size: 681.6 MB (681618026 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6095b83882ccf9b8fa968e24adeb7b300cf94138c6c34f21c5d0425dc8a63803`  
		Last Modified: Wed, 11 Dec 2019 17:59:52 GMT  
		Size: 1.2 KB (1162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0ef265483c55cd7da66e93c38349c14181390c9b0f7a03184e94d5ae891aa1`  
		Last Modified: Wed, 11 Dec 2019 17:59:52 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a051857c9fb004b4a19669e3808328a717f3696ea52fcc34870f575f04fc41d`  
		Last Modified: Wed, 11 Dec 2019 17:59:51 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99d67a5c5687fc2e62d4d04181ed090c8c3f50d85c0fd78cc6247d1c2ba6085`  
		Last Modified: Wed, 11 Dec 2019 17:59:51 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8540b851618b7bae77ab211f4c08828c1da97c1c9bb696f0a4dad6ac33f3a078`  
		Last Modified: Wed, 11 Dec 2019 17:59:50 GMT  
		Size: 1.2 KB (1211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4cab78afaca635c7a0a1776575961cc75fdb0aee1bc550bda75ded0896eef2`  
		Last Modified: Wed, 11 Dec 2019 17:59:48 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d975cbe50b3ea9a761a9fc8dcafc69b10a98164bbd1b204f08625b9f31567976`  
		Last Modified: Wed, 11 Dec 2019 17:59:49 GMT  
		Size: 4.6 MB (4576526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9f5076043a1655cd87980d5f63c3ab2ff9ca11472166fe291b154bdcdca9396`  
		Last Modified: Wed, 11 Dec 2019 17:59:50 GMT  
		Size: 12.9 MB (12921896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f6ceed09ae73f88afbf5043074801a8102c5f2109f542d26d77b7798e41f5d`  
		Last Modified: Wed, 11 Dec 2019 17:59:47 GMT  
		Size: 321.0 KB (320985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:105bfaf430ce4b7b06c9e02cea99a0372516016b27ecc344f9d08762b7f4008b`  
		Last Modified: Wed, 11 Dec 2019 17:59:43 GMT  
		Size: 1.2 KB (1175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83c48ed25a4cadb16680120bcf4e09da2f50f68a7159a626fccd347ddd6f084b`  
		Last Modified: Wed, 11 Dec 2019 17:59:45 GMT  
		Size: 2.1 MB (2148926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25725206bcf68829eb653349a92f610815b8044be99f8dd2a14e500d2e9ffd55`  
		Last Modified: Wed, 18 Dec 2019 02:53:36 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a166690f344c8ee3031fcc9b018b773d432117776643e6fefb43709916bb2e8d`  
		Last Modified: Wed, 18 Dec 2019 02:53:57 GMT  
		Size: 11.5 MB (11508014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37672d5859da7f4e8c8bf8fff8f8b2d1623e2107e03122a88f608ba12a8ca230`  
		Last Modified: Wed, 18 Dec 2019 02:53:35 GMT  
		Size: 348.6 KB (348637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ed5bfc9dea7f6a4a5fdefb22342ace2b985ebe48f19f4699e1c225818db3ae`  
		Last Modified: Wed, 18 Dec 2019 02:53:31 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a45b11617feb90be9ea34ffbc59a71ac932335d03e61720076bcbeb3ec6b8930`  
		Last Modified: Wed, 18 Dec 2019 02:53:31 GMT  
		Size: 352.1 KB (352080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8aff52c11a3c4e78f99d22e28f9c0345416ef3fd843d90f7a77184f10e59ad9`  
		Last Modified: Wed, 18 Dec 2019 02:53:31 GMT  
		Size: 369.9 KB (369905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413d60e3a5c58ffe3f6215840b94012e0f97ca1fd0778c69f3bde46ae0e9bb0a`  
		Last Modified: Wed, 18 Dec 2019 02:53:31 GMT  
		Size: 382.2 KB (382162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7f1650df81741b36b960e391fee2a0ac5e2ebf910322a8d5206636e85d02c65`  
		Last Modified: Wed, 18 Dec 2019 02:53:31 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3384; amd64

```console
$ docker pull haxe@sha256:f7057b54eb3187f792432e7dc6b73add2fffa30a0f8599cd557b050d34afe6d8
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5800781195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ae4f9b54392d537e63de0de18eb8a064bfb17a9bff13f5382a6ca588028bea`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Nov 2019 14:43:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Dec 2019 15:47:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Dec 2019 15:47:06 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 11 Dec 2019 15:47:07 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 11 Dec 2019 15:47:09 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 11 Dec 2019 15:47:10 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 11 Dec 2019 15:47:11 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 11 Dec 2019 15:48:35 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Dec 2019 15:50:37 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 11 Dec 2019 15:51:41 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 11 Dec 2019 15:51:43 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 11 Dec 2019 15:53:12 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 01:57:12 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 18 Dec 2019 02:02:26 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 18 Dec 2019 02:03:28 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 18 Dec 2019 02:03:30 GMT
ENV HOMEDRIVE=C:
# Wed, 18 Dec 2019 02:04:35 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Dec 2019 02:05:44 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 18 Dec 2019 02:06:53 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 18 Dec 2019 02:06:55 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:55d044e60c8959ce88aee467913bb11827c1ec057a2fd108a293e274dbd74f1d`  
		Size: 1.7 GB (1652717978 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d23dffb4f7b6ebd1cceaac955d664d79467da76c4749d2a37d98556996d8bb0a`  
		Last Modified: Wed, 11 Dec 2019 18:01:38 GMT  
		Size: 1.2 KB (1206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:578736d491bc62a9ba84bf67b0f0c9b9aa1fb4a336436f1d85d867c40b9fba91`  
		Last Modified: Wed, 11 Dec 2019 18:01:37 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e98cae39e78ecccced45ff44c0f67911b1698b1691796b479326f2a06e8acf8d`  
		Last Modified: Wed, 11 Dec 2019 18:01:37 GMT  
		Size: 1.2 KB (1203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59d589c064df5b9c5c3b56817bb6455a68c3fd56cfc73e96408af7864c95a4f4`  
		Last Modified: Wed, 11 Dec 2019 18:01:36 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb71cf8321e0a37285f08347e04a8fa8c0ef050cba65610397ddb9679347592c`  
		Last Modified: Wed, 11 Dec 2019 18:01:34 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535dabcafe68f916176cce244deb58bc5dec10bc1586d79e951aac6c1c92cb8a`  
		Last Modified: Wed, 11 Dec 2019 18:01:34 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f902dc18a6a313b2c448810ba6d93cb868038db8b7eeb37c796cd43ed77dbe65`  
		Last Modified: Wed, 11 Dec 2019 18:01:33 GMT  
		Size: 5.4 MB (5361611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e60ba2427e6cf8f8857f93342d6f39853555f70d5c0271fd24b6cc9a4cf4031`  
		Last Modified: Wed, 11 Dec 2019 18:01:36 GMT  
		Size: 22.4 MB (22365534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c531188f7c61919057e84f56ff43133f0393f5261395c34efa29815959ba43d`  
		Last Modified: Wed, 11 Dec 2019 18:01:31 GMT  
		Size: 5.3 MB (5303654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d08673b81d7f2ad04f242de6c35726b371a544e7be546a73b1f1193fb6a53463`  
		Last Modified: Wed, 11 Dec 2019 18:01:25 GMT  
		Size: 1.2 KB (1205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a1085a1b8efea2f9551c2e69d192d1907f2df7b945c6aeda58c9b541e714579`  
		Last Modified: Wed, 11 Dec 2019 18:01:28 GMT  
		Size: 7.1 MB (7128526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b56a9fd2f47e6592bb20f1e32d2753d1ad1ace3d734dce3e7a48738ffba641e`  
		Last Modified: Wed, 18 Dec 2019 02:08:54 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fadf93dbbbfdd71ec9f7907f84252afd4565ecd8bda481e3cccfb8d074e94dc`  
		Last Modified: Wed, 18 Dec 2019 02:09:16 GMT  
		Size: 16.6 MB (16623356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cf872287ef2b6536493da088a8d9ebbbc0d047108a27080d6e458c23c806b1`  
		Last Modified: Wed, 18 Dec 2019 02:08:54 GMT  
		Size: 5.3 MB (5318923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb15e126a693f3af0203e5e7455534940ac4780211081efa5f70368295d9c52`  
		Last Modified: Wed, 18 Dec 2019 02:08:49 GMT  
		Size: 1.2 KB (1187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c8fb3d42db3c57e13bc4678f20b5f96f0a463720e4f4cd63d0d157407330c6`  
		Last Modified: Wed, 18 Dec 2019 02:08:51 GMT  
		Size: 5.3 MB (5317954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601591ac44f0f1f3ef3eb7e01c3d686a44a585e0ed6617ef5bebbbbc8bce662d`  
		Last Modified: Wed, 18 Dec 2019 02:08:50 GMT  
		Size: 5.3 MB (5322263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51422cff48894cd9bb2046f8c5a8b9e14f478335506f8a245024c0490706e0ab`  
		Last Modified: Wed, 18 Dec 2019 02:08:51 GMT  
		Size: 5.3 MB (5323599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb0528e3f759b2f2078f072718d764a6b32263c6cde075a965c5e2b8b3317f13`  
		Last Modified: Wed, 18 Dec 2019 02:08:49 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
