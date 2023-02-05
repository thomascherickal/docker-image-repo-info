## `haxe:latest`

```console
$ docker pull haxe@sha256:46f7fa746f6788c08966c1a79844335ab07e87836b1ed73e1ae3ec588c681428
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.1487; amd64
	-	windows version 10.0.17763.3887; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:e897ae116bd4cbb476c9ef4588aa031db0182f9e3ca63958f4b87effc35dd2ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (140013422 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c97188c64b301d913dfd3287f59c91a3e0d712de4dfaf741a1afc3e5d2ab45e`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 04 Feb 2023 06:51:26 GMT
ADD file:cc6a56676703ec7ab5db8f2f7bc18a3169c0816d38703845b6b77ae5342ab41c in / 
# Sat, 04 Feb 2023 06:51:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 07:22:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 07:22:32 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 07:22:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:19:15 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 05 Feb 2023 00:19:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 00:19:20 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 05 Feb 2023 00:20:52 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 05 Feb 2023 00:20:52 GMT
ENV HAXE_VERSION=4.2.5
# Sun, 05 Feb 2023 00:20:52 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 05 Feb 2023 00:23:40 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 05 Feb 2023 00:23:40 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:699c8a97647f5789e5850bcf1a3d5afe9730edb654e1ae0714d5bd198a67a3ed`  
		Last Modified: Sat, 04 Feb 2023 06:55:53 GMT  
		Size: 55.0 MB (55025312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86cd158b89fde67a8a4c428a844985f930eba450ec3fde1c9ef5df3884128c62`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 5.2 MB (5165476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a226e961cfaa2d1d171e429e9db314feec6201f5cba1487b20e7aee311e4a54f`  
		Last Modified: Sat, 04 Feb 2023 07:29:25 GMT  
		Size: 10.9 MB (10876697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cec535da207f5d811fda01a346f5561fd2f77c2d09a080925b7455b84f0959e`  
		Last Modified: Sat, 04 Feb 2023 07:29:44 GMT  
		Size: 54.6 MB (54587320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3505f4b99c6569cd863134678b48c36f8a569daf7d4c9d5bdbf6b63e04ed99d`  
		Last Modified: Sun, 05 Feb 2023 00:48:15 GMT  
		Size: 1.4 MB (1369607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02564c7c4a9b7962a5d733cdcd64ee6d70dca78bbda4a3012b51c2f348e756fc`  
		Last Modified: Sun, 05 Feb 2023 00:48:15 GMT  
		Size: 1.4 MB (1447328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:999a901822b6a4c03183ed590bcb95cf42cebb0b7267e0bc0e63f4dfe8cd9e2f`  
		Last Modified: Sun, 05 Feb 2023 00:48:18 GMT  
		Size: 11.5 MB (11541682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:c667e94ce64cafafa362c10a0610fc980dedffa7e5cb5e787e264afc55b2b8b7
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129476958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20328dfed07fd283ea88f0bc9fa6917b72865c2094e3bdbb37b791662bc0bf2b`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 04 Feb 2023 09:59:19 GMT
ADD file:239b5255d05e0742f381f82fb7cd586fcc6d9a427263238a2be3372c494ae933 in / 
# Sat, 04 Feb 2023 09:59:20 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 10:49:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 10:49:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 10:49:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:09:26 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sun, 05 Feb 2023 05:09:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sun, 05 Feb 2023 05:09:31 GMT
ENV NEKO_VERSION=2.3.0
# Sun, 05 Feb 2023 05:10:43 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sun, 05 Feb 2023 05:10:43 GMT
ENV HAXE_VERSION=4.2.5
# Sun, 05 Feb 2023 05:10:43 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sun, 05 Feb 2023 05:14:26 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sun, 05 Feb 2023 05:14:27 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:7a21a86b3957d8c99250334cfb78c55af4f8c9277f2f1d4abd53d0362f96323d`  
		Last Modified: Sat, 04 Feb 2023 10:05:53 GMT  
		Size: 50.2 MB (50190828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aacc3c746ca1bd99005f184b00ee418e015c2090c72bda638766d9fb93d3f065`  
		Last Modified: Sat, 04 Feb 2023 10:59:08 GMT  
		Size: 4.9 MB (4933374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b393b343e4fb3b92027c4741418a04d6475259ee243fbf036c1be41df98212`  
		Last Modified: Sat, 04 Feb 2023 10:59:09 GMT  
		Size: 10.2 MB (10217742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e55fdd5f0aba51b2504973439b1c887364b84bc0d7b211da07aba072b81520`  
		Last Modified: Sat, 04 Feb 2023 10:59:32 GMT  
		Size: 50.4 MB (50356141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec9630837f36a8fafbdea192350b19b1ab5c6ae2d261af66e714da5226f840c`  
		Last Modified: Sun, 05 Feb 2023 05:43:20 GMT  
		Size: 1.3 MB (1282636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077957ef59eda40d2bf9aff6e61df23c79ce1bd97f9beb083482b3866818c56d`  
		Last Modified: Sun, 05 Feb 2023 05:43:20 GMT  
		Size: 1.4 MB (1386820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f551f35520c0987305fd0b662e0bfe2513ac25f0cae024750632ece6d4e8e11a`  
		Last Modified: Sun, 05 Feb 2023 05:43:22 GMT  
		Size: 11.1 MB (11109417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:a82fb8b583943dc926baa4f678f3508fe68027d6b3937e6b7c502c80246bf5dc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.4 MB (140371125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43c0f868f63d5fa53590ac1926fc14b747e092650348f1764c176692b92a7a1b`
-	Default Command: `["haxe"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:26 GMT
ADD file:c5a7c65d67685092faa3456c1a772550aa6d06ac07e1f98a95d39c31e304dbf8 in / 
# Sat, 04 Feb 2023 06:17:27 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 06:45:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 06:45:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 04 Feb 2023 06:46:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 20:51:44 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 04 Feb 2023 20:51:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 20:51:47 GMT
ENV NEKO_VERSION=2.3.0
# Sat, 04 Feb 2023 20:52:59 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Sat, 04 Feb 2023 20:52:59 GMT
ENV HAXE_VERSION=4.2.5
# Sat, 04 Feb 2023 20:52:59 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Sat, 04 Feb 2023 20:55:14 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Sat, 04 Feb 2023 20:55:14 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:fac7262b6510529638951e16807cf1758f42c892ed924e334c27bb8bbcf7d7c2`  
		Last Modified: Sat, 04 Feb 2023 06:21:01 GMT  
		Size: 53.7 MB (53681927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38880e907cdcb0da4f6bddfc0380aaa5b11d6adf12bf87034adce6372ba306ba`  
		Last Modified: Sat, 04 Feb 2023 06:52:03 GMT  
		Size: 5.2 MB (5151209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8181793414caae285b5e035037e19a57765aa12828ef23dd5e47e7606631696`  
		Last Modified: Sat, 04 Feb 2023 06:52:03 GMT  
		Size: 10.9 MB (10873560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43bb9401c1adc4cb3357318434fac52322d8be0895e0085fec8b3448ff7a1619`  
		Last Modified: Sat, 04 Feb 2023 06:52:20 GMT  
		Size: 54.7 MB (54680048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a516fc83ab8d9a4dc1a35f9569dc0e134f967d97d41a7cbe74fc791a46ebb7`  
		Last Modified: Sat, 04 Feb 2023 21:14:34 GMT  
		Size: 1.4 MB (1360105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c53ff2d18ec1d2d4d8a22187d661efe401044d922f85196d090f3498bfa9ed9`  
		Last Modified: Sat, 04 Feb 2023 21:14:34 GMT  
		Size: 1.4 MB (1438145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24525b2e8021be95b3a5a969e1378aa80a2354154e750b8f1405d59000bb31ca`  
		Last Modified: Sat, 04 Feb 2023 21:14:36 GMT  
		Size: 13.2 MB (13186131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.1487; amd64

```console
$ docker pull haxe@sha256:29bed918656d7b76fee2547593e746279f0fbdc6266d6757e5cb3f2550b299b6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.4 GB (1414169643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edfa068d59ca84be693924814c95437832b7d99762d8e32473daa4d46d6d1567`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 06 Jan 2023 23:47:40 GMT
RUN Apply image 10.0.20348.1487
# Thu, 12 Jan 2023 04:01:09 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 05:44:17 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Thu, 12 Jan 2023 05:44:18 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Thu, 12 Jan 2023 05:44:19 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Thu, 12 Jan 2023 05:44:20 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Thu, 12 Jan 2023 05:44:21 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Thu, 12 Jan 2023 05:44:44 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 05:46:06 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 05:46:29 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Thu, 12 Jan 2023 05:46:30 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 12 Jan 2023 05:47:10 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 05:47:11 GMT
ENV HAXE_VERSION=4.2.5
# Thu, 12 Jan 2023 05:51:44 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 05:52:13 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 12 Jan 2023 05:52:14 GMT
ENV HOMEDRIVE=C:
# Thu, 12 Jan 2023 05:52:35 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 05:52:58 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Thu, 12 Jan 2023 05:52:59 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:1a65b089bc835b0c3700397b1935e97cf469b0891bb4de3942c8dfbe4b672d47`  
		Last Modified: Thu, 12 Jan 2023 02:33:52 GMT  
		Size: 1.4 GB (1386029089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a81c906622aa010adfaf1dd8c570ad750108a9b1a91ee1eb148e409e3e4fe68f`  
		Last Modified: Thu, 12 Jan 2023 04:37:06 GMT  
		Size: 1.4 KB (1423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11cbaf5fba15e6c593a48fd6c18e5a848a9633647d24cbc93d35fa460835b561`  
		Last Modified: Thu, 12 Jan 2023 07:08:42 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12cf36e6894612da4a01d9dbfe0e70b7ed05a2b672e2c1d0ccf4de4cf078edd`  
		Last Modified: Thu, 12 Jan 2023 07:08:42 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45441fc5b5f471fa99b539af034736c29e48e0c20813d63a7a279dc85c916dab`  
		Last Modified: Thu, 12 Jan 2023 07:08:41 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9139caf496456aae868e8c1a9ae988ffa7d67ac418c620bced3edfa2b1fa561a`  
		Last Modified: Thu, 12 Jan 2023 07:08:40 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e01e0dafe5b6b277920d23073ef62bac1ab822512a36f1f3215e44ca14da054`  
		Last Modified: Thu, 12 Jan 2023 07:08:40 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7bc28d7fbfffa8d4b9418f21d5eb77c0711bfed24e1fc1d063df8899f98f30d`  
		Last Modified: Thu, 12 Jan 2023 07:08:39 GMT  
		Size: 612.0 KB (612043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:350b1aefb0bf68f502cef448822439342aac63aac3cfadc7c5819b047b103ed7`  
		Last Modified: Thu, 12 Jan 2023 07:08:41 GMT  
		Size: 13.1 MB (13139159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c67509434068dc76cf390bd4349fbd8daf2a6df5f936e09e9e18bd4cf0f0771`  
		Last Modified: Thu, 12 Jan 2023 07:08:37 GMT  
		Size: 560.9 KB (560883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7290e481ee7afd57f2618c02a941d8a22b7294c456f766c82292614b853c69`  
		Last Modified: Thu, 12 Jan 2023 07:08:36 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20cde23b0f0b8a9d4b2ad2d52f32a5fcc635a12e2e00171ae9677b1973328321`  
		Last Modified: Thu, 12 Jan 2023 07:08:38 GMT  
		Size: 2.4 MB (2403770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1065245e84e100b0e0ea28d9d27f35a0f123b73990040d1194133c7d9079fc2`  
		Last Modified: Thu, 12 Jan 2023 07:08:36 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6e61c056c6f7379d31380eb763e4cbbc1a410ab761ac6a6e15caff25805fea`  
		Last Modified: Thu, 12 Jan 2023 07:08:43 GMT  
		Size: 9.6 MB (9553362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f007f2380cdec9d1d772f0d08b0c09ed4f587c6238b67b5dd39d5311bc49c22a`  
		Last Modified: Thu, 12 Jan 2023 07:08:34 GMT  
		Size: 609.7 KB (609717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d092ec6cab6dc5e27a71529fdcb240231c7280c75f13c6f7e0249f17c48ba052`  
		Last Modified: Thu, 12 Jan 2023 07:08:34 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82ec77852e063a954b97b858096430b88f255b73b74d270644b9ce8507146884`  
		Last Modified: Thu, 12 Jan 2023 07:08:34 GMT  
		Size: 616.9 KB (616934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c1eea239036cd9ae1f20f4310617448dc97592ad70595e11b5f8b5207a2a1b`  
		Last Modified: Thu, 12 Jan 2023 07:08:34 GMT  
		Size: 630.8 KB (630815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f91aa7332ec6a709146744f884005ab644899910ef9390d88531ed5b10526b`  
		Last Modified: Thu, 12 Jan 2023 07:08:34 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.3887; amd64

```console
$ docker pull haxe@sha256:eb027f45a1e1324015b8fc6c987fcf79f752616b2de457fe83c4a3d701668153
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **1.7 GB (1738507317 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9771ee2334e26f16f02939439a62cc421efb85f7b5022dc2d96288d4c6b4d93`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 07 Jan 2023 05:37:58 GMT
RUN Apply image 10.0.17763.3887
# Thu, 12 Jan 2023 04:04:12 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Thu, 12 Jan 2023 05:53:05 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Thu, 12 Jan 2023 05:53:06 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Thu, 12 Jan 2023 05:53:08 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Thu, 12 Jan 2023 05:53:09 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Thu, 12 Jan 2023 05:53:10 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Thu, 12 Jan 2023 05:53:35 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 05:54:57 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 05:55:27 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Thu, 12 Jan 2023 05:55:28 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 12 Jan 2023 05:56:13 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 05:56:14 GMT
ENV HAXE_VERSION=4.2.5
# Thu, 12 Jan 2023 06:00:52 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Thu, 12 Jan 2023 06:01:24 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Thu, 12 Jan 2023 06:01:25 GMT
ENV HOMEDRIVE=C:
# Thu, 12 Jan 2023 06:01:51 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 12 Jan 2023 06:02:21 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Thu, 12 Jan 2023 06:02:22 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:6e222c5ada69382aa2b4fe30b23ae56c7e3ada92712109d20f3edd457a6120b6`  
		Last Modified: Thu, 12 Jan 2023 02:40:02 GMT  
		Size: 1.7 GB (1707943932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99eee4cf5f23d13a762e719b10916801f19f9df4bd7ff9b4c5cf57133b3dc04`  
		Last Modified: Thu, 12 Jan 2023 04:39:02 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c2d75cdee0543186cf4b7f911336be2a76e8d62d4e1c0acbdcaf9b5488f416`  
		Last Modified: Thu, 12 Jan 2023 07:08:58 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2c12fe145d16a5418ea35422b3f63b25dc6291f5cde5b13d478a2425c555bca`  
		Last Modified: Thu, 12 Jan 2023 07:08:58 GMT  
		Size: 1.3 KB (1283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:913767c362d7457d4e6a7ef858cdf1faf7ab9711d47dab38874f09cfabc5cf51`  
		Last Modified: Thu, 12 Jan 2023 07:08:58 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f804895b8825971e6c3881f6e737cecd327af9d0fd8a0acbc573b95e757ed95b`  
		Last Modified: Thu, 12 Jan 2023 07:08:57 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b5d85f36723b131fe9e80379f1411cdff8ca30781c06074dce33a8d4be2228a`  
		Last Modified: Thu, 12 Jan 2023 07:08:56 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12093de43c404a2920de718cddbee5f82625ff2b11781131b6f485df1ce59bd`  
		Last Modified: Thu, 12 Jan 2023 07:08:56 GMT  
		Size: 364.8 KB (364777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cb1fde781e1e326f713095f89c61491a9d3ba50dcf1746f095806d8dc028f9a`  
		Last Modified: Thu, 12 Jan 2023 07:08:58 GMT  
		Size: 12.9 MB (12935734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:005415f2c93a95bf33e8b521404091c52b38c48bbd958bea4bf0050fd27d283f`  
		Last Modified: Thu, 12 Jan 2023 07:08:54 GMT  
		Size: 328.3 KB (328311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d7f8dfb9ed863c1bc3803b94a7cb582cdeacae3c79b5be5fba1b70ff46ad33`  
		Last Modified: Thu, 12 Jan 2023 07:08:54 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c28677e93fb8bf7b617c5cc22249ef6fad5e1f9813b69efb667dc9933da3d8`  
		Last Modified: Thu, 12 Jan 2023 07:08:55 GMT  
		Size: 2.2 MB (2160647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84aee9adbf53fa4209941bbc320e9fe23be8733d97aa83b063e696d5df877f8d`  
		Last Modified: Thu, 12 Jan 2023 07:08:53 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae59958234f32618ac39857eaf38a4da8e2fe315a23defd7eaa692fbc4af7e52`  
		Last Modified: Thu, 12 Jan 2023 07:09:01 GMT  
		Size: 13.6 MB (13627818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fa901d655aa907311afe5c71e9623b9bcd747ee63b22cfcc1d3bac6a1fdf84`  
		Last Modified: Thu, 12 Jan 2023 07:08:52 GMT  
		Size: 364.0 KB (363962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c88b8525ba1c98e5040337f3dd3ed3b45a34027b5311c3e51ff2b9d568818025`  
		Last Modified: Thu, 12 Jan 2023 07:08:51 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e0df10183f356f23e2d0042027a3ad4ef99154cbddffce3c534cbbe9914aff6`  
		Last Modified: Thu, 12 Jan 2023 07:08:52 GMT  
		Size: 372.3 KB (372327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afd4d49e76ffb1e2fddee43a08663f12d94d0dc3c0adf3258f14acd5c3518bf`  
		Last Modified: Thu, 12 Jan 2023 07:08:52 GMT  
		Size: 396.1 KB (396115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957d8f54ba7d6f88a4ecfd350b2294f40f9556f7d38620fe9bfbb6bc23b72f55`  
		Last Modified: Thu, 12 Jan 2023 07:08:51 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
