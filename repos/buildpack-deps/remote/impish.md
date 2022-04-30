## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:b61083933ffd30498a7be820d0a1e4f3f1852d667b19c763fa58d2756e9c31f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:impish` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:952f6b0213b4d63b9f3a36ddd09c044c1660bb0652b69d1f105235b7081b623b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406680969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0fea455216bed7a159018407b8fb77411b664f79aa7280b733225a71beba725`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:21:07 GMT
ADD file:e36038a1f6ee02f3f9a7db183e116f58d277e97cb7e71032634097d802654d02 in / 
# Fri, 29 Apr 2022 23:21:07 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:50:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:51:03 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:51:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:54:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:940122ec7d0c039d048e3bf953a33cd8ef814fd587266a5e732d24d2314af8f1`  
		Last Modified: Fri, 29 Apr 2022 23:22:38 GMT  
		Size: 30.4 MB (30383364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc136e8e3c47f61408398c98287fa53af20236ad2006f834594cc5863aa38b67`  
		Last Modified: Sat, 30 Apr 2022 00:02:21 GMT  
		Size: 3.7 MB (3694309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6afad01b9cdd53ebce85092828446a6cd6f8cfb65ca1a433101b71577c8919a7`  
		Last Modified: Sat, 30 Apr 2022 00:02:20 GMT  
		Size: 3.6 MB (3552457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78329ea85bf6353fcf4a155ac7e13ab65ea7844eef65a748048f03a8c64983c8`  
		Last Modified: Sat, 30 Apr 2022 00:02:36 GMT  
		Size: 38.1 MB (38073735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f15eb19915534a58f6063a1e268b8927ee8fae35f3f197792936f9a1950ef2`  
		Last Modified: Sat, 30 Apr 2022 00:03:27 GMT  
		Size: 331.0 MB (330977104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:98472f23ee60d43d3af85cee2cf8faa4d67722d87437e08d78158df5addb4ac9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **371.1 MB (371093171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a6aa3fb17fc565ab34f73e3f3fb940752fdfd5c42abd54d791114110e297bf0`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:59:09 GMT
ADD file:98b792cccd674eb149eee0fddc60ebe9484757384fe35630fc361ecfc28f9e42 in / 
# Fri, 29 Apr 2022 22:59:09 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:31:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:31:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:32:18 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:34:25 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2a09877f6132d465ce4f615f0c5f4bb1dc0e311ce406712beced416d3257e69c`  
		Last Modified: Fri, 29 Apr 2022 23:03:29 GMT  
		Size: 26.9 MB (26920477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4af27a84ac863174a3e2c6171bf9613a188ce8b1b037ddbc4f0fedd477c695`  
		Last Modified: Fri, 29 Apr 2022 23:49:02 GMT  
		Size: 3.4 MB (3444024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a5bb5b4bcc573ab723569d88c431ee0657394bc927acb599d0f698782c366c`  
		Last Modified: Fri, 29 Apr 2022 23:49:01 GMT  
		Size: 3.7 MB (3743731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e719bc55e12cdb38d3ec4ef091fb6b61c61f0a27074cde39df57783e5d83dc6b`  
		Last Modified: Fri, 29 Apr 2022 23:49:43 GMT  
		Size: 40.3 MB (40288593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0611332f5c484d6fa3b63c78e918bfb8e3fed5e0d63154619d198df88a1e98d`  
		Last Modified: Fri, 29 Apr 2022 23:52:43 GMT  
		Size: 296.7 MB (296696346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:7cb723b800acddf293a68669264fa447dc8c9240006fbcc4a917e366d1ce46c9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.4 MB (399359325 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9ed3abee6e11ab2b6bc2e732c04275127b50095a514200554cc81bc09f50934`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:49:43 GMT
ADD file:d800d571fc22b337baaf45095bd1a303ca66065106c8b943a7a869e145896077 in / 
# Fri, 29 Apr 2022 22:49:44 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:17:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:18:08 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:18:30 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:19:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:924f038c577f5fb37fec4317d1c44a40bae2f6ee798dc0e31394270b30d69e8d`  
		Last Modified: Fri, 29 Apr 2022 22:51:50 GMT  
		Size: 29.0 MB (29029534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e757d57f9b92f1d537667767d80d964200253f44e0fd0450d481d49710944c4d`  
		Last Modified: Fri, 29 Apr 2022 23:25:46 GMT  
		Size: 3.7 MB (3677922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c053745174b0f3dbc495ff442a2793d0657bdd261a9d160f87c6d47424f4d33d`  
		Last Modified: Fri, 29 Apr 2022 23:25:45 GMT  
		Size: 3.3 MB (3327579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f20934735405fc867dbd7cda932a1436395f40e3bf325ddb688d79b5f0c3c53`  
		Last Modified: Fri, 29 Apr 2022 23:26:03 GMT  
		Size: 38.0 MB (38033146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0fc762af538fa97b6190c26f9751c72a216a46af0198b727e6dc2d036f8787`  
		Last Modified: Fri, 29 Apr 2022 23:27:01 GMT  
		Size: 325.3 MB (325291144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:0ab105cffd3e73b9ea329c4a645e2b6e53581d21e3a99bf0992df5a18f603dc9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **414.3 MB (414301215 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c55365a361a1d465b54cb0c1a6cf3982b123e2fc30c04b9a3e91938b17182a3`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:22:47 GMT
ADD file:6fee77e76b27182351bc3f1670478775d45b940b676a9c68b3057638166e1f3e in / 
# Fri, 29 Apr 2022 23:22:51 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 00:14:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:14:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 00:16:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 00:21:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8b9131999f6427d8e2f8c2e6af3dc4889e32c5ea861065b2f8c24539e9c7d81a`  
		Last Modified: Fri, 29 Apr 2022 23:25:51 GMT  
		Size: 36.2 MB (36172344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e32408ebe4867c2297c1f79093340488b3a376d8635067d1db6b9a03f7ae14e`  
		Last Modified: Sat, 30 Apr 2022 00:27:38 GMT  
		Size: 4.1 MB (4147019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739ead4bfe37181451861b7314ee488b7b8e5b129ccc84ce944bd824e2ac556b`  
		Last Modified: Sat, 30 Apr 2022 00:27:38 GMT  
		Size: 4.2 MB (4242321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079a8792118fe241f9ca299c8f67aca281f519ef1c4cdad0693d1ebb40ac4870`  
		Last Modified: Sat, 30 Apr 2022 00:27:59 GMT  
		Size: 42.7 MB (42728803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d20997c6c3326b6bfffe81922556af117d17d97c0c6b3858bae85ecc6e95c9`  
		Last Modified: Sat, 30 Apr 2022 00:29:06 GMT  
		Size: 327.0 MB (327010728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:abb3f5dcd57f83523d9403ecbe95fc48c4e47d716257c80712810562e1b3b131
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.4 MB (266375455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f858510d9953e234a3ada9a5d240edcb29d8f7d19647cb89997dd67a08d4302`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 23:16:52 GMT
ADD file:9b1d81091b302d999994d0aff49d52975044c0786e8d7aa0df0ce41ec3c5902b in / 
# Fri, 29 Apr 2022 23:16:54 GMT
CMD ["bash"]
# Sat, 30 Apr 2022 01:42:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:42:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 30 Apr 2022 01:46:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 30 Apr 2022 01:53:01 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3105f98235ad0afa0e8e8fb758ef0e3a7fa3bc505fc19f49da0968611aa32271`  
		Last Modified: Fri, 29 Apr 2022 23:39:06 GMT  
		Size: 27.2 MB (27210922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95edae64347238ed7479c721c429c7d141a6c1b3ea02127ba646cdf7d9443357`  
		Last Modified: Sat, 30 Apr 2022 02:35:21 GMT  
		Size: 3.5 MB (3491073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71357fe3de61b03bab1dcc8d5c48cfe0a5b87d712f28c6c79da9237cc7e2b4e5`  
		Last Modified: Sat, 30 Apr 2022 02:35:20 GMT  
		Size: 3.8 MB (3804556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11611acc6b35758ddeda628ae39fb5e738635c12bf88dc0d2cae315db01da510`  
		Last Modified: Sat, 30 Apr 2022 02:37:29 GMT  
		Size: 40.8 MB (40767241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0d36b10a728312b40b19624701f90a79b87367faf4719e09b77cab8481c02d`  
		Last Modified: Sat, 30 Apr 2022 02:43:25 GMT  
		Size: 191.1 MB (191101663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:impish` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:2b56d25b490f0e65453120229a32010f966f00bdad2363caba136ece47b5ea2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.6 MB (367581767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7cf47716d0f373f96f5f6882f6a7008f60588067d31d331db405971514b8af1`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 29 Apr 2022 22:50:17 GMT
ADD file:1041ef5c07ca82ee2d7f626a60380e731aa09d0d2b9b6877b03abffa280e452b in / 
# Fri, 29 Apr 2022 22:50:19 GMT
CMD ["bash"]
# Fri, 29 Apr 2022 23:12:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:13:01 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 29 Apr 2022 23:13:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 29 Apr 2022 23:14:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:fe0d74cf06c14c44f5210e7c3b5af279f02a1d45707ee11e6afae132344bf765`  
		Last Modified: Fri, 29 Apr 2022 22:52:13 GMT  
		Size: 30.5 MB (30502867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c98e5deeb0d7fe30f6c49a20d056ebc1bf7817655a9468ead107eb77a50d8911`  
		Last Modified: Fri, 29 Apr 2022 23:20:08 GMT  
		Size: 3.8 MB (3763492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5616be16d6fad891f5d8a2aa1456063444902583f787bdffee6956e7edc2bca`  
		Last Modified: Fri, 29 Apr 2022 23:20:08 GMT  
		Size: 4.0 MB (3963749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaf89d9a6b60361801ac73c8a077956ff03b24783c5219bddd6c7e443196084`  
		Last Modified: Fri, 29 Apr 2022 23:20:20 GMT  
		Size: 38.1 MB (38112171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178a64e991df8134d7241eedbb4df21b1678552d09263ca314bbc9fd486a73fb`  
		Last Modified: Fri, 29 Apr 2022 23:20:59 GMT  
		Size: 291.2 MB (291239488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
