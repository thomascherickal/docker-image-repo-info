## `buildpack-deps:jammy`

```console
$ docker pull buildpack-deps@sha256:70a55ab8f03466a1efa0966f01acbf8fd7817f2f3c6749bfa59d137ebe3605a0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 5
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; riscv64
	-	linux; s390x

### `buildpack-deps:jammy` - linux; amd64

```console
$ docker pull buildpack-deps@sha256:25a0a41afe645852b7adb4bec521d58acb0cabf4d2772b5a216db7dc1c78ce98
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **250.3 MB (250253949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ebe6f8a10fc9404b184a26f3fb95a464edb1a5d5428d0df980d9fc93c8dfecb9`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:21:07 GMT
ADD file:7c41c66243d4fb7f89ee02cc01d5befb32079e87dac32fb83e205e92b9acc0bc in / 
# Tue, 05 Apr 2022 22:21:07 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 22:51:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:52:02 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 22:52:46 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 22:55:31 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:494bf829f3895588d3c99674907f92507f4f902e5e75871dca3149b95cdc86c7`  
		Last Modified: Tue, 05 Apr 2022 13:23:41 GMT  
		Size: 30.4 MB (30444702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93234fc0bfcb4e0bf8b378f5a1de8db64ac6e9b9ad43ebdd0d9012a5f7ece5c6`  
		Last Modified: Tue, 05 Apr 2022 23:00:21 GMT  
		Size: 3.8 MB (3818447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666888d6f19e71d74815a443b4b9b8d2a116717b99a59e7d6ef26f10adafa248`  
		Last Modified: Tue, 05 Apr 2022 23:00:20 GMT  
		Size: 3.6 MB (3559489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f768003be8f8ba370bcd3f1252e005e1600a0626719b3d5ea927f8023910544`  
		Last Modified: Tue, 05 Apr 2022 23:00:37 GMT  
		Size: 39.7 MB (39724446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb1531e6f70870f6775f915e4460d3e4a08b9c9bb7f8246e905d38cc3e64b26`  
		Last Modified: Tue, 05 Apr 2022 23:01:10 GMT  
		Size: 172.7 MB (172706865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm variant v7

```console
$ docker pull buildpack-deps@sha256:4c04f4cde8dc534a12bcb982e8f998c9657abca6b81b496bd427175922ea9ad8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **217.0 MB (216968969 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac357e0426f7740ddbc34b42e63d7c69139ade5d9c949ff32599432a5734f65d`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 18 Mar 2022 07:33:30 GMT
ADD file:19a0584ac22c220c1260894e828ead25579919ba2a0448fb8bcf90ba5dc4ca07 in / 
# Fri, 18 Mar 2022 07:33:31 GMT
CMD ["bash"]
# Sat, 19 Mar 2022 03:18:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:18:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 19 Mar 2022 03:19:13 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 19 Mar 2022 03:20:59 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:559c58962576ae20efaf4338d13982a09d934fa524ef90330d051b6ebcb20608`  
		Last Modified: Fri, 18 Mar 2022 07:37:29 GMT  
		Size: 27.1 MB (27069048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2098a0e581836f2c68e2c4dcdf61d703be4f4ad972816519300cfeb2ff2bb8c`  
		Last Modified: Sat, 19 Mar 2022 03:49:33 GMT  
		Size: 3.6 MB (3568653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d4415fb5c74607390e5a07fdef46a85e56c4f53013f42bbe83c307ac1ef516`  
		Last Modified: Sat, 19 Mar 2022 03:49:32 GMT  
		Size: 3.7 MB (3712132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47b59541b72d3d146846e21d3ad7cd50615cfa031db874fb86d0abe7a2659953`  
		Last Modified: Sat, 19 Mar 2022 03:50:14 GMT  
		Size: 42.1 MB (42106210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a921e4832963610b6bde9e4de9879c5ff5ab2bee66e7933a76c3e882f4ccdf5`  
		Last Modified: Sat, 19 Mar 2022 03:51:49 GMT  
		Size: 140.5 MB (140512926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; arm64 variant v8

```console
$ docker pull buildpack-deps@sha256:83aa961e7b5c251b2f54419895443e4e3e2a9618deb0b427e1e004a14b50cc74
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **241.1 MB (241089205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7017e9198f870f3f7ecbf38d1f2616c30e224accb46e501c985d6b066078f1f5`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:41:19 GMT
ADD file:49571aac1d9686cc3e1be327834e8e0a9d0cdef8501fe221dfa628689bd7459a in / 
# Tue, 05 Apr 2022 22:41:20 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:10:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:10:54 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:11:17 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:12:05 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:b267b9306c29bd8ae0bcc24ca28ea93e4424c701b94c4c0390bed799035db1c2`  
		Last Modified: Tue, 05 Apr 2022 13:24:30 GMT  
		Size: 28.4 MB (28399696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47ebe8351a60fd8356b722173592beda77dcf8c69e0d490eace665f5653e6d42`  
		Last Modified: Tue, 05 Apr 2022 23:18:17 GMT  
		Size: 3.8 MB (3792418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e15399f06b734423260659df4dddbe3348365b046d4083c19ff5a3e30bf590`  
		Last Modified: Tue, 05 Apr 2022 23:18:17 GMT  
		Size: 3.3 MB (3319632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1127a3e2fd930b70ae5dff71a4674a1b08883b753958a066ed29b68b88b875bc`  
		Last Modified: Tue, 05 Apr 2022 23:18:34 GMT  
		Size: 39.6 MB (39594397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b346502008f18d1c56eeb4b43d6c29682b243dae0e8d76a20782e769d1fe3a7`  
		Last Modified: Tue, 05 Apr 2022 23:19:07 GMT  
		Size: 166.0 MB (165983062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; riscv64

```console
$ docker pull buildpack-deps@sha256:f2600b4fede88b8b11c4050ad1307fcfb7f80128a0a82537b3b2cf00213ea8a0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **275.1 MB (275081972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60b511f6d7a41e3d28b70de5d0bed23231814a07ada454f31695b4db2328991`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 23:18:48 GMT
ADD file:111551e70c2dff9b316ca994d22d98c8ba5e95c1aca26a676ef5853a4a5bee48 in / 
# Tue, 05 Apr 2022 23:18:50 GMT
CMD ["bash"]
# Wed, 06 Apr 2022 00:23:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:24:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 06 Apr 2022 00:27:44 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 06 Apr 2022 00:34:12 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:ea8a2d6ff1502b32300464ddef6cd4ed60bf6145940732d4d40778f052881391`  
		Last Modified: Tue, 05 Apr 2022 13:26:01 GMT  
		Size: 27.8 MB (27766317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683d27664434b84a2951fb7dcf39167491c663ad9f7d917f0806586b0a262ccf`  
		Last Modified: Wed, 06 Apr 2022 01:00:30 GMT  
		Size: 3.6 MB (3613224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efcd53caa368566d26cceba725759ad13d6d4e176287234686ed6547317aefb`  
		Last Modified: Wed, 06 Apr 2022 01:00:29 GMT  
		Size: 3.8 MB (3776734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990cb4eed17d0aa25999a27a1ef3eb9383c0aee6761f9dde515173872de1eac4`  
		Last Modified: Wed, 06 Apr 2022 01:02:41 GMT  
		Size: 42.5 MB (42529306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb617fa9261e2b7608651ad600b748bdb46ccebe6872242b6dedc2a2fb34d708`  
		Last Modified: Wed, 06 Apr 2022 01:08:48 GMT  
		Size: 197.4 MB (197396391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `buildpack-deps:jammy` - linux; s390x

```console
$ docker pull buildpack-deps@sha256:7ec161c8eb60bba25349ef9e6ad73635f7d721d7a7a96d31f2003a638dd617d7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **223.9 MB (223898903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:615e0cba9c89bee39a070da67aefe00fe83ef4ac31b42e5c73059d89e6c9e2b2`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 05 Apr 2022 22:42:27 GMT
ADD file:7aad5c77da83037f339871c8ca7310f8cd5d58dd9a50ab570634c982c75e7456 in / 
# Tue, 05 Apr 2022 22:42:29 GMT
CMD ["bash"]
# Tue, 05 Apr 2022 23:22:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 		tzdata 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:23:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Tue, 05 Apr 2022 23:23:23 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 05 Apr 2022 23:24:06 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
```

-	Layers:
	-	`sha256:55309136b47b0ec4d120192cf0f514ed61a8af3893247381a7bca1302c435af6`  
		Last Modified: Tue, 05 Apr 2022 13:26:31 GMT  
		Size: 28.7 MB (28660261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e65bae07b6e5a390ef4626c948a042edee489f033d29712ba6287e125ba8dba`  
		Last Modified: Tue, 05 Apr 2022 23:29:25 GMT  
		Size: 3.8 MB (3820201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8aab658e91f73334e7a3bb1502db3b8a7aff7d84df50868d9b1c5f948c322d8`  
		Last Modified: Tue, 05 Apr 2022 23:29:24 GMT  
		Size: 3.5 MB (3470709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5801a2d0f19bc69cc7f242d8556fea3cfbfae40a55041ac6eb70d6159a991746`  
		Last Modified: Tue, 05 Apr 2022 23:29:37 GMT  
		Size: 39.6 MB (39620241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5631b709c041ad51386910999684e00cbc2e81eaae5985e4720827f031b7af5`  
		Last Modified: Tue, 05 Apr 2022 23:30:01 GMT  
		Size: 148.3 MB (148327491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
