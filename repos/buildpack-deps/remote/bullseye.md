## `buildpack-deps:bullseye`

```console
$ docker pull buildpack-deps@sha256:fff779972b1bc7ca422e20e656c3b0ed4a41c444f1760aac17538b52d2bca397
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

### `buildpack-deps:bullseye` - linux; amd64

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

### `buildpack-deps:bullseye` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:1028d636dfbc80413d3240a7019cf9a7e4b824ade6eece361ae0432fa30c69fe
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.3 MB (294345991 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bdc6935dc7d9b2db8cd00c60a12524a115ebab6a80d7928392780f8d3ff43f1`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:25 GMT
ADD file:cd3f4cae9b31b83faef159941db546ad620281a9de9ad8b4c2e2230e329f629c in / 
# Wed, 26 Feb 2020 00:46:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:30:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:30:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:32:05 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:35:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b5f1b944f6f81b9832613484a0ab69b94fc4d7e69cec7cf9246276a84f198955`  
		Last Modified: Wed, 26 Feb 2020 00:58:09 GMT  
		Size: 49.9 MB (49859431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2309dee70eab6e2c15144731cd3a34dc25e8045f43ccebd56bca46a938673eb9`  
		Last Modified: Wed, 26 Feb 2020 03:59:01 GMT  
		Size: 7.5 MB (7497952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ebfbc2424c96e6f6b0bd4ccb126243789b984e1df82dfcc07372cbdd3c2ec46`  
		Last Modified: Wed, 26 Feb 2020 03:59:03 GMT  
		Size: 10.0 MB (9974390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aba36494b890743c5415594ee83949a59b8e97262545880ca23c5428e07c583d`  
		Last Modified: Wed, 26 Feb 2020 03:59:28 GMT  
		Size: 52.6 MB (52597859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2303a8ee26125f67cb9709860f190ae5d28b43de99a2fa438b08d624631fbe`  
		Last Modified: Wed, 26 Feb 2020 04:00:26 GMT  
		Size: 174.4 MB (174416359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; arm variant v7

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

### `buildpack-deps:bullseye` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:20d94de1435af732b206400d6dd6f40336bad4bc8ed01997bfa872e56a0306b0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **314.9 MB (314913682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e09bab82a76076c1962be7388bfd21d34b233215b53087020006392628fbe57f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Feb 2020 00:45:20 GMT
ADD file:6771f02669c2a4d080cd86fa10f39851d26351e4a29f9ff3d63a76e1865f96ad in / 
# Wed, 26 Feb 2020 00:45:22 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:45:36 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:45:52 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Feb 2020 03:46:38 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:49:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f822750796cfd016baf6c8125f67a171683174c26da351c46b78a6cc9d234372`  
		Last Modified: Wed, 26 Feb 2020 00:55:10 GMT  
		Size: 50.8 MB (50808549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f2d34813aa8b1aea79c2e14a664c47e0950cb8413f1af463215020fbe6ad26`  
		Last Modified: Wed, 26 Feb 2020 04:03:59 GMT  
		Size: 7.8 MB (7797144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74820b1316f035b3f4e91222feb71d75980d5a8b243cd3ea1a4ef519acca4774`  
		Last Modified: Wed, 26 Feb 2020 04:04:00 GMT  
		Size: 10.3 MB (10252863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a934273fe78141239ebcd7f15bd23d865d400ab5e8f9a91732fa22672bd4308d`  
		Last Modified: Wed, 26 Feb 2020 04:04:23 GMT  
		Size: 55.1 MB (55124898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ef0773851157e2e0c420349d0e49d160217a749dfa20214808ad4ea46b9d8d3`  
		Last Modified: Wed, 26 Feb 2020 04:05:16 GMT  
		Size: 190.9 MB (190930228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bullseye` - linux; 386

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

### `buildpack-deps:bullseye` - linux; ppc64le

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

### `buildpack-deps:bullseye` - linux; s390x

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
