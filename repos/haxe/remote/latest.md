## `haxe:latest`

```console
$ docker pull haxe@sha256:3dda9050b8cc846020e084ce5d6167adf05fa691edf1fac83815b0f9c00511f8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.1757; amd64
	-	windows version 10.0.14393.4225; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:3f7e945216fc70334cb723ea9ed39ac4e3db938b8ec91275112b1a7c19a6fad9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **132.2 MB (132207076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6c28817c7847e2da0ac50d77d9d138dbcd3c5826e339c5a2cb4c7df86711c91`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 12 Jan 2021 00:32:36 GMT
ADD file:53e587afdbeaee60cc14bd95907f14c8303c04b98c72f98e2c54d4343f15dd38 in / 
# Tue, 12 Jan 2021 00:32:37 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 03:57:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 03:57:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 03:57:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:27:59 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 23:28:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 23:28:04 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 12 Jan 2021 23:29:21 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 12 Jan 2021 23:29:21 GMT
ENV HAXE_VERSION=4.1.5
# Tue, 12 Jan 2021 23:29:21 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 12 Jan 2021 23:34:57 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.1.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 12 Jan 2021 23:34:57 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:b9a857cbf04d2c0d2f0f6b73e894b20a977a6d3b6edd9e27d080e03142954950`  
		Last Modified: Tue, 12 Jan 2021 00:38:49 GMT  
		Size: 50.4 MB (50399171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d557ee20540b597f518df05bc6888778cfc92bf46040c701d4a622389feb6807`  
		Last Modified: Tue, 12 Jan 2021 04:05:56 GMT  
		Size: 7.8 MB (7812018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9ca4f00c2e4896c65625d678544b764d7483dca9dcab92b62093db72f21d3e`  
		Last Modified: Tue, 12 Jan 2021 04:05:55 GMT  
		Size: 10.0 MB (9996375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667fd949ed9338da3c1e09f9b75408c214368c637c448e0fd839467f6f7717b5`  
		Last Modified: Tue, 12 Jan 2021 04:06:20 GMT  
		Size: 51.8 MB (51830144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c5810e086d75bda5736ae2a911d2784c7210750432bc5745fca9b116679ef09`  
		Last Modified: Tue, 12 Jan 2021 23:59:53 GMT  
		Size: 1.3 MB (1312120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e96547e2453f9cf865f47929a65e6a63b24807d325d86d05888a479b5e9eef`  
		Last Modified: Tue, 12 Jan 2021 23:59:52 GMT  
		Size: 2.3 MB (2307318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5143b0c4e623ce2b2233d5458b43dfff05c0f2e9e9346e08f78995a7c4431cf`  
		Last Modified: Tue, 12 Jan 2021 23:59:54 GMT  
		Size: 8.5 MB (8549930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:7c7086184abf5cc7784742e48daff5a501315f6f62b270cbefc2d7cf0eb9e0c1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.7 MB (122664169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e59bc2cbff0551b4a85fdefc097809967f7e9b7726863b93988ce2fb04a4e2fe`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 09 Feb 2021 03:00:29 GMT
ADD file:817a4ff41fcac0be44e95d3f0a51c9fa878d16dac7cdab68bfc445f630c43c22 in / 
# Tue, 09 Feb 2021 03:00:33 GMT
CMD ["bash"]
# Tue, 09 Feb 2021 04:25:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 04:26:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Feb 2021 04:26:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 22:32:00 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Feb 2021 22:32:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Feb 2021 22:32:11 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 09 Feb 2021 22:35:29 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 11 Feb 2021 23:15:54 GMT
ENV HAXE_VERSION=4.2.0
# Thu, 11 Feb 2021 23:15:55 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 11 Feb 2021 23:25:01 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.0 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 11 Feb 2021 23:25:03 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4c2a0a79594a20b9c2f0bfbd535f875ca1b079625052cdd801afb1cc0362d6d0`  
		Last Modified: Tue, 09 Feb 2021 03:09:18 GMT  
		Size: 45.9 MB (45867053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06c11c595f6421f88e1b10286a766ae8db88f67c2c0f41cedd170640aee498ab`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 7.1 MB (7123173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47cb22b679409f00e04b8d645444df7181f05cb2967ed73f1a377e7f774b6873`  
		Last Modified: Tue, 09 Feb 2021 04:39:37 GMT  
		Size: 9.3 MB (9343495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e90d4e143c069feee70f90eea83d55b7b0761c67fbbfb7f3734c16c0811ac13`  
		Last Modified: Tue, 09 Feb 2021 04:40:02 GMT  
		Size: 47.4 MB (47355624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11626afa2ca0d0a64d62c37451fe150134e720d62f0f247546810556a8078db`  
		Last Modified: Wed, 10 Feb 2021 00:25:48 GMT  
		Size: 1.2 MB (1234803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5961e428c5969a3daa5d20ba4d74fe279dbcfbab59438ecc8b00e7a8f9cf09`  
		Last Modified: Wed, 10 Feb 2021 00:25:49 GMT  
		Size: 2.2 MB (2249825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd933fec1c94ab208b79c7dbbc7bb6637395630b33b86b592f365ea43cde4e0f`  
		Last Modified: Fri, 12 Feb 2021 00:00:20 GMT  
		Size: 9.5 MB (9490196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:4dd57cd4acc4b5f6b22e7c4d75c2ef9953b1f1fa4f38f24df8357aa8051d1b86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.2 MB (133159224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b238113e7c5b7999cb8dce245be124f81ed491aa8fc26991f8bf26a15c908bd`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 12 Jan 2021 00:40:39 GMT
ADD file:849d424ecc8572facb3ca68eff836dce211bc677cb32d3c3eaa129d364d33878 in / 
# Tue, 12 Jan 2021 00:40:43 GMT
CMD ["bash"]
# Tue, 12 Jan 2021 01:23:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 01:23:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 12 Jan 2021 01:24:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 20:25:25 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 12 Jan 2021 20:25:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 12 Jan 2021 20:25:35 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 12 Jan 2021 20:29:51 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 12 Jan 2021 20:29:53 GMT
ENV HAXE_VERSION=4.1.5
# Tue, 12 Jan 2021 20:29:54 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 12 Jan 2021 20:38:04 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.1.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 	&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 12 Jan 2021 20:38:05 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:6e5587ff5efa4e647ae927194fac9b961a68d46b23b68a3119c90016e58f17aa`  
		Last Modified: Tue, 12 Jan 2021 00:51:18 GMT  
		Size: 49.2 MB (49183736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:439dbbb05ea0aa8484ae8a51d0fbb1c7609176a1b0d3f15dad69d52e9a83af66`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 7.7 MB (7682325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b89c8b4e5b232c040d5905808ee62cdfcc9d697de10183d6bc4767468859d92`  
		Last Modified: Tue, 12 Jan 2021 01:38:27 GMT  
		Size: 10.0 MB (9984327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a53f70a43c3c83782c39cad75aa09ccddb893b3fd54762416fca4d48a3b44b5`  
		Last Modified: Tue, 12 Jan 2021 01:38:54 GMT  
		Size: 52.2 MB (52163502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e7dee233c6c26a01e647c6dcbebb2c4a6e43268d482bda60786c2871b46bd90`  
		Last Modified: Tue, 12 Jan 2021 21:20:52 GMT  
		Size: 1.3 MB (1303533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef2d2e4315af7165b970be7fc9a53a6685fecabf0384f41eac833776d4cb2f0`  
		Last Modified: Tue, 12 Jan 2021 21:20:52 GMT  
		Size: 2.3 MB (2303622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b9903b2c6c65e8b96d09c14debc4fd2590b3eadb82059294af06c9e8a2545ab`  
		Last Modified: Tue, 12 Jan 2021 21:20:54 GMT  
		Size: 10.5 MB (10538179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.1757; amd64

```console
$ docker pull haxe@sha256:a46ae341d9f3e52317c191c257a65620082cf0fd4d00144b204ba83f789224bd
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2496495809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb69bf4e19cd8be188b7029a29b815f1c30a2cdcd7caff72665d44904d70b93c`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Sat, 06 Feb 2021 05:03:14 GMT
RUN Install update 1809-amd64
# Tue, 09 Feb 2021 20:26:38 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 13:53:09 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Feb 2021 13:53:10 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Feb 2021 13:53:10 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Feb 2021 13:53:11 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Feb 2021 13:53:11 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Feb 2021 13:53:48 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 13:54:45 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 13:55:04 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Feb 2021 13:55:05 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Feb 2021 13:55:41 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 11 Feb 2021 23:15:22 GMT
ENV HAXE_VERSION=4.2.0
# Thu, 11 Feb 2021 23:19:29 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.0/haxe-4.2.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (83be481d03892562155ed77c4f0f2ac30f34683cb0b55b57765ef90fc1d623ee) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '83be481d03892562155ed77c4f0f2ac30f34683cb0b55b57765ef90fc1d623ee') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 11 Feb 2021 23:19:49 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 11 Feb 2021 23:19:49 GMT
ENV HOMEDRIVE=C:
# Thu, 11 Feb 2021 23:20:09 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Feb 2021 23:20:32 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Thu, 11 Feb 2021 23:20:54 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Thu, 11 Feb 2021 23:20:55 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db4edcf0861ff3fdc41851a5a218965ecb2ab6cf4ec9448fb80cc4b6792fd46c`  
		Size: 720.9 MB (720933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:751b8860e89a7e6999d74a11dc393620b118057ad881cb87f1d6e3653cb2db43`  
		Last Modified: Tue, 09 Feb 2021 20:48:09 GMT  
		Size: 1.3 KB (1337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99fbcc77e52a42ad787e6f69de7b00e550f0603987949cc946fe2d18e30e18c`  
		Last Modified: Wed, 10 Feb 2021 15:27:21 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad40ba0a2655a9e06e035bc0e899c9bce5f808987628cdfbd04db7bec9b07e4`  
		Last Modified: Wed, 10 Feb 2021 15:27:20 GMT  
		Size: 1.3 KB (1342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fdde18cb7a12873e3be61565052b8d0541dae497f88d456c33fe3e821fdd81e`  
		Last Modified: Wed, 10 Feb 2021 15:27:20 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872f2e1d85c12130846494c2d4ab040202c1881e99f6ca6c33dcab0454237322`  
		Last Modified: Wed, 10 Feb 2021 15:27:19 GMT  
		Size: 1.4 KB (1377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021c542803a39ff956d7e0b42a6310a8d5fae91748d7cd339503b857274abe29`  
		Last Modified: Wed, 10 Feb 2021 15:27:14 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1803b749c05db1df3edae1565ed39ebbb7963add96dae664529cb5117b048254`  
		Last Modified: Wed, 10 Feb 2021 15:27:18 GMT  
		Size: 9.4 MB (9412179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b003b55a048c6ce848b1f2027e2d83cb6b85d3a3f021d2977bdacb20801a5b`  
		Last Modified: Wed, 10 Feb 2021 15:27:18 GMT  
		Size: 17.3 MB (17303684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24da63debd5e065efb6dda2d53c070948a201d391adb5c21d96d31bb142acce5`  
		Last Modified: Wed, 10 Feb 2021 15:27:10 GMT  
		Size: 319.4 KB (319416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61e9c491bb1509bc78fc93f662dbf20918a90e468b7c6bb45d0b7656bc23691b`  
		Last Modified: Wed, 10 Feb 2021 15:27:10 GMT  
		Size: 1.4 KB (1369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35873f382524a562f245d40631e092b5d2d10bfd0a1b3f29a097533e6a9eccdf`  
		Last Modified: Wed, 10 Feb 2021 15:27:17 GMT  
		Size: 6.5 MB (6535711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e84549a4b8e341ab8d49b9b14202f3167ded4ae73b36d00123e3f8722da726`  
		Last Modified: Thu, 11 Feb 2021 23:33:49 GMT  
		Size: 1.4 KB (1358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8b73d134b0c6129e2f003f8a8eb8ab881295ffc39e78b896321249154bbdd7`  
		Last Modified: Thu, 11 Feb 2021 23:33:56 GMT  
		Size: 13.4 MB (13405687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977bdd0046452f376fb8bdfab1900c774ea5ec1b08d78f6a6ac61c4316e43873`  
		Last Modified: Thu, 11 Feb 2021 23:33:49 GMT  
		Size: 343.0 KB (342951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822b6db5eb52c9484fe7f2d0b529eac18ac8d100b7ab84b0fcd7633e50efe4f9`  
		Last Modified: Thu, 11 Feb 2021 23:33:45 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:864de7e35cde3f2d188a0a6290c8629a21feb206a574545f08e98c4cf54791a8`  
		Last Modified: Thu, 11 Feb 2021 23:33:46 GMT  
		Size: 362.3 KB (362291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68baa2eb1a3efd9ae07f638539366e15a1b5d0530830ad2207031384c4d00118`  
		Last Modified: Thu, 11 Feb 2021 23:33:48 GMT  
		Size: 4.8 MB (4760750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b9155ba123e36bf22dfb423367de0c8913155f3a8219455098b6dfe324e88f`  
		Last Modified: Thu, 11 Feb 2021 23:33:47 GMT  
		Size: 4.8 MB (4772919 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4610c91a3d4c73a29810d8eae8df82dea9f4023dd6f5aa5af06021a22b44e48f`  
		Last Modified: Thu, 11 Feb 2021 23:33:45 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.4225; amd64

```console
$ docker pull haxe@sha256:8fac7e0b5061f3b9e8e93aaa527e75ea0e8d77fb6e790f81362e9f0187773003
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5895805775 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ad2c6b1cf76728a1589de436f53412e552e7e61958748290690d467220e95c3`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 27 Jan 2021 18:11:00 GMT
RUN Install update ltsc2016-amd64
# Tue, 09 Feb 2021 20:28:50 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Feb 2021 14:00:54 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Feb 2021 14:00:54 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Feb 2021 14:00:55 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Feb 2021 14:00:56 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Feb 2021 14:00:56 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Feb 2021 14:02:08 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Feb 2021 14:04:00 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Feb 2021 14:05:10 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Feb 2021 14:05:11 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Feb 2021 14:06:48 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 11 Feb 2021 23:21:05 GMT
ENV HAXE_VERSION=4.2.0
# Thu, 11 Feb 2021 23:25:36 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.0/haxe-4.2.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (83be481d03892562155ed77c4f0f2ac30f34683cb0b55b57765ef90fc1d623ee) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '83be481d03892562155ed77c4f0f2ac30f34683cb0b55b57765ef90fc1d623ee') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 11 Feb 2021 23:26:51 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 11 Feb 2021 23:26:52 GMT
ENV HOMEDRIVE=C:
# Thu, 11 Feb 2021 23:28:01 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 11 Feb 2021 23:29:17 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Thu, 11 Feb 2021 23:30:33 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Thu, 11 Feb 2021 23:30:34 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:62c48323ed8ac695b8cbe0ecedcc28ba185a234673ad9241df2b151dd00f9181`  
		Size: 1.7 GB (1725027107 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ac4a230905430e1aea27172a9432f576cc4a530e72bea516a2b304d2b7e9c101`  
		Last Modified: Tue, 09 Feb 2021 20:49:11 GMT  
		Size: 1.4 KB (1356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39fdeaa47a05b046ea99b54a9e1d867444cc110227ffb42c62a19d1402793f6`  
		Last Modified: Wed, 10 Feb 2021 15:28:02 GMT  
		Size: 1.4 KB (1382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a443a3aea5823e7319d0e17c252f6d89c1595930392b85a853c84c008024107`  
		Last Modified: Wed, 10 Feb 2021 15:28:01 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7619bbcd37e5b47191537c63fe6cc551b0c0bb9cdefe6946cb3804161541c4f7`  
		Last Modified: Wed, 10 Feb 2021 15:28:01 GMT  
		Size: 1.3 KB (1278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d375941f1d2d221bbbebcbc9f67065bb2cb8e6da2c27b543653c7b66ae43e1eb`  
		Last Modified: Wed, 10 Feb 2021 15:27:59 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5e38e584304bed68c0264fafc0aabad35b35706d2bacd0ecf27176a2749738`  
		Last Modified: Wed, 10 Feb 2021 15:27:58 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4485d0ac16ca20dfd834c1a6324899c43d6ea275644bc22a773d4dcf402dfd42`  
		Last Modified: Wed, 10 Feb 2021 15:27:58 GMT  
		Size: 10.2 MB (10173318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c67a2d6f6d32a96ef9dae645e304a1e2638bdf0ea5d6c67a413090cd61871e`  
		Last Modified: Wed, 10 Feb 2021 15:27:58 GMT  
		Size: 22.7 MB (22679369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e244832caaa160c44305fa1000362a1a7db2f688b1e5a384f7978ea56c54f31`  
		Last Modified: Wed, 10 Feb 2021 15:27:51 GMT  
		Size: 5.6 MB (5609341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22d6ee4c72cd286304a20e4e655ab85176f9ea0d342a2c9caa837994ef264d72`  
		Last Modified: Wed, 10 Feb 2021 15:27:49 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285f60483b297d3236ae16998e8a9621642fa936cf9589010dce23ecfde8f24f`  
		Last Modified: Wed, 10 Feb 2021 15:28:01 GMT  
		Size: 11.9 MB (11946075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833985ca9d223253af53afb69b2703cf25140fb71e4e5f2890ff72ec1b928aee`  
		Last Modified: Thu, 11 Feb 2021 23:34:14 GMT  
		Size: 1.3 KB (1303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4df4117641e8ec253892067b14e33094e5af20f1a5aeb931462eeb5e8dec62b5`  
		Last Modified: Thu, 11 Feb 2021 23:34:19 GMT  
		Size: 18.8 MB (18825004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e2ef5467ef0a669ceccd0a11149bcd79a283782139d2dc6f23413d5f48bb08`  
		Last Modified: Thu, 11 Feb 2021 23:34:14 GMT  
		Size: 5.6 MB (5626789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34cac28fe3356bd4f247131b8773fd8018e9ad73c4a4ca327764281541b283ba`  
		Last Modified: Thu, 11 Feb 2021 23:34:09 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf539154451382b7b98b293c5a2525825d485d7add07a35d5f1ad6c54d4d2d8`  
		Last Modified: Thu, 11 Feb 2021 23:34:10 GMT  
		Size: 5.6 MB (5627105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f745ca9f35a68beaac6e08ef0d69089e1005c65362dcafcea1d1258e9a579abb`  
		Last Modified: Thu, 11 Feb 2021 23:34:21 GMT  
		Size: 10.1 MB (10148652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19031baf945ce1be44ec6053447a2afc1a29decb797d6f62e4989dd0a869f167`  
		Last Modified: Thu, 11 Feb 2021 23:34:12 GMT  
		Size: 10.1 MB (10143900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d3f68da4142ac32c9ca92d5d0f12a4f30a33f3625e79e0f283f489bf112c24`  
		Last Modified: Thu, 11 Feb 2021 23:34:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
