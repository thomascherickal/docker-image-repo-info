## `haxe:latest`

```console
$ docker pull haxe@sha256:f1b91154017e3279fc732ef30bfa7399fd583f054bc97f2013fe05ef23389a46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2366; amd64
	-	windows version 10.0.14393.4825; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:6dec703c3515cd055c51b5650dccdc37788a02f6f9a4cbdbd315cb50cde7a96d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.9 MB (139859041 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba39d6a1198372491e4e9accf3956d42ea616b3473b4e86e283d7a2f8747fb36`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 21 Dec 2021 01:22:32 GMT
ADD file:c03517c5ddbed4053165bfdf984b27a006fb5f533ca80b5798232d96df221440 in / 
# Tue, 21 Dec 2021 01:22:32 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 01:51:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 01:51:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 01:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:13:08 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 08:13:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 08:13:13 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 22 Dec 2021 08:14:38 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 22 Dec 2021 08:14:39 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 22 Dec 2021 08:14:39 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 22 Dec 2021 08:18:30 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 22 Dec 2021 08:18:30 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:0e29546d541cdbd309281d21a73a9d1db78665c1b95b74f32b009e0b77a6e1e3`  
		Last Modified: Tue, 21 Dec 2021 01:27:20 GMT  
		Size: 54.9 MB (54919034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b829c73b52b92b97d5c07a54fb0f3e921995a296c714b53a32ae67d19231fcd`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 5.2 MB (5152816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5b7ae361722f070eca53f35823ed21baa85d61d5d95cd5a95ab53d740cdd56`  
		Last Modified: Tue, 21 Dec 2021 02:01:26 GMT  
		Size: 10.9 MB (10871868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6494e4811622b31c027ccac322ca463937fd805f569a93e6f15c01aade718793`  
		Last Modified: Tue, 21 Dec 2021 02:01:49 GMT  
		Size: 54.6 MB (54566215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0faaf68f2ca6bc4f42335fca8082626d8c74914413fb0c0692eba65b2715531`  
		Last Modified: Wed, 22 Dec 2021 09:05:45 GMT  
		Size: 1.4 MB (1366597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5166aa1165ffc95a40b40e95211a9970cea70857f9ec29f41f1ab97674886c50`  
		Last Modified: Wed, 22 Dec 2021 09:05:44 GMT  
		Size: 1.4 MB (1446197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2377564f8e2faee41bdb3b32e37f1d936370607475f3cd0203f06b686df599b8`  
		Last Modified: Wed, 22 Dec 2021 09:05:48 GMT  
		Size: 11.5 MB (11536314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:61ab9c4b7435b21e96ad31ea46c111ed5887b80732d8f791f71ce6e2845fe215
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.4 MB (129357229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84d4d07b2a8be10f38f2f1ea9512e9c8f2c2850a1cce19537ea3066615efddd0`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 21 Dec 2021 01:59:11 GMT
ADD file:848bf729bc16d3b188567f096ee1c0386cb49825a06eef396401278afee2f4c7 in / 
# Tue, 21 Dec 2021 01:59:12 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:46:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:46:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:47:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 16:32:58 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Dec 2021 16:33:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Dec 2021 16:33:09 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 22 Dec 2021 16:36:23 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 22 Dec 2021 16:36:24 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 22 Dec 2021 16:36:24 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 22 Dec 2021 16:42:13 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 22 Dec 2021 16:42:14 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:fd92fbcda272f5935dcd0dfea445cba0152208f83c8fc8d2cb74c85379145c42`  
		Last Modified: Tue, 21 Dec 2021 02:14:41 GMT  
		Size: 50.1 MB (50121433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a6987ee02fad9d702adbd7921b8e1776b1a091773dd47886055113b1d7ba62`  
		Last Modified: Tue, 21 Dec 2021 03:11:46 GMT  
		Size: 4.9 MB (4922490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6d85cbb278c8e4845f79838154b77c36931e65f9b5bb9b8f56c92f41f72e27`  
		Last Modified: Tue, 21 Dec 2021 03:11:47 GMT  
		Size: 10.2 MB (10217004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46bd566d277d8d03e1b76768a074dd92306bc287eef88c42a08ef5b48b842fa1`  
		Last Modified: Tue, 21 Dec 2021 03:12:37 GMT  
		Size: 50.3 MB (50328047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d71b199c3723f8195e65583fa807e89a8d7931acf90356f7651670a8d2f50d`  
		Last Modified: Wed, 22 Dec 2021 17:56:30 GMT  
		Size: 1.3 MB (1280013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4547bb94ae8041f87a94636c80669115e9bc092937d7ece0c25de953b0f31e3`  
		Last Modified: Wed, 22 Dec 2021 17:56:31 GMT  
		Size: 1.4 MB (1386973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b1afe29cb6b112ae4956f5aa83b26337b4a05ad61d097aa5b71830e4e5b9f9`  
		Last Modified: Wed, 22 Dec 2021 17:56:38 GMT  
		Size: 11.1 MB (11101269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:a27724e2a8d8774ef7d4eefbde0885b54bc24573c38681877b3c19334fefe78d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.6 MB (139591602 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:845542786ba00b4d4e165a4972e45175f34ce7f96d77632a37af08e5d4aff5b6`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 21 Dec 2021 01:42:08 GMT
ADD file:9d88e8701cd12aaee44dac3542cc3e4586f6382541afff76e56e8fb5275387d3 in / 
# Tue, 21 Dec 2021 01:42:09 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:12:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:12:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 02:12:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:50:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 21 Dec 2021 18:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 18:50:31 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 21 Dec 2021 18:51:44 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 21 Dec 2021 18:51:45 GMT
ENV HAXE_VERSION=4.2.4
# Tue, 21 Dec 2021 18:51:45 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 21 Dec 2021 18:54:30 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 21 Dec 2021 18:54:31 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:94a23d3cb5be24659b25f17537307e7f568d665244f6a383c1c6e51e31080749`  
		Last Modified: Tue, 21 Dec 2021 01:48:23 GMT  
		Size: 53.6 MB (53604608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9d381bd1e98fa8759f80ff42db63c8fce4ac9407b2e7c8e0f031ed9f96432b`  
		Last Modified: Tue, 21 Dec 2021 02:22:29 GMT  
		Size: 5.1 MB (5141526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9c5b49b9db3dd2553e8ae6c2081b77274ec0a8b1f9903b0e5ac83900642098`  
		Last Modified: Tue, 21 Dec 2021 02:22:30 GMT  
		Size: 10.7 MB (10655891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841dd868500b6685b6cda93c97ea76e817b427d7a10bf73e9d03356fac199ffd`  
		Last Modified: Tue, 21 Dec 2021 02:22:52 GMT  
		Size: 54.7 MB (54668906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6bdfc152f27222e2e4026cee2479e9f195c380af3d3853d580e9f2dff2ceddf`  
		Last Modified: Tue, 21 Dec 2021 19:32:51 GMT  
		Size: 1.1 MB (1133599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b1faa2e66ee9a81258d0b26f0b4dffa469bae4cd6b1fdfa60660d733e4ea98`  
		Last Modified: Tue, 21 Dec 2021 19:32:51 GMT  
		Size: 1.4 MB (1432107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69397f7345ced593bc83acf4b6963cd33ddc9f4901632deaa11a9a8097262fb6`  
		Last Modified: Tue, 21 Dec 2021 19:32:54 GMT  
		Size: 13.0 MB (12954965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2366; amd64

```console
$ docker pull haxe@sha256:2b7aee6c76c8ca981d2c53c31e3cbf94b462cefdaedce3385a0d9ce8aebb9691
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2735320068 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a0ff484a920e6cc9fafe9e1ae5916122624accd5a731e10509b93cc146e15d9e`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Tue, 07 Dec 2021 04:56:01 GMT
RUN Install update 1809-amd64
# Sat, 18 Dec 2021 01:40:43 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 01:40:44 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Sat, 18 Dec 2021 01:40:45 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Sat, 18 Dec 2021 01:40:45 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Sat, 18 Dec 2021 01:40:46 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Sat, 18 Dec 2021 01:40:47 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Sat, 18 Dec 2021 01:42:05 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 01:43:55 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 01:44:55 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Sat, 18 Dec 2021 01:44:56 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 18 Dec 2021 01:46:18 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 01:46:19 GMT
ENV HAXE_VERSION=4.2.4
# Sat, 18 Dec 2021 01:51:29 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 01:52:38 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Sat, 18 Dec 2021 01:52:39 GMT
ENV HOMEDRIVE=C:
# Sat, 18 Dec 2021 01:53:35 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 01:54:32 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Sat, 18 Dec 2021 01:55:29 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Sat, 18 Dec 2021 01:55:30 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5ee7a7ea9cf22f75886179907a41810a992e21f3d0c57cc10d2147ce9237701c`  
		Size: 990.3 MB (990271574 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d22d2238b031d3f13bcd6c144e80f8f8402332b8ee8e53cc54b7912c3ac808cb`  
		Last Modified: Sat, 18 Dec 2021 03:59:34 GMT  
		Size: 1.4 KB (1444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf8992680ce2d4af9c0ad9ae585616431f1ef34200773550bba65740d3b498f`  
		Last Modified: Sat, 18 Dec 2021 03:59:32 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f8b22240f3643204aabbb321fff4feca4704c5b1dcac9c206b832eb6e95dfbf`  
		Last Modified: Sat, 18 Dec 2021 03:59:32 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d7615dc0c85a2150156a25e25936b93743f2550ceb67c5a297d03ee5306ef9f`  
		Last Modified: Sat, 18 Dec 2021 03:59:32 GMT  
		Size: 1.4 KB (1449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cdf96740d548343f53aa07eec9f0f09856f790b5a80efb87bd69bdc03e2c2a3`  
		Last Modified: Sat, 18 Dec 2021 03:59:30 GMT  
		Size: 1.4 KB (1397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1dd0eff5377209ca80f30ae095b223b0052566f0dd731d9c8d65e89f2522fac`  
		Last Modified: Sat, 18 Dec 2021 03:59:29 GMT  
		Size: 1.4 KB (1393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a67606011496c42ed988c613d6f1b64f7705d20fbe403b84ea6202f55206535`  
		Last Modified: Sat, 18 Dec 2021 03:59:29 GMT  
		Size: 370.5 KB (370463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48fc01004dedd8643cf047fcf3d61459c7677a0868d584039f297546be7893c2`  
		Last Modified: Sat, 18 Dec 2021 03:59:41 GMT  
		Size: 13.0 MB (12950611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d22e89d57d59a91ece0417f7cf2f88e3f42c0073d904828824c6d4c706cee942`  
		Last Modified: Sat, 18 Dec 2021 03:59:27 GMT  
		Size: 344.3 KB (344347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5782f8bf7e0d38139bd37d7a8129693a6512d1aca6bef5bbb663ef2b28db748`  
		Last Modified: Sat, 18 Dec 2021 03:59:25 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4004c471b4fc8ca30a4bcd7eb31cb054c6d9750f98cafe16e6e8d7dba1f8d4e`  
		Last Modified: Sat, 18 Dec 2021 03:59:26 GMT  
		Size: 2.2 MB (2176634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed613e5bddffe26995cabbbb5b801e32da07c22b90f6cb5f87bd807ed05c551`  
		Last Modified: Sat, 18 Dec 2021 03:59:25 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43e7d5738c5fbe1f28ead025b13cdf625b0937d1b4468ea15b6daeb25c5ac523`  
		Last Modified: Sat, 18 Dec 2021 03:59:36 GMT  
		Size: 9.3 MB (9279666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dc9e79b19e73cbd5ead1406e2d01de46c52ea0b586a330d9e9060c1851db17`  
		Last Modified: Sat, 18 Dec 2021 03:59:25 GMT  
		Size: 374.2 KB (374219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9330ef58b37f636d19ebb5ec615194fb87fb2b9377a56a26f922e163310e3f84`  
		Last Modified: Sat, 18 Dec 2021 03:59:22 GMT  
		Size: 1.4 KB (1398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9e5ff78d2715bb27ffd5983145de83a0089f3262ef46da912d5be4e6c60806`  
		Last Modified: Sat, 18 Dec 2021 03:59:23 GMT  
		Size: 385.1 KB (385108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0cd0726c7d242a9d54b05d591d51152d2a40135ad570827abc01ab0c9494bd2`  
		Last Modified: Sat, 18 Dec 2021 03:59:23 GMT  
		Size: 402.4 KB (402417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4716d0a002925f290957606ee58684846c67c4a94cd28218402ecc709cdbff49`  
		Last Modified: Sat, 18 Dec 2021 03:59:23 GMT  
		Size: 418.1 KB (418063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:541e6cd80aff89651c02b86c9336457f43e9103e35985673cb0f1184794a2a61`  
		Last Modified: Sat, 18 Dec 2021 03:59:22 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.4825; amd64

```console
$ docker pull haxe@sha256:0a394ca679d417b9beaeb5c2f50e457876e31261f845a6652fa40e1345c9fe2e
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6309802925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eaa4f04bfb0fdecef3d5adc395e9b9aeb11941ac57873750c24b0b6793cdc05f`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 08 Dec 2021 08:38:00 GMT
RUN Install update ltsc2016-amd64
# Sat, 18 Dec 2021 01:55:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Sat, 18 Dec 2021 01:55:45 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Sat, 18 Dec 2021 01:55:46 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Sat, 18 Dec 2021 01:55:47 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Sat, 18 Dec 2021 01:55:47 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Sat, 18 Dec 2021 01:55:48 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Sat, 18 Dec 2021 01:56:55 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 01:58:41 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 01:59:44 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Sat, 18 Dec 2021 01:59:45 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 18 Dec 2021 02:01:07 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 02:01:08 GMT
ENV HAXE_VERSION=4.2.4
# Sat, 18 Dec 2021 02:06:08 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Sat, 18 Dec 2021 02:07:18 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Sat, 18 Dec 2021 02:07:19 GMT
ENV HOMEDRIVE=C:
# Sat, 18 Dec 2021 02:08:19 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Sat, 18 Dec 2021 02:09:18 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Sat, 18 Dec 2021 02:10:14 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Sat, 18 Dec 2021 02:10:15 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d026d646213ccf73d9f0584941d108253d62e73df2a74e070776884b7b0242b`  
		Size: 2.2 GB (2204728802 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6bffd19db3f71ba2031bea25a529c67034869e7e1bbf9e2431d5ee747bd6d6d`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33d653277249e5990a8dda22ec0129398448a0e0d0444c688db0dbf5346985b6`  
		Last Modified: Sat, 18 Dec 2021 04:00:01 GMT  
		Size: 1.3 KB (1321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886c32f684de6b912b34abf5867c4afca31eaa13e96fecf0a9cb5083d386714d`  
		Last Modified: Sat, 18 Dec 2021 04:00:00 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32ae69ff81f435b844c5d682172d7ebf29f3f05575d302b1fb0a8045c649ad5f`  
		Last Modified: Sat, 18 Dec 2021 03:59:58 GMT  
		Size: 1.3 KB (1295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3204508cf2d3a66009579b3b310c46018c609629eaaa4fd90dad017347462f53`  
		Last Modified: Sat, 18 Dec 2021 03:59:59 GMT  
		Size: 1.3 KB (1332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0490fac80047e9268972b975a9de1e32d16ea615514093bdcebab34a76a6eb4`  
		Last Modified: Sat, 18 Dec 2021 03:59:58 GMT  
		Size: 1.3 KB (1316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c88cd9012ca0fdf2c5238797a6f92661eda97181a911812e7194d2e6b0c857`  
		Last Modified: Sat, 18 Dec 2021 03:59:56 GMT  
		Size: 332.7 KB (332724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5052f01aed104a9d176c0ae0d602326dbb22b24b2ac39e9fa13a91b52facb8af`  
		Last Modified: Sat, 18 Dec 2021 04:00:15 GMT  
		Size: 17.4 MB (17382081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ade96f46ba499b84706549de203af397e3310d06fa952f47fbb8bf722ec39c`  
		Last Modified: Sat, 18 Dec 2021 03:59:56 GMT  
		Size: 291.4 KB (291389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e018d267a734cf863823558dd8c0e455bd8fc63ef0aaf06b20f8beda7bb23fdd`  
		Last Modified: Sat, 18 Dec 2021 03:59:54 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fec399c5a120704550ef9a34ad3ca5fc4c026b435a8dc850886dac3def63c119`  
		Last Modified: Sat, 18 Dec 2021 03:59:55 GMT  
		Size: 2.1 MB (2115370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67164ff43f13f0eeb60a84bde8219058953bcc061fc10ab9a4aae8f95a56bc29`  
		Last Modified: Sat, 18 Dec 2021 03:59:53 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b825f5fcb9f2b837d8a66768684c4d24ce1427e50bf6ab221978af0270d3ceaa`  
		Last Modified: Sat, 18 Dec 2021 04:00:09 GMT  
		Size: 13.7 MB (13700491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40611e133d72b59f6ff42c570a66ffd756c0c660694659efa5f6275ecf0c9bbd`  
		Last Modified: Sat, 18 Dec 2021 03:59:53 GMT  
		Size: 309.2 KB (309204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d830ac5ff5cf07f553efeb3edf608977c4e38a3f5f960338e6dade23dcce6eab`  
		Last Modified: Sat, 18 Dec 2021 03:59:51 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96bc535fb5ea4fd05ccce0078c63c87551a627aadfb386b20527b14a2bb4e755`  
		Last Modified: Sat, 18 Dec 2021 03:59:51 GMT  
		Size: 309.6 KB (309613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c1d97e8b388a7d07015e6fc392b1dafcb48485ffe9aae4815c86877e1f3a146`  
		Last Modified: Sat, 18 Dec 2021 03:59:51 GMT  
		Size: 316.7 KB (316735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7808551a260e7f0548bd7dd3211da60470739cae0aa6c80f6a14c4a69675642b`  
		Last Modified: Sat, 18 Dec 2021 03:59:51 GMT  
		Size: 317.2 KB (317224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503ac3a4112cab0aaa0d59ff2c63f0f130f378c6fafef82a8df815139973326b`  
		Last Modified: Sat, 18 Dec 2021 03:59:51 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
