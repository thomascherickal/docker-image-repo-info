## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:7c1563d9d203395a0e4602f42c4e2d77ac3afc094f39e1e7829e05c5979264bc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 9
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:sid` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:34d17f62f167127906dbf16ab20e8066d4499cb25ffd9092ca36354eb2137ffa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.5 MB (333469815 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6ac910bceae2addcab7681cef83d1216406cbb5ab8fe827ecc0cfd88657b1f`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:23:26 GMT
ADD file:10087b555ac457b6a577fbbc8206355ac696e76dd49ff2a4eeeb27ac8b9f4cec in / 
# Tue, 29 Mar 2022 00:23:27 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 17:32:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:32:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 17:33:01 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 17:33:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48f4b65c158eb45a0eb2daaee21a00efa6f1ed6e8943806281db050162c30174`  
		Last Modified: Tue, 29 Mar 2022 00:29:32 GMT  
		Size: 55.8 MB (55804401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946c2e447bb7ab1f67caa661b736f358b21370caba6f7c21d7093309266655c9`  
		Last Modified: Tue, 29 Mar 2022 17:40:25 GMT  
		Size: 5.3 MB (5269081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edad27b0c9c2e208a688817fa78f09e8d4f79e064a058415035ecdc886a7e1c4`  
		Last Modified: Tue, 29 Mar 2022 17:40:26 GMT  
		Size: 10.9 MB (10924339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7adf21f150ff42a12da611d2d8abc786d9d5e6025c4274194eb2f048a06d044b`  
		Last Modified: Tue, 29 Mar 2022 17:40:44 GMT  
		Size: 57.5 MB (57460981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d742ccdefba7abd96ef7c732dcf30936fab48f8c0ae7f4070e6afaccd706a7c`  
		Last Modified: Tue, 29 Mar 2022 17:41:18 GMT  
		Size: 204.0 MB (204011013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:3840fdb969ba659fae3bab9864cf0077d44f9a4e47713762aa318ed56fe1a3f4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304337073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb103a87152d0db2c13382a63d583dee0cb3e0041bc187dadff1b6bab40fabf3`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:53:53 GMT
ADD file:8fcd736cc488ae6bc3f8a0a57f5454dbd34b0c05fd62d2bf748eeb34723c2a85 in / 
# Tue, 29 Mar 2022 00:53:53 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 07:51:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:52:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 07:53:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 07:55:14 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:07dd120b73b0ec25351ce0c0743306437c1d81e0ee7e06f053f28a0e58bfa81f`  
		Last Modified: Tue, 29 Mar 2022 01:09:52 GMT  
		Size: 53.2 MB (53206463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182e180f96ffc4d0dea65f46ebf08c1601dba09f8a2bb20ff2f15148ff227cfc`  
		Last Modified: Tue, 29 Mar 2022 08:11:41 GMT  
		Size: 5.2 MB (5164114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3369a2a9d3d9efecc9720a25d251260ac8afb4a7a974b188960c5a1759c27c2a`  
		Last Modified: Tue, 29 Mar 2022 08:11:43 GMT  
		Size: 10.6 MB (10597701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc501bba1675670306129a4d527e61027cd5077d145db1dbda301297e9f32004`  
		Last Modified: Tue, 29 Mar 2022 08:12:34 GMT  
		Size: 55.1 MB (55076642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4546533e2959c2ce0c1816df5458d2432baf3263de84565527da8f6f5e819313`  
		Last Modified: Tue, 29 Mar 2022 08:14:07 GMT  
		Size: 180.3 MB (180292153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:5d126e3e1621d581fe49bea7f6611fcf991fa6f89c76bde7d97ced1e00c8c35f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **293.0 MB (292995514 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6ff4229230bad5268276e82a4983543d6913f1713db0ebdad884b99b1ab5ed7`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 09:34:34 GMT
ADD file:9aa47fa903f49c3cddd2c04ea6dfc8adc7cb3e1b8f49392eb4ef30199e306b55 in / 
# Thu, 17 Mar 2022 09:34:36 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 02:59:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 02:59:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 03:00:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:02:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d5abaa3393d9da88a4f8667cc7ed186e0fcf756926f31ba33f3b531a2db42031`  
		Last Modified: Thu, 17 Mar 2022 09:51:00 GMT  
		Size: 51.0 MB (51008095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a92e937e95ec8c4708c51bf5b42788af6dc7933017024adfe3755af9a222a4`  
		Last Modified: Sat, 19 Mar 2022 03:34:48 GMT  
		Size: 5.0 MB (5023856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f9c704ba15933d332549e911b8ecf5197b7956ef44f600fb06943964d50581`  
		Last Modified: Sat, 19 Mar 2022 03:34:50 GMT  
		Size: 10.2 MB (10244633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59b84168887f66171a81e384a0ec065ccce1eed8938b60a25c845862b96da581`  
		Last Modified: Sat, 19 Mar 2022 03:35:37 GMT  
		Size: 52.8 MB (52834495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9a49bc4f8ca4cbddbb3456d9c8e52b57be4cbdf7a555fd7b4179fb2a0da4dc2`  
		Last Modified: Sat, 19 Mar 2022 03:37:25 GMT  
		Size: 173.9 MB (173884435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:ef9de6e4f596758293eeb2344168dbf055e87dbe126c9f14d2ddaa26cc1f9f82
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **327.7 MB (327711371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34b32d2fbe518a5e74d8120809d1f96b98af3b39be146af4bee3e9d21b645b0b`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:23:19 GMT
ADD file:1d38d88879da25d9a1bc7a4c5e36bc54d45209f4c931e6da3f7a5121498cecf5 in / 
# Thu, 17 Mar 2022 03:23:20 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 22:13:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:13:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 22:14:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 22:15:02 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d1bb23fb7eb3b065e76a0f28cfe8d85ecc762b7cff467fdbcda2f70363c88087`  
		Last Modified: Thu, 17 Mar 2022 03:31:11 GMT  
		Size: 54.9 MB (54916866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94c42e541f9a190ed5b1572f38d77d9a07c7899f7b9640e25460c12e849991f1`  
		Last Modified: Thu, 17 Mar 2022 22:23:20 GMT  
		Size: 5.3 MB (5255457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556c64db2922b5a87b5591ed9b67221014a21677b094903b77fc24099a5a1f3c`  
		Last Modified: Thu, 17 Mar 2022 22:23:21 GMT  
		Size: 10.7 MB (10693240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a84215e2a63ae365e4e0fa67da1b0c8f3b996b8f6f063442e4530fbcc3411e5`  
		Last Modified: Thu, 17 Mar 2022 22:23:40 GMT  
		Size: 57.2 MB (57227764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c549492ab6887e2141e7f726464a89ee0d1f13e7f1faf4fc4601e35c1879aac5`  
		Last Modified: Thu, 17 Mar 2022 22:24:17 GMT  
		Size: 199.6 MB (199618044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

```console
$ docker pull buildpack-deps@sha256:8032cf6e93d99e4bc4281272cc14fc7613b880fd2d8a7fa21370a4288c41fa3f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **336.5 MB (336535254 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a88e32f611eb58fb249f7448433e44000800a2b18aff1acc2b59b91675f9f68`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 00:43:25 GMT
ADD file:a09b15a232ef12356f8a381e48ebbc75da16b46600e0cc9849189196595b48b3 in / 
# Tue, 29 Mar 2022 00:43:26 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 18:00:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:00:22 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 18:00:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 18:01:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:0847c00642d4fc3cd086952d88bb1c62b35fc1592abb8bb98b5f2580cbdf5cc5`  
		Last Modified: Tue, 29 Mar 2022 00:51:53 GMT  
		Size: 56.8 MB (56838514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358597cf26cb0d69578f67ae8478edc056e17062702b8e9b5223d5ef224bce7`  
		Last Modified: Tue, 29 Mar 2022 18:17:32 GMT  
		Size: 5.4 MB (5399988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:229c59efca77e15f2eebc343a63ccaff506b30dec30f8514f410554d9016a9db`  
		Last Modified: Tue, 29 Mar 2022 18:17:33 GMT  
		Size: 11.1 MB (11104016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33c14fb78209a987db23cdb8ca3da7ea675992fd648530b5b3cf73a82bc0598e`  
		Last Modified: Tue, 29 Mar 2022 18:17:53 GMT  
		Size: 58.9 MB (58873710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30d4fd10171e3b0790d15012da0c252098c97efc803d5e1391555a963fac102e`  
		Last Modified: Tue, 29 Mar 2022 18:18:27 GMT  
		Size: 204.3 MB (204319026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:37e38d5015949e03668a65e7362e7c98e8cb1f1ee31e1049d3cbdff2e95610fd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.8 MB (313772151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2a0d37a3af4023a855af820d639472145413a2456d8582a67c9f5a19dd01eaa9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 29 Mar 2022 07:45:15 GMT
ADD file:8f554d1fa0414c8c5592687851c7ff4646547038f7d464423b75f57ecade0e16 in / 
# Tue, 29 Mar 2022 07:45:20 GMT
CMD ["bash"]
# Tue, 29 Mar 2022 08:45:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:46:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 29 Mar 2022 08:48:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 29 Mar 2022 08:53:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:024c5d1fff33205caaf39b2903eafbff594af3ca19d825c46db9f726a37cdcd1`  
		Last Modified: Tue, 29 Mar 2022 07:56:21 GMT  
		Size: 54.5 MB (54453471 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1267a248cdd21e2291d70a49d2f9b0a81d371a99832c18a5c27c5cdfcd4ec4`  
		Last Modified: Tue, 29 Mar 2022 09:41:08 GMT  
		Size: 5.2 MB (5222051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:240eba6da1031777a8269c912451066c83703897876489a9be1d5150c27d785b`  
		Last Modified: Tue, 29 Mar 2022 09:41:10 GMT  
		Size: 10.7 MB (10672619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9f55cdc16bc7b9ebb3d30b72adac432c7463267759bd2df4d8aef6337988df`  
		Last Modified: Tue, 29 Mar 2022 09:41:58 GMT  
		Size: 56.2 MB (56209506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afedd46a003bdce17969c8f9f181ab2e675877e74792702500724ad14e46506`  
		Last Modified: Tue, 29 Mar 2022 09:44:05 GMT  
		Size: 187.2 MB (187214504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:d9ba1b8cde069181d8569cba60eb2549ed5485e6510f0d5fe41501c46c312af7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **345.6 MB (345624007 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f587dac2210ffbe656137c9dab26ad24804802bf26a06f686f42fbe35f18265`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 11:20:22 GMT
ADD file:52ac257bb3e9b43a436c32541c15e9c3a00323e3e1d0b20273b81a572fb8d66f in / 
# Thu, 17 Mar 2022 11:20:27 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 05:59:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 05:59:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 06:01:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 06:08:08 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d022277e505c1e9a57478a80b1b82e11b58551ebc0afcb5e723535b6ee105cc8`  
		Last Modified: Thu, 17 Mar 2022 11:30:38 GMT  
		Size: 60.4 MB (60406211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5191baf63a49f74aafee330281325a08a8d65451cc0ac632e8aa56129d9dca63`  
		Last Modified: Sat, 19 Mar 2022 06:45:43 GMT  
		Size: 5.5 MB (5543862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471dd71263fc10a8a1efc9a8fc7652bc8d0e227dafa1f6f9493a5a9779600d7a`  
		Last Modified: Sat, 19 Mar 2022 06:45:43 GMT  
		Size: 11.7 MB (11702261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b11bc794149909ceb1decbb8091901df40d21ad217894f0b435df98f07d5ec`  
		Last Modified: Sat, 19 Mar 2022 06:46:35 GMT  
		Size: 61.9 MB (61922448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3ae284d96f0fad1536b463086fcf157b6739852e7262f87b4fa0c60d4a6415`  
		Last Modified: Sat, 19 Mar 2022 06:48:47 GMT  
		Size: 206.0 MB (206049225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:8eba6bd76e364d31f470138d12d10a3c1604ee5a3cef225f1a3f478f5abfc74c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.7 MB (342740508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62a6357ff1e99d258d501d195f32663948044cc626d7fe2fa1ec67b1a910baae`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 21 Dec 2021 02:14:08 GMT
ADD file:1dc8a81ea9c954e594eb32623a82cdfb528586b569a915ba8f70a49f68a6f7fd in / 
# Tue, 21 Dec 2021 02:14:10 GMT
CMD ["bash"]
# Tue, 21 Dec 2021 02:56:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 02:57:57 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 21 Dec 2021 03:02:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 21 Dec 2021 03:10:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f6b741955e06623f1924320507da1630323c4cf1d6489febc99917464e765860`  
		Last Modified: Tue, 21 Dec 2021 02:30:31 GMT  
		Size: 51.5 MB (51541457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91689f9aadadd96fe4e4ad4ed92ff1cb6a48034aedc9f41e14d54cf85bcdd039`  
		Last Modified: Tue, 21 Dec 2021 03:34:04 GMT  
		Size: 5.1 MB (5089016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a290be0dbc2a1d1f5f12db96d9dc0949f33b55d33712a23f37c71cb89606a3`  
		Last Modified: Tue, 21 Dec 2021 03:34:07 GMT  
		Size: 10.3 MB (10320854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44222df82131b4d925c2f594e50c018b1fb6d67154b22de79d99eb4cd4a356c9`  
		Last Modified: Tue, 21 Dec 2021 03:36:17 GMT  
		Size: 52.8 MB (52817006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f71e08edf3534b3a52b84e74759377bd253863a9cf43fa9dde36a31debd1990a`  
		Last Modified: Tue, 21 Dec 2021 03:42:27 GMT  
		Size: 223.0 MB (222972175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:d032eaf0f6770565c875255fc4e20e3400fa595724ba6fdb2245f5b9cbc50d62
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.1 MB (307058105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b595ff544d0290d392654fee44bf11f86b57e77578bdf8def010699f612de0a`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 17 Mar 2022 03:08:11 GMT
ADD file:4a7b0c9e8bc60d35d06240af5417427853918fe6624688050d4aca10a22b433f in / 
# Thu, 17 Mar 2022 03:08:14 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 18:23:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:23:47 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Thu, 17 Mar 2022 18:24:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 17 Mar 2022 18:24:48 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8e1d6cb1e553f745f248c4d7a409401acdb697f1bd597e8c1c08d6fcd5db0f2d`  
		Last Modified: Thu, 17 Mar 2022 03:13:59 GMT  
		Size: 54.2 MB (54246705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99267e3e8ccd599670f5059d59cf2f80cafc0773fc8b74ba953d5d5cb2189fed`  
		Last Modified: Thu, 17 Mar 2022 18:30:46 GMT  
		Size: 5.2 MB (5245707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3282440b854d7908290c041b1619604c86d6fb3ec5e2ed67356bbd4ef1847863`  
		Last Modified: Thu, 17 Mar 2022 18:30:47 GMT  
		Size: 10.8 MB (10819596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d19b2ec710aa05189651236530efc7d84062cf9d7d6fd4a3d22965342a45839`  
		Last Modified: Thu, 17 Mar 2022 18:31:01 GMT  
		Size: 56.6 MB (56562096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bec8b2539c0c5adea8d81224f6f73686970403543edd954440ee04cb16bc0f`  
		Last Modified: Thu, 17 Mar 2022 18:31:28 GMT  
		Size: 180.2 MB (180184001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
