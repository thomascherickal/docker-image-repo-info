## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:61ef152e1ab7a8a64a9c039ae6c294167c710ee649f4abc2c58a4fb2b923f512
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:testing` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:8b6f26fe57884240852713a9ef617140f56dea6e5672cb369e4abdace025a635
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **322.0 MB (321998656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60a40af9f20b56fdcb0bd6afbb5591d31b97c13fbd69e9172814479f4696f077`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:36:28 GMT
ADD file:7d01effeba890adb1756ba0a76c42c1dde5a189003943fbf4cb9fae0c0e1a046 in / 
# Wed, 26 Feb 2020 00:36:28 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:04:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:04:34 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:04:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:05:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7a4501da464e996edc2ef85325afe9881a58061a9a35b142ca7f0ba598553e49`  
		Last Modified: Wed, 26 Feb 2020 00:43:35 GMT  
		Size: 51.9 MB (51852739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00055416d483b70a8fceb7d6e7685e08d5c76fd449df312352288b650f0a5f83`  
		Last Modified: Wed, 26 Feb 2020 01:19:20 GMT  
		Size: 7.9 MB (7921881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eab3db52671a6130df45784942f13ea891360cc3cd5d39ad4208321078246c`  
		Last Modified: Wed, 26 Feb 2020 01:19:21 GMT  
		Size: 10.3 MB (10258054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a471741589e2b8271d8be85e5a2d0ba4eb2667b7207711b99787dc20fa3eb6`  
		Last Modified: Wed, 26 Feb 2020 01:19:37 GMT  
		Size: 54.9 MB (54915618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c7c134b6bb2a68bcfd3f52e845622d97570fdb6fd7a88d9868cf0c4cdb1a88`  
		Last Modified: Wed, 26 Feb 2020 01:20:18 GMT  
		Size: 197.1 MB (197050364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b9df4842dd6d8cb0552ec90a9ef8ee7208d084a33378ff98b706f185dc34b82f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **292.5 MB (292462696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9230b4d13d86ec64525ccf954a16e4c904c7614020048b399f8f94f13a5db9a8`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:49:39 GMT
ADD file:b4c3e18bbf2b51c4f777d44bb8ef76a6fd78e8e9e057ffeb792fa8e041d3b40d in / 
# Sat, 01 Feb 2020 16:49:41 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:19:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:23:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1758f12059aa2a6d57dcc649233827a3b49cc528e7868081891f2a12944a479b`  
		Last Modified: Sat, 01 Feb 2020 16:56:07 GMT  
		Size: 49.5 MB (49485065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4449c159b35252b02eefe1b4989bc90d10d35fd6d17600ae5d662ba279c259ad`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 7.5 MB (7494059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a6070fc56cb0dfa20ffac6472ce9dc9a8aead19638f495a62bff5206bf6ec7`  
		Last Modified: Sat, 01 Feb 2020 17:43:56 GMT  
		Size: 10.0 MB (9969002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5ef05714eb441ecaca79d450dfa2444ca3fe859d6c1080d660e208a78633f7`  
		Last Modified: Sat, 01 Feb 2020 17:44:18 GMT  
		Size: 52.2 MB (52219763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcb9a5a15d5e44eabb292a2a87d9bab5c97a2f3fd76d3cc2016425b8601e8ce`  
		Last Modified: Sat, 01 Feb 2020 17:45:14 GMT  
		Size: 173.3 MB (173294807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:f99f095dad97a24dba7594dc00afa425ce4d7950835b10ea89c25920058b2680
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **287.7 MB (287712804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a181a40fc4d1d0d1e3b25668b858c3de038221339353d78db5bdd9e105d5da`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:49:40 GMT
ADD file:516c2d0189c8132f97d954209787ec2c833e16a9d8a4056cc9ed22510c721b48 in / 
# Wed, 26 Feb 2020 00:49:43 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:07:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:07:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 02:08:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:11:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d46b4a12bd08cdd498cc190f7d350b7bfa151e105942f36a185990c238f53695`  
		Last Modified: Wed, 26 Feb 2020 01:06:24 GMT  
		Size: 47.6 MB (47581289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab620fe7c5ae5218251dd6127456072d85bebc5b47b3359937f36ce071d355df`  
		Last Modified: Wed, 26 Feb 2020 02:32:01 GMT  
		Size: 7.2 MB (7237740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba007f6e72abf7b8df1b3d1009db9b497e33953f02bd91c28566d6700b3e462`  
		Last Modified: Wed, 26 Feb 2020 02:32:01 GMT  
		Size: 9.6 MB (9638411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db97fc91eb5d6d855e20ee37328160b266216205b0e2f0b9dbcefbb09c48b38`  
		Last Modified: Wed, 26 Feb 2020 02:32:24 GMT  
		Size: 50.3 MB (50332192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b42f7e1d7b1d44f30e4a93d459555968f199a6490be6183cf812f3c433baa4`  
		Last Modified: Wed, 26 Feb 2020 02:33:12 GMT  
		Size: 172.9 MB (172923172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ea3e7fa49e9200c6f6ec1dc4f85bdf3ad822be5d42c67df0ab7409a66ad4559e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.9 MB (312905591 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c4a95adbd15cef3cc4a71e78b4d641a3c4574bfebf3f9978f1861f1130705b2`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:13 GMT
ADD file:485f0f88566199683d3683f547dbd33fa9cb4897121b104dd7c852162fa06cf7 in / 
# Sat, 01 Feb 2020 16:40:16 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:14:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:15:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:15:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f625aea7552a55d9aac253c9834ea6e645ae1e9d641ccec7e167585699e5d1b3`  
		Last Modified: Sat, 01 Feb 2020 16:45:20 GMT  
		Size: 50.5 MB (50453025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2bd511eb67667a40782667bc3dd7eb41f584de23c5a106085d2a1db980df9`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 7.8 MB (7792989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03f4fcee540ca05f3c8904722b70f13e10600fced1073a2612d04d995a93d210`  
		Last Modified: Sat, 01 Feb 2020 17:33:39 GMT  
		Size: 10.2 MB (10245802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c5c01ce24c138f20821dc546f2dafea1d7baf1be4863e4de4f1957f18bb1577`  
		Last Modified: Sat, 01 Feb 2020 17:34:01 GMT  
		Size: 54.7 MB (54722057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b0a0a19a3e7ec87ea68eb660a968feafe74386f958cdb4ba3f24fa8f06a1814`  
		Last Modified: Sat, 01 Feb 2020 17:34:51 GMT  
		Size: 189.7 MB (189691718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:59167ce4f3b35e9d39d1163cb1eb6308aee846c8da1bcf26e79cad313442c2bb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.7 MB (331721353 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d391fee13591420300163d3b5262ccad5eadbaf6770b3ee187703771cca8f79`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:31:20 GMT
ADD file:d6037ec8e49283f4a0fd36cfd0bc4723725164526c4c56459e4c9f3d73c61d06 in / 
# Wed, 26 Feb 2020 00:31:20 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:04:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:05:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 01:05:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 01:07:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1d581a0f5f74a9924d3ed374e49a0171892551a9eef1c8d7efea523bdb4334da`  
		Last Modified: Wed, 26 Feb 2020 00:37:37 GMT  
		Size: 53.0 MB (53002659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095cc9a34f8e935c2fbfb4ac9eb3644923f64856d1434b4ac0f9dd4e3db91c92`  
		Last Modified: Wed, 26 Feb 2020 01:25:50 GMT  
		Size: 8.1 MB (8098985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab82912141b87280af1133876199f3de73be0b8797e7c31724505f58ede4e01b`  
		Last Modified: Wed, 26 Feb 2020 01:25:51 GMT  
		Size: 10.6 MB (10622833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010e0c448a96676d2209e4a820484ca9c98f8a0cc07d29c7c7cf70b27ca66976`  
		Last Modified: Wed, 26 Feb 2020 01:26:14 GMT  
		Size: 56.8 MB (56757528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a8fa9cc1d8d34522aa1ee0310c7a1c3d878aad51bd761c30a1b6fca4945a5b`  
		Last Modified: Wed, 26 Feb 2020 01:27:07 GMT  
		Size: 203.2 MB (203239348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:a73c163e1ccacb1ffe4d70da6b9d240c0984d88fa05ece3b4b8db6269654b001
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.3 MB (340257204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b925aabfb4247ca36f593a88b8c3e40c851b90fff386f9e7d17d6f2fa61d34`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 17:17:00 GMT
ADD file:1a064022bd5caf45345b7a91191b82f0d2bb576e88e99652a4c3d68c399b1578 in / 
# Sat, 01 Feb 2020 17:17:04 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:25:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:26:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:28:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:36:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c80e92e9d0447b759db73a162ee40f56912d3ae4c251aa735339219ad9bc7a68`  
		Last Modified: Sat, 01 Feb 2020 17:24:16 GMT  
		Size: 55.3 MB (55316324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0367678cef47c5fbcdebd74948fd485de617cb36ea2d6182b1dfd3d5b1429b7f`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 8.4 MB (8352503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc091c35bf183343a79cfcaaa09372d04e69e60e2bf829bb74249782b5c28826`  
		Last Modified: Sat, 01 Feb 2020 19:14:34 GMT  
		Size: 10.9 MB (10933935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e665ecd4edbee998fa55d04d8629974e0da14b478ba821db4e2a9cda1bcf25`  
		Last Modified: Sat, 01 Feb 2020 19:15:22 GMT  
		Size: 59.8 MB (59801015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662927948fd7f5b1206f57f8c1e950eb28862902e46543b4635806ca9d09a824`  
		Last Modified: Sat, 01 Feb 2020 19:16:57 GMT  
		Size: 205.9 MB (205853427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:ab7617cda1a4efb7b267f4d8c15197cd725b465b5fd00444073015a1f933e262
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **301.6 MB (301623222 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3eda77d7d1465a41e81007dd8b703031e609c6d9157a79e23b13aa9fe37df55d`
-	Default Command: `["bash"]`

```dockerfile
# Sat, 01 Feb 2020 16:41:48 GMT
ADD file:cce6a1a9e391072489b92618430aad507d896a0892b4ab746b46f65aeb50e142 in / 
# Sat, 01 Feb 2020 16:41:50 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:47:55 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:48:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:48:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:49:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:821c3e818de5d8d85868e03fa7647e09cacd5ec4fc251a32c8469652dc6a136f`  
		Last Modified: Sat, 01 Feb 2020 16:45:08 GMT  
		Size: 50.1 MB (50133126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf95eab022dfcbfcacdc7e34c79e2393c47272871cba3199d2f185d32eed6346`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 7.6 MB (7592340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3fc4d83f881a25a8f4d4dbecfe9212342061b813cb745e8c7fffaa872c5ce04`  
		Last Modified: Sat, 01 Feb 2020 18:02:40 GMT  
		Size: 10.1 MB (10141537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddb6114085d29f6feadc52b85130bb556649dad85820b38ee5a001c7aaf15842`  
		Last Modified: Sat, 01 Feb 2020 18:02:53 GMT  
		Size: 53.8 MB (53804304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fda09474751f4fa484b95ff4301ce498089bba6071b9a170113a87c2505db2`  
		Last Modified: Sat, 01 Feb 2020 18:03:44 GMT  
		Size: 180.0 MB (179951915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
