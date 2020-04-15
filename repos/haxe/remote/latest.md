## `haxe:latest`

```console
$ docker pull haxe@sha256:b57fae347317063cec7d4fdd494c162a4c71c6f71ab9430184f20d90137187d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1158; amd64
	-	windows version 10.0.14393.3630; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:00952255d486c06a70061f1d429fa6ccd0b4894c621e2ca4c5a0a9232d291777
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.0 MB (131954243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec3ef83e02c8e7c102c7c1aebe541c30c372cf6ec4d1c4182cd7dbd602b944a2`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 31 Mar 2020 01:20:44 GMT
ADD file:c027885123a178148eb4f51f10f4924740859f1f6e941e55580517f6d234e935 in / 
# Tue, 31 Mar 2020 01:20:45 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 01:56:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 01:56:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 01:57:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:26:21 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Apr 2020 00:26:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 01 Apr 2020 00:26:27 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 01 Apr 2020 00:28:22 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 01 Apr 2020 00:28:22 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 01 Apr 2020 00:28:23 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 01 Apr 2020 00:34:55 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 01 Apr 2020 00:34:55 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:f15005b0235fa8bd31cc6988c4f2758016fe412d696e81aecf73e52be079f19e`  
		Last Modified: Tue, 31 Mar 2020 01:26:22 GMT  
		Size: 50.4 MB (50382041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41ebfd3d2fd0de99b1c63aa36a507bf5555481d06e571d84ed84440d30671494`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 7.8 MB (7812166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b998346ba308e3362a85c7bf7faed28d0277c68203696134192fe812f809abb2`  
		Last Modified: Tue, 31 Mar 2020 02:09:57 GMT  
		Size: 10.0 MB (9996302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01ec562c947a8ca1b168415da6a4a8f8920808f9b5d6f420ef8fa9af249b1f1`  
		Last Modified: Tue, 31 Mar 2020 02:10:13 GMT  
		Size: 51.8 MB (51790297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:604cf1656545406db853dff017a371f04d6cca7f06d92e6ff58ed49e864a4335`  
		Last Modified: Wed, 01 Apr 2020 01:23:11 GMT  
		Size: 1.3 MB (1311105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565c7b3a7a7098b28b4634d29161ddfbcc63a50bd042a9ba78e86a09914591c9`  
		Last Modified: Wed, 01 Apr 2020 01:23:12 GMT  
		Size: 2.3 MB (2307353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73266e4b49d4fe8afcfdb5360b50714f933dfea8b347ea52c9182cd42c1eaf4c`  
		Last Modified: Wed, 01 Apr 2020 01:23:14 GMT  
		Size: 8.4 MB (8354979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:73e04824d455934b2c9fa3baaf5eee0091b78f4416a0ae62b3ac0978532ba37e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.2 MB (121153615 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5dfb04117ed00f1927125e4461cbec84732cf7d451c2f67d721eb0035d961c99`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 31 Mar 2020 01:47:44 GMT
ADD file:57841d22461f051368fcd3488aab2f2ce27ec7583af772026a228feeb5d00cd9 in / 
# Tue, 31 Mar 2020 01:47:47 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 03:38:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 03:38:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 03:39:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:28:53 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 19:29:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 19:29:12 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 31 Mar 2020 19:32:44 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 31 Mar 2020 19:32:45 GMT
ENV HAXE_VERSION=4.0.5
# Tue, 31 Mar 2020 19:32:46 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 31 Mar 2020 19:41:42 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 31 Mar 2020 19:41:43 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:a893843c75627d21c8a132a2b8559c62371e185dc82e30169102b547264b4f20`  
		Last Modified: Tue, 31 Mar 2020 01:56:02 GMT  
		Size: 45.9 MB (45862803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc1ccae1d4101dbc423377c1f13fb143fc7f5f566816f142268a0b9eede632c`  
		Last Modified: Tue, 31 Mar 2020 04:00:06 GMT  
		Size: 7.1 MB (7096554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d70cde97b6034a1ace45418fd5089f2085511e27ce09ceecf11de34da5f286`  
		Last Modified: Tue, 31 Mar 2020 04:00:05 GMT  
		Size: 9.3 MB (9343329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0366079d8c5e32134b3904853bf6d4d06f84f999018179add69b5cc225bf6194`  
		Last Modified: Tue, 31 Mar 2020 04:00:30 GMT  
		Size: 47.3 MB (47315564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586a31945ea925241fd8ea41ffe2f1c72679f6f36ed45f49f5bbe793c3d049dd`  
		Last Modified: Tue, 31 Mar 2020 20:20:23 GMT  
		Size: 1.2 MB (1233790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f29b8b440de84bdc28a0be5abb87ed6e48b87d7ef4aa437d15052c1dc4f5291`  
		Last Modified: Tue, 31 Mar 2020 20:20:23 GMT  
		Size: 2.2 MB (2249445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f65ec8e2c45352a63e23a5fc9e0e58fc94fcffbd60c7405c3283cae772b6ee02`  
		Last Modified: Tue, 31 Mar 2020 20:20:24 GMT  
		Size: 8.1 MB (8052130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:3084cf15c4fd737e37c58f099cfc75f1492b5d09cb52eddb63bb0197026b8153
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132890962 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1935dde36afe14901554df2d9a550222b0c9b89e56270c6cd15b15be59b2e8ea`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 31 Mar 2020 02:05:07 GMT
ADD file:d0df7ac13226f8d35c078941a20d8a465b09a4e226c5ca37709fa23599cd56dc in / 
# Tue, 31 Mar 2020 02:05:09 GMT
CMD ["bash"]
# Tue, 31 Mar 2020 04:33:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 04:33:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 31 Mar 2020 04:33:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 23:24:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 31 Mar 2020 23:25:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 31 Mar 2020 23:25:07 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 31 Mar 2020 23:28:40 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 31 Mar 2020 23:28:41 GMT
ENV HAXE_VERSION=4.0.5
# Tue, 31 Mar 2020 23:28:42 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 31 Mar 2020 23:36:42 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 31 Mar 2020 23:36:43 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:5767fbcc7692f25971758138978eed9bd3add831a79561cd58bf281e60a5159f`  
		Last Modified: Tue, 31 Mar 2020 02:11:54 GMT  
		Size: 49.2 MB (49169998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b632de0573ae234fd668631d1aba00e13ea3a66cdd1732e58533b119480e4e9`  
		Last Modified: Tue, 31 Mar 2020 04:46:42 GMT  
		Size: 7.7 MB (7681336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f852028d4482a56b904b98dfe16c9781cb55380b9a7f6b6cf59622e3ef0de0`  
		Last Modified: Tue, 31 Mar 2020 04:46:38 GMT  
		Size: 10.0 MB (9983948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac5b037e60412fbff475fee9a38acf16d3117f0709631a272dd03197bf45378`  
		Last Modified: Tue, 31 Mar 2020 04:47:07 GMT  
		Size: 52.1 MB (52102789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abfbf3c5c7e5d7c0a053ef298fad0e95a66c1197b9e2fc66b991becbbdc6d5c`  
		Last Modified: Wed, 01 Apr 2020 00:10:22 GMT  
		Size: 1.3 MB (1302378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ef27744306306323e7be9d2e3614b41d1fb1b9efe5379ff27b594e40ac2a03`  
		Last Modified: Wed, 01 Apr 2020 00:10:23 GMT  
		Size: 2.3 MB (2303647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fdadc7f6c2b4ae299e4b3ddfd464f967f638ff71365490035b6f89cc7dae6b3`  
		Last Modified: Wed, 01 Apr 2020 00:10:26 GMT  
		Size: 10.3 MB (10346866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.1158; amd64

```console
$ docker pull haxe@sha256:0c00e74452476c14b512f2264cd07ba0a6110365be881fb3337d49ff24376ca8
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2299254842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9fb76b0844ae496fe30b0fdb843e6c7213e7a73d4181056f7e69519051c30c82`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Apr 2020 03:38:38 GMT
RUN Install update 1809-amd64
# Wed, 15 Apr 2020 12:44:53 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 12:44:54 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Apr 2020 12:44:55 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Apr 2020 12:44:55 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Apr 2020 12:44:56 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Apr 2020 12:44:57 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Apr 2020 12:45:29 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Apr 2020 12:46:35 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 12:46:56 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Apr 2020 12:46:57 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Apr 2020 12:47:32 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 12:47:33 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 15 Apr 2020 12:51:12 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 12:51:32 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Apr 2020 12:51:33 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Apr 2020 12:51:53 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Apr 2020 12:52:14 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Apr 2020 12:52:36 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Apr 2020 12:52:37 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:eac6fba788c9781d6f989eb0932cb33bf72c2cce4eb234cc6decdcab89e183bc`  
		Size: 736.0 MB (736021953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:442da5a04696895ce6580924a45188bbec9a9db9f81cb7dcef41fc1d4b119130`  
		Last Modified: Wed, 15 Apr 2020 15:29:13 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f216d2ccb2288332e0a47bbb41d72554ab36bfed020e6944c3ed61de98ebdbfd`  
		Last Modified: Wed, 15 Apr 2020 15:29:14 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec75d6feddf3c78628321d15a2f8de036bb7c917d8a6a4aad6986727ecc6888`  
		Last Modified: Wed, 15 Apr 2020 15:29:12 GMT  
		Size: 1.2 KB (1156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f2faecb5f48d00d105cc8cabfe5a7f257f7dff021475f2fd4f3d51ae0fd27f1`  
		Last Modified: Wed, 15 Apr 2020 15:29:11 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd9c3efa71c20af1c9fec8509f4ab7fa54bd6508e38383406c37fec008d09214`  
		Last Modified: Wed, 15 Apr 2020 15:29:11 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe099180cb17d23902490bb0ed93cbfe62c25cd00e59ef4979e3cbcacd441dc`  
		Last Modified: Wed, 15 Apr 2020 15:29:09 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5601b44f748e79451d33b0d8dd0afeed6b9f73dc5297560b04db6b38a0d06b`  
		Last Modified: Wed, 15 Apr 2020 15:29:10 GMT  
		Size: 4.7 MB (4669228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e1357d27d6a481a61ef67165de1e2ca9523b111cd7557157f43c99816f57b2`  
		Last Modified: Wed, 15 Apr 2020 15:29:10 GMT  
		Size: 12.9 MB (12905260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3e7219fe36b3afc93ef1d7ac35f907b7d6f43c6ff05b1132f85bff8c1eb35f7`  
		Last Modified: Wed, 15 Apr 2020 15:29:08 GMT  
		Size: 303.2 KB (303237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a2a237c15fcd672c03528f05ac6c1328a73638d38604248642c96e95931acb`  
		Last Modified: Wed, 15 Apr 2020 15:29:05 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3fae04dc6aed863d412c2ba24147a52afb70ee9feccb77b896a7a2048b618f7`  
		Last Modified: Wed, 15 Apr 2020 15:29:06 GMT  
		Size: 2.1 MB (2130826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f9fc42e721b0ca1e64e3a05938cf619f75ca0953c1cd5b5990bb647f8d0131`  
		Last Modified: Wed, 15 Apr 2020 15:29:05 GMT  
		Size: 1.1 KB (1121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e3470f19e701a72f00aedfed12dbc007f1f4d995201e7532059b134b9a2b255`  
		Last Modified: Wed, 15 Apr 2020 15:29:10 GMT  
		Size: 7.2 MB (7165423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0c4e2ae7e2f44d1ed96f688be1b6762dbff0b9fa9a60369f6c733f2eb223f4`  
		Last Modified: Wed, 15 Apr 2020 15:29:04 GMT  
		Size: 326.6 KB (326555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39954b0cc296fe6342faf457c66a5f4b53324d4f62a8a95b3a20f54d8176140`  
		Last Modified: Wed, 15 Apr 2020 15:29:02 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fed5a1d10d3ba3d2ee8cf06576c84041ff9def96af1f625146b8f79ff0975ec`  
		Last Modified: Wed, 15 Apr 2020 15:29:02 GMT  
		Size: 329.4 KB (329425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d8b96848c604b855759fbbb9408875ac12aa2a54f4b19bdd94a3d0d2f40a2b`  
		Last Modified: Wed, 15 Apr 2020 15:29:02 GMT  
		Size: 347.5 KB (347480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c17f6ae0e890e422d245fbda17a12fa15a9668806cb4fe99243c24b332a032`  
		Last Modified: Wed, 15 Apr 2020 15:29:02 GMT  
		Size: 358.8 KB (358780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6964a655453795dbc6ffe5323155d0c22497c64d95b9d801e60124389f535abe`  
		Last Modified: Wed, 15 Apr 2020 15:29:02 GMT  
		Size: 1.1 KB (1138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3630; amd64

```console
$ docker pull haxe@sha256:9b5c87ce83ec7e530212b02385b4a4e728527256ddbb21f52e89aeb8462ccb54
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5806465337 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d77920646af0d78d5956fd68eb0edb2a9c8e247283061eae0ec9ebc9bb42c670`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 07 Apr 2020 17:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Apr 2020 12:52:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Apr 2020 12:52:52 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Apr 2020 12:52:53 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Apr 2020 12:52:54 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Apr 2020 12:52:54 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Apr 2020 12:52:55 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Apr 2020 12:53:55 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Apr 2020 12:55:52 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 12:56:57 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Apr 2020 12:56:58 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Apr 2020 12:58:20 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 12:58:21 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 15 Apr 2020 13:02:25 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Apr 2020 13:03:32 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Apr 2020 13:03:33 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Apr 2020 13:04:35 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Apr 2020 13:05:42 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Apr 2020 13:06:43 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Apr 2020 13:06:44 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d0099407ec8ccaf0472e55152e38b262bdf0b2cf8dfd2e8afcc89d728ba3f5a0`  
		Size: 1.7 GB (1658081673 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5171ed01a0687a59b2bdf59e2df29a8932abe0ee22a4a6ff6368f8a8295a97d1`  
		Last Modified: Wed, 15 Apr 2020 15:29:42 GMT  
		Size: 1.1 KB (1128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4f23ebac6c5b6cbf39366d2a5aa9b8d0d236a37e33970fa1515f1f0f0a1539`  
		Last Modified: Wed, 15 Apr 2020 15:29:40 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c21b1ff69a937423b2d969a88c7b2797c732a74388aa3116de98e4628eace07`  
		Last Modified: Wed, 15 Apr 2020 15:29:40 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9b45c211992e6e6f35163023874f19c8bbdc5e956dc7939ab9465acc2a28d7`  
		Last Modified: Wed, 15 Apr 2020 15:29:40 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:192a0d1acc7971459c434a6a09919654e4696bb66ac6d20028c9962fcd8cfd2c`  
		Last Modified: Wed, 15 Apr 2020 15:29:37 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f27a076f11cc8e33ab00c50e02bc83172ee01ffccee1e8aee97e13afc7626d`  
		Last Modified: Wed, 15 Apr 2020 15:29:38 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc70447ab674f46e620125d9d711759011320079dc67f92f5ebc5bb6cf76ee47`  
		Last Modified: Wed, 15 Apr 2020 15:29:37 GMT  
		Size: 5.4 MB (5384610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12e4afa4407fae97b569cb9450b8b9b3fbce4fe03bf3eefc8b537d3f8b42f95`  
		Last Modified: Wed, 15 Apr 2020 15:29:39 GMT  
		Size: 22.4 MB (22429439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c91f4762e898908f6ea120daa57c89bab45720470dfeb03cadc19365d8601aad`  
		Last Modified: Wed, 15 Apr 2020 15:29:34 GMT  
		Size: 5.3 MB (5325274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b3f86b6481e5e356ec65b10850abdeeb215a187468657f206384a88592bb97`  
		Last Modified: Wed, 15 Apr 2020 15:29:30 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0766dc734d0b54a088b3d5e07b7d362ea9b50e16b157967b36724b9f42910a8d`  
		Last Modified: Wed, 15 Apr 2020 15:29:34 GMT  
		Size: 7.2 MB (7150951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4457af3fbf5dd4d9d3678588e20148d90d773c5b4854c63c0792debd52b10aa0`  
		Last Modified: Wed, 15 Apr 2020 15:29:29 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db8d1b1e19be54cb799b09ab688aad5a9425d84c68316c83f2e6badf7163e74`  
		Last Modified: Wed, 15 Apr 2020 15:29:37 GMT  
		Size: 16.7 MB (16733258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea841d0da5c1ea6f9cde13d50133f2ca9c6f6cbb615df7038638a13e554562d`  
		Last Modified: Wed, 15 Apr 2020 15:29:29 GMT  
		Size: 5.3 MB (5340562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee16316cae372462105a8184b86b57235bd646aae40d98219ccf8d0c8d213108`  
		Last Modified: Wed, 15 Apr 2020 15:29:24 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbac49c91e3a7c4049c22ecb79a379f6b66df14b7c3877871b46630f0e82974`  
		Last Modified: Wed, 15 Apr 2020 15:29:26 GMT  
		Size: 5.3 MB (5338368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41bb5c3b2346fa98691e2197e3e9b01a88b977653f9a012de12e082c7e79d3f7`  
		Last Modified: Wed, 15 Apr 2020 15:29:26 GMT  
		Size: 5.3 MB (5340981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ccec423900ff50b63ed11b9234d1da54ee540129e9151a1c9d7f50879f1253`  
		Last Modified: Wed, 15 Apr 2020 15:29:25 GMT  
		Size: 5.3 MB (5343046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:952fa28e5624da5ae6028c0603c53dc0b14a83c09bd067afb940dda397a28c59`  
		Last Modified: Wed, 15 Apr 2020 15:29:24 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
