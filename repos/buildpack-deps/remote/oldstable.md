## `buildpack-deps:oldstable`

```console
$ docker pull buildpack-deps@sha256:dce59d5e483272f2b8141f4e1be3bcabce396fda811ffd137f401d629dc85fb8
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

### `buildpack-deps:oldstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:55a13a9e94bcb109664c4ce618dc8fa542b9a2d1cd788305360d9ff80faa7937
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **325.5 MB (325455760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f755ddd86e2e64e5cb11d69e41690ecfde09261956cd2e81eeb988d39f422b4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:23:20 GMT
ADD file:6e16bc9cf28c19a1fb1fb516411643e33cbd2bdb7b6c2ce2468c6583c89871a2 in / 
# Tue, 09 Jun 2020 01:23:21 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:56:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:56:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:56:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:57:41 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:81fc1918191541a2ffb6ed1cd8386ef8302aea1b0613ebc768a00e76c1f34bb9`  
		Last Modified: Tue, 09 Jun 2020 01:27:59 GMT  
		Size: 45.4 MB (45375796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee49ee6a23d1c7e6b8b574c905dcd4a53efb869a539a957d3e47bc3698f01dc8`  
		Last Modified: Tue, 09 Jun 2020 02:02:39 GMT  
		Size: 10.7 MB (10749020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82851092453815ec861754ded7101fcfa3b648d09a0818ced17ea80478f179a3`  
		Last Modified: Tue, 09 Jun 2020 02:02:38 GMT  
		Size: 4.3 MB (4339890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f58c4fcca04f9622e97db77618075b618c24a58cce6c6860ca54c9a887745b`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 50.1 MB (50082718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33699d7df21edc5ded5b679bc283e5890ed92c5bf20e53b48edcd9096c8a5962`  
		Last Modified: Tue, 09 Jun 2020 02:03:29 GMT  
		Size: 214.9 MB (214908336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e9642b91e66e7d49d94e4518f5ebc60c72315e456bf7c9346ff4ad371774df97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **309.4 MB (309439845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a79aaf2a6d41fcf4d8e74fd6d8361702726054cfe603dc2a64e1f12284746344`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 00:55:26 GMT
ADD file:f75089c5817628b287da52c6067110dff0b6f4efb6fecf5feafa8e2daea1fecf in / 
# Tue, 09 Jun 2020 00:55:29 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 01:50:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:51:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 01:52:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 01:55:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc933a187a21289c01459e983ea69dee29bfb61a3aa7a3a8ae010865977afb50`  
		Last Modified: Tue, 09 Jun 2020 01:02:51 GMT  
		Size: 44.1 MB (44069276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68c7016c4c1d54a8db75f1447c8c65687212f5e02de9f8e71e96be5abfb19eb7`  
		Last Modified: Tue, 09 Jun 2020 02:02:28 GMT  
		Size: 9.8 MB (9822538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f44c27923f5148de038dcd58d2b75b2ecca861b7107bfc51bb816b60c3b0f2`  
		Last Modified: Tue, 09 Jun 2020 02:02:27 GMT  
		Size: 4.2 MB (4158984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f7ae1f234399a8d90f81be560a4083dd91474c8d9c8e1e1c2b60792951bed5d`  
		Last Modified: Tue, 09 Jun 2020 02:02:52 GMT  
		Size: 48.3 MB (48305440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd08eb1370e2d5955e3abb6c394a6615d87b1142eb6953c577ac5a583e7295a`  
		Last Modified: Tue, 09 Jun 2020 02:04:03 GMT  
		Size: 203.1 MB (203083607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:dc1dd9fcc86b14c5d80e78e29862328bfa8adbc5b578b5effe24c52f8b44bf76
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.4 MB (297444474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:29cdad7efddd4dd63dbac784a6727e4bdbe27d05d697faff6bcba7503a80342c`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:06:07 GMT
ADD file:c0b9ed1244ec0acfc9054c7cb80c768878e3da99740f981ba3a82bdd854305db in / 
# Tue, 09 Jun 2020 01:06:09 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:02:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:02:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:03:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:20 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2566ca784846d2d0d4f9105084d94d68d8ea1a82a06a76c5bcd991ce5a10cda1`  
		Last Modified: Tue, 09 Jun 2020 01:13:35 GMT  
		Size: 42.1 MB (42102504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3f976b5a12722f5e6e115157695654d36452b713c7fa64a860f8c9e14859402`  
		Last Modified: Tue, 09 Jun 2020 02:15:15 GMT  
		Size: 9.4 MB (9443335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35142ef6ea6c722cd0397799ab151e5da354eabc784b3acef29def7fa34e9bc`  
		Last Modified: Tue, 09 Jun 2020 02:15:13 GMT  
		Size: 3.9 MB (3918433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773eda6b7a8801a6f09bd4ce443b7e88397ed16265ecd37f55af57db56c4658`  
		Last Modified: Tue, 09 Jun 2020 02:15:36 GMT  
		Size: 46.4 MB (46412697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbf8c80047f39ca1669cf85bbab477a59e35f498d269e058afe91bf9850b7c52`  
		Last Modified: Tue, 09 Jun 2020 02:16:37 GMT  
		Size: 195.6 MB (195567505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:2fd7911c8f47eb8eef0dbe40c1168966297ba8afebea39b587ec37a7b717cc27
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.3 MB (307324039 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a010d561dccab4798a529e53a4bd266c7a47ebcedaa93d93ac98f1748fba712c`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 15 May 2020 12:48:07 GMT
ADD file:251053dbd1ce0b3744de3eecf53a3ef8ccf92ea509678e59800952c3dbd1b32c in / 
# Fri, 15 May 2020 12:48:09 GMT
CMD ["bash"]
# Fri, 15 May 2020 20:13:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:13:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 15 May 2020 20:13:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 15 May 2020 20:15:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e144e997aec62ed9c3bb1ff83ae2a62cbea252858abfb48ac60bb2078817a6c`  
		Last Modified: Fri, 15 May 2020 12:55:43 GMT  
		Size: 43.2 MB (43163052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163052fbe4313f145cec99e4a4a1a7cc17d923a69c5354de191ecb396ef2a210`  
		Last Modified: Fri, 15 May 2020 20:22:01 GMT  
		Size: 9.7 MB (9748415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1173269921f10e4e86f34bf51752d9013d60db88a02c2dd476d5b8116e417476`  
		Last Modified: Fri, 15 May 2020 20:22:00 GMT  
		Size: 4.1 MB (4094349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693886e01d5a56a275694733a4d7bcf3854ae8ad4f5f789561237999e3e58498`  
		Last Modified: Fri, 15 May 2020 20:22:23 GMT  
		Size: 48.0 MB (48035115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53bfa0cbf65b2d83e4d7fde39e3884c9b88fae8c8c8f6ea03e3a24cc3d2c6f9f`  
		Last Modified: Fri, 15 May 2020 20:23:23 GMT  
		Size: 202.3 MB (202283108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:18759092ebd2bba4953eca3ab2a11cc5f64c4c384eefe6daf95b98a82e54c5d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.0 MB (333005450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06722fa3492225e28f91a91d4524f99fe611f0be5ce17d0eff2f4e450dac6d74`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:42:17 GMT
ADD file:6bbeeb0773b96fccb4cd5ba81dd19ec3580f8d8a3cdd3f1d6a3d2b514fbd6eb1 in / 
# Tue, 09 Jun 2020 01:42:18 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:26:35 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:26:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:27:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:28:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9e88f215fab896e3a7d1d2ce75c0d79960b236066e9033b97e76ca7f01ff2fdc`  
		Last Modified: Tue, 09 Jun 2020 01:48:12 GMT  
		Size: 46.1 MB (46094854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1130784446f3179c75741e18b159e7bca5d46db60bb1f9f57d67953023a50899`  
		Last Modified: Tue, 09 Jun 2020 02:37:03 GMT  
		Size: 10.8 MB (10772863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e32fbc0a9c533b460544bce821a796b4f02dd4da61100073a18fba329807ae`  
		Last Modified: Tue, 09 Jun 2020 02:37:01 GMT  
		Size: 4.6 MB (4561121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62e9df71276e8af2305be9b32aca4dd788168bd7fe3c6029ddd8e4e8057f7d33`  
		Last Modified: Tue, 09 Jun 2020 02:37:31 GMT  
		Size: 51.6 MB (51615859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c496d702f58d364bb0ec81531f18a35844eb95f0f9e0dff097b6588eaa8fb7`  
		Last Modified: Tue, 09 Jun 2020 02:38:54 GMT  
		Size: 220.0 MB (219960753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:1bf9f7a144ab9691ef3acb16a8bb8e112ee987d80ea523f3939c694d3a7c93ce
```

-	Docker Version: 19.03.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.8 MB (318815865 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:739719a006ad9234b87db3b81f124a183a429852a674f9b4d29c69a44fe006f4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:12:47 GMT
ADD file:de9470ab1a8469c3a824a48056d16d354ec41a887b8b0e6f7b13cedc73a3f316 in / 
# Tue, 09 Jun 2020 01:12:48 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:00:47 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:01:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:02:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:06:10 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:5fdce7db54786a0dce8a238fc9218fa25a9ccc5d0ac32920fd67f03f5571b347`  
		Last Modified: Tue, 09 Jun 2020 01:22:55 GMT  
		Size: 45.0 MB (45049756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffa9955e6182b5a1d2e59bd120f03d4bbf4c0e4c86773a33e7f98fea4f73a0d`  
		Last Modified: Tue, 09 Jun 2020 02:18:06 GMT  
		Size: 9.8 MB (9789501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2d1a085f35901bc4dc96d415aa9abf95233373a94aa4e89e20c50cd9fc6cb1`  
		Last Modified: Tue, 09 Jun 2020 02:18:02 GMT  
		Size: 4.4 MB (4394502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:968e741ea7d876279f8195bfcd9ef6e5eab8463b6e69fb92b9cb61225e843228`  
		Last Modified: Tue, 09 Jun 2020 02:18:56 GMT  
		Size: 49.5 MB (49475249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240b35a809489927e64f8c8276fd287dc6051053e7d4539a963f0c156904aba4`  
		Last Modified: Tue, 09 Jun 2020 02:21:40 GMT  
		Size: 210.1 MB (210106857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:fff8a5bfa64f261c8438acb6fb62d06b4974d2e76c754806bbefb6b44a22aed6
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.6 MB (320557822 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5eb0f6c84207946ea9d5d91863179e9272f9869a889d4e883066bbc4493803b9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 13 May 2020 22:39:29 GMT
ADD file:fa4c7e3ca04f092e53cc791a32c929663412df3f68de2733bb867053577bf1d1 in / 
# Wed, 13 May 2020 22:39:34 GMT
CMD ["bash"]
# Thu, 14 May 2020 00:08:16 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:08:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 14 May 2020 00:10:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 14 May 2020 00:22:48 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7732483b686efe14a1cf8add89a1568b83892e243798fba30808f1fc6287210b`  
		Last Modified: Wed, 13 May 2020 23:02:10 GMT  
		Size: 45.6 MB (45646193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df33ef5c6dd4781defd528815174987b67a617a4fbddd5e5241a2f67a34098cb`  
		Last Modified: Thu, 14 May 2020 00:37:47 GMT  
		Size: 10.0 MB (10002565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02507bd450f72bbb529f56f9579bb7169fc9be7900bc5b9b0587e4855e51ad8d`  
		Last Modified: Thu, 14 May 2020 00:37:41 GMT  
		Size: 4.3 MB (4296673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a5abe5a03ebb35ed027af57237427bf1650677f1d4c6a907f88cf889b5e403`  
		Last Modified: Thu, 14 May 2020 00:39:16 GMT  
		Size: 50.1 MB (50081278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e26879e4c99689db7dde317c0cef4c2586bcab4f29e2ca00e86e28101d2d88`  
		Last Modified: Thu, 14 May 2020 00:42:00 GMT  
		Size: 210.5 MB (210531113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:oldstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:166050211e2b14232f44b9326c18da1631efd9baafe405e6a1df2c8c36a7ceaf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **317.3 MB (317324665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a423fbc94a1ada04d0de1e579b1a6ffa709de2bbf411445d2a7dd1265cd159e2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Jun 2020 01:44:05 GMT
ADD file:ce4b8c76522cbe8599502985424901aee9d30d37296761d47dbcb9b0770f7aa2 in / 
# Tue, 09 Jun 2020 01:44:08 GMT
CMD ["bash"]
# Tue, 09 Jun 2020 02:13:24 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:13:28 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 09 Jun 2020 02:13:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 09 Jun 2020 02:15:38 GMT
RUN set -ex; 	apt-get update; 	DEBIAN_FRONTEND=noninteractive 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cc8faf537ff83acc994f80bcea99d8e073aa05b5eb0dab5ce495510af0b6d1f6`  
		Last Modified: Tue, 09 Jun 2020 01:47:50 GMT  
		Size: 45.2 MB (45232505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9816eeae17f469b3b58481bdbae04cc1b7b69f8d8a6ef15f6972d91ba2f29ee8`  
		Last Modified: Tue, 09 Jun 2020 02:19:43 GMT  
		Size: 10.3 MB (10280522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a7344ca59dab92a8238f2df0ea3779840ec21afc295e24f39259558c3bfc05`  
		Last Modified: Tue, 09 Jun 2020 02:19:48 GMT  
		Size: 4.4 MB (4372414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a9332093631759dcfd58267f270de204b0c9388802581c972141e78700c0bb`  
		Last Modified: Tue, 09 Jun 2020 02:20:00 GMT  
		Size: 50.5 MB (50510977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6abb293160bb369db1a3815bce0f615b6d0d75a3a6f4152e6d68933bfa3653ee`  
		Last Modified: Tue, 09 Jun 2020 02:20:29 GMT  
		Size: 206.9 MB (206928247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
