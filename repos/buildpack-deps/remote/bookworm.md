## `buildpack-deps:bookworm`

```console
$ docker pull buildpack-deps@sha256:fc52bc3ee56b14503162c7b591f8efbbe7d3a26cf5f417c0b83f7f069eb9995d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `buildpack-deps:bookworm` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:447d4afda9a12fb2dee2fb03bc3cd35ca0a0c148b52f4e21c89ff632bc939b80
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **331.4 MB (331407099 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b54676ae2886b7995379212fb4fb47a792829619f1e3bcf7a22d78b646ff575`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:57 GMT
ADD file:049a34b0a455f2d6bb7472efc8b4fe28600f9b16fcf86c66e654f0d7f96c617b in / 
# Wed, 26 Jan 2022 01:39:57 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:10:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:11:42 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:174dc37d1760a198250a591524de55fe80951eb332d1b5fda14aa58b2d0274ae`  
		Last Modified: Wed, 26 Jan 2022 01:45:22 GMT  
		Size: 55.6 MB (55560743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ad4f3c5938976e31cd1193f27047d074e6094f3e599687768b82217ddd84ef`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 5.3 MB (5280293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be1ef7f4634c596ef4c86e1e87d912ed9ac6798192b66dbec54ebf05b66e5023`  
		Last Modified: Wed, 26 Jan 2022 02:20:50 GMT  
		Size: 10.9 MB (10915315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a045598fc6de01a49583f44ade3b3b00e5820b17344162c2fbdea94eb012469a`  
		Last Modified: Wed, 26 Jan 2022 02:21:11 GMT  
		Size: 56.8 MB (56784857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79387dd27afaa42b35635410ba4d76071a75219b91e6a3adb2f96bb8bff04b97`  
		Last Modified: Wed, 26 Jan 2022 02:21:55 GMT  
		Size: 202.9 MB (202865891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v5

```console
$ docker pull buildpack-deps@sha256:025cd704993053094976a8f3b0b3f2ffe339f8c47757e25241fe9e8b3f43f4cd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **302.5 MB (302528231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77efd20f89310355d0f969756be791c74bc649818dc6e732b844a618d4bd26e0`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:23 GMT
ADD file:2b96a854a3c9d11256be667f9d982d7d8b9dc55dbebd8b4b5fd405cb278a1c64 in / 
# Wed, 26 Jan 2022 01:40:25 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:25:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:25:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:45 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:29:30 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:63d07b82886a825f18700c37fbcff6322772ad2aa7c6337ed53204a0fa13480d`  
		Last Modified: Wed, 26 Jan 2022 01:55:24 GMT  
		Size: 53.0 MB (53020183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786dbbcc14b50d4e55a52a72c123614a491ab523193b076c2c3567fdc1888969`  
		Last Modified: Wed, 26 Jan 2022 02:51:24 GMT  
		Size: 5.2 MB (5182484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae1bb97567a73aef32ddc428fed052ca711f5df4a1975daa855a68c2d3ce1ae`  
		Last Modified: Wed, 26 Jan 2022 02:51:26 GMT  
		Size: 10.6 MB (10582661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ba482fdbbd02271877b484e0ea6a914eeb789145001e985ecb8effcc2fe524d`  
		Last Modified: Wed, 26 Jan 2022 02:52:19 GMT  
		Size: 54.5 MB (54451328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921171ea13f2299fd20e38e518a6f540999e61e1d7c0cdb1b18a0a186ee00529`  
		Last Modified: Wed, 26 Jan 2022 02:54:20 GMT  
		Size: 179.3 MB (179291575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:44f3ca55306b3d178f89e0ae8641bc58ef590df3f3392663e3669d39764460b4
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **289.5 MB (289522761 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4eb89fd5d09eb00693e09506e6ff4535cf3a21f9a87730b7aab058358150d601`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:29 GMT
ADD file:0d5c36134a34929922dcd5c83256b9539a94c46d5b7dcd23ae6cc29721bdc320 in / 
# Wed, 26 Jan 2022 01:40:30 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 16:33:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:33:59 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 16:34:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 16:37:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:9276ec53f1a5aac51c0a8a27bcc855b50a696f144903a4c1dfab1a458f7f7af0`  
		Last Modified: Wed, 26 Jan 2022 01:55:58 GMT  
		Size: 50.7 MB (50662778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6faba8178fd562af6ed1b6193d73a2eefb5dbc9bc34e5e155d0b644f8d23281a`  
		Last Modified: Wed, 26 Jan 2022 17:00:54 GMT  
		Size: 5.0 MB (5040739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de84da60e6b5c715dc34fc6124ae223b3288b8777242a15fdfb7dd0d91a9261`  
		Last Modified: Wed, 26 Jan 2022 17:00:56 GMT  
		Size: 10.2 MB (10241353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3548f7f03a19175e426fc70dd9fcd2f355f5cc861cbc242716094aa8d3f704d9`  
		Last Modified: Wed, 26 Jan 2022 17:01:39 GMT  
		Size: 52.3 MB (52310560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1221c786b8cfe9790ffbade36b9404f126bd6b960189d8575269b65fa75acda1`  
		Last Modified: Wed, 26 Jan 2022 17:03:27 GMT  
		Size: 171.3 MB (171267331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:dfa15397131918f58fb56169119ba855bd22dfbc6c9c748232dc17e0555daf8b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **324.1 MB (324052315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bce7649115aa58126549651592c9456887e3b5fe653bf61005d9968e25d7361`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:51 GMT
ADD file:585d9a04ed59d36d1ee8be3ad5a7a488962b12f0b7d737826e25a7ab617521fe in / 
# Wed, 26 Jan 2022 01:41:53 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:10:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:10:56 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:11:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:46 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:f9f8cc8e22fa2c53a109b770bcaab20fb907dd9957eb312d9f49000ff4185f8c`  
		Last Modified: Wed, 26 Jan 2022 01:47:52 GMT  
		Size: 54.5 MB (54535243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f8a0926c8b86f048958ba5be5355985e20305f2a6df3fd52b867ac3cfcb7ee`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 5.3 MB (5269783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7042a90d872d1ef29a580051968c7437ef7f8f185841fa2ddf3e7bf37bb0593`  
		Last Modified: Wed, 26 Jan 2022 02:22:37 GMT  
		Size: 10.7 MB (10676573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b7233b23063ef3fe482c0973a9442a36485028dadbd3cb2d8bf3bb8269274f7`  
		Last Modified: Wed, 26 Jan 2022 02:22:58 GMT  
		Size: 56.8 MB (56825175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7eeab825e0d90da9cc97a2f862aaa656e6795a97aace95a5c083be0e8e3fec5`  
		Last Modified: Wed, 26 Jan 2022 02:23:35 GMT  
		Size: 196.7 MB (196745541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; 386

```console
$ docker pull buildpack-deps@sha256:5f07688d74b9c5ef180c72cba755756b8c516aca5828c1aa24d851f80503ad06
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **334.8 MB (334763963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d1cbdbe4f5919d2acf9a1a901d8fa4dcd0f35daf17c4dd646e0e7d053c94d3bc`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:39:06 GMT
ADD file:49bb0653fde7eea7609e6ad9bea8c405d8a514818936cff57f87f5fa321d2582 in / 
# Wed, 26 Jan 2022 01:39:06 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:12:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:12:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:13:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:14:43 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:1308dabb988bd1e94f15ca40572eaddec8a0de059ca7c28b6a83e6821441d6f8`  
		Last Modified: Wed, 26 Jan 2022 01:47:24 GMT  
		Size: 56.6 MB (56598143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec7ba5a7115e901688cba13f3ffc91e6ab2cedb7a7cff304d4bbb5606c507f4`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 5.4 MB (5412384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7645e93b83f1c523ab6c715a08bbfd71c80611ee830755b1e36db82d26c1eb2`  
		Last Modified: Wed, 26 Jan 2022 02:26:42 GMT  
		Size: 11.3 MB (11307381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b85a21b4a33dd378fe3c4484dab108da9bbae3464368991728734991ec15143`  
		Last Modified: Wed, 26 Jan 2022 02:27:11 GMT  
		Size: 58.2 MB (58201530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d9ad6bc8263eddb11f50de4f531cae90340b9d38ad022d51d1b5ea3fae36af`  
		Last Modified: Wed, 26 Jan 2022 02:28:04 GMT  
		Size: 203.2 MB (203244525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; mips64le

```console
$ docker pull buildpack-deps@sha256:891fcf417fddbcc48317714706d348b2cf68ee135ebc4d101d9347e50d85cd3a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **312.3 MB (312335928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9be0941b0552f8f85003dc1d9ad012dfbb081cbbc3dc4d83be99082eb7f1074`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:41:27 GMT
ADD file:cb994d31e0dc06b73ce5e197fffe27837867fce8ab87a858b9668290c97bd7af in / 
# Wed, 26 Jan 2022 01:41:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:15:14 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:15:40 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:16:52 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:20:21 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:45126d37a1c34eefb327242a121bbca1be988e1e2e1cf037fde7eaa131fd6db7`  
		Last Modified: Wed, 26 Jan 2022 01:49:20 GMT  
		Size: 54.3 MB (54262039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a9463250f8710e43e5aff116a08f617cbc14f10997bd69f2bda7a81f002b2e7`  
		Last Modified: Wed, 26 Jan 2022 02:34:27 GMT  
		Size: 5.2 MB (5235335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20371ca4b02d263c2ebdd04847579505ac45245b979462f3374b0acdda280fb2`  
		Last Modified: Wed, 26 Jan 2022 02:34:29 GMT  
		Size: 10.9 MB (10874712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca4c2df8a803e41441178f5ffe30f7ee30d91807c496750ff0cae99fc163063c`  
		Last Modified: Wed, 26 Jan 2022 02:35:20 GMT  
		Size: 55.6 MB (55624962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5649fbf214df60c04e059d985d970374507c685293eabb9c33b46f665d0dac30`  
		Last Modified: Wed, 26 Jan 2022 02:37:31 GMT  
		Size: 186.3 MB (186338880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; ppc64le

```console
$ docker pull buildpack-deps@sha256:6d26c277e578ae70fc07da169bd2c9f7bc0fb3ba463b80694c4b12c54d0d6997
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **341.5 MB (341483154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7951d8e301c4c859d6e551c802f3a6566c70ea7b8b877f4d6d3ea4a0908b4443`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:45:20 GMT
ADD file:815d918aa7e03d3a0e2d0dd87d7d9696feb37b5054d103e1ac83847b08e877a2 in / 
# Wed, 26 Jan 2022 01:45:26 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:23:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:24:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:26:56 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:35:39 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:2fe2b17ea8278b5a905731f1d003664a61c7774f4a23cda61a596487a1b51210`  
		Last Modified: Wed, 26 Jan 2022 01:54:29 GMT  
		Size: 59.9 MB (59942176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4cbdc2b57b1d5abc56a5ce2448279d438e672ad3740a30808c6aca777b1ba7`  
		Last Modified: Wed, 26 Jan 2022 03:13:11 GMT  
		Size: 5.5 MB (5544663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46175642455b8055d9ddc0cbcac8518413ed6ae29f42a87871058a9c7df76e08`  
		Last Modified: Wed, 26 Jan 2022 03:13:14 GMT  
		Size: 11.7 MB (11693166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2209b60fdeff528905267562368c5bb713edc81a5b929e3c31387a9f3cb62a6`  
		Last Modified: Wed, 26 Jan 2022 03:14:10 GMT  
		Size: 61.5 MB (61468948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9abeffa132ae31c5417aeefeaef389fe0141f2bac5bfb078135b40dc4ee438b7`  
		Last Modified: Wed, 26 Jan 2022 03:16:09 GMT  
		Size: 202.8 MB (202834201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:bookworm` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:c890c4d67b294a70fb8ca9ca239f70144ac9df6f07bb144db0a4476ffae05eab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **303.8 MB (303792173 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f927e9ab954205d4f3d5283a06b9b19b4087d105f26b5e9d600f7dbd68bd1427`
-	Default Command: `["bash"]`

```dockerfile
# Wed, 26 Jan 2022 01:40:21 GMT
ADD file:b56123b23454cb9db7a2a2e19c5219cf5643b8692bc247ac4212732f2a8d218a in / 
# Wed, 26 Jan 2022 01:40:28 GMT
CMD ["bash"]
# Wed, 26 Jan 2022 02:06:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:06:29 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 26 Jan 2022 02:06:50 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Jan 2022 02:07:40 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:4155c67ca83ba1ee87acdfb0ff7b262e769e0a27829b9b44ca097c4ba1e29ea4`  
		Last Modified: Wed, 26 Jan 2022 01:46:07 GMT  
		Size: 53.8 MB (53837097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c610ffbd8c4fbe8756d41005ec7da9c699f84722392728547ac79401b01064e8`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 5.3 MB (5259010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3ed15a8cf3570b9b0ddac9365776ad36a5024968df38f3bef0cabb5d6a953eb`  
		Last Modified: Wed, 26 Jan 2022 02:17:04 GMT  
		Size: 10.8 MB (10806960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2dea4fec3c6c14a2719bb370e7430d7fa93a34e49038af8e8f1e2c0e5ad8d7c`  
		Last Modified: Wed, 26 Jan 2022 02:17:23 GMT  
		Size: 56.2 MB (56156804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281107fc73cc269120ebd8e4ae40b80bdf5aa07afeea58093aaad054f37defa1`  
		Last Modified: Wed, 26 Jan 2022 02:17:55 GMT  
		Size: 177.7 MB (177732302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
