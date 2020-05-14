## `buildpack-deps:testing`

```console
$ docker pull buildpack-deps@sha256:5b730c666b58eaecb8a231dc6a51e8df1e60e913a8301cfb0d4effe6a3d6101e
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
$ docker pull buildpack-deps@sha256:7635e15b2a6151ca03c50893536dd315e463d85e782c28cd5f12ab528ace56ef
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **323.7 MB (323747572 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b362ed24becf86f835368e07873f6523c0ef16f51252938bc530e0b5928fe6c9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:19:45 GMT
ADD file:19778292422b784c4eb17d79e7632fc1e3619b6bbbcf16a37bb6179a5c725b1b in / 
# Wed, 13 May 2020 21:19:45 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:25:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:25:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:26:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:27:25 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5ce4ab219a2f8bc551eb2502df5b719a1d8a32c4bbb00b3629001ebb6c5e0b94`  
		Last Modified: Wed, 13 May 2020 21:25:41 GMT  
		Size: 51.4 MB (51384672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f458d7d6918561d3665fcf7c6a15ac5f015d15f94fe4c18152b31a6b390477d`  
		Last Modified: Wed, 13 May 2020 22:43:48 GMT  
		Size: 7.9 MB (7934430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a19396f1ca9e830aec22ccedc673036a5d9fa5707ad170217dadb18689b7f61`  
		Last Modified: Wed, 13 May 2020 22:43:48 GMT  
		Size: 10.5 MB (10463198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:131834a7118626dab711b9bd62471ab667200154b199826ed2ae74c2733ea3e2`  
		Last Modified: Wed, 13 May 2020 22:44:10 GMT  
		Size: 55.7 MB (55658350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ef9101bc45d641716eea2e2782e37c10b0dbfa4ad403ad65a6d7613364fd2c`  
		Last Modified: Wed, 13 May 2020 22:45:00 GMT  
		Size: 198.3 MB (198306922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:c01dbef4ab6f64499710b19b9df7f7dbb70c92fd63e5e5854a37f098fb6a916a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **295.2 MB (295155045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:583d5a47d280ec03b087e3f89e0a39781759394f6e56bdc2b0b721e1b5414849`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:48:54 GMT
ADD file:e9c6ac7bf8b044473fb44adc857ae60fa2e57fd69c08908b01eef97b087e3aaa in / 
# Wed, 13 May 2020 21:48:57 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:25:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:26:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:27:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:30:54 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:320cb68d32ad923f9944bd8a4839f75e3e1b446fca01a999d67c9a756e55e632`  
		Last Modified: Wed, 13 May 2020 21:58:23 GMT  
		Size: 49.4 MB (49358454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba87e7b395f65b77fc7adc10d5b082bf26da938cfc39952a2c778fefe01abbb`  
		Last Modified: Wed, 13 May 2020 22:53:37 GMT  
		Size: 7.5 MB (7514341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cbc2e3e25ce7b85de9e1d951a3097b9fce980d94c1f8057796afe92a9caab58`  
		Last Modified: Wed, 13 May 2020 22:53:37 GMT  
		Size: 10.2 MB (10157745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c30dd7626fa8f7db8c898aa5539da563d7599d5f8b5a67074b71bd6bd58f2054`  
		Last Modified: Wed, 13 May 2020 22:54:02 GMT  
		Size: 53.3 MB (53295562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7c4e982b8388785b84fc6ce9f9fca37fad45ec6ffdfed6d5cf40d0d8240650`  
		Last Modified: Wed, 13 May 2020 22:55:02 GMT  
		Size: 174.8 MB (174828943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:b4cabca29e9dda0f83ab4ee61f6dd364041fb1761311c76b7730347c5e95bf80
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.6 MB (289560585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7b84f3dd66c71d6ede13ce7f918914fc720a0ce9186fe3cdccbb6f2fb0449e`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:12:36 GMT
ADD file:6043fa3a64fc1fc92478b236dc9d857c2a161dafe05b2c17c95d16215a7488fa in / 
# Wed, 13 May 2020 21:12:40 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:51:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:51:27 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:52:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:55:44 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e3d0ed714eb8acd6cc43ddf13830c6dbe31523db4962134b70f31da0774c2de6`  
		Last Modified: Wed, 13 May 2020 21:22:37 GMT  
		Size: 47.2 MB (47162349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9410321c9d6846391c2c00276788966a82b6c2f4e1cbd96f8417d39b2668cc8`  
		Last Modified: Thu, 14 May 2020 00:18:46 GMT  
		Size: 7.3 MB (7257008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c897e7828d6f38dbee8e4f232bdd8c3fa793f6b47f6f6c5475f1129bf3abdaa3`  
		Last Modified: Thu, 14 May 2020 00:18:46 GMT  
		Size: 9.8 MB (9804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:189988b527b263cb4274855818ffdd3c0935715297ef16f2774cf9572da73ee2`  
		Last Modified: Thu, 14 May 2020 00:19:08 GMT  
		Size: 51.1 MB (51080528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3940c420b4645e4ba34be9306014b718483b40726e66ecfefe7bd3f221a1192d`  
		Last Modified: Thu, 14 May 2020 00:20:04 GMT  
		Size: 174.3 MB (174256072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:88f31219ca47a6aa978648e39d1128b8853932ccbddff72145b8f808f5ed6d11
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **315.7 MB (315681707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4ec611dd64d1c036b5edabfc4a13e9b2f69bcaf9c2ce2c379eb6d22b00d0ef1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:52 GMT
ADD file:642f1f8b3928c38913b91b5770e5ef77e0467db31d0e7342848c66b97b0cefce in / 
# Wed, 13 May 2020 21:41:58 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:19:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:19:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:20:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:23:19 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:da14fdea4bf7eaa36b82ecde9ee461379c7eb32fac279c7d1bce1452edd5bf2f`  
		Last Modified: Wed, 13 May 2020 21:52:10 GMT  
		Size: 50.3 MB (50328349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d18f3d952fdbc982edca77fab71409bebc6a0b410a5f13ffe6fd2685b6020c`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 7.8 MB (7809463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:382abc5b67b7c0e46916f728a90e7aa0866070c3a67e581de6b5904092e6ca45`  
		Last Modified: Wed, 13 May 2020 22:38:11 GMT  
		Size: 10.5 MB (10459917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b30ad6c82e2b7a536da67a837bec581308704d1e15eaf6e92c24578b56e187d9`  
		Last Modified: Wed, 13 May 2020 22:38:32 GMT  
		Size: 55.8 MB (55803040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12f9ea2188013c93873ab0b43ec267f4b3fce432d19b3fd05e94e773d13bf4`  
		Last Modified: Wed, 13 May 2020 22:39:31 GMT  
		Size: 191.3 MB (191280938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; 386

```console
$ docker pull buildpack-deps@sha256:71e0daa3caa543ff6a2be8d3e9518983851c1c338b2bebf18ddb500c998cdeac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.6 MB (333573934 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:879dac49a9204fea39d3c6fbbde228fcf0c9cc11ae5e8e59ba9f025a42a99022`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:38:36 GMT
ADD file:ad345e25a8b64e5d96a8875a8c7eceb747745ed11d495c0de132b2a33e48e29d in / 
# Wed, 13 May 2020 21:38:36 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:39:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:39:35 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:39:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:41:15 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:424ac85ac099fddf73c8eff4a7e1e7a3ad318011cb2070285233ed10f3794d6f`  
		Last Modified: Wed, 13 May 2020 21:44:40 GMT  
		Size: 52.5 MB (52480291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80cf73924a61888429404a98bf52d320053b3f0ae8798a7c67213f15e472cc5f`  
		Last Modified: Thu, 14 May 2020 00:00:27 GMT  
		Size: 8.1 MB (8112084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1954931eaa7cbd6f17b8d579de74c26f37b042c1f3ce12b5d23001279df88d72`  
		Last Modified: Thu, 14 May 2020 00:00:27 GMT  
		Size: 10.8 MB (10841303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f332097843cd69961a7ff7436166d07cb2effed696640def8da3aaf7403af379`  
		Last Modified: Thu, 14 May 2020 00:00:49 GMT  
		Size: 57.5 MB (57517925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a267afca9bd993ed9d4b40d8223ebc03ba9ffbd85f11b8bdad3b99c996e4c0d9`  
		Last Modified: Thu, 14 May 2020 00:01:48 GMT  
		Size: 204.6 MB (204622331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0ea97ac1e43e2102c0a2e82fa410c1ac981db98a686cd1f910d131a388d8774b
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **306.0 MB (306001465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4bddebc6e5cb871a29dc964bd839f1d8c59a261873d0333e5a785fc6e0aca970`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:47:32 GMT
ADD file:f2d8d152f2c12223430241ba470d074182fc4071fbe07696ef9a7ac73d7e31c8 in / 
# Wed, 13 May 2020 22:47:33 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:50:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:51:19 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:52:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:56:31 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9fe8ffba560af94cfc9c2199a294b5143a198e0cbe44469cb586e1986f063ea`  
		Last Modified: Wed, 13 May 2020 22:55:41 GMT  
		Size: 50.1 MB (50131081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0640353f1b9db4814a57a569a8417ac7dca26baae0a3342a2575bad188f9e2d`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 7.5 MB (7460937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ce2184377077db50bd5cfbf56505a742cce1db802c2fa42946c103a34a61969`  
		Last Modified: Thu, 14 May 2020 00:11:53 GMT  
		Size: 10.5 MB (10484779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648af14339d9e6a970776b9e7d360437621c1a759c25c603b49426eb0a234705`  
		Last Modified: Thu, 14 May 2020 00:13:18 GMT  
		Size: 54.6 MB (54597041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d7d42bb62001330948795ae948b127672b4fdb31ccdf0f61607751bb12e4e1`  
		Last Modified: Thu, 14 May 2020 00:15:44 GMT  
		Size: 183.3 MB (183327627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eb8b0234f630adc76ecdbf65aa9b9f45e295f8a111ec6e1932197ba88e65a1eb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **343.1 MB (343128137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdbf9fc05e4f527f8a86883252cf6e199ee9e6cdd5a17ef6ce16fef352abe567`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:16:05 GMT
ADD file:890f814706ea242af3d8f4b729aed7d590611deabe25d4adae7468f0058d7a4c in / 
# Wed, 13 May 2020 22:16:10 GMT
CMD ["bash"]
# Wed, 13 May 2020 23:29:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:30:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 23:32:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 23:42:16 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f2f9956082054d1fabd5ea1a9e08b145fa7f68b93b5601b36e05386466487664`  
		Last Modified: Wed, 13 May 2020 22:56:07 GMT  
		Size: 55.1 MB (55110307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9e43969f6c0ff55aa4240214980deed196b68292106e0144d8d1290495d9b7`  
		Last Modified: Thu, 14 May 2020 00:25:02 GMT  
		Size: 8.4 MB (8356860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eacce9e1d274d8f139e9d384ceb5e66a86ca1857d025523765b1b099330719b`  
		Last Modified: Thu, 14 May 2020 00:24:57 GMT  
		Size: 11.2 MB (11176806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12dd448830e6ab4491686ac42b85cc8f50e9b182a8b19722842140e7e06c1af`  
		Last Modified: Thu, 14 May 2020 00:25:53 GMT  
		Size: 61.0 MB (61049897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:394e509d495da37eb010696bb333af1093f653da43115bc762475c7d7b145b1e`  
		Last Modified: Thu, 14 May 2020 00:28:34 GMT  
		Size: 207.4 MB (207434267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:testing` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b88d11833f6e177b8bcbf1dd5f86cc64a2dbbbb0e3571740e64f1686c8a610a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.6 MB (304558726 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2746386a823c70b1c7ce44d30cfd66cc9db0d3492b1e6487093822358b44ab16`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 21:41:47 GMT
ADD file:fbad911feb95f3e7b45e9aa72be8710716eb8fbf3ba846fcaea87309eb9ba2be in / 
# Wed, 13 May 2020 21:41:49 GMT
CMD ["bash"]
# Wed, 13 May 2020 22:37:14 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:37:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 13 May 2020 22:37:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 13 May 2020 22:39:33 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9ac9db0ba497fe825137b138e8deceb06a532f1ba6b367b8e68834caedf8e442`  
		Last Modified: Wed, 13 May 2020 21:46:15 GMT  
		Size: 50.0 MB (49994654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160b7562ce5394b96e6b7064989f4900b8d47965a7aab9b7f344e8f1514b24d2`  
		Last Modified: Wed, 13 May 2020 22:47:29 GMT  
		Size: 7.6 MB (7600664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b048fed0769ebce58b27d4fdbbae456c1810f6b85546360e3b80e36bb4be9d4`  
		Last Modified: Wed, 13 May 2020 22:47:37 GMT  
		Size: 10.3 MB (10347812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1e2837c528350ba56db4cda999ef6e93553ecf1d30819aa7eb54b31808155e`  
		Last Modified: Wed, 13 May 2020 22:47:50 GMT  
		Size: 54.9 MB (54900683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de18e2a5be7ad42c6500897b71704b2568498670ba5073c55dcbb9c2e1d04df3`  
		Last Modified: Wed, 13 May 2020 22:48:17 GMT  
		Size: 181.7 MB (181714913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
