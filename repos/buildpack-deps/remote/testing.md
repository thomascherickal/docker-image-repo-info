## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:584154eb2261c84d76248173c138df8501bdb0993a3838d41fffcf5f2daaad7d
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
$ docker pull buildpack-deps@sha256:d582b60b8fadf217583329602c7581ce65866517e8ad7fffe50376bcd74802c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **571.1 MB (571116303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f315aa40a0484571eb393bbb9de01c09c69e4b8c9799ec1c4e3455213781b754`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:24 GMT
ADD file:fa865518757ef9e0af03796e7abd6cbfd59e20f5ae325422e41524615051a2d1 in / 
# Tue, 17 Nov 2020 20:20:24 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:27:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:55 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:28:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:30:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d004aa4da82e9e47169ac4cccf33df9b52bef6dda8aa5f7b0bcb03af34078173`  
		Last Modified: Tue, 17 Nov 2020 20:26:32 GMT  
		Size: 55.6 MB (55578105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5514b41a34cf855f2908da965f01f2b0f68fc62b29b9fb67811a07e7c61d16`  
		Last Modified: Wed, 18 Nov 2020 00:47:23 GMT  
		Size: 5.1 MB (5063216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3985bf4e3bf68c52363fd7853ecc6142b55501eb8457558d27ae10a0358e8907`  
		Last Modified: Wed, 18 Nov 2020 00:47:24 GMT  
		Size: 10.6 MB (10645972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f00fbcbbd3c3783e061ff8d861834c157f06601ed495383250dabb36682027`  
		Last Modified: Wed, 18 Nov 2020 00:47:43 GMT  
		Size: 53.5 MB (53498354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea11244fb3f5d36092406898f5b457e9f31dff55684878b37961efee3354135`  
		Last Modified: Wed, 18 Nov 2020 00:49:33 GMT  
		Size: 446.3 MB (446330656 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b1c8aca80042a85159deaa58efda30e8e6e6913c67b623b36d729c5bca4c1783
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.1 MB (454051293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a02becd64b99391c856953db94e180cc798ef4ca5d00e45c913565ea41a6dab`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:03:07 GMT
ADD file:8b9117df3f1a986438250b725bc8ec117cf1caba2e6953cf9a870edbcda4c565 in / 
# Fri, 11 Dec 2020 02:03:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:37:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:38:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:39:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:44:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:69233e69b29a579de45732361ee762ae02ccbe96b0f2a09fc2a48a802a25b265`  
		Last Modified: Fri, 11 Dec 2020 02:13:31 GMT  
		Size: 51.1 MB (51053259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d208cbc2dd055b46a0eb797352719db7e40a64bb90bab94b3d64b5b3b1c4a6bf`  
		Last Modified: Fri, 11 Dec 2020 03:04:31 GMT  
		Size: 7.4 MB (7444057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b8ae15eeacf7f92e597567cdb02de06832bdbbcbbc72e66d77dba4a1854f649`  
		Last Modified: Fri, 11 Dec 2020 03:04:34 GMT  
		Size: 10.3 MB (10335286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d63c9e301bf107aaab041c8ea9ccf08104e472540b7fad385a3c0c9b14a93cb1`  
		Last Modified: Fri, 11 Dec 2020 03:05:00 GMT  
		Size: 51.5 MB (51532328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5276b0b1d22c077a3b8cd1dfa6a8a1e6635155ccc897894fa14a9a7d3882bfb`  
		Last Modified: Fri, 11 Dec 2020 03:06:48 GMT  
		Size: 333.7 MB (333686363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bb2c852ead60a5a2321b9d94195cfcc08f6de863f5a00193d56c017eb75af053
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.7 MB (427701769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd74f1798dedcc68a72c110725622d30852e6e61d0f272f26256944ae5c1b8c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:22:18 GMT
ADD file:f1ca2b90268fd790612e08e0e01b5ea1b63749dbec2ebb79b37a6168e5e82815 in / 
# Fri, 11 Dec 2020 02:22:20 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 16:18:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:18:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 16:19:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:23:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3354b3972c3003db2792ea643d0250983d6938232305c0bd0b2f3f8ee458c9ca`  
		Last Modified: Fri, 11 Dec 2020 02:32:03 GMT  
		Size: 48.7 MB (48731592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c32f0027df82d0578bcc2d43af7c68680af181d153ad76b785b97e3ffb1a53e8`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 7.2 MB (7185940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ce3f21be10a21df5869d3131ec5a4c6715acb9e45fe541b0050baa4013a18f0`  
		Last Modified: Fri, 11 Dec 2020 16:41:21 GMT  
		Size: 10.0 MB (9974110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cd80ba9b81350feb3d9ed853fd31625b9a1308882fe61f8cee95c338f871d7`  
		Last Modified: Fri, 11 Dec 2020 16:41:50 GMT  
		Size: 49.6 MB (49588792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b6b76458bac5d526785ce1d4519b14033e0ae15e809ee02655e518d0f06eb36`  
		Last Modified: Fri, 11 Dec 2020 16:43:27 GMT  
		Size: 312.2 MB (312221335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:895a78fc9ac9ba086e07be640403bbd60569de798579bd194b7eeab72ec213c2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **547.4 MB (547430153 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439e820d1e3d83cf7165e1fc16ea00ea4e7066f78e8eac2ca47e25578964bffd`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:22:08 GMT
ADD file:58908becb64a88c580fc5d9fea54a7e73507d1e537e70b5567f5d58c26ad000d in / 
# Tue, 17 Nov 2020 20:22:10 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 22:15:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:15:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 22:16:19 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 22:20:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:df1866c47e1fa1c26619e32544732be4853c6b58bfe5ea76c192ae970daf5da7`  
		Last Modified: Tue, 17 Nov 2020 20:30:56 GMT  
		Size: 54.3 MB (54323419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a71907b4dd26e793f4e9841e590a1a930f7265a02f7c07e57767ef9cbe91f8b`  
		Last Modified: Tue, 17 Nov 2020 22:33:52 GMT  
		Size: 5.1 MB (5055744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d2cf86d1130240ba8633c0151d4a4a4b9e6a251bf8ec2bf14d72ce40a67727c`  
		Last Modified: Tue, 17 Nov 2020 22:33:53 GMT  
		Size: 10.6 MB (10648270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c6056c2ca2fb8c36f5f80c875444bbf38dab5bc7ebf358fd257bac133169fb`  
		Last Modified: Tue, 17 Nov 2020 22:34:20 GMT  
		Size: 53.6 MB (53614998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f24020986f5e30e52733c264f645d35dacf69520bc2abf1c13b0608aed506fe`  
		Last Modified: Tue, 17 Nov 2020 22:36:18 GMT  
		Size: 423.8 MB (423787722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:c92030662a686441a5e93e32096e01bedc2b544bf5910ab2eb7f2b7bebe1d900
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.7 MB (332725177 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d43fa2dee6195f96591017ac3f63ef37c728e91f82616bcda99c5cc0273b94a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:01 GMT
ADD file:df88ece8f6b35ea6811921d958952eb8431b76449597cb6d5151e88c62167964 in / 
# Tue, 17 Nov 2020 20:19:01 GMT
CMD ["bash"]
# Tue, 17 Nov 2020 21:01:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:01:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 17 Nov 2020 21:02:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 17 Nov 2020 21:03:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d9137c9a05e5bbf8d80413499157abbe788cac975a7926ded72bd9ff285f7520`  
		Last Modified: Tue, 17 Nov 2020 20:25:46 GMT  
		Size: 56.7 MB (56728874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bbd9994454c4b84708c2d9754f396aac9f662a7169c2322418210f8d161ac4d`  
		Last Modified: Tue, 17 Nov 2020 21:22:12 GMT  
		Size: 5.2 MB (5182817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87786a5db1b57a9ac7c14addd518c4d55f9ac878f951e8110866257d83d6d82c`  
		Last Modified: Tue, 17 Nov 2020 21:22:13 GMT  
		Size: 11.0 MB (11022570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88de8fd349f0d1c859351edc10905c5adca2e975f84e43d737a1933c7ee86944`  
		Last Modified: Tue, 17 Nov 2020 21:22:35 GMT  
		Size: 54.8 MB (54828092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b5e03aa9f809ea152b55fbb2eb45ba9f45b0e5e35e08a60e6843fab15388e7`  
		Last Modified: Tue, 17 Nov 2020 21:23:39 GMT  
		Size: 205.0 MB (204962824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:c27f0db1ff27e78b5e003527a14a53eb4df43ba35041f9d412bd1b746c03d9d0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.6 MB (306636152 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d62dbd85d7f7dc1f80d897149e8f3edcaee67aac8e8dc680ba102441a18e59`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:02:20 GMT
ADD file:1c9d3b0dae65df3d925c78ab44bc00642c930f3deef925694dc0c1a3213de35a in / 
# Fri, 11 Dec 2020 02:02:21 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:44:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:44:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 02:46:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:49:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ede4ac036d71d6e9539de8a220d9f79c46f7c9cb9bf53f8498188327ec302195`  
		Last Modified: Fri, 11 Dec 2020 02:08:06 GMT  
		Size: 51.8 MB (51829610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff97d6058f001d48012d3119e7be581954924dd50d584771418ffecb191be4d2`  
		Last Modified: Fri, 11 Dec 2020 02:58:53 GMT  
		Size: 7.4 MB (7410105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b5e05d9ca9fe9992047f5f69faf9d8cc20423eba1ebf9226cd16e85d820255c`  
		Last Modified: Fri, 11 Dec 2020 02:58:54 GMT  
		Size: 10.7 MB (10656688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7f67c25b93b905661111d2e1ac9d028619abd3d68daf06b9e2d83aae2342219`  
		Last Modified: Fri, 11 Dec 2020 02:59:45 GMT  
		Size: 52.6 MB (52583584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edfcae934f4e293114b560782cb19479da91c1fff63cf90f98092ecededd24e4`  
		Last Modified: Fri, 11 Dec 2020 03:01:56 GMT  
		Size: 184.2 MB (184156165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fd7586f661f470ff2a3328fca299e6986406142fec6dbaad24cdb0a5377dccd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **559.5 MB (559476450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59e7a6caa6285ad7b140fc30838cf11bebfa4013ff678d0996ead5d30a666bad`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 17 Nov 2020 23:21:22 GMT
ADD file:2194006ac3b70de157ecb2806ad599d0c7994e239170bef461ecd9ac5f7f7528 in / 
# Tue, 17 Nov 2020 23:21:31 GMT
CMD ["bash"]
# Wed, 18 Nov 2020 00:26:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:27:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 18 Nov 2020 00:30:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 18 Nov 2020 00:51:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:bc7190938049d8573412a9fa0fdcbaffd5e24ad75693e87ff89a4f37791f0907`  
		Last Modified: Tue, 17 Nov 2020 23:29:22 GMT  
		Size: 59.8 MB (59761557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4c36e5042edb900f63e80ffd0e14c80fc84b50d9d0983b6e7f46898e988fa5`  
		Last Modified: Wed, 18 Nov 2020 01:46:30 GMT  
		Size: 5.3 MB (5302380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a2b5d04b45968683b84bbca4828b6ba15fe17909e3c64cfe7678a9d180f99b`  
		Last Modified: Wed, 18 Nov 2020 01:46:30 GMT  
		Size: 11.4 MB (11408115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4953d5427968cc8c9a1c8ddb3e8a07c98b8fc47806f8cd1fd0f6eb9428e8fe9c`  
		Last Modified: Wed, 18 Nov 2020 01:47:45 GMT  
		Size: 57.8 MB (57825151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd57890e822f0f0fd259e8b4e4070a42b569998ec3a6202c40b9f58c8d7f1ef`  
		Last Modified: Wed, 18 Nov 2020 01:52:41 GMT  
		Size: 425.2 MB (425179247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0a3158bef0f01ff03678614017eb4cb637eceea8925f24f7c7af3327b9a21ad8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **427.0 MB (427005261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c695c13aed2c6b7a18e2a7d0eb44d97392632d8d105d800e6e0c0516ce7679ed`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:03 GMT
ADD file:74a0f68651d74636caec45b24b97289c444300a4e20ead2e9dd4ecad9a89b149 in / 
# Fri, 11 Dec 2020 02:11:10 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 15:56:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 15:57:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 11 Dec 2020 15:58:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 11 Dec 2020 16:01:52 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8c1102ca26cfeafe4e6f6b885fc1f8b1c19daafd157e556c9eb528d215f3ec2a`  
		Last Modified: Fri, 11 Dec 2020 02:16:10 GMT  
		Size: 51.7 MB (51656809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5318fd9b9f903620dcea8eebe0d1b3e4c22fbc8b859c0bf46ac13755d1a52a`  
		Last Modified: Fri, 11 Dec 2020 16:14:25 GMT  
		Size: 7.6 MB (7565720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:845cbfbba3746772baf57c643c9a8edde11b111c4a69407f278d0c47ace4f158`  
		Last Modified: Fri, 11 Dec 2020 16:14:26 GMT  
		Size: 10.5 MB (10525441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739f79a56621b8c3834393733c04a12d896e7ec992d0f284d592926bb45255ae`  
		Last Modified: Fri, 11 Dec 2020 16:14:42 GMT  
		Size: 53.3 MB (53325128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1a9b3abbdf49dfa5c86ec9deeeaa90d9fc003d3a4f117142987d9e974aa138`  
		Last Modified: Fri, 11 Dec 2020 16:15:34 GMT  
		Size: 303.9 MB (303932163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
