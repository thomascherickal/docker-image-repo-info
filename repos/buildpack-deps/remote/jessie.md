## `buildpack-deps:jessie`

```console
$ docker pull buildpack-deps@sha256:e719fdb541ff37e89a44c9d0d2a49513fffff3a576bff076365162cef916b6f7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:jessie` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:76a7fdd5cecbdc9e015734d6999fbe8259822fba5ca96bcc57b58a9872159628
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247172715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9ff0df3f474b032ecc85b28f93f3375b0b73ef1ff0a2f7c7b72541b9542cc3a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:21:09 GMT
ADD file:0419e8fcec7ce7e70dc1f1e19558f15ebcd61d43a3b9955811783ac3a56c79ac in / 
# Tue, 09 Jun 2020 01:21:10 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:49:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:49:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:51:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:54:18 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0cd7281e66ed488ba431fd1e41a3c5fd628ed921f059ddbba2597487962ab380`  
		Last Modified: Tue, 09 Jun 2020 01:26:04 GMT  
		Size: 54.4 MB (54388052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041e5427efd77699a148fcef4a48824bba787ed6c2db375aa3f3d8b97ac92ad6`  
		Last Modified: Tue, 09 Jun 2020 02:00:55 GMT  
		Size: 17.5 MB (17545709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43cd1bce0fad2e8c8c996f62251321b38f07c985eec3022deb89a6d9d2d33932`  
		Last Modified: Tue, 09 Jun 2020 02:01:08 GMT  
		Size: 43.3 MB (43334949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c37abb5d843525117fda6fcac42341739f63ff40dd7f7e97d3ea4ed3734b9c8`  
		Last Modified: Tue, 09 Jun 2020 02:01:32 GMT  
		Size: 131.9 MB (131904005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:2b7cd5ec837a17435755fb619fbd54d5cdf8a8828bf2103278c44119a3d038d6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.1 MB (227149281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a2e7f67080ad1e2a2231ca0e435d2312cfdfef87918697be86d765c0abe3832`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:52:16 GMT
ADD file:4714dbb428f38b9b79a0b0234718dfa1c624973506e8a75c52a1753f4202bf13 in / 
# Tue, 09 Jun 2020 00:52:19 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:33:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:33:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:35:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:39:01 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d40938239771bc3bd6ddf7de365dee7a73a438f26b51bd64c09fa994cda5c2a4`  
		Last Modified: Tue, 09 Jun 2020 00:59:47 GMT  
		Size: 52.6 MB (52581526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5029f3fc63be5c726f83ec3d4ab5012e35c3267c5eaa1e83f1614de2fa36622b`  
		Last Modified: Tue, 09 Jun 2020 01:59:39 GMT  
		Size: 17.0 MB (17037281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440d38088bf0cd4439b7454b48c07c745841f10b8ae034fe13636553f0d6aa6f`  
		Last Modified: Tue, 09 Jun 2020 02:00:00 GMT  
		Size: 41.2 MB (41156037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e5a83a21a7d44364f67061483655dfd0991129367f8861f5a37f39d503b1bb`  
		Last Modified: Tue, 09 Jun 2020 02:00:39 GMT  
		Size: 116.4 MB (116374437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5526dee1d545e92f09162695f701768d1846bd386970a3bc4601760e9553d56b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221423320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09c5a34c0da7455c158dd4054401bd45fd789cfc90760ab6a0f0f03fd40ee3dd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:01:53 GMT
ADD file:e29fa406906c6574ad0eb78b933031cfcc111886562a056ec9634129c964dc87 in / 
# Tue, 09 Jun 2020 01:01:57 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:53:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:53:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:55:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:58:20 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:909e57799b0753688e459363ca5a8b3b97160ae637423d0533fd72503e5ef9a3`  
		Last Modified: Tue, 09 Jun 2020 01:10:48 GMT  
		Size: 50.3 MB (50304486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be3c793af972342b8657d56ce6f318a17f6707d23555d7407bde9347f0349ea`  
		Last Modified: Tue, 09 Jun 2020 02:12:44 GMT  
		Size: 16.7 MB (16723388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dadf04af03a5d22b88d6e1682515b77bd2de6c1ce68c80712fb63ce0df2065c`  
		Last Modified: Tue, 09 Jun 2020 02:13:05 GMT  
		Size: 39.8 MB (39778513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0043c2c453d52e874632bae481a6e044798f09b24bf0dfe2258aeaa631c324`  
		Last Modified: Tue, 09 Jun 2020 02:13:41 GMT  
		Size: 114.6 MB (114616933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jessie` - linux; 386

```console
$ docker pull buildpack-deps@sha256:901dec997ca036b2be76abd06dfd1693afd931e892544ff2fb490612c47d5828
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254330544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b8c6e57de2c047ef72e6d788d723ffddffd69a33a80c39064b54476e3172427`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:40:03 GMT
ADD file:e6be478576ebd8d188f0f0507591d45863e225be60ae0e6381a7c54446efe116 in / 
# Tue, 09 Jun 2020 01:40:03 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:15:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:15:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:19:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:23:34 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f753419b4b3c0070d8de5c715f2097d69b60f7b505cc1c31085c9871d67952d5`  
		Last Modified: Tue, 09 Jun 2020 01:45:23 GMT  
		Size: 54.6 MB (54607842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6c6dd78519f2dfee7b28710545708cb946bbad983c2e4327254a388e0e2b024`  
		Last Modified: Tue, 09 Jun 2020 02:33:35 GMT  
		Size: 19.9 MB (19855839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df6d85ba7b1ab6cba5194944d26a4436d3039d76f3a26d0bbd94c3c787ee8e2e`  
		Last Modified: Tue, 09 Jun 2020 02:34:00 GMT  
		Size: 44.0 MB (43989996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268bd815cb5944d8162aa6a413eba19c5185005a370faeb218e0502b5cfb4b99`  
		Last Modified: Tue, 09 Jun 2020 02:34:58 GMT  
		Size: 135.9 MB (135876867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
