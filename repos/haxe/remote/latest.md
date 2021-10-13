## `haxe:latest`

```console
$ docker pull haxe@sha256:53c4431d72114c3974ad1f4fcd66ddb5da66265b9bc47c22a4b69034f7b5da27
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2183; amd64
	-	windows version 10.0.14393.4651; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:e8e43799d92f925a484ce999fbcb29dad3bb8c5ab03e83d13470d72aee95d205
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133604009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562b95db539d23795010b82dca9359d4a1d15197649db682c4a5a8ce17eafd1c`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 28 Sep 2021 01:22:54 GMT
ADD file:f2a417d653b625cf79b88a517dc7e0ce5ace15a7acbd952daeee3bb4bf6042a1 in / 
# Tue, 28 Sep 2021 01:22:55 GMT
CMD ["bash"]
# Tue, 28 Sep 2021 01:51:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 28 Sep 2021 01:51:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 28 Sep 2021 01:51:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:44:35 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Sep 2021 05:44:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 29 Sep 2021 05:44:41 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 29 Sep 2021 05:46:04 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 29 Sep 2021 05:46:04 GMT
ENV HAXE_VERSION=4.2.3
# Wed, 29 Sep 2021 05:46:05 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 29 Sep 2021 05:51:58 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 29 Sep 2021 05:51:59 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:5e7b6b7bd506c12399d65977c0ba8dd02824dc5d0e65fc55d7382da889bdac7d`  
		Last Modified: Tue, 28 Sep 2021 01:29:21 GMT  
		Size: 50.4 MB (50436209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd67d668d6911bf21ad4701522e1ed3af416837433fdba3f88cff06a23e23861`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 7.8 MB (7833602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ae016bc26876abbd5e952133b02b04d4c1dae1bc75a3d9386250e4797ccd87a`  
		Last Modified: Tue, 28 Sep 2021 01:59:09 GMT  
		Size: 10.0 MB (9997190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0af05a4d868593f859eaa5815fc1c3596d77318a4ed756f3865a5fa3f290c6`  
		Last Modified: Tue, 28 Sep 2021 01:59:27 GMT  
		Size: 51.8 MB (51841311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77330925c79047eceb9b8a448bbc76adec84f055eb6985a9ac6e7f33a338cfcb`  
		Last Modified: Wed, 29 Sep 2021 06:22:41 GMT  
		Size: 1.3 MB (1314626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d061a4bf01047a08e3e6c8dfcd27e5e6fcc66f48a78eac28d9ff5b6e1176f177`  
		Last Modified: Wed, 29 Sep 2021 06:22:41 GMT  
		Size: 2.3 MB (2308400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53473ff07b5aedfd60fa62546a16a8a1beee58aa0cf8d02a1873439e20235836`  
		Last Modified: Wed, 29 Sep 2021 06:22:44 GMT  
		Size: 9.9 MB (9872671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:7b3a17dfd6aa16eafc78f20807335d28e47ad9ab399a783ddba890b2d42a206e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122756766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dc379f3d4d42c04079035a22fffbb845b0a891db40f74ab72f2997104023394`
-	Default Command: `["haxe"]`

```dockerfile
# Thu, 30 Sep 2021 18:03:34 GMT
ADD file:da3730d9c05fab2433637063dc9d51b2505bb6023c391d606419bc9a0874c131 in / 
# Thu, 30 Sep 2021 18:03:35 GMT
CMD ["bash"]
# Fri, 01 Oct 2021 05:35:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 01 Oct 2021 05:35:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 01 Oct 2021 05:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 14:07:37 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 02 Oct 2021 14:07:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sat, 02 Oct 2021 14:07:49 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 02 Oct 2021 14:11:03 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sat, 02 Oct 2021 14:11:04 GMT
ENV HAXE_VERSION=4.2.3
# Sat, 02 Oct 2021 14:11:04 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sat, 02 Oct 2021 14:19:08 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sat, 02 Oct 2021 14:19:09 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:2d333743b3b21fdfd6ba3f4a0624204b620b72c3d0eb2c3dd9e39d23f3a87e9c`  
		Last Modified: Thu, 30 Sep 2021 18:20:10 GMT  
		Size: 45.9 MB (45917880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376d8928e133ca4adc2e7f254a958f120743ac165e45332c8f2713144cf1e1c5`  
		Last Modified: Fri, 01 Oct 2021 05:55:55 GMT  
		Size: 7.1 MB (7124916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a975074459ff1f9c6b99644b138401f840f49a4dc1ef138661e138db9cd00038`  
		Last Modified: Fri, 01 Oct 2021 05:55:56 GMT  
		Size: 9.3 MB (9343736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a11c276eb14e33bd12beadc8185183d0805aee55492c4f89cf581d75ed1b203`  
		Last Modified: Fri, 01 Oct 2021 05:56:40 GMT  
		Size: 47.4 MB (47356508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e574f263a96dbe1069763a9b80a4e9cc3f944ce2d1a55e8e94f719afab313d4e`  
		Last Modified: Sat, 02 Oct 2021 15:07:04 GMT  
		Size: 1.2 MB (1237417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cfb28e9a7b02dceec5822c32a1fb53d9f52574a0cbeeac9dc909fb1ddaeb31e`  
		Last Modified: Sat, 02 Oct 2021 15:07:05 GMT  
		Size: 2.2 MB (2249775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fe84c62defa9baeedf29a29680390beb052104ea8c316dd9471c2130d6df13`  
		Last Modified: Sat, 02 Oct 2021 15:07:11 GMT  
		Size: 9.5 MB (9526534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:d10ac06b456229eda693e52c9577fcac926f9e6e9f4b144ef115604c6e2f1825
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.3 MB (134306590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fb2b7a105e2b620b887d3684b15f6c309ebd683761f0047d6c3a65388d09538`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:28 GMT
ADD file:aed1709ccba6a81b9726b228fad7b81bcf4c16bafe723981ad37076322d78986 in / 
# Tue, 12 Oct 2021 01:41:29 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 02:11:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 02:11:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Oct 2021 02:11:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:13:24 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Oct 2021 20:13:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Oct 2021 20:13:31 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 12 Oct 2021 20:14:53 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 12 Oct 2021 20:14:54 GMT
ENV HAXE_VERSION=4.2.3
# Tue, 12 Oct 2021 20:14:55 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 12 Oct 2021 20:18:41 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 12 Oct 2021 20:18:41 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:2ff6d7a9e7d73e4a01b9417518d18c001728c45fa8109ed8f55aaa50e7981482`  
		Last Modified: Tue, 12 Oct 2021 01:48:38 GMT  
		Size: 49.2 MB (49222756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10bebdb41abf00ce2793427be3560666b324dbc582685d67cbd222fd9a96c780`  
		Last Modified: Tue, 12 Oct 2021 02:20:12 GMT  
		Size: 7.7 MB (7696033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67efbd5f352709c5700a9d20834d4ba77810ddf79e37c3802037f213ffc2d375`  
		Last Modified: Tue, 12 Oct 2021 02:20:12 GMT  
		Size: 10.0 MB (9984354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599d6477f8aa708e13d4a2801c0ffe0d3f4ed2060acb2ebb516fb609f358cf3b`  
		Last Modified: Tue, 12 Oct 2021 02:20:31 GMT  
		Size: 52.2 MB (52165774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beeb880cfecf2d0e1143d5c71804ca66291d581570bf0ed05e190f9afd856ec9`  
		Last Modified: Tue, 12 Oct 2021 21:50:41 GMT  
		Size: 1.1 MB (1083675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51b23d8066ec1568030b822668939272640beb7b0fc2ef6339bf01b5ef853c30`  
		Last Modified: Tue, 12 Oct 2021 21:50:41 GMT  
		Size: 2.3 MB (2282107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd52c2655cbcac87538d07f805f2100ee323ad5061a6ec7d05f66eb11905cdad`  
		Last Modified: Tue, 12 Oct 2021 21:50:44 GMT  
		Size: 11.9 MB (11871891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2183; amd64

```console
$ docker pull haxe@sha256:03d181ef45b570915340291a508bf8958d0e1f3d24823897d89ccf30dd2d298b
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2713222722 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:89851be1ac277f81ce1c2379a2bd67feb6dfad5f24e50a931b29ff91ee6dd29a`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Mon, 13 Sep 2021 04:08:33 GMT
RUN Install update 1809-amd64
# Wed, 15 Sep 2021 13:14:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 13:14:13 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Sep 2021 13:14:14 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Sep 2021 13:14:15 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Sep 2021 13:14:15 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Sep 2021 13:14:16 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Sep 2021 13:15:12 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 13:16:32 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:17:22 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Sep 2021 13:17:23 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Sep 2021 13:18:25 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:18:26 GMT
ENV HAXE_VERSION=4.2.3
# Wed, 15 Sep 2021 13:22:44 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.3/haxe-4.2.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:23:32 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Sep 2021 13:23:33 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Sep 2021 13:24:22 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 13:25:11 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Sep 2021 13:25:55 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Sep 2021 13:25:56 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a0ddf88812f10c7d6edc858aa9784ff5ca9de4a7bb631909c090090343abd059`  
		Size: 968.4 MB (968365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6c4091e033b8590db7b89fded6d31ac2224162744daa4d7a7a66cbebd4b8c228`  
		Last Modified: Wed, 15 Sep 2021 15:04:44 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4bf2f9de6d0690ec307aa7ae3e887dfa6e4c098acf2d2cbb1d2c7500b57318`  
		Last Modified: Wed, 15 Sep 2021 15:04:43 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa57ef34506aac4c09acc76c7ccd5520b96922bbcce0a89921827c79a7b81d5`  
		Last Modified: Wed, 15 Sep 2021 15:04:42 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba824f569a6227c52a7f2268028fc72f454669fc3cf56f6fd3a447dc1294d5d`  
		Last Modified: Wed, 15 Sep 2021 15:04:41 GMT  
		Size: 1.5 KB (1456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:124c38214ca903c190b5bd5b0b303be1ae81bc8656b4f9309548ec9bf91fb4ce`  
		Last Modified: Wed, 15 Sep 2021 15:04:41 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c399cb6bf356814c0a040600ae5c65bedb10faea4e19c47e16bd365c8f7674`  
		Last Modified: Wed, 15 Sep 2021 15:04:40 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a26194f6a2e4d4c3380182dc390fb75f129711a4ded824d6079127f5840769`  
		Last Modified: Wed, 15 Sep 2021 15:04:39 GMT  
		Size: 353.9 KB (353948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd5a7f61c2e061040b957d8b19b148b536d4d8da99d6349b5fadfa69dd8bde2`  
		Last Modified: Wed, 15 Sep 2021 15:04:53 GMT  
		Size: 12.9 MB (12940205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57266b37b24f40b6627684cc653ecb7ca25ecf0f5dd7ad2a4900d591b6a8e4a`  
		Last Modified: Wed, 15 Sep 2021 15:04:38 GMT  
		Size: 326.7 KB (326661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa382991530ae2bb237a1d8e17bb8de32687807e31f1f4d577e95d0e2558b350`  
		Last Modified: Wed, 15 Sep 2021 15:04:36 GMT  
		Size: 1.4 KB (1376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e30c22063a403723a85bff67c91b52962211c95d2da8655fa470509d38920aba`  
		Last Modified: Wed, 15 Sep 2021 15:04:38 GMT  
		Size: 2.2 MB (2155568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd5db11ad49499d8cb5e5b5d2ee6f2cef2a73f08c298049f2c9bb6c6d1b9d66`  
		Last Modified: Wed, 15 Sep 2021 15:04:35 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e784adebb1e6564dded05249f4364288ad5640150972cd7e977b38bbf2b6d1c7`  
		Last Modified: Wed, 15 Sep 2021 15:04:39 GMT  
		Size: 9.3 MB (9253493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c08ed2077d1842c963b92dd86d1eb99da25964509c905542566c74391d52a5c2`  
		Last Modified: Wed, 15 Sep 2021 15:04:35 GMT  
		Size: 347.3 KB (347340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc50d23a2db96b7f816f141fae2c26daab38478111d4517daf5e5e1de3b28e0`  
		Last Modified: Wed, 15 Sep 2021 15:04:32 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ea7e641e25915a619ca1d744cca8730f66f1a28305e4f8eda16a4d540c4fca`  
		Last Modified: Wed, 15 Sep 2021 15:04:33 GMT  
		Size: 359.1 KB (359107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d403cf083f189600ed8e056529f4bb21bd399d58b2ae2d86e46e761ef02db68`  
		Last Modified: Wed, 15 Sep 2021 15:04:32 GMT  
		Size: 381.7 KB (381672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787d1ca92f9e412bd28ba088d2022dbca61e300a1db89df189bc35a3efc11615`  
		Last Modified: Wed, 15 Sep 2021 15:04:33 GMT  
		Size: 392.8 KB (392844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a44a57d6c35fb28428d8486797235ba3ad4d3f48ffafef7878707bfc5b440f`  
		Last Modified: Wed, 15 Sep 2021 15:04:32 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.4651; amd64

```console
$ docker pull haxe@sha256:e855ab1315554bb4ed3561bc60e1298dfb3d6a3e6250d7af9430b920537f61fb
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6301947027 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a43fa6e28eb0c8dcbcb5ba532c96870163e80c98d5281d129c400e96b9ab3e6`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Mon, 13 Sep 2021 01:03:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Sep 2021 13:26:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Sep 2021 13:26:09 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Sep 2021 13:26:11 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Sep 2021 13:26:12 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Sep 2021 13:26:13 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Sep 2021 13:26:14 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Sep 2021 13:27:20 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 13:28:55 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:29:46 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Sep 2021 13:29:47 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Sep 2021 13:30:53 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:30:54 GMT
ENV HAXE_VERSION=4.2.3
# Wed, 15 Sep 2021 13:35:02 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.3/haxe-4.2.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Sep 2021 13:36:01 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Sep 2021 13:36:02 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Sep 2021 13:36:51 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Sep 2021 13:37:43 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Sep 2021 13:38:31 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Sep 2021 13:38:32 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:e9b8281bf21e46c781fb54e4f15f5728e2c44dea4219c9e6deeb732f1d909d3b`  
		Size: 2.2 GB (2201342322 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5796468f91731000e9a76e836156826a1cd4ed963bcd80e6558c538a12c2132d`  
		Last Modified: Wed, 15 Sep 2021 15:05:15 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb81cf9111761ddfe646e14b3995aeb31cc62dfdd52e54bc224970ba4eba8fb3`  
		Last Modified: Wed, 15 Sep 2021 15:05:14 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa94e80ecf939b785e7cff1a96d5ea8dba0c7ef90c11cdc973895e5c5d6973b5`  
		Last Modified: Wed, 15 Sep 2021 15:05:14 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3cbb5076880a04d79b3f4bfedd245af485d5c68b239477df5344707a1ff8608`  
		Last Modified: Wed, 15 Sep 2021 15:05:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338090c51a577c50769f47c0591d8743479d61d3a73b5368efc88b0abe3ee29a`  
		Last Modified: Wed, 15 Sep 2021 15:05:13 GMT  
		Size: 1.4 KB (1386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178a93c88e06aecb15e50d3916f8bf334090343631079254cd294fc520490c1d`  
		Last Modified: Wed, 15 Sep 2021 15:05:11 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2375ea7a4a97e136359a714deebf459d9074a80c577b796050c0799829022a`  
		Last Modified: Wed, 15 Sep 2021 15:05:11 GMT  
		Size: 343.1 KB (343060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65edc0426667f07b34281a4ac33bbd8435c1048ac15561ee397b356f42f88852`  
		Last Modified: Wed, 15 Sep 2021 15:05:12 GMT  
		Size: 12.9 MB (12887941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25818b3c69036482575c269a2afbe8a4df05b24898f1af31a8295e9848aae663`  
		Last Modified: Wed, 15 Sep 2021 15:05:10 GMT  
		Size: 289.0 KB (289035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a5aef79e155774c5b3a2bd63ff1045491fb5952220cb3b63dd8181f54942083`  
		Last Modified: Wed, 15 Sep 2021 15:05:07 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b9012de45d3e8f06775620e164d1a17f285478cd5861383568cfc4b331d41c`  
		Last Modified: Wed, 15 Sep 2021 15:05:08 GMT  
		Size: 2.1 MB (2112213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0556781b179bae5076ae10759e3163fba02e0c1d334ac40888e8256dd45fcc76`  
		Last Modified: Wed, 15 Sep 2021 15:05:07 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ebc180479f4a02205f2832bcd6e11983a98523d0e6894b6724359a338111aa8`  
		Last Modified: Wed, 15 Sep 2021 15:05:23 GMT  
		Size: 13.7 MB (13724078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b7994ed5cfa8f1053335e40379c87dccd19d79e74732232fb0d0fc7bd4741a`  
		Last Modified: Wed, 15 Sep 2021 15:05:07 GMT  
		Size: 309.3 KB (309302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9a98187ffd7976b27af88a09e9cea507b9d36b1248b3f515b8717b7ace6d5a`  
		Last Modified: Wed, 15 Sep 2021 15:05:04 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d5b19b1fec749752e6ce7f84b02935f62d2d956c5b731dff5b961e064287e3`  
		Last Modified: Wed, 15 Sep 2021 15:05:05 GMT  
		Size: 309.5 KB (309452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007727fcce29825265badb12e4adc700c8c65c0ba7b4b2575f353bd92e9e6dee`  
		Last Modified: Wed, 15 Sep 2021 15:05:04 GMT  
		Size: 314.8 KB (314781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33538dbf2b65b26b76d53126978517724ce20950bad530306028abd5769bd41`  
		Last Modified: Wed, 15 Sep 2021 15:05:05 GMT  
		Size: 315.1 KB (315110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9989736e44fa355640d02b1090faf02c49e6e4ed209a8e15c5f19921b3c91328`  
		Last Modified: Wed, 15 Sep 2021 15:05:04 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
