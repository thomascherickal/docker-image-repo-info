## `buildpack-deps:groovy`

```console
$ docker pull buildpack-deps@sha256:6162e0bc033bac864944fda9196cdb14e7a9fe6cf106a59bf9708bea126b2cf7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; ppc64le
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:groovy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:33661232bc6f6000ed7fe66b9a43fe6e18da41e057d0a4d80ca184a971f2a621
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **254.5 MB (254501848 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d003709c3f8eb24161b2f00d63d8afecbfad9968a0e8c598bd085893cd03f4f`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:21:47 GMT
ADD file:23ff7ae476ddf97e5dbaf417c06418ae4d8d49a88acb92738bf03fb4a22eeca3 in / 
# Mon, 26 Jul 2021 21:21:47 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:50:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:50:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:51:33 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:54:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:32f3531c8415258308e8d8dda886004bc90cdf4793f9b97c6f33e7903036294f`  
		Last Modified: Mon, 26 Jul 2021 21:23:27 GMT  
		Size: 31.3 MB (31342970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f6d92cca49e420ae1a96a98a170c6c6f4d0cfafc25512a58edbb283cb30eec`  
		Last Modified: Mon, 26 Jul 2021 22:12:20 GMT  
		Size: 5.4 MB (5405030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:975758a58780cd2adab51b5973557d092bcde9cdd6c9d23cd120f85919671daa`  
		Last Modified: Mon, 26 Jul 2021 22:12:19 GMT  
		Size: 3.7 MB (3664052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746170fb973f7fb3cefba229af451c7bd2ef9e1410913ef79ed93718b053ed8e`  
		Last Modified: Mon, 26 Jul 2021 22:12:41 GMT  
		Size: 55.5 MB (55478859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42c0ce084a954b4ca9a4e9c8913c16ddd3b2c54d2cff7583129488e0873cbed`  
		Last Modified: Mon, 26 Jul 2021 22:13:17 GMT  
		Size: 158.6 MB (158610937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:cfefe6871c081a029b704048fea0ab885ba557e3fe7204a5375b02f0e297474f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **214.8 MB (214844248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:73b40e41fc34b091288b7658320c453c24df7624485cbb7aedb366939ec4004a`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:21:33 GMT
ADD file:80b5f21ffac906a8416f39204cb526afaf64f15559123cb3a8fb311e312a703f in / 
# Tue, 13 Jul 2021 23:21:34 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 01:55:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:55:38 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 01:56:32 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 01:58:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:7ad80ac50e31c20115b0366841c81a92d1916a7f2113255fe1125324250475e7`  
		Last Modified: Tue, 13 Jul 2021 23:26:54 GMT  
		Size: 26.3 MB (26312397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f87836ed84bb5f0e1d7b61439e8458826efce0a52158d32f928c2efc41367ac4`  
		Last Modified: Wed, 14 Jul 2021 02:19:01 GMT  
		Size: 4.8 MB (4840704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a0657bf22de96a1925b7c31d415ed9eff49f3b00971444459ee9b696832ef`  
		Last Modified: Wed, 14 Jul 2021 02:18:59 GMT  
		Size: 3.1 MB (3140633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e419af2ccab0c7223c92ce4cd8deaa2cdea7e08e02b9636ce5f7193b06162f6d`  
		Last Modified: Wed, 14 Jul 2021 02:19:51 GMT  
		Size: 50.3 MB (50301608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d23fccf18c2c25afdbd5f5c752e3d98caedd067df7b81922dee720a356aba7`  
		Last Modified: Wed, 14 Jul 2021 02:21:27 GMT  
		Size: 130.2 MB (130248906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b43b476cdb6c53cd9d20f5a020aa7058a1e97da4ab2494f61831a7da045d2ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **246.3 MB (246293207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639e286028a2648ecb097a9a5c51188d8f9248b3abc8c0ae3f9985de6caa1640`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 21:49:05 GMT
ADD file:3a4e8fe51fe7ca76be749ef0b92043e9e9b241a7b6f196fbe2a8bcde49c5b3e7 in / 
# Mon, 26 Jul 2021 21:49:05 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 22:30:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:30:43 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 22:31:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 22:31:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:06dd9de3e7a96bf4bd49de5d681cb7062c5b3012c0f1b1bcd9d059380f55a1d2`  
		Last Modified: Mon, 26 Jul 2021 21:51:22 GMT  
		Size: 29.9 MB (29876744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:647214296e105ce8a92eb9ba4b666f72064bb32c3394b392673e54540e1f06d3`  
		Last Modified: Mon, 26 Jul 2021 22:41:30 GMT  
		Size: 5.4 MB (5372238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ff548ea8c26b94143a36cf8245ff00840af96ba22465a184cf4390eb135cb0`  
		Last Modified: Mon, 26 Jul 2021 22:41:29 GMT  
		Size: 3.6 MB (3634615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba06c5b905e953629da8a61f68f094e7248c4f5be8b4bc879a509cfa3c27bb0`  
		Last Modified: Mon, 26 Jul 2021 22:41:52 GMT  
		Size: 55.5 MB (55470630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a958313d25a6895d3979d55d8eed9109ea82b97ddb302227c04b1d2d6d696a66`  
		Last Modified: Mon, 26 Jul 2021 22:42:27 GMT  
		Size: 151.9 MB (151938980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:504e8ba181b570eaef3ef5c3d4d5cafecbef0673a95f350757e3487eee9b2f68
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **273.2 MB (273180579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1030cd605ec9b4d40447f0f22d1463d420e5206614def290ca4b9499a7442da4`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jul 2021 23:22:45 GMT
ADD file:d810eebdcea73da6a0b9c4546fc356b13b60da24827c29923375b8e08f2195b4 in / 
# Tue, 13 Jul 2021 23:22:53 GMT
CMD ["bash"]
# Wed, 14 Jul 2021 02:27:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:30:49 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 14 Jul 2021 02:35:11 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 14 Jul 2021 02:49:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:97b0da8da7b9eb227e28852cb467ba3f76ac379708648200f035c072d3bbf4eb`  
		Last Modified: Tue, 13 Jul 2021 23:28:00 GMT  
		Size: 36.6 MB (36562496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19019a66a1c7600fb2159a63b0e68f36b9d9f55e9e56ae7b70139ac7565616c1`  
		Last Modified: Wed, 14 Jul 2021 03:24:17 GMT  
		Size: 6.0 MB (6040945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b7e113d40008d7a4f01ffb65b6bee553ec1af6ea5935387bfc2677d6a9888ba`  
		Last Modified: Wed, 14 Jul 2021 03:24:01 GMT  
		Size: 4.5 MB (4522053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f499186162dbbd18ecdc41e48723d94384601a434160e441c62890afc5a08b62`  
		Last Modified: Wed, 14 Jul 2021 03:25:24 GMT  
		Size: 63.7 MB (63743445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65e3158288b5ef034817618aa0df8c144e091a87018c0cd3a8c2d3d2ea551b3`  
		Last Modified: Wed, 14 Jul 2021 03:28:07 GMT  
		Size: 162.3 MB (162311640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:fad5a07d432a58ed110430951ac1bd79fbd709f82ac01614745ad4475f2bce79
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **262.7 MB (262740327 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a45c2eb63ff91b0c674ee6671806ad3200eb26a293b3f6490a82462d78adfe41`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 23:22:55 GMT
ADD file:b6af3eb17fceb12f32687c7392bcce88c50d169e89e08ce383b0d151f15e35b4 in / 
# Mon, 26 Jul 2021 23:22:57 GMT
CMD ["bash"]
# Tue, 27 Jul 2021 00:04:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:04:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 27 Jul 2021 00:08:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 27 Jul 2021 00:14:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2854584d46af51653126c966b1f675e9fc2d73b12251e85306724f0c3caeabb0`  
		Last Modified: Mon, 26 Jul 2021 23:42:20 GMT  
		Size: 26.5 MB (26524072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22b0f3794b3c283f9fbabd391721114f4de25a212c0905b7daf2ebc9b710aee`  
		Last Modified: Tue, 27 Jul 2021 01:01:13 GMT  
		Size: 4.9 MB (4922828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fe037d460c34fe039d04c5bb4e64cc63b97f55de632b48bdbc5320d075dfb`  
		Last Modified: Tue, 27 Jul 2021 01:01:10 GMT  
		Size: 3.2 MB (3179172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8939850a31790ac98d18e8170f151d862abcd74592a8b0d488c2b6ea0b7d29`  
		Last Modified: Tue, 27 Jul 2021 01:03:21 GMT  
		Size: 50.7 MB (50725184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8ae2e05ca2a2c86aa442c018ad37235ec00e6cd59354de7cc56dae0bf64e24`  
		Last Modified: Tue, 27 Jul 2021 01:08:50 GMT  
		Size: 177.4 MB (177389071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:groovy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:1b6ddf43e2d6311dcfd54806d9e0d4cf5001e5e2544bd53ae05d5ab3002fe0bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **249.4 MB (249441619 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5397f637f81b05ae6f57236f2354d6ffd6108b9ab6a1ff36982a37f72a84c6b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 26 Jul 2021 20:55:22 GMT
ADD file:2f05dac9c72fd83b64830702accb3e1582661b82178055406f437be01591b038 in / 
# Mon, 26 Jul 2021 20:55:24 GMT
CMD ["bash"]
# Mon, 26 Jul 2021 21:42:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:42:31 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Mon, 26 Jul 2021 21:42:53 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		bzr 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 26 Jul 2021 21:43:36 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6ebc30c62ba1234efc4428ed9d6d0f4f9b031ce916310c2d82b099cf9d02d1dc`  
		Last Modified: Mon, 26 Jul 2021 20:57:18 GMT  
		Size: 31.6 MB (31578338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbe77f2c779c381b74f333923da8ee43a24119720802950c7670ba4d2f1b887a`  
		Last Modified: Mon, 26 Jul 2021 21:49:18 GMT  
		Size: 5.6 MB (5629737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac8e5f5f1362b078cf4da3e0b61a4088d2fba405fabc3eeca03b446a08e083f`  
		Last Modified: Mon, 26 Jul 2021 21:49:18 GMT  
		Size: 4.2 MB (4156776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c02853a663b300cdcbfdbee7dbb15c142f5751d95622acbf369d1cf462a63385`  
		Last Modified: Mon, 26 Jul 2021 21:49:35 GMT  
		Size: 60.7 MB (60667196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4f283d4ad1d79f32e3448ac71aa9e738dd9159e19b12cdaabc894a0140e9bd`  
		Last Modified: Mon, 26 Jul 2021 21:50:00 GMT  
		Size: 147.4 MB (147409572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
