## `haxe:latest`

```console
$ docker pull haxe@sha256:b9467872f79012a0b5af52a0bd3243fe3fc81735a821fdaa87edf1a1ad2e5f1d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1098; amd64
	-	windows version 10.0.14393.3568; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:f8d1537dea0c074ad6f01d88c2bc3788b3b31c89aacc010f455bec26ecdc2039
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.9 MB (131933281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f8005e328ceea82c581d35dc2d2a2b653492ad4eb55fe6831a3eaeec8dcdfb5`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:07 GMT
ADD file:e05e45c33042db4ec7f71a5952d65ee8cb3786dcd76fa7a990f48a2def1344e2 in / 
# Wed, 26 Feb 2020 00:37:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:06:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:06:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:06:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Feb 2020 02:30:11 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 27 Feb 2020 02:30:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Feb 2020 02:30:16 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 27 Feb 2020 02:31:31 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 27 Feb 2020 02:31:31 GMT
ENV HAXE_VERSION=4.0.5
# Thu, 27 Feb 2020 02:31:31 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 27 Feb 2020 02:36:51 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 27 Feb 2020 02:36:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:50e431f790939a2f924af65084cc9d39c3d3fb9ad2d57d183b7eadf86ea46992`  
		Last Modified: Wed, 26 Feb 2020 00:44:04 GMT  
		Size: 50.4 MB (50381971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8c6d374ea51e3dd671f71b28d025a7794ebea181b00838987d0b4d8a51372f`  
		Last Modified: Wed, 26 Feb 2020 01:20:25 GMT  
		Size: 7.8 MB (7812140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85513200d847a64a6e8f2cb714e2169f559b24b7736c586ff7b9aaedf71f410`  
		Last Modified: Wed, 26 Feb 2020 01:20:25 GMT  
		Size: 10.0 MB (9996282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55769680e8277a4ff083d05f0993d1483b3d26b93a8814cf3c6f04fe5975ffa0`  
		Last Modified: Wed, 26 Feb 2020 01:20:44 GMT  
		Size: 51.8 MB (51790538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c58dc0a4b9250beb10e362b3824b444d149e21c66819280e92b7c4e6a014fd`  
		Last Modified: Thu, 27 Feb 2020 03:23:18 GMT  
		Size: 1.3 MB (1311085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:002a1f523519b1edc211d4ce4fc4ef0cb543d8da531a7fe43621f2719b629cbe`  
		Last Modified: Thu, 27 Feb 2020 03:23:18 GMT  
		Size: 2.3 MB (2307248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ee14a1339a1049e66d04fa52da3cd5cbb1337a139cbe2aace216c1cf5af49b`  
		Last Modified: Thu, 27 Feb 2020 03:23:24 GMT  
		Size: 8.3 MB (8334017 bytes)  
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
$ docker pull haxe@sha256:5781c4305cf1e5e266ead25e2b25987013ccfb0f88afc7ce9bd169a23de69eef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.9 MB (132870496 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38f1cb79174fb466ce8722dda4d9cf5fb7f078529629defc8fd46d6cfb865131`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:50:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:50:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:51:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:50:57 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 26 Feb 2020 19:51:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:51:11 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 26 Feb 2020 19:56:58 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 26 Feb 2020 19:57:00 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 26 Feb 2020 19:57:00 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 26 Feb 2020 20:27:02 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 26 Feb 2020 20:27:04 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:194f1ca8932d9ee1727375561698745fa548546f609956c4aca9fed0b48d41a1`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 7.7 MB (7681467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88425686f799f708ae776f78a6d01c179a52f55fc5b32de874db3c4ace2dd156`  
		Last Modified: Wed, 26 Feb 2020 04:05:25 GMT  
		Size: 10.0 MB (9983767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c349f2c39d405d81a454ff62bdd8753ad71aeb8e8c1e300f3d7d19cd78eaced`  
		Last Modified: Wed, 26 Feb 2020 04:05:53 GMT  
		Size: 52.1 MB (52102940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1158cc87ea08868c42860755609c55f8ccf00ae533ae7851147b4495cdd13883`  
		Last Modified: Wed, 26 Feb 2020 20:59:48 GMT  
		Size: 1.3 MB (1302446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14aaac49e35691c6bcf9efa9b33e998487c840ebdbac0f2eda6f42fa743fae3`  
		Last Modified: Wed, 26 Feb 2020 20:59:48 GMT  
		Size: 2.3 MB (2303549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c2d4dfc2ca8d31f2d9b06b9ae78507a3a7568aefba18b68ec34a5ceb12cd8d`  
		Last Modified: Wed, 26 Feb 2020 20:59:49 GMT  
		Size: 10.3 MB (10326353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.1098; amd64

```console
$ docker pull haxe@sha256:0219d4eecc2cb25e276d63a23d7ebb5826be804af49c273fb1af99b9485f7e01
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2293796264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:467718c203873625e1e0db5434b7e3c343ba520a77c8fe92d529e55d8a644516`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Tue, 10 Mar 2020 23:23:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 11 Mar 2020 12:51:12 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 11 Mar 2020 12:51:13 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 11 Mar 2020 12:51:14 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 11 Mar 2020 12:51:16 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 11 Mar 2020 12:51:17 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 11 Mar 2020 12:51:54 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Mar 2020 12:53:05 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:53:29 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 11 Mar 2020 12:53:30 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 11 Mar 2020 12:54:12 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:54:13 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 11 Mar 2020 12:58:54 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:59:17 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 11 Mar 2020 12:59:18 GMT
ENV HOMEDRIVE=C:
# Wed, 11 Mar 2020 12:59:40 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Mar 2020 13:00:07 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 11 Mar 2020 13:00:32 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 11 Mar 2020 13:00:33 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb49f89affc2d69b541463d095fdfbe61fa62e02b0aa5fa6d26bc134fb66bf35`  
		Last Modified: Wed, 11 Mar 2020 00:30:48 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210514177d8dc4c2da39342d4f01387f731f5800d4ccba5171d3f92c3a3e3088`  
		Last Modified: Wed, 11 Mar 2020 14:26:55 GMT  
		Size: 1.2 KB (1190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa04b026bb2846d9ba6c9c5d9908d7c26ec4c76e7cfb9cfd9b926a2b0c0eb44f`  
		Last Modified: Wed, 11 Mar 2020 14:26:55 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433f362ebf7fe7e63a7b3182a23f449218c5f1665b57c626c3a31f9c273f42cb`  
		Last Modified: Wed, 11 Mar 2020 14:26:53 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b12d502a3e523e75ab5c806d7ba075ba90060ce308d059400f08e76d89a92340`  
		Last Modified: Wed, 11 Mar 2020 14:26:50 GMT  
		Size: 1.2 KB (1193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50b7a2c37fae959e5a887beace79a5ca1f9759c54f54231eefb2aad20b0f53f`  
		Last Modified: Wed, 11 Mar 2020 14:26:48 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b78f99a2cf2333df02c94fcf06576f1ac2bb480d119ac859afb2ee02768debe`  
		Last Modified: Wed, 11 Mar 2020 14:26:49 GMT  
		Size: 4.7 MB (4655864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e162a617ca627205a06c57f9be4521ed5085e76434a866c0f5f1197337d6d64`  
		Last Modified: Wed, 11 Mar 2020 14:27:07 GMT  
		Size: 12.9 MB (12897183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f310d3d88cf8e4f454ff30ac15cec62c4c73547db3faaab46848603c633cde1b`  
		Last Modified: Wed, 11 Mar 2020 14:26:44 GMT  
		Size: 295.9 KB (295853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bac7cb52da2f95c11fd7ad885527ec87e346f96d48c1852df4de0e3644053cc`  
		Last Modified: Wed, 11 Mar 2020 14:26:41 GMT  
		Size: 1.2 KB (1176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e85d950ac1fd1cdb40b5441d63801daf02fc7da5faa7cba6183bfb8d3d83efc`  
		Last Modified: Wed, 11 Mar 2020 14:26:42 GMT  
		Size: 2.1 MB (2123686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa88656c441523d06089c990f10a4d16c0776deefdba3e02b4e4770717e0e15b`  
		Last Modified: Wed, 11 Mar 2020 14:26:40 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0843fca693cc6c6480cccdce4129a082e3f1d6be64ffe6f05c808b295bba984`  
		Last Modified: Wed, 11 Mar 2020 14:27:21 GMT  
		Size: 7.1 MB (7139818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f54561682eeadb8d018032d0973063b4e5bc6fe9b4d163e9c9c2bd0fbd30bd68`  
		Last Modified: Wed, 11 Mar 2020 14:26:39 GMT  
		Size: 320.6 KB (320564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98186ce8c105235135b31b79a3af5059bd085b836a72e20c0d12f46d641964c1`  
		Last Modified: Wed, 11 Mar 2020 14:26:36 GMT  
		Size: 1.2 KB (1165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6bfc6de93c1f6921600df97ac094003a18ae77e1255d523645d2cd4e2fde1d0`  
		Last Modified: Wed, 11 Mar 2020 14:26:37 GMT  
		Size: 324.1 KB (324071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ffca698ac04a5873c5bccf8fa163de62e5dea525d89f1ddf1bf437b2b9d0f2d`  
		Last Modified: Wed, 11 Mar 2020 14:26:37 GMT  
		Size: 338.7 KB (338664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1be53742b5aba2f92642aa5c323719a04f8fd92e34d4ecbe407e93ff465392c`  
		Last Modified: Wed, 11 Mar 2020 14:26:37 GMT  
		Size: 352.3 KB (352321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356a4010c8ca900014dc5a4ffba12c8884b378de378b27014955f133703a0489`  
		Last Modified: Wed, 11 Mar 2020 14:26:36 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3568; amd64

```console
$ docker pull haxe@sha256:6903ae30e2295879281c736fa5509f9b5a4b53558ccc4135af72d506febc80b1
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5807123293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11d7de06d3d98e2e02f8d4bed5e9e9c30ec74eb810fde18e945047dfd4f6e4b9`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 12:27:51 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 18 Mar 2020 12:27:52 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 18 Mar 2020 12:27:53 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 18 Mar 2020 12:27:54 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 18 Mar 2020 12:27:55 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 18 Mar 2020 12:27:56 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 18 Mar 2020 12:29:02 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Mar 2020 12:31:00 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 12:32:13 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 18 Mar 2020 12:32:14 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 18 Mar 2020 12:33:42 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 12:33:44 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 18 Mar 2020 12:37:53 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 18 Mar 2020 12:38:58 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 18 Mar 2020 12:38:59 GMT
ENV HOMEDRIVE=C:
# Wed, 18 Mar 2020 12:40:10 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 18 Mar 2020 12:41:30 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 18 Mar 2020 12:42:51 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 18 Mar 2020 12:42:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8cd5aa189dca96a2d4bcc0e2516d85f8a69d277957f44aca08575ecf42e5bc2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:17 GMT  
		Size: 1.1 KB (1107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:839fbc7351ebac73a82f4ae624606c6e468192e8d825ad264af1eb4da45a8ab0`  
		Last Modified: Wed, 18 Mar 2020 13:22:16 GMT  
		Size: 1.1 KB (1125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adb09a56547c0380a1fba91592d787ff57888ef96224d7aebccc53790b1af988`  
		Last Modified: Wed, 18 Mar 2020 13:22:16 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a318c4f2e51d616d6627c18c7f0a2600231268764f79e04e37c8c1a0ebb4bda4`  
		Last Modified: Wed, 18 Mar 2020 13:22:15 GMT  
		Size: 1.1 KB (1141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c617b76ac1f009351b1ed3ca98ebc3303f8bdf8ae61ca43018305767e42a4ff`  
		Last Modified: Wed, 18 Mar 2020 13:22:14 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3209e7e39bfec2639e4f67c9cefc2b27d78d2ff511aab603ee4516821f0a5dd`  
		Last Modified: Wed, 18 Mar 2020 13:22:13 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6fd1b77a6d323229fc2535e1c89f7558cefe01a530eb28ca9af989184f91047`  
		Last Modified: Wed, 18 Mar 2020 13:22:13 GMT  
		Size: 5.4 MB (5385623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b12101e9c633827c950810d15fcc5c6a3b024811382bd38a23ad99d66a5b2f`  
		Last Modified: Wed, 18 Mar 2020 13:22:13 GMT  
		Size: 22.4 MB (22427597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad089c03bfd1fad90ab013e127ac359b316ca981882cb262e9a4edf0308eb5a`  
		Last Modified: Wed, 18 Mar 2020 13:22:10 GMT  
		Size: 5.3 MB (5331136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a83b2b14d95d9e9be5109a9fbe8b5c29139e72dd21d68567dd6f61fbcf0c9e`  
		Last Modified: Wed, 18 Mar 2020 13:22:05 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f963db038e8c66d55564147ae98992ba3f07a3b65c9e07bc4f436f9fb9561c26`  
		Last Modified: Wed, 18 Mar 2020 13:22:07 GMT  
		Size: 7.2 MB (7153736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f1b7ca885555551f680fdb6f3cb67dca38c8169080d77bf7ce06621cc1d1674`  
		Last Modified: Wed, 18 Mar 2020 13:22:05 GMT  
		Size: 1.1 KB (1120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0a1e7fb6f9f27449bc73ca2de826ebf3d2b04b716581f3525c1601e1dd64793`  
		Last Modified: Wed, 18 Mar 2020 13:22:09 GMT  
		Size: 16.7 MB (16663076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93308d4a0767d411c4dd95bc49c07e09f8bbefaa88e492ce0395fb414b1bb4e`  
		Last Modified: Wed, 18 Mar 2020 13:22:12 GMT  
		Size: 5.3 MB (5345592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeefc10b65e97ad57fd48965679827f5be5c27311e97a314ba2d4363d8ace58a`  
		Last Modified: Wed, 18 Mar 2020 13:21:59 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32f433a767c23a816d976f25c864c58743b89d83c00f8bb9edbac517cc9e59d5`  
		Last Modified: Wed, 18 Mar 2020 13:22:01 GMT  
		Size: 5.3 MB (5344972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d3ff214ae499a99e57262b9bc8bb8879303855a964d4b34f8680f10df39fd9`  
		Last Modified: Wed, 18 Mar 2020 13:22:02 GMT  
		Size: 5.3 MB (5349175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49a64075839f03064acc0dac2beb26c4782790450ddd071ea2edbf4e19b13abe`  
		Last Modified: Wed, 18 Mar 2020 13:22:01 GMT  
		Size: 5.3 MB (5349989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6804790d1033dba5c5432b757ce03c42d8bb8c0246a02ba08d5335382df311c`  
		Last Modified: Wed, 18 Mar 2020 13:21:59 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
