## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:2f079a472b02649087a2cc8e6b712c92a6b29c1ad5eb7a98ab2951a44786759c
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
$ docker pull buildpack-deps@sha256:236b590f51db766ab35b991a9f4aa16338288ca52fddf098a1a23797c43627f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324138958 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:490c91d844d571329144152be5f8d76b5f1806abe8b09fa95715fa01b3dad158`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:21:21 GMT
ADD file:d8f8a66e04b091b1ee6d1d330b5cd80472768f8cef96db861ba4dfaa2472fe20 in / 
# Thu, 16 Apr 2020 03:21:21 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:57:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:58:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:58:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:22:37 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3d9ec154a243cb2fcf510aa97241fa4d7c075add5b018b19db3f1dca9f93c83a`  
		Last Modified: Thu, 16 Apr 2020 03:30:54 GMT  
		Size: 52.0 MB (51968339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f52bafd3e8510b30e30d2ccb5e044a4647586a4b5dcdee4e79b63b54296a77`  
		Last Modified: Thu, 16 Apr 2020 04:14:57 GMT  
		Size: 7.9 MB (7932617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61caa2b6b1a3f079feb31d0b6ce33740955163e262ec2f624070129b13ebc779`  
		Last Modified: Thu, 16 Apr 2020 04:14:58 GMT  
		Size: 10.3 MB (10298054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c043d752dd56512f49ba5efa050e0701eadb2605cd22b197ccffd7aef9ba742`  
		Last Modified: Thu, 16 Apr 2020 04:15:13 GMT  
		Size: 55.3 MB (55327131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:452c15fe109790b5789fb9e2d3a95897f842a3b78bf53e3cfefdc173bc3b6858`  
		Last Modified: Tue, 21 Apr 2020 01:37:26 GMT  
		Size: 198.6 MB (198612817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:d69bf71063bd73da4f91400844eb353ebcea71113deb758cc8d13812690f8a64
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.5 MB (295456428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73f9f187646c94d1015371ac9df7281ea0074289e266b56c397d69ba865d1474`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:48:51 GMT
ADD file:34972a3f69849271a3928351165da58547b7e747a95139712188aa70c0b57364 in / 
# Thu, 16 Apr 2020 00:48:53 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 07:35:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 07:35:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 07:36:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:52:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:562c28f550656170c3977f83af3b203cf461b48e55905e20714735c0da33f6af`  
		Last Modified: Thu, 16 Apr 2020 00:57:24 GMT  
		Size: 49.9 MB (49911580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6e10c95bf2fb0d9afd80c213468dbbf9c1ad4730788858911322bf24add94a`  
		Last Modified: Thu, 16 Apr 2020 08:03:59 GMT  
		Size: 7.5 MB (7514410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e617dda0a7a661e7f311626e566d0268d79bc1e83eb5b8e533776c9cd3991592`  
		Last Modified: Thu, 16 Apr 2020 08:04:05 GMT  
		Size: 10.0 MB (10008531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85850fe957d69f2c749872a598fb5b37adbebb598130616ccab029087a446243`  
		Last Modified: Thu, 16 Apr 2020 08:04:30 GMT  
		Size: 52.9 MB (52902217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:886d3861aeb9685a5ae5eaaa4561df3f15a774ae5c7f3d1e149bfd4ae9ebd135`  
		Last Modified: Tue, 21 Apr 2020 02:08:40 GMT  
		Size: 175.1 MB (175119690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:e026381674b1138c303a09ec717bc5899f7cffd6101ef2777c7a23eb8aab3e37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.8 MB (289769326 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dff7ee908a9e70cc0e9e2efeaafc630b123dc316bf063b36b98b9d23ce6b8b25`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:58:05 GMT
ADD file:353f89e64e5475f2d99be1c5e0eaa80d5aeb89e02c274ba507df4def8f7ccc8a in / 
# Thu, 16 Apr 2020 00:58:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:33:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:33:45 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:34:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:03:47 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a287a7fa81e293e147ba52c36ae34e643e975ef88ebe9a6f226a048dbb7ee9fa`  
		Last Modified: Thu, 16 Apr 2020 01:08:03 GMT  
		Size: 47.6 MB (47646389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47358f6975165f42a9cd9b867f0d03e95a00b52627d5e833781a9eb45eca84cc`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 7.3 MB (7255347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376a0294fac4492ac4a3da9b92cdf02ee87e6bfd519ee19fb996c5db96da33ae`  
		Last Modified: Thu, 16 Apr 2020 01:54:57 GMT  
		Size: 9.7 MB (9672922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010ce0dbcbdea4c6cbef9d1bda1fb769c382107cb837edfcdc6258b8421fc200`  
		Last Modified: Thu, 16 Apr 2020 01:55:21 GMT  
		Size: 50.7 MB (50666643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3377ddf0c33d5009404340d82643e6d6987781b8d454e73fd114a2fdeeaee35`  
		Last Modified: Tue, 21 Apr 2020 01:23:29 GMT  
		Size: 174.5 MB (174528025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:a4a3bb36a6bf44704bed9127b55665173dfa1af51c2e133d8b5c11e04d0df0c5
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.9 MB (315943291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b594d60ba62425c7a516772bc6f6236b5fb5ee6df98d9db4e3b2dbf56451e8f8`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 02:40:12 GMT
ADD file:27c25cdd69090f4b15f9f2f4a147879d1d7510b7b2f8c231a92fc74832325413 in / 
# Thu, 16 Apr 2020 02:40:14 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 03:09:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 03:09:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 03:10:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:45:03 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6c6bfde49c5261423574a9f9bc077a0cd0057775509f9d9e061556a16b84e1d7`  
		Last Modified: Thu, 16 Apr 2020 02:48:01 GMT  
		Size: 50.9 MB (50901465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c744c6854f291e264392cb87f79c4675b05d5383ca93df9f5b4be8f447aba3a7`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 7.8 MB (7807688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e0a53c53b80bd91c029938e07ae8fb49e75ae1d45620212fa6fc041e97f5750`  
		Last Modified: Thu, 16 Apr 2020 03:26:27 GMT  
		Size: 10.3 MB (10294224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee1bd7b8a02f00bba05f898a3f2c91d213d6fff20796effafce1437c9b6cab9`  
		Last Modified: Thu, 16 Apr 2020 03:26:51 GMT  
		Size: 55.4 MB (55385347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b088443a3522b619d268de28a4e8351aa9182c642694e31b35cf650dff343ab5`  
		Last Modified: Tue, 21 Apr 2020 02:05:15 GMT  
		Size: 191.6 MB (191554567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:2a539354d1be0344e8f56bbed84015443e9cd8d519c298adb389a77b85485c13
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.0 MB (333993688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae01f2c3f84a170385c3c1ea949bce4328b3a91bcad746559551cd1210c11db9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:38:50 GMT
ADD file:1d78edb74644d640409b64831c000f00654603e8888b50c46ac37ca0c186c3e9 in / 
# Thu, 16 Apr 2020 01:38:50 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 02:16:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 02:17:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 02:17:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:42:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d162d6311c3b7618a8b9a80392bb71455272c7ef63938e132282070923f16ead`  
		Last Modified: Thu, 16 Apr 2020 01:45:26 GMT  
		Size: 53.1 MB (53116500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d42814ec88fe50214d62dfdaf2c1a27abf7c61f1718b16dc664b952cc85492`  
		Last Modified: Thu, 16 Apr 2020 02:35:50 GMT  
		Size: 8.1 MB (8110131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b97139d647978bbac84cf0fbb6575ccf2950e262ccf617d10aa0e60e479481bb`  
		Last Modified: Thu, 16 Apr 2020 02:35:51 GMT  
		Size: 10.7 MB (10657214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a29d09c18686eb52024c1b28dd62d1ffe2ca03f040d1f82bf9fcfa657d41bb5d`  
		Last Modified: Thu, 16 Apr 2020 02:36:12 GMT  
		Size: 57.2 MB (57154439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fd748dc1b9db82833e85d728555cd8956944cc286223539d3c2d7b174f84016`  
		Last Modified: Tue, 21 Apr 2020 01:58:07 GMT  
		Size: 205.0 MB (204955404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dd0cf0e9bdb749624d0fc9d18e04b4d8a348b2fa79facbf9e28992524bcd0d15
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.3 MB (306346759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b7816c43aec165ee23d4f186ebfd938114baddbd69a1d198f49ac2ae4efdea0`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 03:29:03 GMT
ADD file:571d620a73f63f0bce6937ced0e2a2f7dbd127e0fecf9e97790d0941cc6bce5b in / 
# Thu, 16 Apr 2020 03:29:05 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:06:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:06:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 04:08:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:11:25 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:02267d0e0eb88e51f19069b5cba14fd409e92034ffa2d476e3692b85e83addca`  
		Last Modified: Thu, 16 Apr 2020 03:54:44 GMT  
		Size: 50.7 MB (50678841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb4f080ce8cb9f9c9b928bdf65ce27246d82edfff61aa1f7897eacde7012a6b`  
		Last Modified: Thu, 16 Apr 2020 04:31:14 GMT  
		Size: 7.5 MB (7459912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82100df7296466c11c6b4ac15634db8168d4618b3226c40897edace4a237a2a0`  
		Last Modified: Thu, 16 Apr 2020 04:31:16 GMT  
		Size: 10.3 MB (10324443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1a595cb267827df6d653c7f6bb665d87184787ea82d990902cf4edb2b88804d`  
		Last Modified: Thu, 16 Apr 2020 04:32:43 GMT  
		Size: 54.3 MB (54264268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4da90949ff4c950fcc375b8b34c1c0cb5777483ef96c856d052c8ac8116b312`  
		Last Modified: Tue, 21 Apr 2020 01:22:57 GMT  
		Size: 183.6 MB (183619295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:59c937010b134cc890ae44711d835f12774216ee5c7cb0e51538dfbf0a6cb0df
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.4 MB (342390196 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e3e060d33b253edfe3d62c0b0b24abd4f257d4fb6c170f2d4b4c418cd12af5e`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 01:32:12 GMT
ADD file:2efc2c0f69b08c32feb2685a63906c73b19fb52d2b93f97e10252433820bc5da in / 
# Thu, 16 Apr 2020 01:32:20 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 05:28:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 05:29:21 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 05:31:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 05:39:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5bebe00a0631d47861daeee3fc26571ca333821c566ce1b711e981ca7685ea53`  
		Last Modified: Thu, 16 Apr 2020 01:50:59 GMT  
		Size: 55.8 MB (55848114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82799cc8d738aec7df8ddf9bb9deae49b2ebb048ae3ff658fab69e938e9eed79`  
		Last Modified: Thu, 16 Apr 2020 06:16:14 GMT  
		Size: 8.4 MB (8355958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b8d71962ead5ce3976d8ea0a1c6a27893344557398f8d2b314c28d2b065fd7`  
		Last Modified: Thu, 16 Apr 2020 06:16:16 GMT  
		Size: 11.0 MB (10975758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51294330fdb8f00471b393961669925b313ea4466f89528adcdb5a6fe85b497`  
		Last Modified: Thu, 16 Apr 2020 06:17:41 GMT  
		Size: 60.6 MB (60622119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39d1a14873ea46aeb20152a5bf3c977dd4a4de4da55d8319873e1e4b8083b20f`  
		Last Modified: Thu, 16 Apr 2020 06:19:48 GMT  
		Size: 206.6 MB (206588247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:e9194043381c5b58b55a69edca65d632980f38758dd8a3b34cb0a14199faf6f7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.8 MB (304839642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37460a03ea20ea089815902ec8bc62d9ace55ebf7ca99b22b085542a624e8c17`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 16 Apr 2020 00:41:36 GMT
ADD file:91904e1cbd0660c7c48420aa34dd58c0e8619c69afe6c1412a495c364773b5bb in / 
# Thu, 16 Apr 2020 00:41:39 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 01:56:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 01:56:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 16 Apr 2020 01:56:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Apr 2020 01:44:25 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:929a8c37dff5f4096f453d7847637ff8b3e3fa702bd1043408eb37af338237d4`  
		Last Modified: Thu, 16 Apr 2020 00:45:37 GMT  
		Size: 50.6 MB (50569040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625f45e55816a01b4e47db24dfb9857e953051816a723f6999906fa8fe1cb40e`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 7.6 MB (7600032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af726635ebace664ecb1c229bba4cbd77183a3411aacacaae74f1cbb0882eadb`  
		Last Modified: Thu, 16 Apr 2020 02:05:36 GMT  
		Size: 10.2 MB (10183890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:216e30525b6ed08c23f0a9ee26e1498e8ad2fa322601120a5936a44f2ddbfa87`  
		Last Modified: Thu, 16 Apr 2020 02:05:50 GMT  
		Size: 54.6 MB (54565876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd4d8769aca7f2c9f55b382d88506fb47eae70d9b1d08776f4015c38242ba36`  
		Last Modified: Tue, 21 Apr 2020 01:52:45 GMT  
		Size: 181.9 MB (181920804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
