## `buildpack-deps:buster`

```console
$ docker pull buildpack-deps@sha256:0a2a9772694c7f103b516f39f0c45d6a3c31ca02cceb1476436d2a7cc9ebfcd0
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

### `buildpack-deps:buster` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:fd66239afaaffca7e5c313f24ee4ea78ed09f621618ef757043e68162e709c56
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.4 MB (312411119 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aff731f5464e315af6c60123c32bb1fab79f4256a055c48e559f12bf0f65d686`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 02:20:27 GMT
ADD file:575bf0d00d72810609a4118728923f11625b43de536352fe69a341086e4ebfd1 in / 
# Fri, 12 Mar 2021 02:20:28 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:49:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:49:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:49:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:50:51 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e22122b926a1a853d61887fa35c3fe53e05ee7dc0f2f488936dc9838bd0e230d`  
		Last Modified: Fri, 12 Mar 2021 02:25:38 GMT  
		Size: 50.4 MB (50400353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29e09ae83733d697508e34827538cc0129b8719b85db943041c5d37287bcb81`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 7.8 MB (7832474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e319e3daef68c36099bf3b534377a78d373f67bde3d156119c2463f5fe133ac5`  
		Last Modified: Fri, 12 Mar 2021 03:19:09 GMT  
		Size: 10.0 MB (9997147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e499244fe254b6f980c82ea555f38e7a6527e5105545922005e88a6b81b01cac`  
		Last Modified: Fri, 12 Mar 2021 03:19:36 GMT  
		Size: 51.8 MB (51839506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6ebed20e89bafb5798e66484bd3f1bb41f6e8f6443d231f85b9b6eb2fec334`  
		Last Modified: Fri, 12 Mar 2021 03:20:20 GMT  
		Size: 192.3 MB (192341639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:09466d4352cf33a36e4646eedef162e0446f3686dc33f6f769d256098998d02f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **286.0 MB (286039867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a1ce310506f15274ba76fa9cbfb90cb4bc247185140157753c3e7874ccdffe8`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 07:51:21 GMT
ADD file:8451124009ea487b77e0efd08279d813677a58a69c3e008efffe72456f5b4cd4 in / 
# Fri, 26 Mar 2021 07:51:25 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 09:10:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:10:50 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 09:11:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 09:14:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d38b01f6f9cb629c11a3283c08ac8942a1dabc09a0fd1cf882e144886c4d4c2d`  
		Last Modified: Fri, 26 Mar 2021 07:59:52 GMT  
		Size: 48.1 MB (48111655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b79e4c1a18c62ae0b58fc10bc99ce795232cbcd2cd5aacdda45457357bf228`  
		Last Modified: Fri, 26 Mar 2021 09:27:37 GMT  
		Size: 7.4 MB (7376462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4722e17bbecf50bf547d60af44536f7fe5f2e819630c31abb41dd678e56c40b0`  
		Last Modified: Fri, 26 Mar 2021 09:27:38 GMT  
		Size: 9.7 MB (9687518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02aedf3b95b92593cff7caa2a868b2adc310bc9b40c76820162cfb61f4467959`  
		Last Modified: Fri, 26 Mar 2021 09:28:02 GMT  
		Size: 49.6 MB (49573869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3952d5d93c54c5c1b47b9f0baaa648e341fe8da32b3fc962b059bf140aa1ed0c`  
		Last Modified: Fri, 26 Mar 2021 09:29:00 GMT  
		Size: 171.3 MB (171290363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:97af7621ed24f0c2e1a84eab59226cfe794741c509e05a95eed075a70fcef4a8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **278.2 MB (278240949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09803e44e9353631027de1ea702e5049dc0b813510962cda9c47d3dacc62d0d9`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:10 GMT
ADD file:b3e1f7b8ae0587f7850210420c8dd6da7fb60fa87c5863e6fe5a8bab1bdc7abc in / 
# Fri, 26 Mar 2021 11:17:11 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 13:22:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:22:46 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 13:23:34 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 13:25:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2703ee001e01b49055599d26cac8b1a472b75d8643e8a00ab281b97e3fe6aefd`  
		Last Modified: Fri, 26 Mar 2021 11:26:53 GMT  
		Size: 45.9 MB (45868006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f00d516e34bfa5a11e13fd33e0649e2bfcfa443418341f1cda5463ed8ee8046`  
		Last Modified: Fri, 26 Mar 2021 13:51:18 GMT  
		Size: 7.1 MB (7123912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac789cd7e7d8f8003e7ac6b6bbf96d3859a2318c4569114ccb686ffd779ce119`  
		Last Modified: Fri, 26 Mar 2021 13:51:16 GMT  
		Size: 9.3 MB (9343659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e16bfec3cd4c49403ed5b98e6216074d4f3c68c5dc09e6e12252c09aa8952cc`  
		Last Modified: Fri, 26 Mar 2021 13:52:03 GMT  
		Size: 47.4 MB (47356546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd8364950cc87a0ab5051809b3c724b0484c8ed4b04704e823d1683dc82a32d`  
		Last Modified: Fri, 26 Mar 2021 13:53:22 GMT  
		Size: 168.5 MB (168548826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:d9283f761b6114bfcbdee774810d18d714151075153f36f337971cdac8dad2b1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.9 MB (302928303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e01adb67574e60449b05807a2f3f83bc7cc7e96fea696f590a02381c61e3aa29`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 12 Mar 2021 01:53:16 GMT
ADD file:b2e2cca51e131b97e6a7e02af893c7f9b1f7a491b3d5fdaafa80409ed248a706 in / 
# Fri, 12 Mar 2021 01:53:20 GMT
CMD ["bash"]
# Fri, 12 Mar 2021 02:29:21 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:29:33 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 12 Mar 2021 02:30:12 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 12 Mar 2021 02:32:17 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:e9742a63e95a88f8685c4f23a73f7dd15e4039ac1862ce5753c53406a5f7c04a`  
		Last Modified: Fri, 12 Mar 2021 02:01:14 GMT  
		Size: 49.2 MB (49195763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90273c85fdda8648cee9282aa7b01faf0ec1f45451931985b3504c37cf1ac3e6`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 7.7 MB (7694407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685f873e984153af9a44cf556c7679b430b9c557d901c7d476725134f28754e7`  
		Last Modified: Fri, 12 Mar 2021 02:43:30 GMT  
		Size: 10.0 MB (9984339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34041dfaf60ca49c213d83e89205fc2b7e222817c9728a4aa4f7d3f09d579c9`  
		Last Modified: Fri, 12 Mar 2021 02:43:54 GMT  
		Size: 52.2 MB (52165212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9688107c15585cc88b559730b6668481b4b5d142a662c94868eb4d7fa262a80`  
		Last Modified: Fri, 12 Mar 2021 02:44:48 GMT  
		Size: 183.9 MB (183888582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; 386

```console
$ docker pull buildpack-deps@sha256:a035a0f9fa66778516cd12c7ed9940c06833a8996b9bfc687e703dac5dcb11c4
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **321.8 MB (321821743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1465ae430be90035d98953208432488523be1d8f8cab49f49830cb6efdef8aa6`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 13:52:53 GMT
ADD file:631a0d940844da5859827f6532f16d070023eb5af86b98b26e8225892a728141 in / 
# Fri, 26 Mar 2021 13:52:53 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 22:43:28 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:43:36 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 22:43:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 22:45:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:94f8ae80c7bd585581d232dff8e781c1feaab54ea8d41718d95f0c1059908488`  
		Last Modified: Fri, 26 Mar 2021 14:00:56 GMT  
		Size: 51.2 MB (51160351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75f4518622de265d7d3f5069177f5b74a159365d671532dd8008b136906f5bc2`  
		Last Modified: Fri, 26 Mar 2021 22:56:04 GMT  
		Size: 8.0 MB (7997773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a088421a3906a0c48a07e35676054ae4ed2982936d931624723f6d6c6c1e53e`  
		Last Modified: Fri, 26 Mar 2021 22:56:05 GMT  
		Size: 10.3 MB (10340027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46f38ff13dccaac573470e0e14ff2b88a265abe995ffaa863e5690821b2ee7a`  
		Last Modified: Fri, 26 Mar 2021 22:56:41 GMT  
		Size: 53.4 MB (53437511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c9835606549334ddcb60c816a40c05e319d77fb747ce09981f18c4b1f84ae1`  
		Last Modified: Fri, 26 Mar 2021 22:57:57 GMT  
		Size: 198.9 MB (198886081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:dc5c54890eddccf3eeaf8ab0c6b7ac4c05da40fecfdb7078ac3544d25e544ac1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **297.0 MB (296977313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8e85db0e5cb67965f182f9e17ad8a6c34699a54bcc704524eb40a72a04e7484`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 08:09:33 GMT
ADD file:24fb0f672b9623c5b9e2dc416fe7b91a485519962826a3def620d449c72052f6 in / 
# Fri, 26 Mar 2021 08:09:34 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 18:19:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:19:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 18:20:10 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 18:22:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45e930b5a161529bdb19c7b813062fdeb224d004c1a5a716c817094752214853`  
		Last Modified: Fri, 26 Mar 2021 08:15:45 GMT  
		Size: 49.0 MB (49029292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63ad80a148224544b054bd02d9e38d4e3faab1fd0f5fc036b1fef76b47e3fdee`  
		Last Modified: Fri, 26 Mar 2021 18:30:40 GMT  
		Size: 7.3 MB (7251155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f469c4240f70d8f2677ee4262b580b494bdb76348d54127726bc52308ef1504d`  
		Last Modified: Fri, 26 Mar 2021 18:30:37 GMT  
		Size: 10.0 MB (10016333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834b70d7b92eec946956f610ecfb902f11596ce8501cb6ec617e44f7d3608ca5`  
		Last Modified: Fri, 26 Mar 2021 18:31:32 GMT  
		Size: 50.8 MB (50843088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb73d00aacee035255d5c019f5d0c868ad7ff4ad8914d8b907fed18ed0d8861e`  
		Last Modified: Fri, 26 Mar 2021 18:33:44 GMT  
		Size: 179.8 MB (179837445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:cb1fd1c4561bd2139246286408045d3f826614fd4ef132f46b58fd299cee5944
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **333.8 MB (333773461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23af64f87612a0d961d18d082ecbc44b60f6bc2fb5b7abf87072e6d3a1438985`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 15:13:48 GMT
ADD file:2e3cbe75ac7fb7b716e5b7411062bb9ce510f3317d00ddbfd608a5057931cc9a in / 
# Fri, 26 Mar 2021 15:13:55 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 17:37:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:38:11 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 17:40:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 17:55:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2280757cb36e3eef6465890eb70453bb9f66e271e373f08ae5e9d7a3307c5fe4`  
		Last Modified: Fri, 26 Mar 2021 15:21:30 GMT  
		Size: 54.1 MB (54136619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8de5b549e9718d8f1d72fed2093ec025063ce0d94eb6fe18e4f59d6233dc1231`  
		Last Modified: Fri, 26 Mar 2021 19:40:42 GMT  
		Size: 8.3 MB (8271707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8700bf4e1832c58cc634f3cc177e25538b86637e529844e6f8e340f5b4acd876`  
		Last Modified: Fri, 26 Mar 2021 19:40:32 GMT  
		Size: 10.7 MB (10727704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3650b3afac8fc5a8b47e5ce2681df05154740219a9355d33d04418e90f4b78`  
		Last Modified: Fri, 26 Mar 2021 19:43:11 GMT  
		Size: 57.5 MB (57456809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2201bcb3f7630cea267e25821259e17467f146339142332ea0b0f14ab8d92be9`  
		Last Modified: Fri, 26 Mar 2021 19:47:30 GMT  
		Size: 203.2 MB (203180622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:buster` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:0cbfbc9ba80b22244ebcb6dd0b1cd77c9cdf4fab570874b4280d72dff14afd27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **294.5 MB (294479936 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50ef3583c988bb37a9819fbf488bd8164f0be595d8433d4bed39db4f0f9a1287`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:31 GMT
ADD file:a8707fa1aa1620bd4a2cfb08af992575ed92583d76d9bc5cdf7512c966ef97ec in / 
# Fri, 26 Mar 2021 10:53:35 GMT
CMD ["bash"]
# Fri, 26 Mar 2021 15:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:44:37 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Fri, 26 Mar 2021 15:45:15 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Fri, 26 Mar 2021 15:47:20 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:c1b0086a5cca01c7491d8c2f15dbad8cb1c1829a7d6d1edd7f8c3dd02be85f2b`  
		Last Modified: Fri, 26 Mar 2021 10:57:27 GMT  
		Size: 49.0 MB (48968913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b853ff3a647fb66a2e5b7307061cdfcb221462bf3a73b0a84e58f90ac3b881a`  
		Last Modified: Fri, 26 Mar 2021 15:55:02 GMT  
		Size: 7.4 MB (7399988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:286674edc11eb23904d49908925aff4fe5babc031d3c022fff443a078dd87e21`  
		Last Modified: Fri, 26 Mar 2021 15:55:02 GMT  
		Size: 9.9 MB (9883250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e62476e7ae0d7567aa0af0346254446c4959eb64b48882d260b31cdd605477fa`  
		Last Modified: Fri, 26 Mar 2021 15:55:21 GMT  
		Size: 51.4 MB (51380222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198ee48346222bfcd069741f6da6532c1279cf5e837291f69ca43429e9e5784f`  
		Last Modified: Fri, 26 Mar 2021 15:55:53 GMT  
		Size: 176.8 MB (176847563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
