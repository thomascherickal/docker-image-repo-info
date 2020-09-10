## `buildpack-deps:oldoldstable`

```console
$ docker pull buildpack-deps@sha256:4202c7c08dc366510b3a07a0fa4c6926da8484dcc99ea284a1ee1df78810463b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; 386

### `buildpack-deps:oldoldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fbf16e7c228db3727647bc52ce90282796f698686ab562606c70f7e0c5091c1e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **247.2 MB (247182744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d819310eca30be6edda7ec0950a0c1c6de826521911c986443971f283fc8415`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 10 Sep 2020 00:24:00 GMT
ADD file:ca64ef47722e4bf4beeab729a34cd854fe7293a0a2a0a2a92e6f1347c071dfe9 in / 
# Thu, 10 Sep 2020 00:24:01 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 01:03:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:03:09 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 01:05:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 01:08:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:290431e500161a90ac38ac8631791acb27e14a913613b60b3df58f839168df40`  
		Last Modified: Thu, 10 Sep 2020 00:34:21 GMT  
		Size: 54.4 MB (54389019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcaf1dd00a337044e2c0421947b13d7390883ef55a08ff9ea58d13ce59784328`  
		Last Modified: Thu, 10 Sep 2020 01:16:59 GMT  
		Size: 17.5 MB (17545982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:478d2f36706aba42a38a1d269f4e5f9e733730c04955e96a04d508b1cd9d589f`  
		Last Modified: Thu, 10 Sep 2020 01:17:17 GMT  
		Size: 43.3 MB (43334104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a94a50b39f16528d3bf36d3579aaaa7375c54edffd686c944f42b151b2476d`  
		Last Modified: Thu, 10 Sep 2020 01:17:51 GMT  
		Size: 131.9 MB (131913639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:b5d788b26b95577fb583f21d5cc5e1015edff05bb9a2b83852e81ab3db98bada
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **227.2 MB (227154588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43e1237c5e76f0169bb6d2ee5cdd480c2a64976d0db2778b2dc202a4ef18021f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 09 Sep 2020 23:54:15 GMT
ADD file:b5770ada526014c416df31779f0c640c62a5e53e8e018a6201d507999ac34e18 in / 
# Wed, 09 Sep 2020 23:54:19 GMT
CMD ["bash"]
# Thu, 10 Sep 2020 00:37:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:37:12 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 10 Sep 2020 00:38:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 10 Sep 2020 00:42:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:82ebff95f0e21d655344637482b367c7ea0db41b80cbc667bd980d2141287029`  
		Last Modified: Thu, 10 Sep 2020 00:03:15 GMT  
		Size: 52.6 MB (52583713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f40e46cda9c751ff385c796d48a3c39740220c3885866739fe62640f9437afa`  
		Last Modified: Thu, 10 Sep 2020 00:55:04 GMT  
		Size: 17.0 MB (17037321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9bd6814b5011e45af4aaee011465ebcf614eef4d29dab5a87d8a3fed3655f0`  
		Last Modified: Thu, 10 Sep 2020 00:55:28 GMT  
		Size: 41.2 MB (41155851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793f4aaab1b4b812ca4076ce91369874ff9de166e35aca03da1a7b38341b8b19`  
		Last Modified: Thu, 10 Sep 2020 00:56:25 GMT  
		Size: 116.4 MB (116377703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:a10ed8edecb70247adca081ac14a8ef96e6680a1a90e98d06f1214dc04fb06c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **221.4 MB (221441863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45e0c02f75032cc2ae8fe909c341fecac152cc2425996324af0db80bec407bd1`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 04:57:16 GMT
ADD file:1b4bf8acda0b906341b6a17ca6eccc23744ba196c78c5bc59c3e26d0b2ebe596 in / 
# Tue, 04 Aug 2020 04:57:18 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:00:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:00:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:02:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 01 Sep 2020 00:17:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7c58b357cec76336de1011b56cc2999a53017c6a4b3cf93f2b8362b7a055c544`  
		Last Modified: Tue, 04 Aug 2020 05:05:41 GMT  
		Size: 50.3 MB (50305564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f64410aa4323d878bbe3be9802befcd90ffd5681624e0e325a80f25a038fa6cc`  
		Last Modified: Tue, 04 Aug 2020 08:27:38 GMT  
		Size: 16.7 MB (16723645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff21f785d375d1e97b8335d239d9cfbfffe0b0706afae0679ffd7f6c202157`  
		Last Modified: Tue, 04 Aug 2020 08:28:04 GMT  
		Size: 39.8 MB (39778943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd64843fe227c124340b00a6f9b25d333edafcb3e9799b51ad043abda75f96f3`  
		Last Modified: Tue, 01 Sep 2020 00:35:15 GMT  
		Size: 114.6 MB (114633711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldoldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5a576450d4dbacdda87cc1fc53365190a4c0ca45ee70ba4d09673b5f7d3e07ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.3 MB (254342842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbb022d22f27e9fe0286f991f8c6b65ce8e2bc4239ae96d311ac7443e59cd5d9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 04 Aug 2020 03:37:49 GMT
ADD file:85c105a2f2f0c7bff57c73bff9ecdb5ae2cb04074a0129fc1a82d4da85b95ec0 in / 
# Tue, 04 Aug 2020 03:37:49 GMT
CMD ["bash"]
# Tue, 04 Aug 2020 08:11:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 04 Aug 2020 08:11:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 04 Aug 2020 08:14:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 31 Aug 2020 23:45:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:49a2d30c774cb18fa05d4cb6f730f97f4965b1162debd13f35bf1733bb737735`  
		Last Modified: Tue, 04 Aug 2020 03:42:50 GMT  
		Size: 54.6 MB (54609569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb76cc7bc12f41ea0e34f0355c0a2d2c5689a14b42947760e1caf7b92ff80dc`  
		Last Modified: Tue, 04 Aug 2020 08:27:50 GMT  
		Size: 19.9 MB (19855978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d975d21db51982cf56382647589c692e4b2d94ca28355895c5bd8514ad38b0`  
		Last Modified: Tue, 04 Aug 2020 08:28:07 GMT  
		Size: 44.0 MB (43990467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a65a23076ba7258f89aa266e6fd26d1fc57d4dc97782ce8a289d92c06d815d5`  
		Last Modified: Mon, 31 Aug 2020 23:50:42 GMT  
		Size: 135.9 MB (135886828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
