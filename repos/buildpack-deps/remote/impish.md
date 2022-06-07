## `buildpack-deps:impish`

```console
$ docker pull buildpack-deps@sha256:327dbd4697b18a6ffa9ce819b9c29a9da24076b19440fa52949305f19e4fe3d0
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
$ docker pull buildpack-deps@sha256:8f89dc8cb69af48ab7ae23904c07945d6c7ba9aa4a656bf7ddc99dd4b9d7d382
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **399.3 MB (399338348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5fdccdbdbcdc4e82adfaec66e066af4317dd37edcf53589af935fb7a4e5a47f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 01:25:24 GMT
ADD file:d1932d13ea73e26ad39647db09c23895cf0644ba34851cb87e777778d59b6730 in / 
# Tue, 07 Jun 2022 01:25:24 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 04:46:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:46:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 04:46:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 04:47:54 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:166e0294b8df947d819744f38e21281ed5f29a2a3b19d191deee511cbfb0e473`  
		Last Modified: Tue, 07 Jun 2022 01:27:26 GMT  
		Size: 29.0 MB (29018061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957087bdfdb81f8de1aa677dbf22ddffc44a0634b3562eed0aadaf264402b3a8`  
		Last Modified: Tue, 07 Jun 2022 04:56:01 GMT  
		Size: 3.7 MB (3678996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f19f7c7d5073b3daec192d10dd5c1097243609ac12726bd5f01620361aec36`  
		Last Modified: Tue, 07 Jun 2022 04:56:01 GMT  
		Size: 3.3 MB (3324409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120d5e4039cfbdf78f70f5dd60e8e1801cf51ad91e1f1f4cf8d1af591438521b`  
		Last Modified: Tue, 07 Jun 2022 04:56:18 GMT  
		Size: 38.0 MB (38033376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e13846d5764895a8d08695e67715502ac7bf1558e64838efaeb85a954d179db`  
		Last Modified: Tue, 07 Jun 2022 04:57:13 GMT  
		Size: 325.3 MB (325283506 bytes)  
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
$ docker pull buildpack-deps@sha256:da208886a6fd5549ced4d39d292f89896050978cbcdd8f3ac5cc4f48ba31592d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **367.2 MB (367154087 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2fe58135360ec8129975e830cf65ce9882a22046777c32d801a4e63f7875715`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 07 Jun 2022 04:05:22 GMT
ADD file:cc4245955f965ca283118b525a5660643b47b60228e1c1ca6350d786a2f54a69 in / 
# Tue, 07 Jun 2022 04:05:26 GMT
CMD ["bash"]
# Tue, 07 Jun 2022 05:53:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:53:25 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 07 Jun 2022 05:54:09 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 07 Jun 2022 05:56:33 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ef8f08deb2ebee9069392096f64a14c620b5694921860dc066d66f8418e72b44`  
		Last Modified: Tue, 07 Jun 2022 04:07:58 GMT  
		Size: 30.4 MB (30425743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2497e758347dfbb792ae78569954af6fc4388e3f627db376173aa91653450b`  
		Last Modified: Tue, 07 Jun 2022 06:08:04 GMT  
		Size: 3.8 MB (3763634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd01edb65da54b7b17c9bf0d0f3ef8d36e9d24a14afb5c3fed60ea1694f6dc0`  
		Last Modified: Tue, 07 Jun 2022 06:08:04 GMT  
		Size: 3.8 MB (3819727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb50f8bf00b3ebcd04d6c3f6a8f05f366c9194295127368f0fbee948fed010f6`  
		Last Modified: Tue, 07 Jun 2022 06:08:17 GMT  
		Size: 38.1 MB (38112669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ddc79718325a15a990c0b1e1fa42017fc3f231ed522276bee441e54e1de10a`  
		Last Modified: Tue, 07 Jun 2022 06:08:59 GMT  
		Size: 291.0 MB (291032314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
