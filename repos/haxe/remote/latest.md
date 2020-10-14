## `haxe:latest`

```console
$ docker pull haxe@sha256:e9c47d879bb3c04a00ee950807f6dda89beb4623049f0020cfc3dc1d82affca6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1518; amd64
	-	windows version 10.0.14393.3986; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:b6208372aae999e7f1b9079b88c2d179c690941fe9d97c15744e94dcd30288c8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132201028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c88856609c76bdb6cc20994662f2183817d3307240de320ddb714ff9bad91e92`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:14:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:14:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:15:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:46:14 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 22:46:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 22:46:20 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 13 Oct 2020 22:47:48 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 13 Oct 2020 22:47:48 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 13 Oct 2020 22:47:48 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 13 Oct 2020 22:54:21 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 13 Oct 2020 22:54:22 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:101c41d0463bc77661fb3343235b16d536a92d2efb687046164d413e51bd4fc4`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 7.8 MB (7811737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8275efcd805f9905d7def23603618236284b0be6b9e47455c638fbfb03fa9208`  
		Last Modified: Tue, 13 Oct 2020 02:28:35 GMT  
		Size: 10.0 MB (9996326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:751620502a7a2905067c2f32d4982fb9b310b9808670ce82c0e2b40f5307a3ee`  
		Last Modified: Tue, 13 Oct 2020 02:28:53 GMT  
		Size: 51.8 MB (51829492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c98954df2361456a7e07813020185887790521cc7c9c3a1c78fc0147920c99`  
		Last Modified: Tue, 13 Oct 2020 23:20:51 GMT  
		Size: 1.3 MB (1312181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28b774c18536c3c6c374598f10ec2af64606d6098ad7398e3c591520ac098568`  
		Last Modified: Tue, 13 Oct 2020 23:20:51 GMT  
		Size: 2.3 MB (2307393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9ce61e3264e5ca6ec82b537e8d5aff477044726aabdab7b6895e81cdf1e758a`  
		Last Modified: Tue, 13 Oct 2020 23:20:54 GMT  
		Size: 8.5 MB (8547921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:1c627dffcd9adf5d413ca640f1423f61c9fa42de5ba7635de5cb08e13315ffad
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.4 MB (121384201 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20f25d638433a925796df4bee2249854d3d1b86245e0037bd11c1d16bef11310`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:02 GMT
ADD file:e03270d36cef8171f1f6303860ff31bb1c0eb10642b8173bfdfef9f77fa4f89c in / 
# Tue, 13 Oct 2020 00:59:04 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 01:34:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 01:34:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 01:35:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:48:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 21:49:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:49:27 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 13 Oct 2020 21:56:26 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 13 Oct 2020 21:56:39 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 13 Oct 2020 21:56:53 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 13 Oct 2020 22:06:08 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 13 Oct 2020 22:06:18 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:5c0fdcca2cbb5e316a288f39c8c2006f45544568ea04623c036e0b1faa066bbe`  
		Last Modified: Tue, 13 Oct 2020 01:08:04 GMT  
		Size: 45.9 MB (45869258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8216e147de931a74896e75f60d0a331dd1438bc1ae4b2d4c29c8017548e8dcbd`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 7.1 MB (7097763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf6642121709e17d1419901978da7d29b673d5f936e42ec3241b7d7157e9541`  
		Last Modified: Tue, 13 Oct 2020 01:56:20 GMT  
		Size: 9.3 MB (9343130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5754411f60ee27fceb92d6380a748ae6d60239063cfa8165419be0ebf9de5834`  
		Last Modified: Tue, 13 Oct 2020 01:56:44 GMT  
		Size: 47.4 MB (47355626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12c99e92b3b992c3c720c5b49004749e3569211f9bbae1996f70432525e85d0e`  
		Last Modified: Tue, 13 Oct 2020 23:00:46 GMT  
		Size: 1.2 MB (1234642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320a46bc3d8c3e75a1dcfff4269ebf85163d9f3ef0345fff62b530f2e941e95e`  
		Last Modified: Tue, 13 Oct 2020 23:00:46 GMT  
		Size: 2.2 MB (2249823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d056ab376f355abf25bb628ba4318b39b70be549cda7bf6f157a8d35f4fdd06`  
		Last Modified: Tue, 13 Oct 2020 23:00:50 GMT  
		Size: 8.2 MB (8233959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:46d91c7e9a5f8594d5866452cef44dd73dacbff658bda88ebd1b650c2ecacc10
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.1 MB (133145038 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8545a4e193afb2ffd18083e6646e11f0e8cd90e92d3760153cc914f4a049e68f`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:32:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:33:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 13 Oct 2020 02:33:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:11:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 13 Oct 2020 21:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:11:47 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 13 Oct 2020 21:15:29 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 13 Oct 2020 21:15:30 GMT
ENV HAXE_VERSION=4.1.4
# Tue, 13 Oct 2020 21:15:31 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 13 Oct 2020 21:24:33 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 			' 	&& git clone --recursive --depth 1 --branch 4.1.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 13 Oct 2020 21:24:42 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:136d6e4f4b17bdbefbe60820da5f5711a26d31c075dc69bcaf9b077d7d29262d`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 7.7 MB (7681432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28db65b8364fc73072a0d5b51199cc9c6b108b4229d92e784b92ae67898dd0bd`  
		Last Modified: Tue, 13 Oct 2020 02:47:32 GMT  
		Size: 10.0 MB (9983936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff74fb95e95674d2f0c26f446a2cb7c0ee055d78182a9d61e1578c64c171f2b4`  
		Last Modified: Tue, 13 Oct 2020 02:48:00 GMT  
		Size: 52.2 MB (52163324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4112aeefb96786c451de09a2455b8baa6a131809da1dfeb8c51fa456d286d3`  
		Last Modified: Tue, 13 Oct 2020 22:15:43 GMT  
		Size: 1.3 MB (1303437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57728a9f56c9518bcab7d78b0d1898a5964af13f8dff89cdd1fbda52beceac0`  
		Last Modified: Tue, 13 Oct 2020 22:15:44 GMT  
		Size: 2.3 MB (2303633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2224aed587620059d4cffcc06b7e66c45d83f495ac5bd20889f4e736ca961f`  
		Last Modified: Tue, 13 Oct 2020 22:15:47 GMT  
		Size: 10.5 MB (10533871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.1518; amd64

```console
$ docker pull haxe@sha256:b11e6ceb53d05618dc998432650b06ec3a85a71eee75f5dc9d79881c263237f0
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2429663228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73814eb407e0317df6ff6468bebc259ce4651efd773616032f10a5664453e2fb`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 01 Oct 2020 02:26:38 GMT
RUN Install update 1809-amd64
# Wed, 14 Oct 2020 12:58:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 12:58:34 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 14 Oct 2020 12:58:34 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 14 Oct 2020 12:58:35 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 14 Oct 2020 12:58:36 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 14 Oct 2020 12:58:36 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 14 Oct 2020 12:59:15 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Oct 2020 13:00:17 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:00:37 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 14 Oct 2020 13:00:38 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 14 Oct 2020 13:01:14 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:01:14 GMT
ENV HAXE_VERSION=4.1.4
# Wed, 14 Oct 2020 13:04:50 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.1.4/haxe-4.1.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:05:10 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 14 Oct 2020 13:05:10 GMT
ENV HOMEDRIVE=C:
# Wed, 14 Oct 2020 13:05:29 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Oct 2020 13:05:51 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 14 Oct 2020 13:36:19 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 14 Oct 2020 13:36:19 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:406ffb8432a757e84f7594e85c676620dec6955e0475ac271aa4dd5c0531190d`  
		Size: 655.8 MB (655757265 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d839ec6fa74e5e869036dfd823e95452a7afcde18ac997af483c88c21b92ad8c`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a203aabf27edff709e3ffd11d8fd8e1ce5f37e273b9ca13ffa7b44275b52671a`  
		Last Modified: Wed, 14 Oct 2020 16:02:33 GMT  
		Size: 1.2 KB (1151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f6991ce67829acc5f25eecbad2e3df8dde724316d4e835c011524de1736cecc`  
		Last Modified: Wed, 14 Oct 2020 16:02:32 GMT  
		Size: 1.2 KB (1158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4dbbaf50960b08b51b086cec3e8810aaf51b1c69d4f87aa3cd25a15f7d447c`  
		Last Modified: Wed, 14 Oct 2020 16:02:32 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d1d4f3b2d06578df28cb3cb417aa7b72f6d9a33e40e80c38f4cf0ac3ca3b2`  
		Last Modified: Wed, 14 Oct 2020 16:02:30 GMT  
		Size: 1.1 KB (1148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713f8b1723d1de4ac5b6bae643d1b948b345b50e067134f86c55ee491eebeb0f`  
		Last Modified: Wed, 14 Oct 2020 16:02:29 GMT  
		Size: 1.1 KB (1131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c503ab7835c0262a84ad03492568e4b5aaaa8626db220b71e4d6f32a38a85b5`  
		Last Modified: Wed, 14 Oct 2020 16:02:30 GMT  
		Size: 9.2 MB (9228385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b94547a00b83769ebebe32451b2b3832c27281499029db24187d591952c6b`  
		Last Modified: Wed, 14 Oct 2020 16:02:30 GMT  
		Size: 17.3 MB (17305053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88d94f439ab003d422a4ba49515059a14d4a7bfc5bca40384c4f851d4317d8dd`  
		Last Modified: Wed, 14 Oct 2020 16:02:24 GMT  
		Size: 319.6 KB (319627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0969e32d810ee9864b9a58b6ef51fd19eafb59214ae10ee790f9995228b1501`  
		Last Modified: Wed, 14 Oct 2020 16:02:23 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397500e2a7c8dd0b1b3d20af18d9cc373fd9d236a165cdd8d4ba63266e45e452`  
		Last Modified: Wed, 14 Oct 2020 16:02:24 GMT  
		Size: 6.5 MB (6524906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a41da81c9bf72eddafd838b945ef70d1b327982fe6863c569fb7661943ca1a`  
		Last Modified: Wed, 14 Oct 2020 16:02:22 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db2e18aab686dfcd5bceee52745ae0f19ae51b4766124a187c5d0cd7f373b29`  
		Last Modified: Wed, 14 Oct 2020 16:02:28 GMT  
		Size: 12.0 MB (11979475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4fb4e0bbf7a54f4f4548b3d88c79f2430967ed449939ec8aba42138ea16415`  
		Last Modified: Wed, 14 Oct 2020 16:02:21 GMT  
		Size: 343.1 KB (343115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c86e9c8088c21400b06bfcf34e6a279c8873ae5f67bd2019b267994df3c37816`  
		Last Modified: Wed, 14 Oct 2020 16:02:17 GMT  
		Size: 1.1 KB (1083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbfc2bc4096126c4fec78ff402e9a2efd8285e105f306be422147fc19e464060`  
		Last Modified: Wed, 14 Oct 2020 16:02:18 GMT  
		Size: 350.0 KB (350046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab85b0989d75be0305bd2eb8df355d2f0399b8221abdbab1df7590a96ef58f9`  
		Last Modified: Wed, 14 Oct 2020 16:02:19 GMT  
		Size: 4.7 MB (4744443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46217774ce304593ae1510194ca2cdf3d08270b1ab453bf5c76e18cbec93e1c1`  
		Last Modified: Wed, 14 Oct 2020 16:02:18 GMT  
		Size: 4.8 MB (4766691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032045d079e8682960e65246ab4549edc1625f54df5576c344489ecd8369345d`  
		Last Modified: Wed, 14 Oct 2020 16:02:16 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.3986; amd64

```console
$ docker pull haxe@sha256:7486c6aaa7be7237b66ee50f8376168c5d0cb7048b2de1376d2f8e0d3f8f51df
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 GB (5838367849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c73a2a2e94d4e1349c62aecca66d1436f299435c8c244176215d2ec471361b`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 02 Oct 2020 17:07:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Oct 2020 13:36:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 14 Oct 2020 13:36:28 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 14 Oct 2020 13:36:29 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 14 Oct 2020 13:36:29 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 14 Oct 2020 13:36:30 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 14 Oct 2020 13:36:30 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 14 Oct 2020 13:37:39 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Oct 2020 13:39:25 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:40:37 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 14 Oct 2020 13:40:38 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 14 Oct 2020 13:42:14 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:42:15 GMT
ENV HAXE_VERSION=4.1.4
# Wed, 14 Oct 2020 13:46:49 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.1.4/haxe-4.1.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cb55d37560a4deb227fd8577bc8c880124b0260398456eb34a007a6a4d15f170') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 14 Oct 2020 13:47:59 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 14 Oct 2020 13:47:59 GMT
ENV HOMEDRIVE=C:
# Wed, 14 Oct 2020 13:49:10 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Oct 2020 13:50:25 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 14 Oct 2020 13:51:40 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 14 Oct 2020 13:51:41 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:17a32268498b2feefa5457f0423ac15473596d514e48c694ef54d740a9a5067d`  
		Size: 1.7 GB (1671365753 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb0caa156c690c0274404e38041b8eb56dcd2c15edbc269fc4c619eb667cb7ff`  
		Last Modified: Wed, 14 Oct 2020 16:03:09 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70df663cc4e5e0712ec27338d2a52d7d4ca0da21adf029becdf01e42e5977a60`  
		Last Modified: Wed, 14 Oct 2020 16:03:08 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d36f6597c87cf619ea903c40bbfe1a73083fa5f71de89890f2e648f9b51a0ae4`  
		Last Modified: Wed, 14 Oct 2020 16:03:07 GMT  
		Size: 1.1 KB (1133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38bcd6c53d51f952c90235ce188c7e57672b413dfb9643b8b66273ca34ccf891`  
		Last Modified: Wed, 14 Oct 2020 16:03:07 GMT  
		Size: 1.2 KB (1155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dff53d3b46e892e03cf623580582579895f01b57b85a3d16713fd9ff0a46e1`  
		Last Modified: Wed, 14 Oct 2020 16:03:06 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84bdbf0eb5d1828aea252711369ebc52a1839a34253b85c5a26d59ea04c0ce40`  
		Last Modified: Wed, 14 Oct 2020 16:03:04 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295d04ee5918dbc0a9152571a319530bc1366fd6961f8445a6e0bf98334b2e78`  
		Last Modified: Wed, 14 Oct 2020 16:03:07 GMT  
		Size: 9.9 MB (9916405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78a660a103ebb10d9abfaad2bfbfa6ebfe9e316f6fede56f9e6bd3d2149d6f6e`  
		Last Modified: Wed, 14 Oct 2020 16:03:07 GMT  
		Size: 22.4 MB (22410077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ce7f2d47f47b2b8e99e9a274f5f05bd4a3b634c9e168b4b106adaf84fbc0f4`  
		Last Modified: Wed, 14 Oct 2020 16:03:01 GMT  
		Size: 5.4 MB (5365327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:676c74365815d318c25f950534a271d1a720313e65ff0993f8a3e3e5c3759918`  
		Last Modified: Wed, 14 Oct 2020 16:02:56 GMT  
		Size: 1.1 KB (1146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbc817b57d176418f3f42cde128281d4bd7d95510d2d2124598a0bbe40591daa`  
		Last Modified: Wed, 14 Oct 2020 16:03:01 GMT  
		Size: 11.7 MB (11674295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39b762a9e813900249fc371ab30f572485e800fb4bbb722ad1a46b9eefecedca`  
		Last Modified: Wed, 14 Oct 2020 16:02:54 GMT  
		Size: 1.2 KB (1154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c82a58d3cf239a2e30d1ae369aa5ebbe22497f81b223dd2b097f2b6a41312ed8`  
		Last Modified: Wed, 14 Oct 2020 16:03:01 GMT  
		Size: 17.2 MB (17158253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d377ad5de5b06839f1bb857f04290dbef0d6bf9184045b138c958b3c7ac355ac`  
		Last Modified: Wed, 14 Oct 2020 16:03:00 GMT  
		Size: 5.4 MB (5378135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb25a8e9dbf7e83fccf228c53b327ffdf7e312d7d6e053509e999b192e96e24f`  
		Last Modified: Wed, 14 Oct 2020 16:02:48 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89cb12f2163797ccc564389bb0489403c0fc9bc40bd809adecb68685913c9e9d`  
		Last Modified: Wed, 14 Oct 2020 16:02:51 GMT  
		Size: 5.4 MB (5380389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160a76e33e92ce07c6f86c88d665e0d9b62a3c051782a1f1ff4127fbf617ceab`  
		Last Modified: Wed, 14 Oct 2020 16:02:52 GMT  
		Size: 9.9 MB (9867890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42b0ac0abcb176fca116f080d7b1116aa196eeecced4e8c9333102292204f8d9`  
		Last Modified: Wed, 14 Oct 2020 16:02:52 GMT  
		Size: 9.9 MB (9853965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4239057918c97bb8b4cce3ef2c7505da6b42baa56616b59b99e8f4439b6f5b77`  
		Last Modified: Wed, 14 Oct 2020 16:02:47 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
