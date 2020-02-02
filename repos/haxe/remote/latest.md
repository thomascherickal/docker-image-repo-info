## `haxe:latest`

```console
$ docker pull haxe@sha256:1b0c9908856348dd6fef0acc1c64816477f77477a632c3073f0f2abb690df6f2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.973; amd64
	-	windows version 10.0.14393.3443; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:c9ef17fa673f7268cb665b2135e82ee1dbe3753da5fdde7fd774963dadfe9f1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.1 MB (132061450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e71251ffb5dbd980ea0081ebc88dfd4204c31fccd51c31c934395f8c2d90b7d5`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:11:49 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 14:11:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 14:11:55 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 02 Feb 2020 14:13:13 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 02 Feb 2020 14:13:13 GMT
ENV HAXE_VERSION=4.0.5
# Sun, 02 Feb 2020 14:13:13 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 02 Feb 2020 14:15:57 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 02 Feb 2020 14:15:57 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac92ddf84b35dac36ef6632f8d5a0c9c2d7038f6018f2d4fa1be056d90bd366`  
		Last Modified: Sun, 02 Feb 2020 00:38:05 GMT  
		Size: 51.8 MB (51791113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01edb32150e60b7d7779f8830a9a0b41ca0b58d579de65b88651ba24f585ccd0`  
		Last Modified: Sun, 02 Feb 2020 14:57:26 GMT  
		Size: 1.3 MB (1310662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84da5a46b0492611c3c380f08fdb90e2022192037d975e0b48752fe501ef608a`  
		Last Modified: Sun, 02 Feb 2020 14:57:26 GMT  
		Size: 2.4 MB (2417291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6f3ecdd88c1560338dd97e49b74a7263e87187e6407b7a091933b4cba8c6766`  
		Last Modified: Sun, 02 Feb 2020 14:57:28 GMT  
		Size: 8.4 MB (8354690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:c043f7d587a8c0a65996eb01967fde496bf9d6ec6395974da57cc1e9a5a99252
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121257409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c07c4960daafb074fea2acb2697399d3bcbabf78c201e55289a8e8d09b7a84d0`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 13:38:04 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 13:38:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 13:38:17 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 02 Feb 2020 13:41:26 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 02 Feb 2020 13:41:28 GMT
ENV HAXE_VERSION=4.0.5
# Sun, 02 Feb 2020 13:41:28 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 02 Feb 2020 13:49:18 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 02 Feb 2020 13:49:19 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71b77f0351b9ec2d9a20055b0d19a04b8a3f10da89da18d6b883e3f2e11e422c`  
		Last Modified: Sun, 02 Feb 2020 14:24:06 GMT  
		Size: 1.2 MB (1232765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:389864dff7a41a78f0fc78e18ab0b908d967def43e7f8cb422c8ab821f1e10f3`  
		Last Modified: Sun, 02 Feb 2020 14:24:06 GMT  
		Size: 2.4 MB (2357160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5badcbe028ef2950cbc8d359c7fec5b6c80f7121c75897845e26d940f330c47f`  
		Last Modified: Sun, 02 Feb 2020 14:24:09 GMT  
		Size: 8.1 MB (8052692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:473f88252aa9127d9de16fe21001f72ec285d7b8738444c4020ef0385a65ca39
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.0 MB (133002738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9b6c19075667412df9f5585de7472da04b384c71f35b6339403587ab28af8b8d`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:50 GMT
ADD file:b423f4b0ed41dfe1334031fe9b21f7e1c88ccb031d7e8f2ff165d618323424d7 in / 
# Sat, 01 Feb 2020 16:40:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 13:49:03 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 02 Feb 2020 13:49:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 13:49:16 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 02 Feb 2020 13:53:07 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 02 Feb 2020 13:53:08 GMT
ENV HAXE_VERSION=4.0.5
# Sun, 02 Feb 2020 13:53:09 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 02 Feb 2020 13:59:39 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.0.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 02 Feb 2020 13:59:41 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:bc03a7ced18fc43ea9523dfb256d2c3fbb835dc0bb54bdb7fd309edf936a87e7`  
		Last Modified: Sat, 01 Feb 2020 16:46:06 GMT  
		Size: 49.2 MB (49171687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d528c1473d79c18b401d44ca06b9733d9c51a8699b98e8325c9de60b9739`  
		Last Modified: Sat, 01 Feb 2020 17:34:59 GMT  
		Size: 7.7 MB (7680993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981400d5d268dc989681d5f308b7d2e381809f0bcc82429f443f7539cf6117ba`  
		Last Modified: Sat, 01 Feb 2020 17:34:59 GMT  
		Size: 10.0 MB (9983754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b2d547b8bc79a444406e56d724fb7d961c953e7f2797de4f55b29abee5605f`  
		Last Modified: Sat, 01 Feb 2020 17:35:22 GMT  
		Size: 52.1 MB (52102938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd99e9408745cf82856ec1abbe20a3dedda929e1b7376e88d16b3a5e27caaca8`  
		Last Modified: Sun, 02 Feb 2020 14:29:31 GMT  
		Size: 1.3 MB (1301746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9eb6cfb94494ba636a6a75e7f9a6317ad0615d99f16085392d1d82fd06a6982`  
		Last Modified: Sun, 02 Feb 2020 14:29:31 GMT  
		Size: 2.4 MB (2414824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df38316350953f5e14ee837e54eb022168419622b8cd2f7192e774dec23520f`  
		Last Modified: Sun, 02 Feb 2020 14:29:35 GMT  
		Size: 10.3 MB (10346796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.973; amd64

```console
$ docker pull haxe@sha256:b18749d18d26160a3096e5b7ab683f84ba8f53fc8431518bdfb73823b4724029
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 GB (2250147199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f502bc41b0bf5fd5ce3322308b80c393a3508fd11c7ed8bf4867e781b0a44b88`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 11 Jan 2020 05:23:25 GMT
RUN Install update 1809-amd64
# Wed, 15 Jan 2020 14:40:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 14:40:32 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Jan 2020 14:40:33 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Jan 2020 14:40:34 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Jan 2020 14:40:36 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Jan 2020 14:40:37 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Jan 2020 14:41:16 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jan 2020 14:42:28 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 14:42:52 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Jan 2020 14:42:53 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Jan 2020 14:43:36 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 14:43:37 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 15 Jan 2020 14:48:22 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 14:48:46 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Jan 2020 14:48:47 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Jan 2020 14:49:10 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jan 2020 14:49:36 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Jan 2020 15:20:27 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Jan 2020 15:20:28 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:edbd72df76b46e904108d2f61a63c295b3e3d8092dbd5a03bbeb2fb4d34a3e55`  
		Size: 682.7 MB (682725872 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2397868e5c7aa285f662aaa9309fa4756277739e11d589a663a204df80595f2c`  
		Last Modified: Wed, 15 Jan 2020 17:10:53 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df8e05ad847891168937138971a001c0a8afd61048713fe683f1222e3699c80f`  
		Last Modified: Wed, 15 Jan 2020 17:10:51 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81911356504055f5efca56a0c659d4e1edc5a88bfb1c3c5f3553ca64a32856b1`  
		Last Modified: Wed, 15 Jan 2020 17:10:50 GMT  
		Size: 1.2 KB (1208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8d764c754e0edf2aac68fe0528730de3ed3a1e7d938036f09c01241e19b377`  
		Last Modified: Wed, 15 Jan 2020 17:10:48 GMT  
		Size: 1.2 KB (1209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08e686f6bb7b571cf9c7ce2973285f9919a99be3accea43614d4c3c5e5049119`  
		Last Modified: Wed, 15 Jan 2020 17:10:46 GMT  
		Size: 1.2 KB (1215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93665eda8964b152df18f478de20d6e7eb169672d1e69dc5df27f577bb757bae`  
		Last Modified: Wed, 15 Jan 2020 17:10:45 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185a55a53dfa0aa33571f28e25aacbc06ace195dbc6afa8b40acea995b7c1356`  
		Last Modified: Wed, 15 Jan 2020 17:10:49 GMT  
		Size: 4.5 MB (4546418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc1c21e5b87b6dec4148d0f4aa0a219fb65c47ec5b7790a7a66ab56ca0d41605`  
		Last Modified: Wed, 15 Jan 2020 17:10:57 GMT  
		Size: 12.9 MB (12897358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f423e3adbd2f1b12af4e0e67015ed377316fed50262c6cddb95dff7b4eb30d0d`  
		Last Modified: Wed, 15 Jan 2020 17:10:44 GMT  
		Size: 296.0 KB (295961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920fe55fc0789011321044918378d0a37d1b7710e103ba28f889da92d2dba109`  
		Last Modified: Wed, 15 Jan 2020 17:10:41 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf18c6f9c2d3593d519eb3249fd3ccced6eb70f50b5c1bcbdda7e406a7fabfda`  
		Last Modified: Wed, 15 Jan 2020 17:10:42 GMT  
		Size: 2.1 MB (2124106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d965d1d9c79f0a751f651d8268d15301844e69e12c0f7b92b0ba1247e341ccd9`  
		Last Modified: Wed, 15 Jan 2020 17:10:40 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b017c9ec0ebd48d3aa557051bb908e7c44a63ef428c9511af3bc631091802b50`  
		Last Modified: Wed, 15 Jan 2020 17:11:16 GMT  
		Size: 11.5 MB (11479636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6464b7d955f5f3504b7682faab882c21d3ff15d2e89cab0ee85713a141df5d8b`  
		Last Modified: Wed, 15 Jan 2020 17:10:40 GMT  
		Size: 331.3 KB (331290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f81fbb6c32a4ffc9bbb856bfc484d6a6a4645bc094253f5d97daa91d034bd40`  
		Last Modified: Wed, 15 Jan 2020 17:10:37 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ef3c53d3b566b57c301735d8bded053e2126a43faf2737bba4746e79b93354f`  
		Last Modified: Wed, 15 Jan 2020 17:10:38 GMT  
		Size: 334.5 KB (334465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fe7effdcf18115232a0e147356a8e5f4710c88ff2f6174671a66d064bfcc72e`  
		Last Modified: Wed, 15 Jan 2020 17:10:38 GMT  
		Size: 351.2 KB (351197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f77ad6bba38a97cb2d1a53e1d7025e5d9c07833afee74e0857f3ae9ed25a8eb6`  
		Last Modified: Wed, 15 Jan 2020 17:10:38 GMT  
		Size: 363.6 KB (363623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e8ecc9c43b1dcee656e5a9568f7118dbd95b4d4e11c96ac66e7c825bab59de`  
		Last Modified: Wed, 15 Jan 2020 17:10:37 GMT  
		Size: 1.2 KB (1195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3443; amd64

```console
$ docker pull haxe@sha256:60884354b6457926faba702dbfd1f8829b3b54c0209e234d2b4b72770af1abfd
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5802968544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41f80afe2db4afabdd4a38a4fc6f36a820b031fe46d94fbcf707f5c7091acc8d`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 02 Jan 2020 15:48:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 15 Jan 2020 15:20:46 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 15 Jan 2020 15:20:47 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 15 Jan 2020 15:20:48 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 15 Jan 2020 15:20:49 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 15 Jan 2020 15:20:51 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 15 Jan 2020 15:20:52 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 15 Jan 2020 15:22:10 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jan 2020 15:24:16 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 15:25:21 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 15 Jan 2020 15:25:23 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 15 Jan 2020 15:26:49 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 15:26:50 GMT
ENV HAXE_VERSION=4.0.5
# Wed, 15 Jan 2020 15:32:27 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.0.5/haxe-4.0.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '93130ae2b1083efbcd9b8911afe2ba00d5af995f016149fd7ec629fa439c6120') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 15 Jan 2020 15:33:31 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 15 Jan 2020 15:33:33 GMT
ENV HOMEDRIVE=C:
# Wed, 15 Jan 2020 15:34:37 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jan 2020 15:35:52 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 15 Jan 2020 15:37:01 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 15 Jan 2020 15:37:03 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:31f9df80631e7b5d379647ee7701ff50e009bd2c03b30a67a0a8e7bba4a26f94`  
		Size: 1.7 GB (1654613376 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:43da502775fb34b738d9f908cb549c2825c04f1451d1039ec99749be127e47ef`  
		Last Modified: Wed, 15 Jan 2020 17:12:02 GMT  
		Size: 1.2 KB (1204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03819c236f98096b2616ee8de4f1ed293285823a9e29b5f78177452af780ac91`  
		Last Modified: Wed, 15 Jan 2020 17:12:01 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72d24fce48b6360ed968f6e7319d8f824fc867ca0a8e1ae41975e3a891149f7`  
		Last Modified: Wed, 15 Jan 2020 17:12:01 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158e99927bd1b9a9dbd42445cf763a6d58c31b40af3bba7087a055eb73c3b9c4`  
		Last Modified: Wed, 15 Jan 2020 17:11:59 GMT  
		Size: 1.2 KB (1202 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e72cb6ae9755bc1ebac92d41ecef45d1e00a989e186c9e6091f5b1ca6cce9e`  
		Last Modified: Wed, 15 Jan 2020 17:11:58 GMT  
		Size: 1.2 KB (1199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ba549531c82c5b76fab02a78cfb66493610874203a1f90badff8b76af400735`  
		Last Modified: Wed, 15 Jan 2020 17:11:56 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcc7540434a86e4ae58adc41bf446d96d52f3ac34dde4d2812a7588695a8541`  
		Last Modified: Wed, 15 Jan 2020 17:11:57 GMT  
		Size: 5.4 MB (5386134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00324f0833b7c5e8d2b890f102fd795868ce5bca1874232107e8620399d701f2`  
		Last Modified: Wed, 15 Jan 2020 17:12:00 GMT  
		Size: 22.4 MB (22437308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f7db3f45d9e074052a01c5ce8eaffd225cda710d8c0c99e5f68f135fef819f`  
		Last Modified: Wed, 15 Jan 2020 17:11:55 GMT  
		Size: 5.3 MB (5327754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24e79ac618d5656d741606594adcc52b789a90d66cc9b0e5cf7889a20d6f6d3b`  
		Last Modified: Wed, 15 Jan 2020 17:11:49 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75478d8809c350977efae613a86287a2ec37f45ef33320bcffea4b38a592b626`  
		Last Modified: Wed, 15 Jan 2020 17:11:50 GMT  
		Size: 7.2 MB (7152959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd049cd1f09139dc353aaf43c226314d1db768eee3fe81222b66059f52c74941`  
		Last Modified: Wed, 15 Jan 2020 17:11:46 GMT  
		Size: 1.2 KB (1189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9adec1bfdbd8b8b57723bf77b9ee794c85907101f46acaa9f8929306fa5c91d7`  
		Last Modified: Wed, 15 Jan 2020 17:12:13 GMT  
		Size: 16.7 MB (16682823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ff4e940f84c636e69fae478435c7d014abc0b9c506d81b788463a9f4db2e3e`  
		Last Modified: Wed, 15 Jan 2020 17:11:49 GMT  
		Size: 5.3 MB (5340789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea1858691aeff427896b8271d8f08c5e2c4e1e333cdfba2837e3c397b3710ed`  
		Last Modified: Wed, 15 Jan 2020 17:11:39 GMT  
		Size: 1.2 KB (1163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25685b9b4c8359224394d46f6fce302ca46236dc7cc3b2e9aa86c7c6e1c67dab`  
		Last Modified: Wed, 15 Jan 2020 17:11:53 GMT  
		Size: 5.3 MB (5338958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca2b9f31f104e9e32fccf9304ac5474bc012ab83171910cbe29a60abd7d100bd`  
		Last Modified: Wed, 15 Jan 2020 17:11:43 GMT  
		Size: 5.3 MB (5344735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a7b7bac792b1b1f0e7054e0af5a8cb7abc1292d31bcc694310622328ab3d9b`  
		Last Modified: Wed, 15 Jan 2020 17:11:43 GMT  
		Size: 5.3 MB (5345932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bdd50ffd5af29d806e625b52313a930b024daeb58c042c7e373cb864e10cdce`  
		Last Modified: Wed, 15 Jan 2020 17:11:40 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
