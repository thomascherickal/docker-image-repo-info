## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:2fd2337d544d396840ec58c6e08f228a4caaccfca182a1bd359dca76f72af206
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

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:3e1eff91a5ce250c2f08667fc83930ae83ae996adee707f4559bf5bc7a0d6dc5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.5 MB (312454254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6871d248b38992d77de11c0c45cb104ce5c0039d1106ccff6b9f5822430c1338`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:49:16 GMT
ADD file:c254898ceb4172f05cd40460f8d0b1ca2d39d5178bdddd4e794c7d3fc5a60a03 in / 
# Tue, 30 Mar 2021 21:49:16 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:03:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:03:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:05:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:004f1eed87df3f75f5e2a1a649fa7edd7f713d1300532fd0909bb39cd48437d7`  
		Last Modified: Tue, 30 Mar 2021 21:53:41 GMT  
		Size: 50.4 MB (50432842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6f1e8117dbb1c6a57603cb4f321a861a08105a81bcc6b01b0ec2b78c8523a5`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 7.8 MB (7832608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48c2faf66abec3dce9f54d6722ff592fce6dd4fb58a0d0b72282936c6598a3b3`  
		Last Modified: Tue, 30 Mar 2021 23:14:05 GMT  
		Size: 10.0 MB (9997208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b70d0479d7f16d7ee8d04e4ffdacc57d7d14313faf59d332f18b2e9418743`  
		Last Modified: Tue, 30 Mar 2021 23:14:37 GMT  
		Size: 51.8 MB (51840782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa07a00e2f029c4b2c7f177a2b696f1b3510040cde4f5bb06ddbca98e7fbf76`  
		Last Modified: Tue, 30 Mar 2021 23:15:30 GMT  
		Size: 192.4 MB (192350814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:47a8eba0de423d9fcc59c4c34c23bd0141166c5435d93575173af192121ef0bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.1 MB (286082176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9546a086249941188eb3effdb3f9de830b3cb5cf3478999c59632771df58df54`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:50:44 GMT
ADD file:6faf9c88ecf5029b54207c4a7575a4afa74c06e6655ad84599d4139337866709 in / 
# Tue, 30 Mar 2021 21:50:45 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:47:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:47:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:48:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:50:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8df1bb0713d83752f3588df777df10475afe64f042cf61465992cf6074bf7bfc`  
		Last Modified: Tue, 30 Mar 2021 21:58:15 GMT  
		Size: 48.1 MB (48149101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bd2fd7358baf32fba79f0cd737807891482dd2ef4c726a3b5ce0cc9a2769f5`  
		Last Modified: Wed, 31 Mar 2021 00:01:22 GMT  
		Size: 7.4 MB (7376451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf105079c9c0f9176755263bc667f2dfc33d84f5bf98bde9856d918802d2278`  
		Last Modified: Wed, 31 Mar 2021 00:01:22 GMT  
		Size: 9.7 MB (9687429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73dc4147608173616c34d4a051e7d7d4e6a1d41ba86d7e8afafdcea7ec57193d`  
		Last Modified: Wed, 31 Mar 2021 00:01:51 GMT  
		Size: 49.6 MB (49573641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25326daae66c59c5a8d7749a5fe9c251ddafe6f2359f40ff2aea332bca5f1aff`  
		Last Modified: Wed, 31 Mar 2021 00:02:58 GMT  
		Size: 171.3 MB (171295554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:97af7621ed24f0c2e1a84eab59226cfe794741c509e05a95eed075a70fcef4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.2 MB (278240949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09803e44e9353631027de1ea702e5049dc0b813510962cda9c47d3dacc62d0d9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:10 GMT
ADD file:b3e1f7b8ae0587f7850210420c8dd6da7fb60fa87c5863e6fe5a8bab1bdc7abc in / 
# Fri, 26 Mar 2021 11:17:11 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:22:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:23:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:25:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2703ee001e01b49055599d26cac8b1a472b75d8643e8a00ab281b97e3fe6aefd`  
		Last Modified: Fri, 26 Mar 2021 11:26:53 GMT  
		Size: 45.9 MB (45868006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f00d516e34bfa5a11e13fd33e0649e2bfcfa443418341f1cda5463ed8ee8046`  
		Last Modified: Fri, 26 Mar 2021 13:51:18 GMT  
		Size: 7.1 MB (7123912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac789cd7e7d8f8003e7ac6b6bbf96d3859a2318c4569114ccb686ffd779ce119`  
		Last Modified: Fri, 26 Mar 2021 13:51:16 GMT  
		Size: 9.3 MB (9343659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e16bfec3cd4c49403ed5b98e6216074d4f3c68c5dc09e6e12252c09aa8952cc`  
		Last Modified: Fri, 26 Mar 2021 13:52:03 GMT  
		Size: 47.4 MB (47356546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd8364950cc87a0ab5051809b3c724b0484c8ed4b04704e823d1683dc82a32d`  
		Last Modified: Fri, 26 Mar 2021 13:53:22 GMT  
		Size: 168.5 MB (168548826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:af738370a9adb6142e3f486892e9fcec05ebf5efec59e8949840899e60fc5e39
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.0 MB (302970985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12d22072848fde757b174ceed311dcd7be5338976159173da69caa6f1bda33a1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:46:50 GMT
ADD file:6a5cce92f1039ef2cb7ac6dd999c9f84289a9f6e1c0891d1edf791ea73b7e125 in / 
# Tue, 30 Mar 2021 21:46:53 GMT
CMD ["bash"]
# Wed, 31 Mar 2021 00:15:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:15:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 31 Mar 2021 00:15:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 31 Mar 2021 00:18:11 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef28e7e77ecbd3b3b426832bc12e8f5e629959683767466e9bac149c3286e126`  
		Last Modified: Tue, 30 Mar 2021 21:54:03 GMT  
		Size: 49.2 MB (49225808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344d2d9a9cf41c137b0dbb41df255f95fb812a23771a10ee2ab5a8a5047c62c4`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 7.7 MB (7694530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299f3631f6b52be065a7342da0a46978d55cbd0d15c57fae22f4ca24efcc295a`  
		Last Modified: Wed, 31 Mar 2021 00:29:59 GMT  
		Size: 10.0 MB (9984391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba70c372ae296f23e908bf1e1ed9f4c0c81a8a6d7fc48c0e2db16035bb9b7a54`  
		Last Modified: Wed, 31 Mar 2021 00:30:24 GMT  
		Size: 52.2 MB (52165620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc089388c7ca4407aec7247a44601b896e57e96d53a858fb0e8c6f2f94ab8da`  
		Last Modified: Wed, 31 Mar 2021 00:31:19 GMT  
		Size: 183.9 MB (183900636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:25c138f18f39fe40bdceb65471584ea7d661032994cf5b2634d924277d261884
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.9 MB (321872572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ba11d7f0059932b81ee62f4f6d1049e007160a96de44d816b7cc06f9e808e66`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:39:30 GMT
ADD file:a2981af3d3aa369b11e802f23b175abfdb0f7636cdeec3aed67488d7a1f28a19 in / 
# Tue, 30 Mar 2021 21:39:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:56:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:56:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:57:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:58:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a3a3dbaddd2d56d7418508211551c461f826d1cae349d39a355a1c22fe140b36`  
		Last Modified: Tue, 30 Mar 2021 21:46:05 GMT  
		Size: 51.2 MB (51198756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de970e2d41035ffe1a656cc3d1f8e17bc7b8539b23745405b8fccf25d10fd312`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 8.0 MB (7997659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c27a2cf0e2e609cc89ee5b623626f822424bdc818ac5eab541a7a7b158ef0c01`  
		Last Modified: Wed, 31 Mar 2021 00:08:00 GMT  
		Size: 10.3 MB (10340050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7a5ef36d45f69154fe2b83a8e658d4f08c45428493e8e1cc74a8b03b3c4799`  
		Last Modified: Wed, 31 Mar 2021 00:08:31 GMT  
		Size: 53.4 MB (53438017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e4b62cf2ad846ba0bec17add38106ebdfbe771009574c1a033f9698ba80e36`  
		Last Modified: Wed, 31 Mar 2021 00:09:26 GMT  
		Size: 198.9 MB (198898090 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:cfb0216c521855f6b21330cb40f86fb022d050825b333ba03eb4d578df45b120
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (297044672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e3a2fb480024065213c2576b7ecc8de8e424367107c08babefcd5dbf70937793`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 22:09:25 GMT
ADD file:80bc7c6935e37a30f99582a481ea9ab5b67120ce265a4d29963ea84dbc20e314 in / 
# Tue, 30 Mar 2021 22:09:25 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 23:10:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:11:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 23:12:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 23:14:28 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:eafdc9ff229439b8b9998d865c33e726afd8b6dcef65b7d5f02b39c022d19a13`  
		Last Modified: Tue, 30 Mar 2021 22:15:37 GMT  
		Size: 49.1 MB (49081877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5895125ddf0fc95ea9b30c1869f31950905b89ad0e06af9ab022ff8a288e3059`  
		Last Modified: Tue, 30 Mar 2021 23:22:03 GMT  
		Size: 7.3 MB (7251232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf3955dcf92989b48c4dcc991612fad98cd9c1ce94e1bc4d6aefdef84d2a15b`  
		Last Modified: Tue, 30 Mar 2021 23:22:04 GMT  
		Size: 10.0 MB (10016345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac2a8d35407cc21f77d27cfc4e124b989b953f8f604e862e24a8474df87192b0`  
		Last Modified: Tue, 30 Mar 2021 23:22:57 GMT  
		Size: 50.8 MB (50843479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb591c7ca06660250c51ff63530b49ef1cd27ac0dca85c9a802c6de138700300`  
		Last Modified: Tue, 30 Mar 2021 23:25:08 GMT  
		Size: 179.9 MB (179851739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb1fd1c4561bd2139246286408045d3f826614fd4ef132f46b58fd299cee5944
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333773461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23af64f87612a0d961d18d082ecbc44b60f6bc2fb5b7abf87072e6d3a1438985`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:13:48 GMT
ADD file:2e3cbe75ac7fb7b716e5b7411062bb9ce510f3317d00ddbfd608a5057931cc9a in / 
# Fri, 26 Mar 2021 15:13:55 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:38:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 17:40:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:55:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2280757cb36e3eef6465890eb70453bb9f66e271e373f08ae5e9d7a3307c5fe4`  
		Last Modified: Fri, 26 Mar 2021 15:21:30 GMT  
		Size: 54.1 MB (54136619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de5b549e9718d8f1d72fed2093ec025063ce0d94eb6fe18e4f59d6233dc1231`  
		Last Modified: Fri, 26 Mar 2021 19:40:42 GMT  
		Size: 8.3 MB (8271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bf4e1832c58cc634f3cc177e25538b86637e529844e6f8e340f5b4acd876`  
		Last Modified: Fri, 26 Mar 2021 19:40:32 GMT  
		Size: 10.7 MB (10727704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3650b3afac8fc5a8b47e5ce2681df05154740219a9355d33d04418e90f4b78`  
		Last Modified: Fri, 26 Mar 2021 19:43:11 GMT  
		Size: 57.5 MB (57456809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2201bcb3f7630cea267e25821259e17467f146339142332ea0b0f14ab8d92be9`  
		Last Modified: Fri, 26 Mar 2021 19:47:30 GMT  
		Size: 203.2 MB (203180622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:da1b58b56526ba7cb7ab26cc3313e72507970e1ca56af58a950258f00731bd3c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294531806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:de11a8d28a7455b2f9d5df7ff4eb4849b3caec3bc85b09393cbb516aa2a6b54b`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 30 Mar 2021 21:42:29 GMT
ADD file:79040b5dceaf577162ccacdf7ef9e018f89e7ae399d59b4f80b3860a0471177b in / 
# Tue, 30 Mar 2021 21:42:32 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 22:43:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:43:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 30 Mar 2021 22:43:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:44:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:dd4a1caade48d16285d95f8062825cc6952224e43c64222e0cdcf13bc87b44ee`  
		Last Modified: Tue, 30 Mar 2021 21:46:01 GMT  
		Size: 49.0 MB (49000451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e488b7badadfabcedd6ad7a531fa8681ffb922e9853deb7bb142c86c78fdd05b`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 7.4 MB (7399948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab15bd749c981c81cfe3ea27b9a7aa17ecf7dc0ce0357b9fe7774d8006622fa`  
		Last Modified: Tue, 30 Mar 2021 22:49:21 GMT  
		Size: 9.9 MB (9883132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e972cd743ab6520beed6242099fac9a59889445dfb7a01e42ee1ced09ac0e5`  
		Last Modified: Tue, 30 Mar 2021 22:49:41 GMT  
		Size: 51.4 MB (51379958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df5b10ced3ee54342c6e637945570c630f619af47c72e827eeb7b03dc9dbba8`  
		Last Modified: Tue, 30 Mar 2021 22:50:16 GMT  
		Size: 176.9 MB (176868317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
