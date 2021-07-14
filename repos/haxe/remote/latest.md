## `haxe:latest`

```console
$ docker pull haxe@sha256:94720b87cf251452e7453c94139518d9d072ded8cd729ada3c705155f4c3bcfb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2061; amd64
	-	windows version 10.0.14393.4530; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:a313641205bfb74d23ada75df07453b7228d7fe28a8a7f30eff3d66801f25167
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133596950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:838d368a6058bdd9dfdc43fc02e5136c55b1a1b26e3d147a6350ed1de2f8fb44`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:53:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:38:05 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 00:38:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 00:38:10 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 24 Jun 2021 00:39:27 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Fri, 02 Jul 2021 18:38:25 GMT
ENV HAXE_VERSION=4.2.3
# Fri, 02 Jul 2021 18:38:25 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Fri, 02 Jul 2021 18:45:51 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Fri, 02 Jul 2021 18:45:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd09c11b021b756b7a92a4f70a3d444ce7e63a1c24e5749d236dc2c6e68514`  
		Last Modified: Wed, 23 Jun 2021 01:02:12 GMT  
		Size: 51.8 MB (51841560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c01fa01efe10b5523350b9984337667b233972bd3fd7d0c9da46720e305c488`  
		Last Modified: Thu, 24 Jun 2021 01:29:46 GMT  
		Size: 1.3 MB (1314639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c660af7046821c4fb8f3d36ff5ce9c601c4804e9e8169ab6235fab9afb21856`  
		Last Modified: Thu, 24 Jun 2021 01:29:46 GMT  
		Size: 2.3 MB (2308359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c32999d6313afb8394d4a6a7c53e1b66830e6712175ceb32b184b72d7b57f8`  
		Last Modified: Fri, 02 Jul 2021 19:08:48 GMT  
		Size: 9.9 MB (9866523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:2901b3105e880cb912047e142b4edfe69853de10edc0d1ca971dbe6c9031b27b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122742140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f21a90e6bff0f064c348c39a3f05fb038a02ad4ed1bf2c0a9696d9f714d066e`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:01 GMT
ADD file:3edc1a2322b55593b3cd8e935ca6d837e7618bcaaab27a09c9822728f8272ce0 in / 
# Wed, 23 Jun 2021 00:20:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:47:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 16:32:03 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 24 Jun 2021 16:32:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 16:32:14 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 24 Jun 2021 16:35:23 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Fri, 02 Jul 2021 18:56:34 GMT
ENV HAXE_VERSION=4.2.3
# Fri, 02 Jul 2021 18:56:35 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Fri, 02 Jul 2021 19:04:32 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Fri, 02 Jul 2021 19:04:33 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:a3ac2852d9d20585eb4d19973a45b69522d16832456ea5b52f0298b2937afc09`  
		Last Modified: Wed, 23 Jun 2021 00:31:04 GMT  
		Size: 45.9 MB (45917482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d59952ec0a1da3155a9d9a84f07fc99163c3b5429cae2d6d37e9de664191d9d`  
		Last Modified: Wed, 23 Jun 2021 06:18:36 GMT  
		Size: 7.1 MB (7124226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac8017b9330d1a833e533de62b0525c9033b03c74f0d5c3b28b478231b03803`  
		Last Modified: Wed, 23 Jun 2021 06:18:37 GMT  
		Size: 9.3 MB (9343805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065f215c483cb5ee70970d3a4708cdce964e110f4d6e1c6f19ff783e71842fb`  
		Last Modified: Wed, 23 Jun 2021 06:19:26 GMT  
		Size: 47.4 MB (47357244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87b55225459f3bf34c87af6d9603b14161b662fd4f8a0455a1430e7cfcfed317`  
		Last Modified: Thu, 24 Jun 2021 17:31:05 GMT  
		Size: 1.2 MB (1237416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb75a335c353b58b96e7b18adf1f1574098c61cd8a5e51c7140925c0b4fdbeb`  
		Last Modified: Thu, 24 Jun 2021 17:31:07 GMT  
		Size: 2.2 MB (2249770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d03a942ffbd791c51aebfa6f706d9909f04b35c439d41c86851b1ffdd7411e9`  
		Last Modified: Fri, 02 Jul 2021 19:08:59 GMT  
		Size: 9.5 MB (9512197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:7a4cb1fb1441e4f242b8b66db99f01a9f59fd93561aedc287dcd272943252973
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.8 MB (134764021 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62cc541869d23fe1bf4bd8c6b237eeb2ea4f3190f9d968e19743f0fc0725e60f`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:33:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Jun 2021 17:33:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 17:33:50 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 23 Jun 2021 17:35:00 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Fri, 02 Jul 2021 18:19:59 GMT
ENV HAXE_VERSION=4.2.3
# Fri, 02 Jul 2021 18:19:59 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Fri, 02 Jul 2021 18:24:43 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.3 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Fri, 02 Jul 2021 18:24:43 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785171b903c4d81c5b7539417a7b05f4a9bc6a35840595233bf4e369d8aee387`  
		Last Modified: Wed, 23 Jun 2021 00:33:41 GMT  
		Size: 52.2 MB (52165169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbddee1ea55c22890e4bdaad2f5dac7baf75bfbdb7c08493de32b4804ff49312`  
		Last Modified: Wed, 23 Jun 2021 18:26:38 GMT  
		Size: 1.3 MB (1306690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53bf918e22837bcffa9c51cd28e3967b3c45e5733fca882f5b0bcd0fd974809`  
		Last Modified: Wed, 23 Jun 2021 18:26:38 GMT  
		Size: 2.3 MB (2302988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bdbcc4c20436e8b89c9707ee3b464734e2300a682119e55562973ad1a381dc3`  
		Last Modified: Fri, 02 Jul 2021 18:46:36 GMT  
		Size: 12.1 MB (12088192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2061; amd64

```console
$ docker pull haxe@sha256:ea308ec137c2fd0cb5f6c2832b61e9c6404ba9b3c63f54f557acbda9f5ad6440
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2712086495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4fbdb06fad52b13fa8cfac913e734d51db6bc1fd2246b6627ee9366dd23d8279`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 06 Jul 2021 20:34:18 GMT
RUN Install update 1809-amd64
# Wed, 14 Jul 2021 01:07:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 12:25:36 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 14 Jul 2021 12:25:38 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 14 Jul 2021 12:25:40 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 14 Jul 2021 12:25:43 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 14 Jul 2021 12:25:46 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 14 Jul 2021 12:26:46 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 12:28:33 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:29:31 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 14 Jul 2021 12:29:34 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 14 Jul 2021 12:30:56 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:30:58 GMT
ENV HAXE_VERSION=4.2.3
# Wed, 14 Jul 2021 12:35:52 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.3/haxe-4.2.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:36:53 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 14 Jul 2021 12:36:55 GMT
ENV HOMEDRIVE=C:
# Wed, 14 Jul 2021 12:38:02 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 12:39:22 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 14 Jul 2021 12:40:31 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 14 Jul 2021 12:40:35 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f143c6fed32d477c35b660b2e108ea62e3593c03e44bd9ced208ce52b26b0841`  
		Size: 967.1 MB (967113907 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:adcec6ff907307155c0652222cc9b95a0cc964d4c371e02767e72a5c90472192`  
		Last Modified: Wed, 14 Jul 2021 02:02:19 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02cae031c0896dc2164ed3e3e5a4b1939ade49a7d61ef7ba1be05ab68dee9202`  
		Last Modified: Wed, 14 Jul 2021 14:57:47 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f665f8055b8869cbbac5d9eee3c7d8520b3ebac368594481d7bbbfdfe933ca`  
		Last Modified: Wed, 14 Jul 2021 14:57:47 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cab2bc1f0a73f5d08b39282bd01c224dda25db057920ca9801a06493fb73c5ce`  
		Last Modified: Wed, 14 Jul 2021 14:57:45 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:465c7534c49266311be96348b027380011a1acb7f61f28880ece87196a19ecaa`  
		Last Modified: Wed, 14 Jul 2021 14:57:44 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1cd9ec5f0845d2f7b535f6faebf8cfe2de4a51b697a58022acc4ead735e470f`  
		Last Modified: Wed, 14 Jul 2021 14:57:44 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f581e8e3cfc722c7717703defcb2069afa611c86012d84a267460971411c49a5`  
		Last Modified: Wed, 14 Jul 2021 14:57:42 GMT  
		Size: 369.0 KB (369007 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d1603b84e7d2ad8c7766f947a0706300fea913df72e8c0f86708c27104b4889`  
		Last Modified: Wed, 14 Jul 2021 14:57:56 GMT  
		Size: 12.9 MB (12943198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28350b3475a531f8761cd444e34ad5f824bffc9aa14a2156c9bf92ca8cff0a0c`  
		Last Modified: Wed, 14 Jul 2021 14:57:42 GMT  
		Size: 336.6 KB (336646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9199f6eab98249a2f59f33297e72e105343ebe929d732c071cd5b9937b1c03a`  
		Last Modified: Wed, 14 Jul 2021 14:57:39 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:915ae5c02861ac4c5615c51756b4f7074de7bdf4904c1ec79d4d754c6a8cc751`  
		Last Modified: Wed, 14 Jul 2021 14:57:42 GMT  
		Size: 2.2 MB (2168440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39a66cbecb550dfb4f9fc1aecd86a7b86d424291bc47774c3fcc25843a38338a`  
		Last Modified: Wed, 14 Jul 2021 14:57:39 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60cf61f0428095f91bdc9e3241fce765e8557c392bbf2333a63460bc4c570737`  
		Last Modified: Wed, 14 Jul 2021 14:57:51 GMT  
		Size: 9.3 MB (9262853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f0c2fb85e00acc585729680c4131fa6e6b9fff0bd7e0c1de7274f1fc9446a4e`  
		Last Modified: Wed, 14 Jul 2021 14:57:39 GMT  
		Size: 363.6 KB (363612 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c59eba2b0fc85b599e75ae2aab00c46cafe03d05e40136c19e8be9701d067a2`  
		Last Modified: Wed, 14 Jul 2021 14:57:36 GMT  
		Size: 1.3 KB (1296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04046a8edc55ce5306ffa18d79b46c8c00e6827e2640a93b1224f7ffb20cd2c8`  
		Last Modified: Wed, 14 Jul 2021 14:57:37 GMT  
		Size: 375.2 KB (375247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:961bd50b002860a303b2af2a333cc21fd950bd7b59b31449156809ab525a1347`  
		Last Modified: Wed, 14 Jul 2021 14:57:36 GMT  
		Size: 397.7 KB (397719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dfd518edc7c335a9687db85045a20720e3e6b6e3468cfe7a8d719a39ec7dcf`  
		Last Modified: Wed, 14 Jul 2021 14:57:36 GMT  
		Size: 409.0 KB (408968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:170135c692e8e96114ccef28c5db57cbc4ae1bcb5a094799dbc9e00d9f6db050`  
		Last Modified: Wed, 14 Jul 2021 14:57:36 GMT  
		Size: 1.3 KB (1317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.4530; amd64

```console
$ docker pull haxe@sha256:266101e520e5eda0acb2a0f49376d6691db7c22a400dad2ceb552703dfcea049
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6309444560 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f85fd17891b89d8e8c4d11523d23d72059f02350c69ae4b814750f84e5c7d7b0`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 09 Jul 2021 05:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Jul 2021 01:14:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Jul 2021 12:40:54 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 14 Jul 2021 12:40:56 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 14 Jul 2021 12:40:59 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 14 Jul 2021 12:41:02 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 14 Jul 2021 12:41:04 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 14 Jul 2021 12:42:31 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 12:44:44 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:46:05 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 14 Jul 2021 12:46:08 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 14 Jul 2021 12:48:17 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:48:19 GMT
ENV HAXE_VERSION=4.2.3
# Wed, 14 Jul 2021 12:53:37 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.3/haxe-4.2.3-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '6a5b19f6fa9f46c42c4df9f154b02d55cbacf0cc76ea5a03906cfd8300216a32') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 14 Jul 2021 12:55:02 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 14 Jul 2021 12:55:05 GMT
ENV HOMEDRIVE=C:
# Wed, 14 Jul 2021 12:56:24 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Jul 2021 12:57:55 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 14 Jul 2021 12:59:22 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 14 Jul 2021 12:59:25 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a567de41cc349380b25967f180fb1b6b2431bda61ccaaf69d78a33bc9523614a`  
		Size: 2.2 GB (2199646155 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fed351b78c876c55ec9c7e75d3b9d1b146c5c5dfeb4b5480c0a7c384322df98c`  
		Last Modified: Wed, 14 Jul 2021 02:03:37 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309dc82e836996ad875d1822fac3e5584ae0e0222a97fd030269fdcef96dd528`  
		Last Modified: Wed, 14 Jul 2021 14:58:21 GMT  
		Size: 1.4 KB (1400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6570fb7e30e5e194f19913da68c72c21fa2195a2443b84f1e43df7f75b13dcc9`  
		Last Modified: Wed, 14 Jul 2021 14:58:20 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df1d454140ac54f42bda0828162ff00e63ea0a874f207cce54048cdf48d27b96`  
		Last Modified: Wed, 14 Jul 2021 14:58:19 GMT  
		Size: 1.4 KB (1443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612f6ff3fa70bf748fe89a932d306d032c845afcbb929995543b75500301392`  
		Last Modified: Wed, 14 Jul 2021 14:58:18 GMT  
		Size: 1.4 KB (1384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e4875d17c82c7959f5681bc28cf7b7776cb5d4ce98216e9dfee5cad6084dbc`  
		Last Modified: Wed, 14 Jul 2021 14:58:17 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763be4e0afb4c49ccdb19cbbe7fb8493a3b30b01ccc2dd2b4260a306fda550f2`  
		Last Modified: Wed, 14 Jul 2021 14:58:15 GMT  
		Size: 358.5 KB (358549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8083b767bc2746a163b0b8ac5edfde58156f4bcc269a0b933a9cc4b1c82207`  
		Last Modified: Wed, 14 Jul 2021 14:58:19 GMT  
		Size: 17.3 MB (17316168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c546b1c53e3fdb5b95ca0f397cca7d73d211837721d8cf4dac4fd87426b6345`  
		Last Modified: Wed, 14 Jul 2021 14:58:15 GMT  
		Size: 307.2 KB (307208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2c03ce4a4fcfffe7e97dcfe97f2da65c32db697b4a6c977ed269d98f5d9be4e`  
		Last Modified: Wed, 14 Jul 2021 14:58:11 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f8945706e18d74d2587b0d813064e3cd2dc15c9bdaae1b47c10961cda401226`  
		Last Modified: Wed, 14 Jul 2021 14:58:14 GMT  
		Size: 6.6 MB (6586981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd6b9b50886f069742da8c1139918c3e945b6cdfc6851559287311729e012e5`  
		Last Modified: Wed, 14 Jul 2021 14:58:11 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699e4e317568d3ca63e889d22fa8378b6a175e437e2f33b1a6757042b642ffc9`  
		Last Modified: Wed, 14 Jul 2021 14:58:19 GMT  
		Size: 13.9 MB (13909168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a05e42d95c83133cd99f55ddb94fb8dd6e8206f095bf449ac92d0bf5cc115d6`  
		Last Modified: Wed, 14 Jul 2021 14:58:11 GMT  
		Size: 326.1 KB (326126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e9d534d379223007ed2d445c487c8757d9666ed8694f613552c7fbfaa99cbc`  
		Last Modified: Wed, 14 Jul 2021 14:58:08 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db9c07b8da63147d6f7d5c68140eb064c706517776f0bcc4153f8ccffc19b01`  
		Last Modified: Wed, 14 Jul 2021 14:58:08 GMT  
		Size: 326.7 KB (326701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797fc21c1f55439df8c7e1fd67233398f2b26b0b6a5673cbe74a364b32f51957`  
		Last Modified: Wed, 14 Jul 2021 14:58:08 GMT  
		Size: 333.1 KB (333140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3562b6bd0d061216bedd2bcf4f25267aac61a2af0e6bbe58da413b57147897`  
		Last Modified: Wed, 14 Jul 2021 14:58:08 GMT  
		Size: 334.4 KB (334422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b674d7c31f05296e8335dc67b4bdb05ad3142fdc4059f84d8e414747c14aca5f`  
		Last Modified: Wed, 14 Jul 2021 14:58:08 GMT  
		Size: 1.4 KB (1374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
