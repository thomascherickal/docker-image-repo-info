## `buildpack-deps:unstable`

```console
$ docker pull buildpack-deps@sha256:741b1b82da200ecebf685fab72b029dcaf13a73655a42c6fe26162aa9ac2962b
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
$ docker pull buildpack-deps@sha256:528b5311a9ae6696bcd00391123c4bc54f3b31b58c58e64d74bc86267eb03278
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **351.5 MB (351457721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b9832bf13f8edec5c1794ddc2768c54640f872d1d3ba82cf610164cf5a2e673`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:22:34 GMT
ADD file:8ed2c72091b90575b320038c2ad715760d6382aeea5c416dd16f7ed04e955217 in / 
# Mon, 12 Jun 2023 23:22:35 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:34:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:34:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:35:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2e79cba44192968ca6ea42058e67723ae58bebd2ea54b31f432b1ffed9fea9d9`  
		Last Modified: Mon, 12 Jun 2023 23:28:29 GMT  
		Size: 49.6 MB (49551965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cda7b25305de24c8cc4e88d990c3c3c70e109b190f7411b9d3237528081a161`  
		Last Modified: Tue, 13 Jun 2023 03:39:26 GMT  
		Size: 24.0 MB (24019326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c71d2bfd3c86199eb06493b2f6d0258d7576aca3f851198b940bb3b1505989`  
		Last Modified: Tue, 13 Jun 2023 03:39:43 GMT  
		Size: 64.5 MB (64535333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e75a9b221ba575bef197107054a01083b3dc2b0d4bedc07f7e6c3fcbde4df462`  
		Last Modified: Tue, 13 Jun 2023 03:40:16 GMT  
		Size: 213.4 MB (213351097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:425577d4371532d7a1016ddbb8661097ceb1b3d84c34fd7797ae4b12cd690ad2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **318.2 MB (318155740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b0af6d02dd2c68e48fc43dcbeca22913a6160330fab418584d083f8d500e97b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:49:10 GMT
ADD file:b79d69fc6594f6ca5e9e76165017858724482b88aa3aa49e3db7b07a3dcabc0a in / 
# Mon, 12 Jun 2023 23:49:11 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:40:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:40:51 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:41:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:13ee4e7971510c95d7e625030699b854921da16f6d5ef29884b269a308a37afc`  
		Last Modified: Mon, 12 Jun 2023 23:52:56 GMT  
		Size: 47.4 MB (47417325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8374a5ed08b072c6f518c88ddf07dd3d9e04e3ccc51d0810b12cd2ae53c998`  
		Last Modified: Tue, 13 Jun 2023 07:44:30 GMT  
		Size: 23.6 MB (23622159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c640f3b5ffb5f4fc9722d6fca3f771a8db79e177cf1b0cfd035587f4d4dcf4ae`  
		Last Modified: Tue, 13 Jun 2023 07:44:48 GMT  
		Size: 62.2 MB (62150140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:638239f1655f4299ec88f74ea4b5a44b44817cf56b426104a7b6e23df2031def`  
		Last Modified: Tue, 13 Jun 2023 07:45:23 GMT  
		Size: 185.0 MB (184966116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:bc482d01bcfba9d59704601f01b9f3890277671f0f5ae65064ffc8bfd8a092bc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.0 MB (301978210 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993c7c66f179e1f8a499111f4da05a053490bbe72ab3e5d29a35162ec157f3cf`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:00:33 GMT
ADD file:82567bde3caa9ad83c0c12c0525e6fd51cc833f0b29e733c2da572ed00150220 in / 
# Tue, 13 Jun 2023 00:00:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 05:00:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:00:58 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 05:01:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1d80e7ebc54969ad575378cf66dc58999cbf341e0d2a92c9ff0bfd5b3b9fb1c3`  
		Last Modified: Tue, 13 Jun 2023 00:06:30 GMT  
		Size: 45.2 MB (45234838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a26e461ec0e64583c2acfbef48942f57c9de9da65ff1a078a62e910baf3ce05`  
		Last Modified: Tue, 13 Jun 2023 05:05:32 GMT  
		Size: 21.9 MB (21922951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4da543e1cb7517b023e6ef07f0f0385da6f0c3f832cfd7ade1c7381c2ffe580b`  
		Last Modified: Tue, 13 Jun 2023 05:05:49 GMT  
		Size: 59.8 MB (59799388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a6dd7ea367162c4002f5bdde6db8bbbef4671fde6486cf888d7a0bb5c07e29`  
		Last Modified: Tue, 13 Jun 2023 05:06:19 GMT  
		Size: 175.0 MB (175021033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:9b1e52d6511e5cfbcb6ad379788c4aba30e2dd9ab3e9909a0843477506f3d785
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **340.1 MB (340130427 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4578dc30c4d05d7a1fed527a3d742d540a2f37c1cbac255db25eb945baf702b1`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:41:38 GMT
ADD file:94f1432513f9a03b38028af02b1d1720fb0558559faf3e7f9d7097cf6b962056 in / 
# Mon, 12 Jun 2023 23:41:39 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 03:05:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:05:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 03:06:34 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8ba9ab3e6f12b9702649c2e0c7d78e22ffb9183f68c288b9edef2387bd8d4efd`  
		Last Modified: Mon, 12 Jun 2023 23:46:36 GMT  
		Size: 49.6 MB (49592096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393fb89bae1d5f0307a283cb7c3b5f54cc63fde2e90b7b65ceae29bcd27126f5`  
		Last Modified: Tue, 13 Jun 2023 03:10:09 GMT  
		Size: 23.6 MB (23558237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4483fcef438011d245d9be3906ab5e6a92c139027fe4286dc7e46b975299183`  
		Last Modified: Tue, 13 Jun 2023 03:10:24 GMT  
		Size: 64.5 MB (64490917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cddf934afceb08172df763ffcde92b9665c3c8ae9c4810b008715669ad3d58e`  
		Last Modified: Tue, 13 Jun 2023 03:10:52 GMT  
		Size: 202.5 MB (202489177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; 386

```console
$ docker pull buildpack-deps@sha256:b4764a5e07b05e2bdd8d6d90fa4ff2e34c122e475fc4aa317242bebe454cba77
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **353.6 MB (353591470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27e185958c518f02129b840a8ea93d9703f29c31e0bb0ee3ca1e71acfb27d11b`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:42:10 GMT
ADD file:209e3bb955801ad81eb18a280f9fbd5500a0e1f04565e6c94c9cd24dcba4c0af in / 
# Mon, 12 Jun 2023 23:42:10 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 01:09:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:09:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 01:10:38 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8bce10b6f772acc79b03d87add4bd359f98c767e3599f82d8e351cced14c1a11`  
		Last Modified: Mon, 12 Jun 2023 23:49:26 GMT  
		Size: 50.6 MB (50562699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d6b7d433b6a8b07b01e4b262b82f2b882380e41bcd3a6e8b88ca32ea66321e`  
		Last Modified: Tue, 13 Jun 2023 01:15:14 GMT  
		Size: 24.9 MB (24858532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f1c9493cccdfcd2c44a013f62ecc08283137f3fd2d7a483cf56387dc987b536`  
		Last Modified: Tue, 13 Jun 2023 01:15:36 GMT  
		Size: 66.4 MB (66355536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e30574996c34012fa193dace0f01bb334e773810647079cb6d2a76b7945342d`  
		Last Modified: Tue, 13 Jun 2023 01:16:23 GMT  
		Size: 211.8 MB (211814703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:0d42590a778653226abaaaeba3e4d95d9f165e2cb3520044566e699afa0f811f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **326.3 MB (326264556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:732624570cf9a1dec3651b64baba5195328bdb63e629cb11fed831a9a8341e59`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 00:12:52 GMT
ADD file:b2a9cefcdd223b4cbf9b1abac81e8c0c158a24f9c272910a8822619ea9d55ae9 in / 
# Tue, 13 Jun 2023 00:12:57 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:13:57 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 02:19:15 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:65733d4f161a7d2fd9cef6d80eb7fe00897e936eb78d018361809f7384b08c28`  
		Last Modified: Tue, 13 Jun 2023 00:25:52 GMT  
		Size: 49.6 MB (49561285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cac982d96cd0724a1a282faecd42ae997cf2e6c468441bdcf2ce718f092f4d`  
		Last Modified: Tue, 13 Jun 2023 02:26:09 GMT  
		Size: 23.6 MB (23606470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec621985ebc463298904a643b89d8805cdefe9a156edc65db797295bf5ce37d`  
		Last Modified: Tue, 13 Jun 2023 02:26:58 GMT  
		Size: 63.4 MB (63449697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43067e7ef8f78b7740cb05aa82b22965d78ae240348e6c33c24dca2d27e8f056`  
		Last Modified: Tue, 13 Jun 2023 02:29:12 GMT  
		Size: 189.6 MB (189647104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:eacd16ff9356ba0c57dfa909efcc62d6405fa44679146f06c15e26d48ec5c4a1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **365.8 MB (365821306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00dce918605ba965c51b6e622e0516b98b712cdb92b58dee885ac0e9d72b0b0`
-	Default Command: `["bash"]`

```dockerfile
# Mon, 12 Jun 2023 23:19:31 GMT
ADD file:aded196ce7e0c005fe55d5a92492be8cc5d7934fac082b7ab95b8c946e71e0a2 in / 
# Mon, 12 Jun 2023 23:19:34 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 07:34:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:35:40 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 07:38:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:6e3f8e732e00762188b5ba00db7db3f36c97d0fccdf3d6121db4ca1febc7d190`  
		Last Modified: Mon, 12 Jun 2023 23:26:13 GMT  
		Size: 53.6 MB (53558517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3615faaadea50ed31520dc05aeaebf1283ee0aae09227fb97c1a9de87beec2f8`  
		Last Modified: Tue, 13 Jun 2023 07:43:30 GMT  
		Size: 25.7 MB (25673673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cdc90af7293b0d3b333a9a6a8a60e61400bc5577336008e14e772e6041c6bce`  
		Last Modified: Tue, 13 Jun 2023 07:43:56 GMT  
		Size: 70.0 MB (69985119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ffd035648c807001473ccb0f1a04d6d76990ef3e357d8f0b665979b64afe78b`  
		Last Modified: Tue, 13 Jun 2023 07:44:54 GMT  
		Size: 216.6 MB (216603997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:0150bb87b97db7106a8883b1971dae5b87fbd5391ec9118cf15f6932d83b0f8d
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **584.9 MB (584935368 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77126be424a00a29f764cd8e7f8da503eebb4c14608d89dd3edd5a2278ccba0d`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:09:51 GMT
ADD file:fdcff160dcad587bb28b0cba721c24193be4ab5de90a2d503cba3d329b78797b in / 
# Thu, 27 Jul 2023 23:09:54 GMT
CMD ["bash"]
# Thu, 27 Jul 2023 23:32:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:35:21 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Jul 2023 23:45:03 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f8b93f818da821e670e126126d6da395bdf2888315b8baa1a6912378c2f4e02c`  
		Last Modified: Thu, 27 Jul 2023 23:12:55 GMT  
		Size: 45.7 MB (45656956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebdc8d46a9f89f9d06db33ee07cddd8aa1a54e242cd6463179064bb8e0711848`  
		Last Modified: Thu, 27 Jul 2023 23:45:49 GMT  
		Size: 23.4 MB (23350890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0a627ecd6eb80659b2ec0c3464124a436336a8496c101d36a4e46180fdb32a2`  
		Last Modified: Thu, 27 Jul 2023 23:47:12 GMT  
		Size: 60.4 MB (60386385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8d3e46d641c1277be46ab521cccf04aeac468f053836ff4e0626b3a862cb7d`  
		Last Modified: Thu, 27 Jul 2023 23:57:35 GMT  
		Size: 455.5 MB (455541137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:unstable` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:b0b9dab7c2e1f21c627113aa1c6b9c21050761ca06e8b97d1d0e19434da79de6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **320.6 MB (320614417 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f275f768edd7209671adc00107c2353b50953ca84973ce178959ce461e831127`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 13 Jun 2023 04:30:54 GMT
ADD file:7ea0e5c460c626891cd3fc90639d6bfb9a27beeb7f5c79fd9c348c5b6244bd0d in / 
# Tue, 13 Jun 2023 04:30:58 GMT
CMD ["bash"]
# Tue, 13 Jun 2023 18:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:03 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Jun 2023 18:34:50 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:a129144c9fdcf79f6394b7f7bfa3d7e6a0c8ebfd424dca918695356a1b3bf970`  
		Last Modified: Tue, 13 Jun 2023 04:35:27 GMT  
		Size: 47.9 MB (47920583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d42182bfe271810fa332f879c12433ca046660729997bdce646aa7157138984`  
		Last Modified: Tue, 13 Jun 2023 18:39:25 GMT  
		Size: 24.0 MB (24020404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b53f300fd0adc6e321c844bd2e2fb478de90848743069202361df4928dd446b`  
		Last Modified: Tue, 13 Jun 2023 18:39:39 GMT  
		Size: 63.6 MB (63617737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeb3234b4fe971e1c4b0c7127991671379ecc9df17d1b611ddf4553cd898f10`  
		Last Modified: Tue, 13 Jun 2023 18:40:07 GMT  
		Size: 185.1 MB (185055693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
