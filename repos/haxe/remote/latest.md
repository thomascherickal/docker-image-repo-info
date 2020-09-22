## `haxe:latest`

```console
$ docker pull haxe@sha256:b77156730387bf93728deef21638d8d6523d4f7c4a822287f7e412410e74c839
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1457; amd64
	-	windows version 10.0.14393.3930; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:4c0f53fa084d1ef500284437f1224b3bc12859dd6dfb491dd3cc520daccb32fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132200722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91ebdd70a02bb970874fcf4a3dc5b21c9149c5820772af64e19a581151d11bc0`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 10 Sep 2020 00:22:55 GMT
ADD file:07a6578d6f507bd9c51bdf4fe41402db5dcf3b9fdf51cd4315778c27da1add39 in / 
# Thu, 10 Sep 2020 00:22:55 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:59:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:59:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:59:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 20:51:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 20:52:02 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 20:52:03 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 10 Sep 2020 20:53:24 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 22 Sep 2020 17:22:22 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 22 Sep 2020 17:22:22 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 22 Sep 2020 17:27:27 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 22 Sep 2020 17:27:27 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:57df1a1f1ad841deaf50c8f662d77e93b4b17af776ed66148116607f9aceffa8`  
		Last Modified: Thu, 10 Sep 2020 00:33:42 GMT  
		Size: 50.4 MB (50395913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71e126169501d71bbbd0d3c8d9f35836c41660869fe8432ac606341ed21f7adb`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 7.8 MB (7811567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1af28a55c3f320826db8df3146a2c198f9042877ef679f9e32210aa9a7fac9ef`  
		Last Modified: Thu, 10 Sep 2020 01:15:23 GMT  
		Size: 10.0 MB (9996317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f1c9932170e54fface2382b2550b8052ae3d41f27e66ea1294e2055dd2b2e7`  
		Last Modified: Thu, 10 Sep 2020 01:15:45 GMT  
		Size: 51.8 MB (51829661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ed9e1dfd212b4efae9f5d7707bf3b9d5c725735eaf44475ee26ed395cce992d`  
		Last Modified: Thu, 10 Sep 2020 21:24:58 GMT  
		Size: 1.3 MB (1312196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3955d9be95c9696b39c8a70692549998a77a831114518f1ea73a5afe24974175`  
		Last Modified: Thu, 10 Sep 2020 21:24:58 GMT  
		Size: 2.3 MB (2307299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d738ccaec04e63e5658edebff7592dd850b42aece8cc07a332c633259cc7f71`  
		Last Modified: Tue, 22 Sep 2020 18:03:00 GMT  
		Size: 8.5 MB (8547769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:1f9ed68dddb9c938553bcfc148c2a5313dcf62d6424946f2d9149390d99a812d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121384869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49a2fbb760a626f67b081605588e4daa0476257f7726d93e6ccede930c1fbbe4`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 10 Sep 2020 00:07:32 GMT
ADD file:340663c3add65bd8904ba51984e6080c6aa6d237bd845f4e0aa22626d31497b7 in / 
# Thu, 10 Sep 2020 00:07:35 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:39:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:39:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:40:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:47:41 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 21:47:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 21:47:52 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 10 Sep 2020 21:51:31 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 22 Sep 2020 18:50:36 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 22 Sep 2020 18:50:47 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 22 Sep 2020 18:59:58 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 22 Sep 2020 19:00:05 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:7d9beb74056b685831827b5f21351f021873d8ba1a1170b378e5edf5f46d114e`  
		Last Modified: Thu, 10 Sep 2020 00:17:29 GMT  
		Size: 45.9 MB (45869299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689ccbaccf1b655191aa8867125206ed64238bf9a9e9839c4b10af714b1226f8`  
		Last Modified: Thu, 10 Sep 2020 02:01:37 GMT  
		Size: 7.1 MB (7097950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf7011b92214ace9e792fa4ef39707503be7ea5c29200c9e71ac3f6b1afb81`  
		Last Modified: Thu, 10 Sep 2020 02:01:37 GMT  
		Size: 9.3 MB (9343399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daa216e44ff17d2fdb02fb4a79ef82fd1042dfaefb74d10c5db403575fbb03fc`  
		Last Modified: Thu, 10 Sep 2020 02:02:02 GMT  
		Size: 47.4 MB (47356064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad0bf51a537454149c7a9993c833f63ee72e22350c76fdf944443bab5e13a98`  
		Last Modified: Thu, 10 Sep 2020 22:48:21 GMT  
		Size: 1.2 MB (1234689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbbcd9c45ee79a65bff874dc2dd60c1a2921accbf49de2c1cd4c7e382a5be28`  
		Last Modified: Thu, 10 Sep 2020 22:48:24 GMT  
		Size: 2.2 MB (2249605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a3eb9b7eee3d578d838369568569838dc17679dd970f28a18dcdf0cbfe0496`  
		Last Modified: Tue, 22 Sep 2020 19:01:26 GMT  
		Size: 8.2 MB (8233863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:ef5266fc58fcc9ca6c4dc4e7ff35053eaf100fa0c6060daab1c543eae4693f81
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133145944 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9e11d2b1ee5cd59de0f7cb1713e4cb243105d730f3fed5761c9f1c17990d49`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 09 Sep 2020 23:50:21 GMT
ADD file:c8c11e622b1b8a1e31f32e2457ff4d1314d5cd4a7ad22b3991ab9d0542db23fd in / 
# Wed, 09 Sep 2020 23:50:22 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:28:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:28:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:29:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 22:12:43 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 10 Sep 2020 22:12:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 22:12:58 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 10 Sep 2020 22:16:47 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 22 Sep 2020 17:50:46 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 22 Sep 2020 17:51:00 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 22 Sep 2020 17:59:19 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 22 Sep 2020 17:59:31 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:d3a32671b6316bd11f4bf18cb034394ac94d2bb3bc6d09de388b19b06fb94b91`  
		Last Modified: Wed, 09 Sep 2020 23:58:45 GMT  
		Size: 49.2 MB (49175549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b1202c4ddac582c7164a6b65b13a2442759bc04660da9ca7d62fabf75225482`  
		Last Modified: Thu, 10 Sep 2020 00:42:35 GMT  
		Size: 7.7 MB (7681394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f110d64c20212ec5e7a7f0622d610346edbd6e508fde94679db44e0f2827b2f9`  
		Last Modified: Thu, 10 Sep 2020 00:42:34 GMT  
		Size: 10.0 MB (9983858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7c41999aa9f871546022553f35d4fbbd39cd2bfe8e1a03cce7b1bd78d2a5b0`  
		Last Modified: Thu, 10 Sep 2020 00:43:02 GMT  
		Size: 52.2 MB (52164372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2a17daac8618d2417e046aef9fcca3c13c855257c9fd729ff98ff59c8da3f85`  
		Last Modified: Thu, 10 Sep 2020 23:12:26 GMT  
		Size: 1.3 MB (1303368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76925839481c365b3c5f0eed9ac4198746cd8fd66afd51f2e11255887b727f84`  
		Last Modified: Thu, 10 Sep 2020 23:12:27 GMT  
		Size: 2.3 MB (2303611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cc373e353e547ef2523b1527e03283cdbe58beff60ca339d65d0bd37fee1f6`  
		Last Modified: Tue, 22 Sep 2020 18:48:34 GMT  
		Size: 10.5 MB (10533792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.1457; amd64

```console
$ docker pull haxe@sha256:3db8931c81478ce8ed68143e3bcb8840a4614ab2b89f6a29ffefeb39309a462d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2406634302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f739d2ea0eb36ca5ab4e28174e647058257d49ff03124269d1378ea8ebd0ecb`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Wed, 09 Sep 2020 13:15:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 13:15:06 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 09 Sep 2020 13:15:07 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 09 Sep 2020 13:15:08 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 09 Sep 2020 13:15:08 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 09 Sep 2020 13:15:09 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 09 Sep 2020 13:15:48 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 13:16:46 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 13:17:07 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 09 Sep 2020 13:17:07 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 09 Sep 2020 13:17:41 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Tue, 22 Sep 2020 18:14:14 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 22 Sep 2020 18:17:50 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.1.4/haxe-4.1.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Tue, 22 Sep 2020 18:18:10 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Tue, 22 Sep 2020 18:18:10 GMT
ENV HOMEDRIVE=C:
# Tue, 22 Sep 2020 18:18:30 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 22 Sep 2020 18:18:54 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Tue, 22 Sep 2020 18:19:18 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Tue, 22 Sep 2020 18:19:19 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:1df31adcc7026c3bf0cb32832a3f307dd6e1e54b8b3e050f8a73b5caee674d88`  
		Last Modified: Wed, 09 Sep 2020 16:48:51 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1894e8b972206cdfe97d38ca02c458ff60a770a58c0e5e036b6715371f2fcd`  
		Last Modified: Wed, 09 Sep 2020 16:48:50 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:718720a1f304eb26dc9adf84a6bcdff57408af840b7d08e24e10353c8843b636`  
		Last Modified: Wed, 09 Sep 2020 16:48:50 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea7d477511e258308b161d7fa385584ca21a8dbbeafdceb51960da3974a4602`  
		Last Modified: Wed, 09 Sep 2020 16:48:49 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63413523f67fc3f4cd42a6be22b87167dee2b59ac5aa43599773e469b2a812ee`  
		Last Modified: Wed, 09 Sep 2020 16:48:48 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b2922f6ef5a885e2d543a0b6be33ff7e68480cc7de9b03c43fe68a47c13a101`  
		Last Modified: Wed, 09 Sep 2020 16:48:46 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d83916756b43b54ceb1ffc8e03454d84b4f0461efbe0cf83c35e3559ff82fff`  
		Last Modified: Wed, 09 Sep 2020 16:48:49 GMT  
		Size: 9.1 MB (9129166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719b18e8c4b78a1db5fe9305fe9cc7661758ad0f0128d5ce74268cf7ba18065e`  
		Last Modified: Wed, 09 Sep 2020 16:48:48 GMT  
		Size: 17.3 MB (17256377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b4d41ce3adcd941564d832dff94c3ebdbcf2f806c4052c62c7adcd51c041a`  
		Last Modified: Wed, 09 Sep 2020 16:48:44 GMT  
		Size: 308.1 KB (308140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af87dd2d40383b01a00913f815b6af815304b6dd8ddc3790ef310bcf7f8d524b`  
		Last Modified: Wed, 09 Sep 2020 16:48:43 GMT  
		Size: 1.1 KB (1126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b0dd4351a3f1076f5fd00bc759d76e1d06cb9fad6af619a8679a2379f4df92`  
		Last Modified: Wed, 09 Sep 2020 16:48:43 GMT  
		Size: 6.5 MB (6479807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c4314c51826550cf9680c1653f7d9e5239dbdf3d174d8681c4bfa275da167b3`  
		Last Modified: Tue, 22 Sep 2020 18:30:52 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1ff4c268afd516cd070ec9688ccd23597d2abe35a1187f87bfd0ee90eb7db7`  
		Last Modified: Tue, 22 Sep 2020 18:30:57 GMT  
		Size: 12.0 MB (11976130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6bf29690566e159b93f0f6da83ae9d7a53c64e20c693f577faa8b46eceaa992`  
		Last Modified: Tue, 22 Sep 2020 18:30:53 GMT  
		Size: 357.7 KB (357717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a44096e782c3aa4c1dddf8d982bbccab7f295babb948c2dbee2f2f44157f06`  
		Last Modified: Tue, 22 Sep 2020 18:30:49 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21333820eafa5bf98e8a501325e314f7083ae30ce0f1b1ca5ac4a80f6976f738`  
		Last Modified: Tue, 22 Sep 2020 18:30:50 GMT  
		Size: 364.2 KB (364203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3515ac1396711aca6258e46bfbafe5868f98b9fb542e1b108efec7e875f1c4`  
		Last Modified: Tue, 22 Sep 2020 18:30:51 GMT  
		Size: 4.7 MB (4727356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d856a1dd283f53e638dabf3e058fbee2b1e36fa0a02b4d45a9f8bfa4e6f15f`  
		Last Modified: Tue, 22 Sep 2020 18:30:54 GMT  
		Size: 4.8 MB (4751852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65595c755433b72d0d7b92e1789bb3af6b34ca0d00479f71e274d4fc1414d269`  
		Last Modified: Tue, 22 Sep 2020 18:30:49 GMT  
		Size: 1.1 KB (1122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3930; amd64

```console
$ docker pull haxe@sha256:2b21631338d469d1b6d8f703d0e36301516f29724820ea3a8e5260ac4f808cb5
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5840566035 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:66cd957e67e3c7047e737843b21b349ba89de4e7bb1466e5bd21e145eebcb7fd`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 01 Sep 2020 19:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Sep 2020 13:23:04 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 09 Sep 2020 13:23:05 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 09 Sep 2020 13:23:05 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 09 Sep 2020 13:23:06 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 09 Sep 2020 13:23:07 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 09 Sep 2020 13:23:07 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 09 Sep 2020 13:24:24 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Sep 2020 13:26:08 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 09 Sep 2020 13:27:17 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 09 Sep 2020 13:27:18 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 09 Sep 2020 13:28:39 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Tue, 22 Sep 2020 18:19:27 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 22 Sep 2020 18:23:52 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.1.4/haxe-4.1.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Tue, 22 Sep 2020 18:25:00 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Tue, 22 Sep 2020 18:25:01 GMT
ENV HOMEDRIVE=C:
# Tue, 22 Sep 2020 18:26:16 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Tue, 22 Sep 2020 18:27:33 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Tue, 22 Sep 2020 18:28:39 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Tue, 22 Sep 2020 18:28:40 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bc202b498d589027cc702b23cf959b8842907508b3465b9d6ff739c9668e5134`  
		Size: 1.7 GB (1669268544 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1d56eeebea105bba2dd1879a89adb012f98cf42708c0f36ca4af683db7162a2`  
		Last Modified: Wed, 09 Sep 2020 16:49:22 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a60be5bafca8b6d48351847bd55c003eb7abbbbccc5fd393343acbff13b4cc`  
		Last Modified: Wed, 09 Sep 2020 16:49:21 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e727742df39ec4cb9172abff56193016b8587633514d13778c9ee351b5a2399b`  
		Last Modified: Wed, 09 Sep 2020 16:49:21 GMT  
		Size: 1.2 KB (1152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afb28a387ea935a5f5e1e1b4b87c083efb51800018bf6ea095ed7adaa4dd15d7`  
		Last Modified: Wed, 09 Sep 2020 16:49:21 GMT  
		Size: 1.1 KB (1119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e296fa8f92255e15a973337a18babd09379bc06d761ef78ea35a294f905a5218`  
		Last Modified: Wed, 09 Sep 2020 16:49:19 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba8c79e2e770f0a32b58eac7723ced9a83e3945eaecc06f8112c71d745fd7ce`  
		Last Modified: Wed, 09 Sep 2020 16:49:16 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6420d129813943ea0c67c19082ae0f7008be4c329170f36cc70a1d7f584ea64`  
		Last Modified: Wed, 09 Sep 2020 16:49:19 GMT  
		Size: 9.9 MB (9880947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34deecf93789bdab69c3cba1239e0f552b3deacb3983156f33db4a205c5abdd`  
		Last Modified: Wed, 09 Sep 2020 16:49:18 GMT  
		Size: 22.4 MB (22393968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19496e374405e2fb53f4bfec4bfbb76bf0294b2042af8fcd78d73a7e33c1d4d4`  
		Last Modified: Wed, 09 Sep 2020 16:49:12 GMT  
		Size: 5.3 MB (5323003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:819de4a23bdf202db0a27c0254a98511cf02399dac2a39a409b638ea4f57d306`  
		Last Modified: Wed, 09 Sep 2020 16:49:09 GMT  
		Size: 1.1 KB (1143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d499ffa3812b053fac5b48e8ae088044916e337f35677cba6dcf3ab192a201`  
		Last Modified: Wed, 09 Sep 2020 16:49:11 GMT  
		Size: 11.7 MB (11650527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867b9c2313084c9a39adc39736d0fc4e1cb075c344d254f47fa03a87803f35e0`  
		Last Modified: Tue, 22 Sep 2020 18:31:17 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4bb1210faaadeb5527d88487d00bb9d0d050dbf32880512d8ecb953c1373ad5`  
		Last Modified: Tue, 22 Sep 2020 18:31:19 GMT  
		Size: 17.1 MB (17133220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279995ae1e59957817b2e9326660c4497524a383a046b8ea7db0b9b5da739612`  
		Last Modified: Tue, 22 Sep 2020 18:31:16 GMT  
		Size: 5.4 MB (5358548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708e488734abb18d6936789b9621bd35a4ea4cda4063a59eadb302023fe25006`  
		Last Modified: Tue, 22 Sep 2020 18:31:09 GMT  
		Size: 1.2 KB (1194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e835ebf8caeb062a2295e07513583e68c576bf538edb0a0232836bef01dacba3`  
		Last Modified: Tue, 22 Sep 2020 18:31:13 GMT  
		Size: 9.9 MB (9852788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cd02cacb29fecf77a4b9ee7228a1be7344daa989d619d96e0bc531f11940a94`  
		Last Modified: Tue, 22 Sep 2020 18:31:15 GMT  
		Size: 9.9 MB (9852486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1939f708c9c162778f1a96907523fc9982bca8bdb8276cd9697f52c545acfa37`  
		Last Modified: Tue, 22 Sep 2020 18:31:14 GMT  
		Size: 9.9 MB (9854678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad8cee6c4535d04dd3b5546a907981cddbf9ac7cabb7ae3c8b271a936ccca71`  
		Last Modified: Tue, 22 Sep 2020 18:31:09 GMT  
		Size: 1.1 KB (1124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
