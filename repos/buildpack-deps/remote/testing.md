## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:262ae78dc56067f1ffc2ff4d5aab05a23ab8306dc45ea03a16efa71d25a4417b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:9fab1092dd6c638eae643898d118ea881a65d5775ac30bef0a1d95f31cf99abd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321831838 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e72ff1f31a17f6443e72f857e2faab189bb54123c83a091a5262e9a61406cfd`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:04 GMT
ADD file:a858c472d72a55a1ed0b7b2fd2751bac78f77e3549a7533c508022aef7204233 in / 
# Fri, 12 Mar 2021 02:20:04 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:47:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:48:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:48:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:13 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da21a291c553cde4f403910fa28fb69cad95f63ce1b378f341eb17738b45a6ac`  
		Last Modified: Fri, 12 Mar 2021 02:24:58 GMT  
		Size: 54.8 MB (54835833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f47dd55341835080544d848892987ce23838db35fe64a0d4338b1494ad6ed1c`  
		Last Modified: Fri, 12 Mar 2021 03:17:40 GMT  
		Size: 5.1 MB (5136253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb0644d825d57df2b92d247999a507695a22522c5fa2bd93de229b003ea515b`  
		Last Modified: Fri, 12 Mar 2021 03:17:40 GMT  
		Size: 10.9 MB (10860722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bb105cb94d3a12e9d1648ac4750f9b7b3f837fc623dff8a5676d1892f8ea7b`  
		Last Modified: Fri, 12 Mar 2021 03:18:07 GMT  
		Size: 54.6 MB (54573567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675c3488479ed98ce102d2010e80208c24e0536cae45d14b1c555b97d2a10269`  
		Last Modified: Fri, 12 Mar 2021 03:18:56 GMT  
		Size: 196.4 MB (196425463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c263f479d38f94e1dc00335b349d309ea1481460fc1bfbb685b3f9c6710d277b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.9 MB (294912138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f53682a61e604eaa55085c85a65580671cd1205ceb7ccaa1fde04bda8d536aa`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:50:33 GMT
ADD file:1b779b19b47bb1848292d2bf671b599eb9041626b747d8016817e0c7d46ff881 in / 
# Fri, 26 Mar 2021 07:50:38 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:04:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:05:07 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 09:06:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:09:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8d862331f8860c127d174052922618c93a166777e5b776e8b08e87702af28cd`  
		Last Modified: Fri, 26 Mar 2021 07:59:08 GMT  
		Size: 52.4 MB (52404525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc6864d5c0a91a133802b130cddb5c9fb77329c250e4f5d77c05e96188cbcb31`  
		Last Modified: Fri, 26 Mar 2021 09:25:47 GMT  
		Size: 5.1 MB (5060013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a0cf03c5e0e5a428fa3a5789c4793210e762dbfb24e1f688a878754fe9ada6`  
		Last Modified: Fri, 26 Mar 2021 09:25:48 GMT  
		Size: 10.6 MB (10569895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1985045f60a052a5d3b4e89129ae9f03ece21620c4b057aa105c0c78cc5775a4`  
		Last Modified: Fri, 26 Mar 2021 09:26:11 GMT  
		Size: 52.3 MB (52314372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6846d74db7fd55b80f3ec7ee2ac5146b6ab9455ce7043c5022f74119885c0a7`  
		Last Modified: Fri, 26 Mar 2021 09:27:26 GMT  
		Size: 174.6 MB (174563333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b925618eebef2c94b576c7b99baac9705ffec6771cb5b50d7b1a83d32735764e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **282.4 MB (282375933 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e13dad972720ac53a49695be1954fe83c267551e5aec0104ce5f648f9d849572`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:15:27 GMT
ADD file:e3651409d9338da981cd9fbd8d9b8511edbde0700ac9e0df8937b859e004990d in / 
# Fri, 26 Mar 2021 11:15:29 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:16:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:16:48 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:17:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:21:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd9021b04def024e25507cdd1b0967a20a384ad5cc255120cfb8c5f43495fa74`  
		Last Modified: Fri, 26 Mar 2021 11:26:11 GMT  
		Size: 50.1 MB (50073977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c6023b28762fcb2cca84dd988c0545da69e2cb9cea40e5fb1a14dce3d7d186`  
		Last Modified: Fri, 26 Mar 2021 13:48:58 GMT  
		Size: 4.9 MB (4920097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94408c405dc2689a60515a2dee289cb3495f53f4b4f9758de6995e07aa073eb2`  
		Last Modified: Fri, 26 Mar 2021 13:48:59 GMT  
		Size: 10.2 MB (10218160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd339501262a81addad6326243dbcf62ca43943542cc42a3b06aeda9a9cdec3a`  
		Last Modified: Fri, 26 Mar 2021 13:49:44 GMT  
		Size: 50.3 MB (50328166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c0e2093ca7e218efcd720cb76df84159a60199e33e382d88d4f9fe16a24f4b`  
		Last Modified: Fri, 26 Mar 2021 13:51:04 GMT  
		Size: 166.8 MB (166835533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:76ee27761779d194ec609dab05a9164abce4cda75326622c7bd546f9a9fc49f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.4 MB (313447854 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5edb6823487cf216272dc601657b98090a8265d50bc201770094919384b61a03`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:52:22 GMT
ADD file:0b6f3c6d396337f2754d539814c02240e0a459436f4c0992dabf1736069b5a51 in / 
# Fri, 12 Mar 2021 01:52:29 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:26:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:26:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:27:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:28:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c214bbe001dfa953738440417693c3487f97b371a108bdd62425a704347faf8`  
		Last Modified: Fri, 12 Mar 2021 02:00:33 GMT  
		Size: 53.5 MB (53521132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1332f0d3a2e68785b75d30a2f0eeb7e0902ecf1068899b78d4a7e90f5201cf7f`  
		Last Modified: Fri, 12 Mar 2021 02:42:02 GMT  
		Size: 5.1 MB (5125702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70aaac2a7c6ebfc86100e530f2607998a0f8d84b4305495031bbfe789e6e1c2d`  
		Last Modified: Fri, 12 Mar 2021 02:42:03 GMT  
		Size: 10.9 MB (10860189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c201b24dcdc8bd225ab1c164d5ff733c78eb97a701f50d2841449244aa6b43`  
		Last Modified: Fri, 12 Mar 2021 02:42:31 GMT  
		Size: 54.7 MB (54675060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89dfecfc0f3ea79ccc220c0a07813a3ab3915b2451535f378adfca5216aaac`  
		Last Modified: Fri, 12 Mar 2021 02:43:21 GMT  
		Size: 189.3 MB (189265771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:d3e134fc44e6eb7dce5c1e0912de5ba1f155fd7ce0a19d4d3adba4840ba5b6b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.6 MB (327608306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7215762e97e201bf4320d7621b85e29b8ea2b3e7fb55036ee22711294f19e649`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 13:52:22 GMT
ADD file:a351d1298a5051f829e330b747943dba9a67cc050d1f23f62be062f669830e9a in / 
# Fri, 26 Mar 2021 13:52:23 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 22:41:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:41:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 22:41:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:43:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fb6fc5804fde9f18c538230f43ec9b5dc9c2466d8fc49f7510911c12de70d991`  
		Last Modified: Fri, 26 Mar 2021 14:00:05 GMT  
		Size: 55.9 MB (55881460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47770a32ee01d7a5a9ea596d431299fafb3e5ec55cda781b4b8ba77139d3b742`  
		Last Modified: Fri, 26 Mar 2021 22:54:02 GMT  
		Size: 5.3 MB (5278994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b619575768f273ceeaf065659966267b58a5378b4b7d52fdcd0648e68b378227`  
		Last Modified: Fri, 26 Mar 2021 22:54:03 GMT  
		Size: 11.2 MB (11248822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce028724865c02e9ace59fe70b5f2ea0c85782a125e91d44e337fc658f84434`  
		Last Modified: Fri, 26 Mar 2021 22:54:36 GMT  
		Size: 55.9 MB (55908864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8fe739fa5fbd5d9a2af56021580582caece781a4d582b5e71a634239d3c8ff`  
		Last Modified: Fri, 26 Mar 2021 22:55:46 GMT  
		Size: 199.3 MB (199290166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:382bf2c7d5526ee89962dd4f194fe82e6c0530423ebbda1b92e4f6d8e5e96b1e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.2 MB (301219509 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7945a4b748a783e99cfa7667a05807967db328fd4eac631bf5cdfec7e69dc6fc`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:08:46 GMT
ADD file:7e11d2e31071a03f4f43a78cd6af64c7034e2267c839bee84afd1e3bb9916f3e in / 
# Fri, 26 Mar 2021 08:08:47 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:13:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:13:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 18:15:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:18:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e3b00636426049a0189d8511a90dd5801df2b5793acbaa564ad20c57c4ff115`  
		Last Modified: Fri, 26 Mar 2021 08:14:22 GMT  
		Size: 53.1 MB (53128793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c11a8343730b68d55c2c17295713c1932bfdeed6cd26ba010cb68214e4f5638`  
		Last Modified: Fri, 26 Mar 2021 18:27:18 GMT  
		Size: 5.1 MB (5112340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503e0f155ade594fd8b18a219ba3f1174ed82e7465c9b852325d8a8a11c870d2`  
		Last Modified: Fri, 26 Mar 2021 18:27:20 GMT  
		Size: 10.9 MB (10870299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5514c276e4dbcbce3dce646bff262cc3c13a68791d15a0585f7a759615c558f`  
		Last Modified: Fri, 26 Mar 2021 18:28:10 GMT  
		Size: 53.3 MB (53299474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ecd84659d1805f9cffa4323fffe456902cf887b01d12696bf67a27c7b98042`  
		Last Modified: Fri, 26 Mar 2021 18:30:20 GMT  
		Size: 178.8 MB (178808603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:05c5ff1d2d777d6b0e8c6140f4328068a61ec87356bf286bc27241def238e093
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **330.3 MB (330278898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc5edc32d331387d4e24476fb2dbd22b3c2b76bd3eb021ac8062174df50a6b74`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:12:40 GMT
ADD file:28f7d129aaacc2de6bb78dec104b788d0aa25aaac87e07873668354a5b755268 in / 
# Fri, 26 Mar 2021 15:12:49 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:11:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:13:05 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 17:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:34:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:18ddfb418fe2dc2d92f9b851d0345827010c7b001ef98bb5a8b1730d80e2eace`  
		Last Modified: Fri, 26 Mar 2021 15:20:35 GMT  
		Size: 58.8 MB (58756702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e58f4581a73db06180cd5d10d619dc8b47cdbf57bed71dbf9eb53d28bc4749`  
		Last Modified: Fri, 26 Mar 2021 19:34:46 GMT  
		Size: 5.4 MB (5399177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55e302f47f5e7c563d0f23745e32bd160587a44a206808295a2ca9d29a6b9d67`  
		Last Modified: Fri, 26 Mar 2021 19:34:51 GMT  
		Size: 11.6 MB (11619666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da9f221c0a34707baac4ad94f19a4bd62b803303c74a200e7d8ced228745c108`  
		Last Modified: Fri, 26 Mar 2021 19:36:24 GMT  
		Size: 58.8 MB (58846493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:309330cad3618c41f1fcedf5b26c33744337ec55b741feddf35bda0d56d9e50c`  
		Last Modified: Fri, 26 Mar 2021 19:40:05 GMT  
		Size: 195.7 MB (195656860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:dabf36507076a0d91e62d0525634f1c9d50fdd355092b12bc441d9f1ca1be056
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.4 MB (295444580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:007d9ede8cf23c52f61396bbb6aed51b515a0fd85d5cc5ab7a8358c1500e7a47`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 10:52:51 GMT
ADD file:6dd7d4b323fd63c8ee8a655a79017b62cdad999e420310b15e9568404d02e856 in / 
# Fri, 26 Mar 2021 10:52:58 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 15:39:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:39:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 15:40:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:43:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7fcb7355b5dda69e2044a1c24be0597b43954f9d3183dde70ac38aac25df7adb`  
		Last Modified: Fri, 26 Mar 2021 10:56:55 GMT  
		Size: 53.1 MB (53147819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4483fa86d703794bc974862181191f13737481044629eefcee195f179e335064`  
		Last Modified: Fri, 26 Mar 2021 15:53:59 GMT  
		Size: 5.1 MB (5134107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e227b0ad592b8d4f1e74bc91d5c854ab0a75abf65452545c61ce392a04f489f5`  
		Last Modified: Fri, 26 Mar 2021 15:54:00 GMT  
		Size: 10.8 MB (10758559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907d7501cb26d3573f807160ae0b0b98d3c254793f034d9f3356af99600645d`  
		Last Modified: Fri, 26 Mar 2021 15:54:24 GMT  
		Size: 54.0 MB (54038949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad24675826b6407d56d20cfddd78c9328ba57bc6264dafda50c9ed0286295dd`  
		Last Modified: Fri, 26 Mar 2021 15:54:54 GMT  
		Size: 172.4 MB (172365146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
