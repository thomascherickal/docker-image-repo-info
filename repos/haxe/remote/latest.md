## `haxe:latest`

```console
$ docker pull haxe@sha256:c7999e063c32e8de2ad36fb24460b7dd0edd2c91016e805a102dc40c3976c2b7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	windows version 10.0.17763.2300; amd64
	-	windows version 10.0.14393.4770; amd64

### `haxe:latest` - linux; amd64

```console
$ docker pull haxe@sha256:a875ec773a19b60659d29a026cafdca980eeeba5f9d19bde226463bc8b676949
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **133.6 MB (133605425 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2951e46c1924409d6621415647b6fa483851de41644fc64ea5794b3284d93d6d`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 17 Nov 2021 02:20:51 GMT
ADD file:cb5ed7070880d4c0177fbe6dd278adb7926e38cd73e6abd582fd8d67e4bbf06c in / 
# Wed, 17 Nov 2021 02:20:51 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 03:15:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 03:15:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 03:16:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 08:54:40 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 08:54:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 08:54:46 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 18 Nov 2021 08:56:05 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 18 Nov 2021 08:56:05 GMT
ENV HAXE_VERSION=4.2.4
# Thu, 18 Nov 2021 08:56:05 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 18 Nov 2021 09:02:58 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 18 Nov 2021 09:02:58 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:1230f17f526cb07307d41462355b10488b994e8bdafe0d8f275a405fa3b33831`  
		Last Modified: Wed, 17 Nov 2021 02:26:06 GMT  
		Size: 50.4 MB (50437098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d17d0de332ca1b34d53ca41c2b39ea52ce72f8c1e81c5200e27a8bade3e6ecbb`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 7.8 MB (7833787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7474d56348f5333567750c1e5f06f899477fd437330627341eafa71bfa1a36ab`  
		Last Modified: Wed, 17 Nov 2021 03:24:34 GMT  
		Size: 10.0 MB (9997183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211c565de40518c5dac4498ccebbf3833fcfaa5db17d4bf94e6bef466136278b`  
		Last Modified: Wed, 17 Nov 2021 03:24:55 GMT  
		Size: 51.8 MB (51840474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1098317a279e1e71338895a9be3b2b61b916b9e11c1fd66898486fd7574aee2`  
		Last Modified: Thu, 18 Nov 2021 09:38:19 GMT  
		Size: 1.3 MB (1314898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934893658aad470bab66c9b4907945593957fe3893f1d4663d2b1e91a876b4b8`  
		Last Modified: Thu, 18 Nov 2021 09:38:19 GMT  
		Size: 2.3 MB (2308327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee76448673dff23112ee229702f16c1b8e6ff6809ac61b707102db5e8d799ef0`  
		Last Modified: Thu, 18 Nov 2021 09:38:22 GMT  
		Size: 9.9 MB (9873658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm variant v7

```console
$ docker pull haxe@sha256:d0653cf690ee160e1d9d86685d56a0c299d323564347cc9945417025ecd6a358
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.8 MB (122755680 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cbad18fbbab9c5766124d883cb7c4e2c374cca685f44ebd6ecf603884840a4b`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 17 Nov 2021 02:00:12 GMT
ADD file:d71807613acdf86685f6d640a90e27b7b63cfe0f13d88668ee943aca089d8876 in / 
# Wed, 17 Nov 2021 02:00:13 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 02:45:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 02:45:53 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 02:46:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 15:40:30 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 15:40:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 15:40:41 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 18 Nov 2021 15:43:56 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 18 Nov 2021 15:43:56 GMT
ENV HAXE_VERSION=4.2.4
# Thu, 18 Nov 2021 15:43:57 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 18 Nov 2021 15:51:58 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 18 Nov 2021 15:51:59 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:10acd81022d17f452439d0385615fa066b8f0ddcf3c1a803872eec5bdc6acf64`  
		Last Modified: Wed, 17 Nov 2021 02:16:00 GMT  
		Size: 45.9 MB (45918099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a9604eb6c465f658d6422593d504030155029fe0c4302451d4369030c29144`  
		Last Modified: Wed, 17 Nov 2021 03:07:14 GMT  
		Size: 7.1 MB (7125194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b043b954c4f0757e89df96897cea2cf1f93c6275466008e4ba7a4b1089c7dd3d`  
		Last Modified: Wed, 17 Nov 2021 03:07:15 GMT  
		Size: 9.3 MB (9343839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf41461745fd89900c4b7cc794c93de081420bd83223b46e1495ff96748685c`  
		Last Modified: Wed, 17 Nov 2021 03:07:59 GMT  
		Size: 47.4 MB (47356485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d150bdcc08581c0ff60e3a708aeef7f43365e41cb7d7ff3f2255396d09dc6942`  
		Last Modified: Thu, 18 Nov 2021 16:46:20 GMT  
		Size: 1.2 MB (1238050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69ee7c04819ff00af0af0376060f0690616b0c5a138dd5edd6f6d63f35239361`  
		Last Modified: Thu, 18 Nov 2021 16:46:21 GMT  
		Size: 2.2 MB (2249673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f77547548d2585f1b5d07d02201e31c542ff32fd06e56eba2e449539b1e6046`  
		Last Modified: Thu, 18 Nov 2021 16:46:27 GMT  
		Size: 9.5 MB (9524340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - linux; arm64 variant v8

```console
$ docker pull haxe@sha256:993b8b98789779b61c663e69c5790b7f792ae0a3934b1b78c50f8756ff0e1958
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.1 MB (134085596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7740de6b274951ff9b22a3ee8626552dd4b537b3e4b98aedba8710ed998715f1`
-	Default Command: `["haxe"]`

```dockerfile
# Wed, 17 Nov 2021 02:40:27 GMT
ADD file:c7e9e884b1494f96e33e9d9a892b51367af8943edb282c4101cc99ea78a7753f in / 
# Wed, 17 Nov 2021 02:40:28 GMT
CMD ["bash"]
# Wed, 17 Nov 2021 13:28:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 17 Nov 2021 13:28:15 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 17 Nov 2021 13:28:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 01:12:20 GMT
ENV PATH=/usr/local/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 18 Nov 2021 01:12:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		libgc1c2 		zlib1g 		libpcre3 		libmariadb3 		libsqlite3-0 		libmbedcrypto3 		libmbedtls12 		libmbedx509-0 	&& rm -rf /var/lib/apt/lists/*
# Thu, 18 Nov 2021 01:12:26 GMT
ENV NEKO_VERSION=2.3.0
# Thu, 18 Nov 2021 01:13:45 GMT
RUN set -ex 	&& buildDeps=' 		gcc 		make 		cmake 		libgc-dev 		libssl-dev 		libpcre3-dev 		zlib1g-dev 		apache2-dev 		libmariadb-client-lgpl-dev-compat 		libsqlite3-dev 		libmbedtls-dev 		libgtk2.0-dev 	' 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends && rm -rf /var/lib/apt/lists/* 		&& wget -O neko.tar.gz "https://github.com/HaxeFoundation/neko/archive/v2-3-0/neko-2.3.0.tar.gz" 	&& echo "850e7e317bdaf24ed652efeff89c1cb21380ca19f20e68a296c84f6bad4ee995 *neko.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/neko 	&& tar -xC /usr/src/neko --strip-components=1 -f neko.tar.gz 	&& rm neko.tar.gz 	&& cd /usr/src/neko 	&& cmake -DRELOCATABLE=OFF . 	&& make 	&& make install 		&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/neko ~/.cache
# Thu, 18 Nov 2021 01:13:46 GMT
ENV HAXE_VERSION=4.2.4
# Thu, 18 Nov 2021 01:13:47 GMT
ENV HAXE_STD_PATH=/usr/local/share/haxe/std
# Thu, 18 Nov 2021 01:18:43 GMT
RUN set -ex 	&& buildDeps=' 		make 		ocaml-nox 		ocaml-native-compilers 		camlp4 		ocaml-findlib 		zlib1g-dev 		libpcre3-dev 		libmbedtls-dev 		libxml-light-ocaml-dev 				opam 		mccs 		m4 		unzip 		pkg-config 		libstring-shellquote-perl 		libipc-system-simple-perl 			' 	&& git clone --recursive --depth 1 --branch 4.2.4 "https://github.com/HaxeFoundation/haxe.git" /usr/src/haxe 	&& cd /usr/src/haxe 	&& mkdir -p $HAXE_STD_PATH 	&& cp -r std/* $HAXE_STD_PATH 	&& apt-get update && apt-get install -y $buildDeps --no-install-recommends 			&& opam init --disable-sandboxing 	&& eval `opam env` 		&& ( [ -f /usr/src/haxe/opam ] && opam install /usr/src/haxe --deps-only --yes || make opam_install ) 		&& make all tools 	&& mkdir -p /usr/local/bin 	&& cp haxe haxelib /usr/local/bin 	&& mkdir -p /haxelib 	&& cd / && haxelib setup /haxelib 			&& eval `opam env --revert` 	&& rm -rf ~/.opam 		&& rm -rf /var/lib/apt/lists/* 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/haxe ~/.cache
# Thu, 18 Nov 2021 01:18:44 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:626979e62c56e192812e818d52b82f063d9f9514b1b7bae14e534e4a7c98117a`  
		Last Modified: Wed, 17 Nov 2021 02:47:40 GMT  
		Size: 49.2 MB (49222990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:134a528370d5dcbf5b6ba2d8c20f576504448e8f2d1debb5d2a4950a38a3ff2d`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 7.7 MB (7695161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e12e3364b52ad043d8e79f750863ed4ca2878c4fdf45ded974508febc55fdd`  
		Last Modified: Wed, 17 Nov 2021 13:37:44 GMT  
		Size: 9.8 MB (9767133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7f2500f9574b0a495bfb031c2d52e83c96dd545ef2185737f8032567e70677`  
		Last Modified: Wed, 17 Nov 2021 13:38:03 GMT  
		Size: 52.2 MB (52165947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d4367ac3437ffe53a2e6ab8ad116fd0e365d3d736d7af4f35cabd8d58fc1d5`  
		Last Modified: Thu, 18 Nov 2021 01:52:07 GMT  
		Size: 1.1 MB (1083697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa9c50f769517306ca7b65909dbcdd6b367a7f4fab37ba5773c427561936574`  
		Last Modified: Thu, 18 Nov 2021 01:52:08 GMT  
		Size: 2.3 MB (2282173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c1b4222242ea402329b9747893f1bd0e60715729cf457e79de22e817490f00`  
		Last Modified: Thu, 18 Nov 2021 01:52:10 GMT  
		Size: 11.9 MB (11868495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.17763.2300; amd64

```console
$ docker pull haxe@sha256:31509b118b421181dfd4441662326a44c3ccc5c42afb5ff4dd8b2abae05428c6
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2732659930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:da39d5477e667264780e8385aecfb986d1592684e2aef9c8d056b4bdcb68b8b5`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 04 Nov 2021 00:30:48 GMT
RUN Install update 1809-amd64
# Wed, 10 Nov 2021 14:18:57 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 14:18:58 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Nov 2021 14:18:58 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Nov 2021 14:18:59 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Nov 2021 14:19:00 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Nov 2021 14:19:01 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Nov 2021 14:20:12 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Nov 2021 14:21:58 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:22:51 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Nov 2021 14:22:52 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Nov 2021 14:23:59 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:24:00 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 10 Nov 2021 14:28:29 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:29:24 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 10 Nov 2021 14:29:25 GMT
ENV HOMEDRIVE=C:
# Wed, 10 Nov 2021 14:30:17 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Nov 2021 14:31:13 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 10 Nov 2021 14:32:13 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 10 Nov 2021 14:32:14 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c1f4c7287c99b95fce227924349d1d139aceb37d97b555144bd5808935b6eab0`  
		Size: 987.8 MB (987788268 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:db1ba835bccbdc73ef254c175ca6ae0dc3f0bd759c1910c3b123cfb9613223be`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ec0f7cb9a95320c537b66172a48669256f28a3a276cedf5193b52e32a07f7dd`  
		Last Modified: Wed, 10 Nov 2021 16:21:11 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6400f955f12e1aa81d99bb12139c641f5d55104411333abf10815642b14c0e2`  
		Last Modified: Wed, 10 Nov 2021 16:21:10 GMT  
		Size: 1.4 KB (1401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9d7feed04629fd5dd8a2db4715f6fd1783e7da241f56ba22ebb04d864cabf0c`  
		Last Modified: Wed, 10 Nov 2021 16:21:09 GMT  
		Size: 1.4 KB (1410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7b12c526c089573fbd57f79a981f209e966de8d6405f8bebb06120b591f8b0`  
		Last Modified: Wed, 10 Nov 2021 16:21:08 GMT  
		Size: 1.4 KB (1439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0d9c9b4069800c59110e297b13ace1e33c036c0ebf66dcb07c7cc252a27f29a`  
		Last Modified: Wed, 10 Nov 2021 16:21:07 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4e8d0c5ea54689e83e7720dbe56f3b076e21fb758ceab186346c103894ce579`  
		Last Modified: Wed, 10 Nov 2021 16:21:07 GMT  
		Size: 356.8 KB (356848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393b02a2537b5ea48207461aeadf650ee974dd4abd3d275bcd00269a72ce59e3`  
		Last Modified: Wed, 10 Nov 2021 16:21:09 GMT  
		Size: 12.9 MB (12936560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd6932b42d6788129c8ca83e7dea7295fcf6ca4f5f0e5d8f8002dfc2ab9b5cb`  
		Last Modified: Wed, 10 Nov 2021 16:21:06 GMT  
		Size: 329.8 KB (329771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad63c2581c81a71d51e690ded03d98b58bfb15fb7c713e8c589234447fbd22a1`  
		Last Modified: Wed, 10 Nov 2021 16:21:04 GMT  
		Size: 1.4 KB (1378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dbfe77a7a0afc027c2e9f6f01a7977d5ccdc4f39a6856e11c8e648120e03846`  
		Last Modified: Wed, 10 Nov 2021 16:21:05 GMT  
		Size: 2.2 MB (2162767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e15184ed061a3c64eab296790f0fe6cb68f9cf37338e32d69ae36cad9a76b4d`  
		Last Modified: Wed, 10 Nov 2021 16:21:04 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea8c1941cd253d773ab4fbb01c09aeb608ef9826cde9a406420b5ae0a43a25eb`  
		Last Modified: Wed, 10 Nov 2021 16:21:09 GMT  
		Size: 9.2 MB (9233066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae1dbba3ea24580bacb4261779bac44976cd8bc07660cd099dbafa872648380`  
		Last Modified: Wed, 10 Nov 2021 16:21:03 GMT  
		Size: 354.0 KB (353990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18893ab05f1293a027097d18bcb4e72d87fcbca01629acf62aaa0ef379182b2`  
		Last Modified: Wed, 10 Nov 2021 16:21:01 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea97bc8536bb4d8946de3349271eca11028e97013e7135cfbc70fd057428405`  
		Last Modified: Wed, 10 Nov 2021 16:21:01 GMT  
		Size: 367.1 KB (367134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce8b0b92f8ab95f59ba8db13145cdad4c7491953544b6720b3924d781fc91f3`  
		Last Modified: Wed, 10 Nov 2021 16:21:02 GMT  
		Size: 384.2 KB (384228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf50baf104a6d7a8e17150d04918ce21e09a3fcaf60733603fb5b1be2d1aea5`  
		Last Modified: Wed, 10 Nov 2021 16:21:02 GMT  
		Size: 400.2 KB (400239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f57dbafef2821c78a5198ecceb7153ede5c7a24628f7e2eabb384100f4fab361`  
		Last Modified: Wed, 10 Nov 2021 16:21:01 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haxe:latest` - windows version 10.0.14393.4770; amd64

```console
$ docker pull haxe@sha256:0db75716a5c5a50f9560165c619935b0443278dc52d60e11517709dbd57afac5
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6308369909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c1609d7e8b3786e26c1c2b880bd6ad78b70cc0d0116f777d16a7aa4da040a6a5`
-	Default Command: `["haxe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Nov 2021 23:35:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Nov 2021 14:32:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop';]
# Wed, 10 Nov 2021 14:32:28 GMT
ENV HAXETOOLKIT_PATH=C:\HaxeToolkit
# Wed, 10 Nov 2021 14:32:29 GMT
ENV NEKOPATH=C:\HaxeToolkit\neko
# Wed, 10 Nov 2021 14:32:29 GMT
ENV HAXEPATH=C:\HaxeToolkit\haxe
# Wed, 10 Nov 2021 14:32:30 GMT
ENV HAXE_STD_PATH=C:\HaxeToolkit\haxe\std
# Wed, 10 Nov 2021 14:32:31 GMT
ENV HAXELIB_PATH=C:\HaxeToolkit\haxe\lib
# Wed, 10 Nov 2021 14:33:38 GMT
RUN $newPath = ('{0};{1};{2}' -f $env:HAXEPATH, $env:NEKOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Nov 2021 14:35:20 GMT
RUN $url = 'https://download.microsoft.com/download/0/5/6/056dcda9-d667-4e27-8001-8a0c6971d6b1/vcredist_x86.exe'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'vcredist_x86.exe'; 		Write-Host 'Verifying sha256 (89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17) ...'; 	if ((Get-FileHash vcredist_x86.exe -Algorithm sha256).Hash -ne '89f4e593ea5541d1c53f983923124f9fd061a1c0c967339109e375c661573c17') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Installing ...'; 	Start-Process -FilePath "vcredist_x86.exe" -ArgumentList "/Q" -Wait; 		Write-Host 'Removing installer...'; 	Remove-Item .\vcredist_x86.exe; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:36:16 GMT
RUN New-Item -ItemType directory -Path $env:HAXETOOLKIT_PATH;
# Wed, 10 Nov 2021 14:36:17 GMT
ENV NEKO_VERSION=2.3.0
# Wed, 10 Nov 2021 14:37:28 GMT
RUN $url = 'https://github.com/HaxeFoundation/neko/releases/download/v2-3-0/neko-2.3.0-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'neko.zip'; 		Write-Host 'Verifying sha256 (d09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b) ...'; 	if ((Get-FileHash neko.zip -Algorithm sha256).Hash -ne 'd09fdf362cd2e3274f6c8528be7211663260c3a5323ce893b7637c2818995f0b') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path neko.zip -DestinationPath tmp; 	if (Test-Path tmp\neko.exe) { Move-Item tmp $env:NEKOPATH } 	else { Move-Item (Resolve-Path tmp\neko* | Select -ExpandProperty Path) $env:NEKOPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path neko.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  neko -version'; neko -version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:37:29 GMT
ENV HAXE_VERSION=4.2.4
# Wed, 10 Nov 2021 14:41:57 GMT
RUN $url = 'https://github.com/HaxeFoundation/haxe/releases/download/4.2.4/haxe-4.2.4-win64.zip'; 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile haxe.zip; 		Write-Host 'Verifying sha256 (cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a) ...'; 	if ((Get-FileHash haxe.zip -Algorithm sha256).Hash -ne 'cdbcec5fee9178a307e6bcbb436f8ff124dd2c18f86ad51e3d0a7a4ef489877a') { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType directory -Path tmp; 	Expand-Archive -Path haxe.zip -DestinationPath tmp; 	if (Test-Path tmp\haxe.exe) { Move-Item tmp $env:HAXEPATH } 	else { Move-Item (Resolve-Path tmp\haxe* | Select -ExpandProperty Path) $env:HAXEPATH }; 		Write-Host 'Removing ...'; 	Remove-Item -Path haxe.zip, tmp -Force -Recurse -ErrorAction Ignore; 		Write-Host 'Verifying install ...'; 	Write-Host '  haxe -version'; haxe -version; 	Write-Host '  haxelib version'; haxelib version; 		Write-Host 'Complete.';
# Wed, 10 Nov 2021 14:43:02 GMT
RUN New-Item -ItemType directory -Path $env:HAXELIB_PATH;
# Wed, 10 Nov 2021 14:43:03 GMT
ENV HOMEDRIVE=C:
# Wed, 10 Nov 2021 14:44:00 GMT
RUN $newPath = ('{0}\Users\{1}' -f $env:HOMEDRIVE, $env:USERNAME); 	Write-Host ('Updating HOMEPATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('HOMEPATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Nov 2021 14:45:01 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://lib.haxe.org') >$null
# Wed, 10 Nov 2021 14:45:52 GMT
RUN (New-Object System.Net.WebClient).DownloadString('https://d1smpvufia21az.cloudfront.net') >$null
# Wed, 10 Nov 2021 14:45:53 GMT
CMD ["haxe"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b07c368b7a04669b63c6c86a881be270ee967474a85892003b8695df3d0d5874`  
		Size: 2.2 GB (2203104946 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f6f303e73635c7923a8c64f8938e7ba4c10210fd15a6ce63aa8a62d5a8ea8c0a`  
		Last Modified: Wed, 10 Nov 2021 16:21:33 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb1d3b976835ae12ec5e1e78df14f1a6366e1887fe56fb379a02438246ca51f`  
		Last Modified: Wed, 10 Nov 2021 16:21:32 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dc0f016722c0d1b4035762134efe8bc017310cf747f4f4af5094cab96f42188`  
		Last Modified: Wed, 10 Nov 2021 16:21:31 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8950a68b6b039e2b7903837874763834e30ecc896a0fa081ee7a3370fe18c4`  
		Last Modified: Wed, 10 Nov 2021 16:21:30 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be5f8f3b7b965123535da75d102670b9d5905c56d00f7d43ed9f6039208c99ac`  
		Last Modified: Wed, 10 Nov 2021 16:21:30 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ebc57d9cea4e5bc66a911692e9d6b9deaa7d9297b15fd204d2b5309e47b7c47`  
		Last Modified: Wed, 10 Nov 2021 16:21:28 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56b1a06ea244a6eafd1368569ef69b97b079a99e1a67462a75452c5c43fb3f4`  
		Last Modified: Wed, 10 Nov 2021 16:21:28 GMT  
		Size: 353.9 KB (353918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d91bb5f80b569a2efc463d3e2319df79b3eb1292b3a16211bac96c878d9a7fa`  
		Last Modified: Wed, 10 Nov 2021 16:21:31 GMT  
		Size: 17.4 MB (17420837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3afe958868f8e1e478c3e908a6a392589b084e2d8b4cfa183b39992226a6101`  
		Last Modified: Wed, 10 Nov 2021 16:21:27 GMT  
		Size: 309.4 KB (309444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7ebf1192d3e4f1cb0c9903cf2d8a9264b7fed0fac5cefc5351886f49a3e8b43`  
		Last Modified: Wed, 10 Nov 2021 16:21:24 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:107ff47542ccf30a2ec5806f3c54908e7f6c2c166b0cf8d19dfb5240e9f0f744`  
		Last Modified: Wed, 10 Nov 2021 16:21:25 GMT  
		Size: 2.1 MB (2132490 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4efca240d62d9f63c718bb98ba89828b4d4ccd8ad422383f5f875b5a1a2a282`  
		Last Modified: Wed, 10 Nov 2021 16:21:24 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489a3cd90e9bd4169c73da2828b8615cd49889e875b3fdd9446d64656d094f34`  
		Last Modified: Wed, 10 Nov 2021 16:21:41 GMT  
		Size: 13.7 MB (13736939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f8e3653695a8c5f31342c2c21068c25f1d41ff3e69f0621b5979d8e4e0fb39`  
		Last Modified: Wed, 10 Nov 2021 16:21:24 GMT  
		Size: 325.0 KB (324976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57e4f4b4fc1f22e94f91e0f53c0abf8467de4d8bedb92e961edd6eb2b0ce966`  
		Last Modified: Wed, 10 Nov 2021 16:21:21 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bf0715ef9907ca1dda108be4f59563d65b8aa5e144d3227c5bbc77ef7765beb`  
		Last Modified: Wed, 10 Nov 2021 16:21:22 GMT  
		Size: 324.9 KB (324889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cfaa6ac84f7a0e1fd603c3b3792ac3a4e9051f0acc9eb195d13a1de2c83e9f`  
		Last Modified: Wed, 10 Nov 2021 16:21:22 GMT  
		Size: 329.9 KB (329922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3434533bcee1b3c9b8258fa69acb52329ea47b14ebcdaf5ca1c1519ebfc4d6df`  
		Last Modified: Wed, 10 Nov 2021 16:21:22 GMT  
		Size: 331.6 KB (331565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693e3e294a1e15a790f6f16efd0c4c1a885a567f1f600dd922bc3b6e48262b18`  
		Last Modified: Wed, 10 Nov 2021 16:21:21 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
