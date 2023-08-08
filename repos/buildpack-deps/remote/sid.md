## `buildpack-deps:sid`

```console
$ docker pull buildpack-deps@sha256:28932bdee3619fa266ed61ecdfe65c23ee0b9152f38c8f9893d25233cea83bd3
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
$ docker pull buildpack-deps@sha256:bc0bb95e08ed205a17de1379a423d4d44e52a9488c7fe9cab2bbfcb7ad141298
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **557.3 MB (557269293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccc38cd003d8e650a25ad517e8d5712030439ce1980704ff4cf2e0d69b818b39`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:26:24 GMT
ADD file:89538c836015e15bfe955d940c080e251ce5b25e2cfaac73d8ce77f8475cd08f in / 
# Thu, 27 Jul 2023 23:26:25 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 03:05:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 03:05:49 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:24:53 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9828fc546889681c4c23160b0ee9abb2a08f99ec58b166856cf38d03e0173700`  
		Last Modified: Thu, 27 Jul 2023 23:32:15 GMT  
		Size: 49.5 MB (49462924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1415ec03edfc71940d466b16992ddd3915658c3368432ddd33223a9bf80a2b`  
		Last Modified: Fri, 28 Jul 2023 03:10:17 GMT  
		Size: 24.3 MB (24286692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32deacfa38b7c02986a841b125a79769d3d74c100e44c5f5b142b35e13831a4`  
		Last Modified: Fri, 28 Jul 2023 03:10:34 GMT  
		Size: 64.7 MB (64674483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c5a779e1a53b62babe3fb9204c1be41796097067190b79b67822f58d7293d`  
		Last Modified: Thu, 03 Aug 2023 03:38:15 GMT  
		Size: 418.8 MB (418845194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:e1e01d107a27bb1aff1a2a57f1b719b7c5bddd76c2d4a96f5de6f0790cea370a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542848473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa9b4c59572774505d5d7c7fa9930bafe284062a4fe5f3895b1983fe9c197986`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:49:08 GMT
ADD file:2673f00e844880d10f415db6b62b0d8686b31b02fca062ce8f3f69f12a911daf in / 
# Thu, 27 Jul 2023 23:49:08 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 06:23:48 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 06:24:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 08 Aug 2023 20:51:16 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:cfd23d2efc358b5d10dee265443e93a7ee2f8ba25de718f6768468d3633354ae`  
		Last Modified: Thu, 27 Jul 2023 23:53:05 GMT  
		Size: 47.2 MB (47221377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24b4f87496ef8bdf1448a907c4d6536736135506ae895a3f8c43e54abfcf401`  
		Last Modified: Fri, 28 Jul 2023 06:27:27 GMT  
		Size: 23.0 MB (22958421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00122d9d2372df69cf047d7f54472fb364cda9c02748c185f9da615a327633ba`  
		Last Modified: Fri, 28 Jul 2023 06:27:47 GMT  
		Size: 62.3 MB (62294001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc6a8415f88458e852f58d95f334304759b35cfa88e8fb8d7e576b3b92d9017`  
		Last Modified: Tue, 08 Aug 2023 20:53:23 GMT  
		Size: 410.4 MB (410374674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:6d0260baa8c3f32ef91e0290b79f45a86ef24c186fee9cf870c63d5e412700e6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **499.2 MB (499216482 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3514ef81be9c50ffa6a057647f0d675b6468e8c1eb0b2c6eb0a8cd2ac1a22ca9`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:59:54 GMT
ADD file:751198e94159fde0051292c0a2bcc0ae0c4b82b34b63913cd6860cbed520b9b6 in / 
# Thu, 27 Jul 2023 23:59:55 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 02:04:54 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 02:05:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 01:07:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:d8947caaed239612a0bd233bb275a710201bd19a169719c1541890b12489b8ff`  
		Last Modified: Fri, 28 Jul 2023 00:06:07 GMT  
		Size: 45.0 MB (45003207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b96bf8c5e8d5b1c11dc8c30975084aa14717c1f1f934dac2277e9e70b442786`  
		Last Modified: Fri, 28 Jul 2023 02:09:27 GMT  
		Size: 22.2 MB (22183145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e7aeb6f855e0c83f2b3af5949abe078751618c4af65d6476e5d01a662d8f4e`  
		Last Modified: Fri, 28 Jul 2023 02:09:44 GMT  
		Size: 59.9 MB (59936194 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06f76cc00a908da72b9677936bddc82e0057601a42d166928ca2f928618946d`  
		Last Modified: Thu, 03 Aug 2023 01:23:56 GMT  
		Size: 372.1 MB (372093936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:143f3021e7e32fa79a6284ec82f0a0abc1f3627b5751e01da1f8f8c4c4514d5a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **542.8 MB (542818999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40049b5dc582d12d396a51d3d8f356d522d39469b7ae151faf75da369b9d9e01`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:44:04 GMT
ADD file:dcd44d784a7d0453b2aba140a48cea6ad00cd9860ae3735af4f338a7e242bcc5 in / 
# Thu, 27 Jul 2023 23:44:04 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:40:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:40:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:31:56 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:08e4368591339a72e0b1d1f2280b8e4ec99150999d73beaf90f0bb0f074ac3bc`  
		Last Modified: Thu, 27 Jul 2023 23:49:07 GMT  
		Size: 49.4 MB (49385801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5715207583ba2736d4e317a197d452354d90b2b0974635872ad69588c6c1c6`  
		Last Modified: Fri, 28 Jul 2023 01:44:37 GMT  
		Size: 23.8 MB (23822124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcb506cc81f7b1d26a7bbb59bd8c08177f30223b1b321d36119bd3672ef3bc1e`  
		Last Modified: Fri, 28 Jul 2023 01:44:53 GMT  
		Size: 64.6 MB (64628275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac909580757cd944f7550b66af5777b53eda91ab44cf5fd2cff60f641579d9d`  
		Last Modified: Thu, 03 Aug 2023 00:49:39 GMT  
		Size: 405.0 MB (404982799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; 386

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

### `buildpack-deps:sid` - linux; mips64le

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

### `buildpack-deps:sid` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:c42a6b9a69942c8bc26f1b849496fdfb3845da729626f32fc13a7670e3d34120
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **551.3 MB (551345596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0788f281e8bb074b21c9acbff223f37545989bde78e8baa0c8f8dd64f42b7e3`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:24:36 GMT
ADD file:c9a8e26186be211989debc20aaaea2b9b0a88ef3c95dc67df08fb292c70fd107 in / 
# Thu, 27 Jul 2023 23:24:39 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:56:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:56:54 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 03:23:24 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:8a2370b39a2d35f89bb2978a591923ded0652ff040aa00a837d799ffdb028e76`  
		Last Modified: Thu, 27 Jul 2023 23:31:58 GMT  
		Size: 53.4 MB (53379244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01d10ad7881963b1a20b168e2bcb81ece809f0540619df3bc4c580ed5340359a`  
		Last Modified: Fri, 28 Jul 2023 02:02:37 GMT  
		Size: 25.9 MB (25939781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a7ffe37ee9b72d23063d94fa331f2cc24e8756c3848a55df61f93481f3fbe7`  
		Last Modified: Fri, 28 Jul 2023 02:03:06 GMT  
		Size: 70.1 MB (70134900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9e36de8f0a05b2ef41f1727e8b2bb63e8e345fda8ac9519410dc5790bea6cb`  
		Last Modified: Thu, 03 Aug 2023 03:49:41 GMT  
		Size: 401.9 MB (401891671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:sid` - linux; riscv64

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

### `buildpack-deps:sid` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:8977149e9944289bcc64d312c73e52b0a2ff9e851a8abea8738d601086bf3599
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **503.0 MB (503046023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcbd5499866fa15fc4b6cf31159db828426558c22a9acdba351c1074e3fc5cc2`
-	Default Command: `["bash"]`

```dockerfile
# Thu, 27 Jul 2023 23:48:26 GMT
ADD file:b143b1c75d100b35ca10aac97e0e6b44c6dc267e1c00c3fa2f3f3dd3c408809b in / 
# Thu, 27 Jul 2023 23:48:29 GMT
CMD ["bash"]
# Fri, 28 Jul 2023 01:59:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		sq 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 28 Jul 2023 01:59:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 03 Aug 2023 00:07:04 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ff8109f0f7ac0173229961049cf524677815675d18f6769369db2d95049f4655`  
		Last Modified: Thu, 27 Jul 2023 23:53:27 GMT  
		Size: 47.9 MB (47858669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd6f879bcfe385fa3b5dee9245ad57b8b234bad70af78eef788bb04fa0802b62`  
		Last Modified: Fri, 28 Jul 2023 02:04:03 GMT  
		Size: 24.3 MB (24299780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5daa176328aab710c51edf5d61e90473578a5a55c56a699cb47bdcae40f56313`  
		Last Modified: Fri, 28 Jul 2023 02:04:18 GMT  
		Size: 63.9 MB (63879617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971d815e147de8d035ddab1bf70ecb16577524197088f371fe1e25cb0d23d156`  
		Last Modified: Thu, 03 Aug 2023 00:20:58 GMT  
		Size: 367.0 MB (367007957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
