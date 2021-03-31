## `buildpack-deps:stretch`

```console
$ docker pull buildpack-deps@sha256:a9f3300e00f8b50089176ffb2b380363756efc5bad00f239f37e83e082f3873b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:stretch` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:c0b695cb7c0817242d0f7b009bb0aa70bea854570c2c81d15b3d2181e3dcd282
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.1 MB (325143595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61ab8d66bf0acd98cdcbec759a96cca57139298291bb3d3a02cf760629009f1a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:43 GMT
ADD file:e52290391b221e1a4e52cf4e41ffe7e14f162475964fa01638e03b3ead673ba1 in / 
# Tue, 30 Mar 2021 21:50:43 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:08:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:08:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:08:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:10:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:00168f89dbe8f3c9985e536784c27517f6cc35ea56263469449a6b73e0bed595`  
		Last Modified: Tue, 30 Mar 2021 21:56:37 GMT  
		Size: 45.4 MB (45379949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da61ad49fa9961d6dfe53dc067fd690133f205498e8045e8f7ef6b9da0d42bd2`  
		Last Modified: Tue, 30 Mar 2021 23:17:25 GMT  
		Size: 11.3 MB (11286658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af62e04c0f85ed10801df4314d8cb9ba5e6c391f6a3c1db1080a0a78c8d4ed9d`  
		Last Modified: Tue, 30 Mar 2021 23:17:23 GMT  
		Size: 4.3 MB (4342466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae835e2c68ef1d48a4ffef72547a79926019aec6a2bbeb5372f1e832ef453dd`  
		Last Modified: Tue, 30 Mar 2021 23:17:49 GMT  
		Size: 49.8 MB (49787075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5254dc317968c943c4321cdbf0364a6a47c833296b3f45e3bd27aa4efe28c865`  
		Last Modified: Tue, 30 Mar 2021 23:18:46 GMT  
		Size: 214.3 MB (214347447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:128868c2ed5b61059bb19bb59130916576a835be86d2ddc8cff32874f6931bde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.1 MB (309086469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b8ddc4f0e984b0c949ce11ee1d9f19eee25b8b97888ed7ff537c89b0f8d9735`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:53:43 GMT
ADD file:471d7a5419df3b812f9a1b0b14c1bfbc2b8fc88652b66cca395a28af61a77f4d in / 
# Tue, 30 Mar 2021 21:53:46 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:55:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:55:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:56:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:58:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a6404a8305ff6dab0e0a06c0c4291401369422bb5ba3e2b49d5447049a0928d7`  
		Last Modified: Tue, 30 Mar 2021 22:01:23 GMT  
		Size: 44.1 MB (44091975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0455c93c80b72e9e001eb0738f044aaf49d57cdee5c4621e362ecc2ceebd6ae3`  
		Last Modified: Wed, 31 Mar 2021 00:04:47 GMT  
		Size: 10.3 MB (10333990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3d70057a6c48834905e9f7b2f91c1c66f824e2665b9704c701c726bdbf572e`  
		Last Modified: Wed, 31 Mar 2021 00:04:42 GMT  
		Size: 4.2 MB (4161473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db4f5b94a18ebcb6b470aa3e8c715877970ee1cae520160603b88c5ed2b2988`  
		Last Modified: Wed, 31 Mar 2021 00:05:15 GMT  
		Size: 48.0 MB (47987617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80964130527536accae4a88a42e55b537bf28d09becf5b5ade65e579083f10d`  
		Last Modified: Wed, 31 Mar 2021 00:06:22 GMT  
		Size: 202.5 MB (202511414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:67ec18126a8bfe5c681e7e591f1117e3ad6ab4894c83d50bcc7d4c40aa5e8117
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.1 MB (297116180 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:663566cd7246cafd6172bcc18b6ba21d6b40cb30c93eab322998ccb0588925de`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:22:16 GMT
ADD file:9ca2a8d5e2b8ba00bb66699e4970399555c20e8f9a4b8afa0b01076b90f0d8e3 in / 
# Fri, 26 Mar 2021 11:22:19 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:31:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:31:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:32:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:35:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:011348b3c4acf7cfad3a8899e3a5f135377a30045eb428e4d759ef7e138740b1`  
		Last Modified: Fri, 26 Mar 2021 11:31:14 GMT  
		Size: 42.1 MB (42119842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87cf4418db1e976b0b84122d61cab9eb3bf7616e363a557275308ca2ccc72365`  
		Last Modified: Fri, 26 Mar 2021 13:55:29 GMT  
		Size: 9.9 MB (9939755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdfe21b354ae04ba513e56799a77ae6f0f57339ee9fec76a66d4e7aaffda99e4`  
		Last Modified: Fri, 26 Mar 2021 13:55:25 GMT  
		Size: 3.9 MB (3921260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:017f4a3c6ff8566959485607b47c6d4748a4e04e25a1b7d98c2e289c887074c9`  
		Last Modified: Fri, 26 Mar 2021 13:55:55 GMT  
		Size: 46.1 MB (46127623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edeb8d7f60b74a9ac7740d9b526df80c4938e293c8acef68f20d20b1d4e6b2d`  
		Last Modified: Fri, 26 Mar 2021 13:57:09 GMT  
		Size: 195.0 MB (195007700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:5e8a7760813980d9bd7dd462d5a88ed9eca3c3d628d7358f8e475c896f799dbc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.9 MB (306930328 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40d57f62eb6580e7d1f33c0f166bd18b494a6a3e286790ad15238a8b2a1808ac`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:45 GMT
ADD file:0546f28e5d1be54699d1e0756275203da731735b3212f2ff1a87cd7f8dcc9049 in / 
# Tue, 30 Mar 2021 21:49:50 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:22:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:23:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:25:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9317dc7ea567b49ade0ea730b5530d1363b065549e8b75a198e0b60bdde1f1d7`  
		Last Modified: Tue, 30 Mar 2021 21:56:46 GMT  
		Size: 43.2 MB (43177588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eaf1b7b1bdfdc23af33da7d1fc9670524e63a8408bb04de9aebdf95979c5635`  
		Last Modified: Wed, 31 Mar 2021 00:33:12 GMT  
		Size: 10.2 MB (10201033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4446041554682b465ef9a0e853a5067e7d794fa1c840946d140beab2ddeb51`  
		Last Modified: Wed, 31 Mar 2021 00:33:09 GMT  
		Size: 4.1 MB (4096741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0b477e68dd7171c7df2dfc66cd994be553e0679dd5c2083048d10d5a29363a`  
		Last Modified: Wed, 31 Mar 2021 00:33:40 GMT  
		Size: 47.7 MB (47735121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8e162dfd38e34eeb2178da6fcb11b12f16ffa8bd96bbd6f0207dd5eceb7732`  
		Last Modified: Wed, 31 Mar 2021 00:34:37 GMT  
		Size: 201.7 MB (201719845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:stretch` - linux; 386

```console
$ docker pull buildpack-deps@sha256:75fcb90673c490a5d7d5634f3da582b5189873f594c2e48a05160a33780cb620
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332686024 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:982289d06cddd1bdb66ac2295b3e612cb966652f5f6c56fe39f7e4dc963f1bc7`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:41:30 GMT
ADD file:1df7a35a36c49061902cf634a894b34a55a9c020976547cf6d2dda96879854bc in / 
# Tue, 30 Mar 2021 21:41:30 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:01:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:01:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:03:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:667bc6614d317ea77075a4e2f4ee7ef7d7b696f50d426cec38048d3ca20f1aa1`  
		Last Modified: Tue, 30 Mar 2021 21:49:28 GMT  
		Size: 46.1 MB (46098556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51d5e0a8886ebed26c676639259bf05d50ff3b0285ea4b8afd1492ea424e7ff`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 11.3 MB (11336592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76cd0bba69d5c567fef7e770351f3ae71bdff83884b1d5af86d4dcd6ea6ff7a9`  
		Last Modified: Wed, 31 Mar 2021 00:11:48 GMT  
		Size: 4.6 MB (4564997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a10652cecac951d9def7d54e1fc469edee3b96dde5d603ef1275742ca7280b`  
		Last Modified: Wed, 31 Mar 2021 00:12:18 GMT  
		Size: 51.3 MB (51264835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5389fa48199130b88a8599594d5da3ddcba8df363150af0bec5248364e36d62`  
		Last Modified: Wed, 31 Mar 2021 00:13:29 GMT  
		Size: 219.4 MB (219421044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
