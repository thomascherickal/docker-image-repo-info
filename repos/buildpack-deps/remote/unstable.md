## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:99c1910a80f3b1b3999622c7ab8e80380c0b6f561ac678a7b081d988d5ea37df
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

### `buildpack-deps:unstable` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:34b21ab83b812012abce45d63f31ead15530a8b379f5f435fb03ccfad1942ea9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **337.2 MB (337235616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6bfd47ae2b7735966a1ed44b90206e95af8b655316908fe967338452a464d491`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:58 GMT
ADD file:69369feb027cb9fcd22f8a4b51431458f4e51eca8bb0c398edde4cc47c3d74e0 in / 
# Wed, 26 Jan 2022 01:41:58 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:23 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:15:42 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:48c02bc8c594d3500557aad8d76d43fb3cd9632de373f64648f0523fd33f3197`  
		Last Modified: Wed, 26 Jan 2022 01:49:14 GMT  
		Size: 55.8 MB (55811672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc05b5335d4dea27f0ba29bd1ce5c5b9d3b0ab8f87964be3312ecadc0f34e96`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 5.3 MB (5274876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dacb71892995084387b6a8a0a9ac7eae9ee1b597031f8e25ee46a18d91140f6`  
		Last Modified: Wed, 26 Jan 2022 02:24:56 GMT  
		Size: 10.9 MB (10915453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b478847de2f32699c8d076c0b8e04755dfe8ff874f85e216f02d790059369ec`  
		Last Modified: Wed, 26 Jan 2022 02:25:17 GMT  
		Size: 56.8 MB (56795023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519a6a856e11f7542d4b66388c5872ea9898f92b46a721d8f87ee990216cf7b4`  
		Last Modified: Wed, 26 Jan 2022 02:25:59 GMT  
		Size: 208.4 MB (208438592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:461312a74cd7c31f8bb7bcc366abdd029f14c28bc65f0c0a74722087d04b33e0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **307.5 MB (307451171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8cf06e7c9a756d32fe71876507f73311d7e34e6e0a9d68287067f42d9e78e934`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:b2ee7e73ad4207feb437f92888b1a73e57515c82fc8325c4604d21a39771e52f in / 
# Wed, 26 Jan 2022 01:45:21 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:39:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:39:39 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:40:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:43:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:248f9d803d87b1b0a005a24c98133b989ced8e0b664be38cb600b683c4593899`  
		Last Modified: Wed, 26 Jan 2022 02:02:42 GMT  
		Size: 53.3 MB (53255788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc4178c3c07ea158cad18d885ec03af227796d71c4a004c8f15b307cc4de474`  
		Last Modified: Wed, 26 Jan 2022 03:01:01 GMT  
		Size: 5.2 MB (5174902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c0983cc859431bb8e8296bbc443587cef8bf5f35a9b346102ec3018f68c610`  
		Last Modified: Wed, 26 Jan 2022 03:01:03 GMT  
		Size: 10.6 MB (10582966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f1901338eb48d32091b355f97f4e8453becf07e5c6f3213246056f8f8c150b`  
		Last Modified: Wed, 26 Jan 2022 03:01:58 GMT  
		Size: 54.5 MB (54451916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8272fd40bd8d5fd0e813ebae3cac944ea5ec5e3e57ce279c519d0553dd04fa`  
		Last Modified: Wed, 26 Jan 2022 03:04:01 GMT  
		Size: 184.0 MB (183985599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:513ab6ae0b39885dc0ff8dc85de19457da4665ba9e2d23c4120e5dd6057fd0ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.2 MB (294228993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d854a52c90bb9302953775ef435d4ee07735e1b833c2e337634ec1d42513ef62`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:42 GMT
ADD file:25bd7c90ec9cba9155b5f5e4b8ba10eee0a84413efe182bfd8e270eec1783ca2 in / 
# Wed, 26 Jan 2022 01:45:43 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:45:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:45:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:46:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:48:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8beb160c955a6211ac47cc7f90ad3b37999d7da6c9b2f0d32e82d6ac9bb4e6a3`  
		Last Modified: Wed, 26 Jan 2022 02:02:50 GMT  
		Size: 50.9 MB (50897789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5033ef8051fa00849de7e1029124d977fce14e2255ef3ea2e9a0aa226e20a793`  
		Last Modified: Wed, 26 Jan 2022 17:09:44 GMT  
		Size: 5.0 MB (5035338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2221dacf46091a2f23a799af18530570a3c4d219f9d87d052eb48e5982c95d9`  
		Last Modified: Wed, 26 Jan 2022 17:09:46 GMT  
		Size: 10.2 MB (10241510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1f76ba35e51e63fcba8c49e3f3d26df6cf84550a69e9a8be7657bff2df3d43`  
		Last Modified: Wed, 26 Jan 2022 17:10:35 GMT  
		Size: 52.3 MB (52316409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be847485a9a04e36e5c1fb9b34bf8785f81b78f959f0e907dc63dda6e9927e0`  
		Last Modified: Wed, 26 Jan 2022 17:12:25 GMT  
		Size: 175.7 MB (175737947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d6517f223d5612ca6817c62ba7f8db23864b3b2c3d4571893d9456fe6cc81202
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **329.1 MB (329108336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98ac843f3264c288d5f92cb2cff90603b7a72602d042a06748cbf35638f625bf`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:43:52 GMT
ADD file:b374f2870285b974edf3ed21e9bcab7b86f3d5f58f504052e4ef7507affd730e in / 
# Wed, 26 Jan 2022 01:43:54 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:16:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:16:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:16:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:17:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:3c162c40f334c8be5b3a873f3af9fdbb3e46d36b02232496f08adc78fd0d1197`  
		Last Modified: Wed, 26 Jan 2022 01:51:38 GMT  
		Size: 54.8 MB (54776771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e5527738d1213690712a506bdfb6a4e4e53f00abc3a857f27e46783342a012`  
		Last Modified: Wed, 26 Jan 2022 02:26:12 GMT  
		Size: 5.3 MB (5263075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cb344bcecb1f1e4eb7e0b7d7ceb695b290ff4e82c3967bc1c646a8c98de6d21`  
		Last Modified: Wed, 26 Jan 2022 02:26:13 GMT  
		Size: 10.7 MB (10676867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3064c5c0474d687b691ad542db19a5af822c25a6bb02dcbdc584dcf2f73154a5`  
		Last Modified: Wed, 26 Jan 2022 02:26:33 GMT  
		Size: 56.8 MB (56834268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c1f652c20e06c8948683dbc64b6032f4dae6fa84dde6693f9e21e7c14d941e3`  
		Last Modified: Wed, 26 Jan 2022 02:27:11 GMT  
		Size: 201.6 MB (201557355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:9a34cf8cd3bc56cee01462e107e62307468bae80f309cf2e66bdeb197f2d862d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.3 MB (340261267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dafe0a2f628c45767cfe2a10e3a939dfe4649c5f904354618f0ae022ac4d986f`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:da0be8aacf1ce5f6b8eac72cc37cf866a1f42436b73a7491a048fc296e2aec59 in / 
# Wed, 26 Jan 2022 01:41:52 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:19:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:19:41 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:20:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:21:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9befaf96f69d02ac54d26fdd6569c9b6bb607e4566ebcdba828f8df0ed688997`  
		Last Modified: Wed, 26 Jan 2022 01:52:27 GMT  
		Size: 56.9 MB (56852445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1205a9ac4da466a85715ecf930f05eece9a89e5b6f512222898eefe087f5697`  
		Last Modified: Wed, 26 Jan 2022 02:31:45 GMT  
		Size: 5.4 MB (5407567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59261fa94d22670274f83195f55b41969e923771145bb95d95eee75fd629f932`  
		Last Modified: Wed, 26 Jan 2022 02:31:46 GMT  
		Size: 11.3 MB (11307649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11174d44c83ac43ad98b9ef06e4e3c5a9d22a22478837f0bcb6e56b78fa74d82`  
		Last Modified: Wed, 26 Jan 2022 02:32:18 GMT  
		Size: 58.2 MB (58197338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:187c7988ecc4fedccb1f545bc8f21e90d8934c50c7e68deacf9acb99536008ed`  
		Last Modified: Wed, 26 Jan 2022 02:33:12 GMT  
		Size: 208.5 MB (208496268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:6b5ad7cd4fd8d9e90048451edd986a9b9b69b41a8e751cd56759b19d390d8bed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **313.4 MB (313389780 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e2c3f6c95e309949b669aa4341425a6b7b43737046cf03055baacac35b939e9`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:44:58 GMT
ADD file:ff5cb17f112000b0283048e51a31c66fa6d3b7b5c73ebbb9e407d66773bd71dd in / 
# Wed, 26 Jan 2022 01:44:59 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:30:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:30:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:31:37 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:33:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:780a90a74dc946c86fcaf8ad99094385c527418934e8729eb8e19bd129202058`  
		Last Modified: Wed, 26 Jan 2022 01:54:46 GMT  
		Size: 54.5 MB (54487249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28747c788a9fd6c864f18d440188468cf9eadd01d3170b173b0dcabaffd1dc0c`  
		Last Modified: Wed, 26 Jan 2022 02:44:18 GMT  
		Size: 5.2 MB (5231642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e77450002c767308f9f932c83fde37fdf6742b761b14caad928f47ea3c8735f`  
		Last Modified: Wed, 26 Jan 2022 02:44:21 GMT  
		Size: 10.9 MB (10875142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6aadb0cded3445b65cafacd82549fdac52529a699b3223b960634edbc065aaf`  
		Last Modified: Wed, 26 Jan 2022 02:45:11 GMT  
		Size: 55.6 MB (55633367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0810f657c5af43d714f0e78b0096d1838f841ed3e8bf6fbef5a18646c1802a`  
		Last Modified: Wed, 26 Jan 2022 02:47:23 GMT  
		Size: 187.2 MB (187162380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:299430777465940626afb0cd679d087a5509f775c29ea0bddff23139970edb44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **342.0 MB (342049379 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3fe1ddc87779531aada5ac25cc0f77018bd1e8e537510879ce691103aa6065`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:48:50 GMT
ADD file:00619ac2b9b09af1ef0989fac7a97e811d92f85cef55887a843850c6edd6397d in / 
# Wed, 26 Jan 2022 01:48:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:58:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:59:17 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 03:00:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 03:09:29 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:207334870a9e08012db59a768343c68c9297e1123cfd3f49c878d325443196c9`  
		Last Modified: Wed, 26 Jan 2022 02:01:42 GMT  
		Size: 60.2 MB (60197594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e44ef395f05a799994decb77ffb1782c89a4c0282be793f404418d1a7f1d81a`  
		Last Modified: Wed, 26 Jan 2022 03:25:17 GMT  
		Size: 5.5 MB (5540064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f233b52a0118c53ec4e4fcbf2d80e0f1a054746b47ff133ba2e3c92eb1246992`  
		Last Modified: Wed, 26 Jan 2022 03:25:16 GMT  
		Size: 11.7 MB (11693400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f445939acd54056bc3389536f9954772ff534bdffa069800f03bfe155736b47`  
		Last Modified: Wed, 26 Jan 2022 03:26:24 GMT  
		Size: 61.5 MB (61473244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc87e4865f8d2b814bd32992f41e2bf6850e5013631d6be1450a6764281f904d`  
		Last Modified: Wed, 26 Jan 2022 03:28:41 GMT  
		Size: 203.1 MB (203145077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

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

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:5c7081c976ca7331e026e502396e8cc86b0e4956bdb088c3eed4fa77594faa12
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **304.3 MB (304314431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00c2469ca95ffd673ad9244bdb1478f5d0ff78ff8674852358a1fa8dd86ce784`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:42:22 GMT
ADD file:3bad388a0bccdbe60c35b9f2f185f24531da6894d5fbaaef83c17aaaf447084d in / 
# Wed, 26 Jan 2022 01:42:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:11:38 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:11:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:12:07 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:13:00 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:018136a50defba2fd8fcf9a0ff234cc3971c8e2e29eaaea1a3db05b950df25a2`  
		Last Modified: Wed, 26 Jan 2022 01:48:18 GMT  
		Size: 54.1 MB (54089891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b646642536852c2c78a0d07f56fe415018ecf441c1ff4bb1f3672347e0a16d0`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 5.3 MB (5254889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716bdea6cf2de7b0ea754b38c3e71201e96482b618ecfe5cdd22d50c44f2853`  
		Last Modified: Wed, 26 Jan 2022 02:20:11 GMT  
		Size: 10.8 MB (10807427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dbff4fde8ad04d5d26795083faa946b6421edd89122c7b1df66bf7226604bf`  
		Last Modified: Wed, 26 Jan 2022 02:20:27 GMT  
		Size: 56.2 MB (56165496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8aa8df13db8e0e51057a08e1b9f7a3c8de26ef2c253b3db530a5fda1de3dbc`  
		Last Modified: Wed, 26 Jan 2022 02:20:55 GMT  
		Size: 178.0 MB (177996728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
