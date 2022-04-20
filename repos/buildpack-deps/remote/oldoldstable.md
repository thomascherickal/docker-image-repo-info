## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:864754aabaca527de9f9fc6b3ea3eee920bf02a8c2c0baf2c29d85525dd0bdec
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:923c1a6fcd1ba83732294a6a2bc8545fcb69c19ec1e0468220076c5a49a0480e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.3 MB (325315541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c719bcd09aeb96380650107fd41c848663f91d941a3d5126585cf69f960599f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:45:14 GMT
ADD file:6ed691b65385dede44a92f9de9e1428af431197c66461aa0f9c61e2f7c8bade5 in / 
# Wed, 20 Apr 2022 04:45:15 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 07:01:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:01:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 07:02:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 07:02:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f5196cdf25181bc7e4411865a2e002932b7b6b0ffce787c04c1bdeaf1f204f20`  
		Last Modified: Wed, 20 Apr 2022 04:52:01 GMT  
		Size: 45.4 MB (45427434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bed1e86f01ee95c76d2c8b4385a47ae336e6d293afade9368469d99daa9369f`  
		Last Modified: Wed, 20 Apr 2022 07:09:06 GMT  
		Size: 11.3 MB (11302268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44e4bdb3a6c1325cc4d40e585ed7a759127c0c87b0388ec0236b1698827d70d`  
		Last Modified: Wed, 20 Apr 2022 07:09:05 GMT  
		Size: 4.3 MB (4342835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f75d131f4060950dd6cc1f580e2fa5504ece8d692113a9cdb0a866637b397d7`  
		Last Modified: Wed, 20 Apr 2022 07:09:24 GMT  
		Size: 49.8 MB (49765440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07dff4ad21ebdb3ce3e329699663b2f81af70152453025f6624584a39a8e22b6`  
		Last Modified: Wed, 20 Apr 2022 07:10:02 GMT  
		Size: 214.5 MB (214477564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:ee6ac31fb99a390c715a3384a89aed4487c0ce2f777619762ac31a3540478b72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.2 MB (309205626 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29be7888d43dd948d6a70c751f17bf90f533643c9f72cddf187ab65ae7c95e2e`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:55:32 GMT
ADD file:4e79cc43996ddc8062073aea4d6352c3ca3c736e9b09f1eb440f913d5a52469d in / 
# Tue, 29 Mar 2022 00:55:33 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:56:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:56:26 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:57:22 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:00:07 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a58c023b263eaa1973763831b149ed127bbe67ee8cae67d60e261db1e9d54b63`  
		Last Modified: Tue, 29 Mar 2022 01:12:11 GMT  
		Size: 44.1 MB (44123307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c0117421f3f6b9a01b30e38d3562bc7a42dc789c5af5f80877e67cd59edcb5`  
		Last Modified: Tue, 29 Mar 2022 08:14:25 GMT  
		Size: 10.4 MB (10352487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c612024a40834a1cb0833f65b0e86ed44bcd14476cd83a108eca13607211c477`  
		Last Modified: Tue, 29 Mar 2022 08:14:21 GMT  
		Size: 4.2 MB (4162114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85145e2987592dd2778a62d3efaf2f38a56d30e11db945369406880db586d665`  
		Last Modified: Tue, 29 Mar 2022 08:15:12 GMT  
		Size: 48.0 MB (47988329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0de54a15c10429cb5d84993513d686a21126831f18f7735ed5da53623182d57`  
		Last Modified: Tue, 29 Mar 2022 08:17:18 GMT  
		Size: 202.6 MB (202579389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:9e414286b18c5acce0c1d74567a63743099512a091c4aabdd1f7964e2abd5382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.2 MB (297239215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5f3b80599dd935351f446edd2216d87dd723322b41418d9c7d5a6d105e1b69c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 02:23:57 GMT
ADD file:3dc1697adfcf63a288e9ec7a2c40438b8ba2ccfff0382a1ed5457f30d7a37f76 in / 
# Tue, 29 Mar 2022 02:23:57 GMT
CMD ["bash"]
# Wed, 30 Mar 2022 20:17:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:17:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 30 Mar 2022 20:18:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 30 Mar 2022 20:20:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:aecfa9e0b0179abf68bebbcfc35453928546e01ad1c8b6eaadf759360762dada`  
		Last Modified: Tue, 29 Mar 2022 02:40:33 GMT  
		Size: 42.2 MB (42151158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc36fcf6b269b843685f3e40183609c9ee393c766145d636666727cc97069e`  
		Last Modified: Wed, 30 Mar 2022 21:38:43 GMT  
		Size: 10.0 MB (9956889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e13cc08b3e8cd7b26260c7597b624d4a45ebc2afb89bb5da193fc824ab69e55`  
		Last Modified: Wed, 30 Mar 2022 21:38:39 GMT  
		Size: 3.9 MB (3921802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842f17f357dbe1ebb8ad0508d83e0bcbf9dd99dd8dc3a9084a153a6c61aec7fe`  
		Last Modified: Wed, 30 Mar 2022 21:39:26 GMT  
		Size: 46.1 MB (46128132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beb172af1ac83eb71aebd908e9027d52767f1d16428e26df4d6cfed89cab71b4`  
		Last Modified: Wed, 30 Mar 2022 21:41:29 GMT  
		Size: 195.1 MB (195081234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:44d5e714e2463d6212b195884ae246fecf4500f95b308de0bf0745a25da37d73
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.8 MB (306839082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28dcc087a39b2790ef0644bf016ba0413fb0a882c2659fc2df8410097bea4d07`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 04:31:19 GMT
ADD file:73f1db8536438ca891f4b507a569e6c561364db0f05914ebea9d3fa97e1bf837 in / 
# Wed, 20 Apr 2022 04:31:20 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 06:48:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:48:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 06:49:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 06:49:58 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a41fbedfa4b1547a2b4fea33de48af745d66a94741d3cf344cb2766f0e80211b`  
		Last Modified: Wed, 20 Apr 2022 04:39:38 GMT  
		Size: 43.2 MB (43212018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a94d3b1a91a1952461644c0005791faf07bf7c6b042272a89113ec795a493d4`  
		Last Modified: Wed, 20 Apr 2022 06:57:40 GMT  
		Size: 10.2 MB (10217775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad88c3c2eedd19cb4e591bedf0013f98bd12344b922299e40887a253d50de12`  
		Last Modified: Wed, 20 Apr 2022 06:57:39 GMT  
		Size: 3.9 MB (3874445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67f90700f5859b0f6187aad3354827bb2b243385f8e4af17fbfd2f81f4867e1c`  
		Last Modified: Wed, 20 Apr 2022 06:57:58 GMT  
		Size: 47.7 MB (47736126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48979b276d7f5d48373126bb88786dfff3c3be121e1102d374ea3cf0b6147dd9`  
		Last Modified: Wed, 20 Apr 2022 06:58:37 GMT  
		Size: 201.8 MB (201798718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:59f638802b06e586ef29a622e97c09674badf016f7f665c0a3223d6847f6c0c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **332.6 MB (332615979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:59d0a8a93a07b44bc38e2d38380f78de1bf325b654fba117ff8332e2e9abc0bd`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 20 Apr 2022 07:39:57 GMT
ADD file:e8c6a60834ed931ccc3c93b1f2c9b9ca2bf190b0d8d2474382ee8e96a7e35b5a in / 
# Wed, 20 Apr 2022 07:39:57 GMT
CMD ["bash"]
# Wed, 20 Apr 2022 10:22:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:22:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 20 Apr 2022 10:22:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 20 Apr 2022 10:24:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cd343d4c0c2fbc67ddea33155621bdf36074fc30ffb6f917e716fbb81645f79a`  
		Last Modified: Wed, 20 Apr 2022 07:48:48 GMT  
		Size: 46.1 MB (46147730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b0c0f848ce870a8686c5b8c6c955359aa284d4e35847ab4c25247e6ad8c855`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 11.4 MB (11358258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:256ca979e8a7a5453cdea6aeecd54c837a03c2c5c037a42ef4cb105a69783071`  
		Last Modified: Wed, 20 Apr 2022 10:31:02 GMT  
		Size: 4.3 MB (4342300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a961561bfa0a5f6fe20a1be17bed015e78fa2cb53a6dfcc0b2b11c2201384fa`  
		Last Modified: Wed, 20 Apr 2022 10:31:21 GMT  
		Size: 51.3 MB (51268708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9942d02cc63116d997915365bdde816a3c783495666add28bb572856bd0b21cd`  
		Last Modified: Wed, 20 Apr 2022 10:32:03 GMT  
		Size: 219.5 MB (219498983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
