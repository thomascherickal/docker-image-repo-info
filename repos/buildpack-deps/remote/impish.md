## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:b1374a6d8afb93e3d501217e42aa658961f8b68a2a74ae158e27a9986149f03b
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
$ docker pull buildpack-deps@sha256:dba813b3b4c9444aa727c8a3cb1e2d0fdcb91e050644367e0f3aa47e897837d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **406.7 MB (406657338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bd7f9268686ae051ad46a67bc5b8adc8a8b3f6169e61e66f019401d2367c2e5`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 22:21:18 GMT
ADD file:d6b83520d39d5b64128115fc97a16a462c38d8e06ef69baad724eda9da91f934 in / 
# Mon, 06 Jun 2022 22:21:19 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 02:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:12:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 02:12:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 02:15:35 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:54b8fda3c9de3a40f0891ce200de55fc92e825315021192957f1bfe3fc807d7d`  
		Last Modified: Mon, 06 Jun 2022 22:22:48 GMT  
		Size: 30.4 MB (30380290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41583b66ca848f858206ad13d445c445a42b861cb9680ee051e0044d4009451a`  
		Last Modified: Tue, 07 Jun 2022 02:25:52 GMT  
		Size: 3.7 MB (3694680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb932530756d3b13de14424901f964ff45c1fa6c30ee51a67696e49cce8fd03`  
		Last Modified: Tue, 07 Jun 2022 02:25:52 GMT  
		Size: 3.6 MB (3552743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaa9fcd7cce0dae69c36b1dd11dca61dc5043a16935e485ca6a08b2bbd2b64e6`  
		Last Modified: Tue, 07 Jun 2022 02:26:08 GMT  
		Size: 38.1 MB (38074213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1925579b9fb5652523fbcf2e47ac0d080b744c11757cb1edaf0e6738af9be81f`  
		Last Modified: Tue, 07 Jun 2022 02:27:00 GMT  
		Size: 331.0 MB (330955412 bytes)  
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
$ docker pull buildpack-deps@sha256:c21199a3c602762b520685d70fb951a85ff3159f169456ef9a6fa786b94f6f14
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **266.4 MB (266353795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2b5a5f7c42a1231293356bb0aa27785e68af31b5961b1ae647029ecd5d89f7b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 06 Jun 2022 18:16:47 GMT
ADD file:4e3bc2c80a7472615f8c75ce5306a21584b9e79bbf9d38909f6931d844d9bdbb in / 
# Mon, 06 Jun 2022 18:16:49 GMT
CMD ["bash"]
# Mon, 06 Jun 2022 19:18:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:18:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 06 Jun 2022 19:22:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 06 Jun 2022 19:28:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3dfa8236861920dda2ce67cef8af1fa06ae6cb669612efbbf4a2c177a1c1e451`  
		Last Modified: Mon, 06 Jun 2022 18:39:09 GMT  
		Size: 27.2 MB (27205258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9da3832471cab1699fe42149beb8fd20cfc97fd0502136045f739495c7ec559`  
		Last Modified: Mon, 06 Jun 2022 20:18:40 GMT  
		Size: 3.5 MB (3492079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56f9964b882c71197b2b0ccbbd484d2f7db67a95789eb4863714c6825ce59d7c`  
		Last Modified: Mon, 06 Jun 2022 20:18:39 GMT  
		Size: 3.8 MB (3803985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c79dd2126e41864bb2c353f31bc4f295d0312fcec13b4af3a1bf2a1ca02d9bb`  
		Last Modified: Mon, 06 Jun 2022 20:20:48 GMT  
		Size: 40.8 MB (40768693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f1c26f210512a43ea874ffa34ca56cab1127df75e16abccb12e158ea15cf8e`  
		Last Modified: Mon, 06 Jun 2022 20:26:49 GMT  
		Size: 191.1 MB (191083780 bytes)  
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
