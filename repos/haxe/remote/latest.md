## `haxe:latest`

```console
$ docker pull haxe@sha256:caceeed165b257a5018b0dca6dd40ee096ea2fcb4063d7b87a636d4a9c5a8ed4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.20348.887; amd64
	-	windows version 10.0.17763.3287; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:bb441b7b3ad661e3fc666b2e411a41bcd2e5ced16686cf273c017de83c5e45e2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **140.0 MB (139972207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb6e499691191dd7b07aa1e4581b9d77b6153766133dbb39bf422f2361cb338`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:46:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:32:45 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 03 Aug 2022 01:32:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Wed, 03 Aug 2022 01:32:49 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 03 Aug 2022 01:34:09 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Wed, 03 Aug 2022 01:34:09 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 03 Aug 2022 01:34:09 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Wed, 03 Aug 2022 01:36:42 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Wed, 03 Aug 2022 01:36:42 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d4b9b6e964657da49910b495173d6c4f0d9bc47b3b44273cf82fd32723d165`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 5.2 MB (5156256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2068746827ec1b043b571e4788693eab7e9b2a95301176512791f8c317a2816a`  
		Last Modified: Tue, 02 Aug 2022 02:18:26 GMT  
		Size: 10.9 MB (10876485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9daef329d35093868ef75ac8b7c6eb407fa53abbcb3a264c218c2ec7bca716e6`  
		Last Modified: Tue, 02 Aug 2022 02:18:47 GMT  
		Size: 54.6 MB (54584071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da0bc05b6548d0abc6a943cc77807079dc9211b76ad6f964e6a9ac8ffa4c26ef`  
		Last Modified: Wed, 03 Aug 2022 02:00:59 GMT  
		Size: 1.4 MB (1368014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fd7e97050aaadf9b0e0e02e7c091652251e720565fd456aa0bc06d85fe6459`  
		Last Modified: Wed, 03 Aug 2022 02:00:59 GMT  
		Size: 1.4 MB (1447179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e635bec27fb85f681b57bf156f5f233a2c26b66425bd44868d7a5f576a53e36d`  
		Last Modified: Wed, 03 Aug 2022 02:01:01 GMT  
		Size: 11.5 MB (11540871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:0b3ae3d78101d13901d716130a8ecd3774d324f96d11c92ade902fdd498a77e7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **129.5 MB (129462464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2556c49cd3dce9cc0d6aedd0751f4780fca7c1f1410049c02ab6dc3fa66fb631`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 02 Aug 2022 00:58:36 GMT
ADD file:4e2780cf1c53cc1c475d2ebae48d4bf03029fa68ba9fbc991be76ac9e3944977 in / 
# Tue, 02 Aug 2022 00:58:37 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:47:18 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:47:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 02 Aug 2022 01:47:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 07:14:39 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 04 Aug 2022 07:14:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 04 Aug 2022 07:14:43 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 04 Aug 2022 07:15:45 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 04 Aug 2022 07:15:45 GMT
ENV HAXE_VERSION=4.2.5
# Thu, 04 Aug 2022 07:15:45 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 04 Aug 2022 07:20:37 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 04 Aug 2022 07:20:37 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:05aa23077de69478dfc20e56aa2d54a2b13bbef07c4d2578524585d098af4e72`  
		Last Modified: Tue, 02 Aug 2022 01:06:07 GMT  
		Size: 50.2 MB (50195271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a47a4ec510d3ede75fd285276ee8b3d9dd3c1d2bce8f21ae0f2de4898c015b9e`  
		Last Modified: Tue, 02 Aug 2022 02:09:14 GMT  
		Size: 4.9 MB (4930860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef792f88dc77db1940eec048a6d0b4d691c7650b28cd058aed9314fea5f708b6`  
		Last Modified: Tue, 02 Aug 2022 02:09:14 GMT  
		Size: 10.2 MB (10217964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f493c1b0c9a50775af17259c793561f1ce1c5ab4bbf3947d8ca612f476bfcf23`  
		Last Modified: Tue, 02 Aug 2022 02:09:40 GMT  
		Size: 50.3 MB (50342099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b2bd2b28208af4c4e845f8567cce954e93a65d3e3b0cdeeb281ea0c56a55fb8`  
		Last Modified: Thu, 04 Aug 2022 08:04:11 GMT  
		Size: 1.3 MB (1281009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc40d463ec8d4325d5509cf436fb5f7050349b8ab8d7b4051f0ee6b3dd6ac2a0`  
		Last Modified: Thu, 04 Aug 2022 08:04:11 GMT  
		Size: 1.4 MB (1387319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e600670968a9fb43deb776c0b9e716d15e5802ae8e8386e75213acc0f460e2`  
		Last Modified: Thu, 04 Aug 2022 08:04:14 GMT  
		Size: 11.1 MB (11107942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:d54e122dae0499810e067a2627ce598d4113c19b0ba1e76b6ea9836a7841ed5b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **139.5 MB (139500886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:913b6906858aa1479d79f715b4e93d6264e4a9e5668a985658e61441cf2403fc`
-	Default Command: `["haxe"]`

```dockerfile
# Tue, 23 Aug 2022 01:52:16 GMT
ADD file:ce6014a27d18915dc6d46c5c1f0f894f0027d1e41fbebb1599c16371b7bab2f1 in / 
# Tue, 23 Aug 2022 01:52:18 GMT
CMD ["bash"]
# Tue, 23 Aug 2022 02:27:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 02:28:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 23 Aug 2022 02:28:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:48:51 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 23 Aug 2022 17:48:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Tue, 23 Aug 2022 17:48:56 GMT
ENV NEKO_VERSION=2.3.0
# Tue, 23 Aug 2022 17:50:12 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Tue, 23 Aug 2022 17:50:13 GMT
ENV HAXE_VERSION=4.2.5
# Tue, 23 Aug 2022 17:50:14 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Tue, 23 Aug 2022 17:53:08 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.5 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Tue, 23 Aug 2022 17:53:09 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:cd84405c8b9e7a8c3d580c2148d25120dd697ea61e1cb55a62f33e67988b7043`  
		Last Modified: Tue, 23 Aug 2022 01:57:29 GMT  
		Size: 53.7 MB (53690830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d98e120b809269e56de468d2b91569789c521011e4d9b1806e43fd04462de2`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 4.9 MB (4944180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cb6be5911b40ca548e48c10b09cb2312f1698b4c84f09711c69389a94b1a8be`  
		Last Modified: Tue, 23 Aug 2022 02:36:44 GMT  
		Size: 10.7 MB (10657442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db608c3c3ce3568556faf63acbc2069811afe242faf8992ccf0ab1986ee38e4f`  
		Last Modified: Tue, 23 Aug 2022 02:37:07 GMT  
		Size: 54.7 MB (54680886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27ff3c6f0f57322e5afe62c7d60912e7787ce225471be7a4e5cd7e8cc166da43`  
		Last Modified: Tue, 23 Aug 2022 18:20:05 GMT  
		Size: 1.1 MB (1135199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d064316d8cda737927aac40b24372cf310150abf7d272a29ca92bfc247f2be4a`  
		Last Modified: Tue, 23 Aug 2022 18:20:05 GMT  
		Size: 1.4 MB (1432826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ece4cfac227e8e840c65cfaa668cc28ab2d33b5d016dd9e338ea8de3832a9bf0`  
		Last Modified: Tue, 23 Aug 2022 18:20:07 GMT  
		Size: 13.0 MB (12959523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.20348.887; amd64

```console
$ docker pull haxe@sha256:334cfac891e7cf3b25144b5e0f65d1525b722db62ce04ba4ad29bfdadbebfdf7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2351079859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f6cdd750fb405430e7a8096d4dd4dc3a166d96154935d6e8cc267359db48b0ef`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Sat, 06 Aug 2022 02:59:35 GMT
RUN Install update 10.0.20348.887
# Wed, 10 Aug 2022 13:33:21 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 13:33:22 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Aug 2022 13:33:23 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Aug 2022 13:33:24 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Aug 2022 13:33:25 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Aug 2022 13:33:26 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Aug 2022 13:34:03 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Aug 2022 13:35:38 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:36:05 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Aug 2022 13:36:06 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Aug 2022 13:37:00 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:37:01 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 10 Aug 2022 13:42:10 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:42:41 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 10 Aug 2022 13:42:42 GMT
ENV HOMEDRIVE=C:
# Wed, 10 Aug 2022 13:43:15 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Aug 2022 13:43:50 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Wed, 10 Aug 2022 13:43:51 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:97b25a378238b615dc51216c4d87ce17fd3cc3dca9db458e8705d1a4c17e3bb7`  
		Size: 880.0 MB (880025531 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:ff9b89cbdb5f88cb926263140643eb2bfad61fb092119830e290c8f8ff711c8f`  
		Last Modified: Wed, 10 Aug 2022 15:05:31 GMT  
		Size: 1.4 KB (1355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14ef8ea2c0d2c51f96183694be32ac2ffd3b26489edb4c0fd0c6f0f9a04ca242`  
		Last Modified: Wed, 10 Aug 2022 15:05:30 GMT  
		Size: 1.4 KB (1385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3c155a66837580dcc8d8677d90add5f7a87fb69d958b975fcd97997c5c8e84`  
		Last Modified: Wed, 10 Aug 2022 15:05:29 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a97c559d333fb963d35f87ebbb6dcf08d57392bfdcb8ee686c77d5522de5f8`  
		Last Modified: Wed, 10 Aug 2022 15:05:29 GMT  
		Size: 1.4 KB (1399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b3024e1c09f21717d4e82d86e00d1f10c33fa77d223fff2d4a8090490c48a40`  
		Last Modified: Wed, 10 Aug 2022 15:05:28 GMT  
		Size: 1.4 KB (1434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91712068c4a84272133a8d0a3225b4ceab1701bb0498c52ea7c98d7576e12b19`  
		Last Modified: Wed, 10 Aug 2022 15:05:27 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10706ea757b7cb654b5feed0a54abd89e5cbd09dbdf898210871216364760f38`  
		Last Modified: Wed, 10 Aug 2022 15:05:27 GMT  
		Size: 622.9 KB (622883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b4005fb7634e6e0b4b81653db2d7f15a04aeffbe9dd648dac1b903ce5c04a34`  
		Last Modified: Wed, 10 Aug 2022 15:05:28 GMT  
		Size: 13.2 MB (13155951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e284cc2cd9b7c169400458b97f37f34808bdf4cfdd18addba048bf0948a76c6a`  
		Last Modified: Wed, 10 Aug 2022 15:05:25 GMT  
		Size: 567.9 KB (567949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9789ad229309ac60bf50525dc7e8a306b83c30ae37f41649cd63b5f7c925464`  
		Last Modified: Wed, 10 Aug 2022 15:05:24 GMT  
		Size: 1.3 KB (1298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e650464fb6141b71c569a631b105dce069455e53980bb64799b54e1392cdba`  
		Last Modified: Wed, 10 Aug 2022 15:05:25 GMT  
		Size: 2.4 MB (2407199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63b435555c313469472dbca56b14015ab0843b1425dc9dc4439fd8a9f0bdb9d1`  
		Last Modified: Wed, 10 Aug 2022 15:05:23 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a4b066e6587d03b971be5f792c8c346a9dc2cab754ce655a045a1adaea8caa`  
		Last Modified: Wed, 10 Aug 2022 15:05:32 GMT  
		Size: 15.5 MB (15541337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de8518d5e1cd59124c8843bd1ff996649fd922669c0cfb777c4432345bdf74d`  
		Last Modified: Wed, 10 Aug 2022 15:05:21 GMT  
		Size: 629.1 KB (629112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a370fea0e70cbf17c1ab95e80103220fbb72e69e26a3a1ea8525efd1bc2729c`  
		Last Modified: Wed, 10 Aug 2022 15:05:21 GMT  
		Size: 1.4 KB (1396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c369f6e10fe0430af08e914abceb799ad803db44c6c2d6b5de7454ea92a74a`  
		Last Modified: Wed, 10 Aug 2022 15:05:21 GMT  
		Size: 620.1 KB (620142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470ff79e09ee4527f80c675c3f5f3432e5db27c8951876b661623b858b0713cc`  
		Last Modified: Wed, 10 Aug 2022 15:05:21 GMT  
		Size: 632.3 KB (632317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa284758bdaa3e91a80e9d0a9af63461fe68d2d9575ed06e9feb2dd63e1e8d96`  
		Last Modified: Wed, 10 Aug 2022 15:05:21 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.3287; amd64

```console
$ docker pull haxe@sha256:fb3a9fb4c2dea07a9c3abe3801e18876dea761b8f8d38d06159cfd430d481728
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2708250123 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96fad7534d718e1a40c8f2208b8380c2ee7766fcb0b03d544daf374d9d3f08ac`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 13:44:07 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Aug 2022 13:44:08 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Aug 2022 13:44:09 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Aug 2022 13:44:10 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Aug 2022 13:44:11 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Aug 2022 13:44:12 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Aug 2022 13:45:55 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Aug 2022 13:47:50 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:48:46 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Aug 2022 13:48:47 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Aug 2022 13:49:58 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:49:59 GMT
ENV HAXE_VERSION=4.2.5
# Wed, 10 Aug 2022 13:54:08 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.5/haxe-4.2.5-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne '9e7913999eb3693d540926219b45107b3dc249feb44204c0378fcdc6a74a9132') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 10 Aug 2022 13:55:01 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 10 Aug 2022 13:55:02 GMT
ENV HOMEDRIVE=C:
# Wed, 10 Aug 2022 13:55:56 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Aug 2022 13:56:51 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org/p/hxcpp/4.2.1/download/') >$null
# Wed, 10 Aug 2022 13:56:52 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:da71148bcd96afa7027d6172acee93aad6002bfbe87cadf468260667c09b3a89`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8469a25bb150f005d3a574107a7f9ea3bcd77f4c7c5db3c95bf50e9bd3082a03`  
		Last Modified: Wed, 10 Aug 2022 15:05:54 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390a51cf7b9534b69f7b2066e957e367d98afa0ade97769dbb642475d053b33b`  
		Last Modified: Wed, 10 Aug 2022 15:05:52 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9556e8d13032c80bc2b559ee9d01bec7029345ffb2d45c1c63bd8169ab69e`  
		Last Modified: Wed, 10 Aug 2022 15:05:52 GMT  
		Size: 1.4 KB (1373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588228d9f632198419ecaf714aadcb047c1b3054d26290d675e8d16e1bafd6e0`  
		Last Modified: Wed, 10 Aug 2022 15:05:51 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b258fc582d9b63b555568fe6e456b813795dcdf000bfe71c51d8d3cf97a236`  
		Last Modified: Wed, 10 Aug 2022 15:05:50 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f597923f60e3f3c3576f44b20f709cfa27d718bd531462017ccb1bb5c8f6eb2c`  
		Last Modified: Wed, 10 Aug 2022 15:05:49 GMT  
		Size: 344.8 KB (344805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6620274df6829240e62ba2d485395e196a7714e19f3e267a1507a244bedb5b2`  
		Last Modified: Wed, 10 Aug 2022 15:05:51 GMT  
		Size: 12.9 MB (12924705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ada7e3553107826bf476b6b0d9650a54566dd7c3034daa7310c6f0cc311526d`  
		Last Modified: Wed, 10 Aug 2022 15:05:47 GMT  
		Size: 317.6 KB (317640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2228376cf8a319bdd685c253985fd46ef2f02f388f808749d8c711defca349f`  
		Last Modified: Wed, 10 Aug 2022 15:05:46 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fe393820ea6de40def1a1c149462cfb33e4c71edc076b9d92685b9023626236`  
		Last Modified: Wed, 10 Aug 2022 15:05:48 GMT  
		Size: 2.1 MB (2149360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb28c0c7fd853d52273b7afb4434443499e13be46b361d9124f12489654b249`  
		Last Modified: Wed, 10 Aug 2022 15:05:46 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ac92f69322edaf4651437b69357d45fdeb1cbf5b57c2de07f22f3755dea95e`  
		Last Modified: Wed, 10 Aug 2022 15:05:55 GMT  
		Size: 13.7 MB (13664169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e00f6941c371e52b27fb302089eb6bd5ed64bd8579660f63ed50fa48eaced37`  
		Last Modified: Wed, 10 Aug 2022 15:05:43 GMT  
		Size: 359.8 KB (359834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9903d92bee5416688f2d5dd207fa442a12c34419b2573da2ef77ae75388d1e58`  
		Last Modified: Wed, 10 Aug 2022 15:05:43 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45312bd8dad94481f7cd0760ed5a6c240bc77616a3764762edad53d865a1934a`  
		Last Modified: Wed, 10 Aug 2022 15:05:43 GMT  
		Size: 369.3 KB (369325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a255924fbde3a29cac1c310770ad85489e73611a25089a51d23757c4af233f`  
		Last Modified: Wed, 10 Aug 2022 15:05:43 GMT  
		Size: 393.6 KB (393567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac796d1810301e651f906a7f21a83a8fbb1064b5a1502e716fd0ed2eb3fccb7`  
		Last Modified: Wed, 10 Aug 2022 15:05:43 GMT  
		Size: 1.4 KB (1392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
